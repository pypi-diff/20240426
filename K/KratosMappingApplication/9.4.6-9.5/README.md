# Comparing `tmp/KratosMappingApplication-9.4.6-cp39-cp39-win_amd64.whl.zip` & `tmp/KratosMappingApplication-9.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,365 +1,603 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                    808455 (00000000000C5607h)
-  Actual end-cent-dir record offset:        808433 (00000000000C55F1h)
-  Expected end-cent-dir record offset:      808433 (00000000000C55F1h)
+  Zip archive file size:                   2231337 (0000000000220C29h)
+  Actual end-cent-dir record offset:       2231315 (0000000000220C13h)
+  Expected end-cent-dir record offset:     2231315 (0000000000220C13h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 12 entries.
-  The central directory is 1181 (000000000000049Dh) bytes long,
+  central directory contains 16 entries.
+  The central directory is 1889 (0000000000000761h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 807252 (00000000000C5154h).
+  is 2229426 (00000000002204B2h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosMappingApplication.pyd
+  KratosMappingApplication-9.5.dist-info/
 
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
-  32-bit CRC value (hex):                         e664068f
-  compressed size:                                159921 bytes
-  uncompressed size:                              444416 bytes
-  length of filename:                             53 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:10 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             39 characters
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
 
-  KratosMultiphysics/.libs/KratosMappingCore.dll
+  KratosMappingApplication-9.5.dist-info/METADATA
 
-  offset of local header from start of archive:   160004
-                                                  (0000000000027104h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   97
+                                                  (0000000000000061h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         cbd50664
-  compressed size:                                607566 bytes
-  uncompressed size:                              1862144 bytes
-  length of filename:                             46 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
+  32-bit CRC value (hex):                         e9d744a3
+  compressed size:                                7240 bytes
+  uncompressed size:                              23499 bytes
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
 
 Central directory entry #3:
 ---------------------------
 
-  KratosMultiphysics/.libs/KratosMappingCore.lib
+  KratosMappingApplication-9.5.dist-info/WHEEL
 
-  offset of local header from start of archive:   767646
-                                                  (00000000000BB69Eh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   7442
+                                                  (0000000000001D12h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         26857d47
-  compressed size:                                23263 bytes
-  uncompressed size:                              545960 bytes
-  length of filename:                             46 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
+  32-bit CRC value (hex):                         90d34e0d
+  compressed size:                                116 bytes
+  uncompressed size:                              148 bytes
+  length of filename:                             44 characters
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
 
-  KratosMultiphysics/MappingApplication/__init__.py
+  KratosMappingApplication-9.5.dist-info/top_level.txt
+
+  offset of local header from start of archive:   7660
+                                                  (0000000000001DECh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
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
 
-  offset of local header from start of archive:   790985
-                                                  (00000000000C11C9h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+Central directory entry #5:
+---------------------------
+
+  KratosMappingApplication-9.5.dist-info/RECORD
+
+  offset of local header from start of archive:   7789
+                                                  (0000000000001E6Dh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         3c00e851
-  compressed size:                                704 bytes
-  uncompressed size:                              2597 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:10 UTC
+  32-bit CRC value (hex):                         3a184b23
+  compressed size:                                678 bytes
+  uncompressed size:                              1316 bytes
+  length of filename:                             45 characters
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
 
-  KratosMultiphysics/MappingApplication/empire_mortar_mapper.py
+  KratosMappingApplication.libs/
 
-  offset of local header from start of archive:   791768
-                                                  (00000000000C14D8h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   8570
+                                                  (000000000000217Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:10 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             30 characters
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
+  KratosMappingApplication.libs/libKratosMappingCore-e2ac717d.so
+
+  offset of local header from start of archive:   8658
+                                                  (00000000000021D2h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         8a96e75f
-  compressed size:                                3497 bytes
-  uncompressed size:                              15467 bytes
-  length of filename:                             61 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
+  32-bit CRC value (hex):                         47f25455
+  compressed size:                                1669763 bytes
+  uncompressed size:                              6392009 bytes
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
+Central directory entry #8:
+---------------------------
+
+  KratosMultiphysics/
+
+  offset of local header from start of archive:   1678541
+                                                  (0000000000199CCDh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
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
+---------------------------
+
+  KratosMultiphysics/MappingApplication/
+
+  offset of local header from start of archive:   1678618
+                                                  (0000000000199D1Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
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
+Central directory entry #10:
 ---------------------------
 
   KratosMultiphysics/MappingApplication/python_mapper.py
 
-  offset of local header from start of archive:   795356
-                                                  (00000000000C22DCh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1678714
+                                                  (0000000000199D7Ah) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         98fa3960
-  compressed size:                                703 bytes
-  uncompressed size:                              2123 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
+  32-bit CRC value (hex):                         51b66594
+  compressed size:                                692 bytes
+  uncompressed size:                              2069 bytes
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
 
-Central directory entry #7:
+Central directory entry #11:
 ---------------------------
 
-  KratosMultiphysics/MappingApplication/python_mapper_factory.py
+  KratosMultiphysics/MappingApplication/empire_mortar_mapper.py
 
-  offset of local header from start of archive:   796143
-                                                  (00000000000C25EFh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1679518
+                                                  (000000000019A09Eh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         8fd5cf35
-  compressed size:                                720 bytes
-  uncompressed size:                              1998 bytes
-  length of filename:                             62 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
+  32-bit CRC value (hex):                         7d046586
+  compressed size:                                3474 bytes
+  uncompressed size:                              15125 bytes
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
 
-Central directory entry #8:
+Central directory entry #12:
 ---------------------------
 
   KratosMultiphysics/MappingApplication/serial_output_process.py
 
-  offset of local header from start of archive:   796955
-                                                  (00000000000C291Bh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1683111
+                                                  (000000000019AEA7h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 12 23:47:42
-  32-bit CRC value (hex):                         0dc8090d
-  compressed size:                                1843 bytes
-  uncompressed size:                              6856 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
+  32-bit CRC value (hex):                         2345c9cd
+  compressed size:                                1827 bytes
+  uncompressed size:                              6713 bytes
   length of filename:                             62 characters
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
 
-Central directory entry #9:
+Central directory entry #13:
 ---------------------------
 
-  KratosMappingApplication-9.4.6.dist-info/METADATA
+  KratosMultiphysics/MappingApplication/python_mapper_factory.py
 
-  offset of local header from start of archive:   798890
-                                                  (00000000000C30AAh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1685058
+                                                  (000000000019B642h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         418c7315
-  compressed size:                                7285 bytes
-  uncompressed size:                              23923 bytes
-  length of filename:                             49 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
+  32-bit CRC value (hex):                         fd8e66d9
+  compressed size:                                712 bytes
+  uncompressed size:                              1959 bytes
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
 
-Central directory entry #10:
+Central directory entry #14:
 ---------------------------
 
-  KratosMappingApplication-9.4.6.dist-info/WHEEL
+  KratosMultiphysics/MappingApplication/__init__.py
 
-  offset of local header from start of archive:   806254
-                                                  (00000000000C4D6Eh) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1685890
+                                                  (000000000019B982h) bytes
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
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
+  32-bit CRC value (hex):                         c6818dec
+  compressed size:                                695 bytes
+  uncompressed size:                              2546 bytes
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
+Central directory entry #15:
 ---------------------------
 
-  KratosMappingApplication-9.4.6.dist-info/top_level.txt
+  KratosMultiphysics/.libs/
 
-  offset of local header from start of archive:   806426
-                                                  (00000000000C4E1Ah) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1686692
+                                                  (000000000019BCA4h) bytes
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
-  length of filename:                             54 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:10
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:10 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:10 UTC
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
 
-Central directory entry #12:
+Central directory entry #16:
 ---------------------------
 
-  KratosMappingApplication-9.4.6.dist-info/RECORD
+  KratosMultiphysics/.libs/KratosMappingApplication.cpython-39-x86_64-linux-gnu.so
 
-  offset of local header from start of archive:   806531
-                                                  (00000000000C4E83h) bytes
-  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
-  version of encoding software:                   2.0
+  offset of local header from start of archive:   1686775
+                                                  (000000000019BCF7h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Feb 13 01:07:38
-  32-bit CRC value (hex):                         e7d92cdb
-  compressed size:                                644 bytes
-  uncompressed size:                              1265 bytes
-  length of filename:                             47 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2024 Apr 25 16:00:04
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 local
+  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:04 UTC
+  32-bit CRC value (hex):                         74d143bb
+  compressed size:                                542513 bytes
+  uncompressed size:                              1580393 bytes
+  length of filename:                             80 characters
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
@@ -1,37 +1,49 @@
-Filename: KratosMultiphysics/.libs/KratosMappingApplication.pyd
+Filename: KratosMappingApplication-9.5.dist-info/
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosMappingCore.dll
+Filename: KratosMappingApplication-9.5.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosMappingCore.lib
+Filename: KratosMappingApplication-9.5.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics/MappingApplication/__init__.py
+Filename: KratosMappingApplication-9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosMultiphysics/MappingApplication/empire_mortar_mapper.py
+Filename: KratosMappingApplication-9.5.dist-info/RECORD
+Comment: 
+
+Filename: KratosMappingApplication.libs/
+Comment: 
+
+Filename: KratosMappingApplication.libs/libKratosMappingCore-e2ac717d.so
+Comment: 
+
+Filename: KratosMultiphysics/
+Comment: 
+
+Filename: KratosMultiphysics/MappingApplication/
 Comment: 
 
 Filename: KratosMultiphysics/MappingApplication/python_mapper.py
 Comment: 
 
-Filename: KratosMultiphysics/MappingApplication/python_mapper_factory.py
+Filename: KratosMultiphysics/MappingApplication/empire_mortar_mapper.py
 Comment: 
 
 Filename: KratosMultiphysics/MappingApplication/serial_output_process.py
 Comment: 
 
-Filename: KratosMappingApplication-9.4.6.dist-info/METADATA
+Filename: KratosMultiphysics/MappingApplication/python_mapper_factory.py
 Comment: 
 
-Filename: KratosMappingApplication-9.4.6.dist-info/WHEEL
+Filename: KratosMultiphysics/MappingApplication/__init__.py
 Comment: 
 
-Filename: KratosMappingApplication-9.4.6.dist-info/top_level.txt
+Filename: KratosMultiphysics/.libs/
 Comment: 
 
-Filename: KratosMappingApplication-9.4.6.dist-info/RECORD
+Filename: KratosMultiphysics/.libs/KratosMappingApplication.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## KratosMultiphysics/MappingApplication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,51 +1,51 @@
-# Application dependent names and paths
-from KratosMultiphysics import _ImportApplication
-from KratosMultiphysics import Mapper as _CoreMapper
-from KratosMultiphysics import MapperFactory as _CoreMapperFactory
-from KratosMappingApplication import *
-application = KratosMappingApplication()
-application_name = "KratosMappingApplication"
-
-_ImportApplication(application, application_name)
-
-# hacks for backward compatibility
-from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
-
-class _DeprecatedMapper:
-    def __getattribute__(self, method_name):
-        IssueDeprecationWarning("MappingApplication", 'The "Mapper" was moved to the Core! (used for "{}")'.format(method_name))
-        return getattr(_CoreMapper, method_name)
-
-class _DeprecatedMapperFactory:
-    def __getattr__(self, method_name):
-        IssueDeprecationWarning("MappingApplication", 'The "MapperFactory" was moved to the Core! (used for "{}")'.format(method_name))
-        return getattr(_CoreMapperFactory, method_name)
-
-    def CreateMPIMapper(self, *args):
-        IssueDeprecationWarning("MappingApplication", 'CreateMPIMapper is deprecated, please use "MappingApplication.MPIExtension.MPIMapperFactory.CreateMapper" instead')
-        from KratosMultiphysics.MappingApplication.MPIExtension import MPIMapperFactory
-        return MPIMapperFactory.CreateMapper(*args)
-
-    def HasMPIMapper(self, *args):
-        IssueDeprecationWarning("MappingApplication", 'HasMPIMapper is deprecated, please use "MappingApplication.MPIExtension.MPIMapperFactory.HasMapper" instead')
-        from KratosMultiphysics.MappingApplication.MPIExtension import MPIMapperFactory
-        return MPIMapperFactory.HasMapper(*args)
-
-    def GetRegisteredMPIMapperNames(self, *args):
-        IssueDeprecationWarning("MappingApplication", 'GetRegisteredMPIMapperNames is deprecated, please use "MappingApplication.MPIExtension.MPIMapperFactory.GetRegisteredMapperNames" instead')
-        from KratosMultiphysics.MappingApplication.MPIExtension import MPIMapperFactory
-        return MPIMapperFactory.GetRegisteredMapperNames(*args)
-
-Mapper = _DeprecatedMapper()
-MapperFactory = _DeprecatedMapperFactory()
-
-'''
-TODO:
-    - Test for Serialization
-    - Test for local-search?
-    - Cleanup how the MapperParams are used
-    - Further cleanup Trilinos and try some things (read up on opt-stuff)
-    - use std::unordered_set for row & column indices-vectors in trilinos => does the map need sorted indices?
-    - Function-Documentation
-    - Delete copy and assignment-constructors?
-'''
+# Application dependent names and paths
+from KratosMultiphysics import _ImportApplication
+from KratosMultiphysics import Mapper as _CoreMapper
+from KratosMultiphysics import MapperFactory as _CoreMapperFactory
+from KratosMappingApplication import *
+application = KratosMappingApplication()
+application_name = "KratosMappingApplication"
+
+_ImportApplication(application, application_name)
+
+# hacks for backward compatibility
+from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
+
+class _DeprecatedMapper:
+    def __getattribute__(self, method_name):
+        IssueDeprecationWarning("MappingApplication", 'The "Mapper" was moved to the Core! (used for "{}")'.format(method_name))
+        return getattr(_CoreMapper, method_name)
+
+class _DeprecatedMapperFactory:
+    def __getattr__(self, method_name):
+        IssueDeprecationWarning("MappingApplication", 'The "MapperFactory" was moved to the Core! (used for "{}")'.format(method_name))
+        return getattr(_CoreMapperFactory, method_name)
+
+    def CreateMPIMapper(self, *args):
+        IssueDeprecationWarning("MappingApplication", 'CreateMPIMapper is deprecated, please use "MappingApplication.MPIExtension.MPIMapperFactory.CreateMapper" instead')
+        from KratosMultiphysics.MappingApplication.MPIExtension import MPIMapperFactory
+        return MPIMapperFactory.CreateMapper(*args)
+
+    def HasMPIMapper(self, *args):
+        IssueDeprecationWarning("MappingApplication", 'HasMPIMapper is deprecated, please use "MappingApplication.MPIExtension.MPIMapperFactory.HasMapper" instead')
+        from KratosMultiphysics.MappingApplication.MPIExtension import MPIMapperFactory
+        return MPIMapperFactory.HasMapper(*args)
+
+    def GetRegisteredMPIMapperNames(self, *args):
+        IssueDeprecationWarning("MappingApplication", 'GetRegisteredMPIMapperNames is deprecated, please use "MappingApplication.MPIExtension.MPIMapperFactory.GetRegisteredMapperNames" instead')
+        from KratosMultiphysics.MappingApplication.MPIExtension import MPIMapperFactory
+        return MPIMapperFactory.GetRegisteredMapperNames(*args)
+
+Mapper = _DeprecatedMapper()
+MapperFactory = _DeprecatedMapperFactory()
+
+'''
+TODO:
+    - Test for Serialization
+    - Test for local-search?
+    - Cleanup how the MapperParams are used
+    - Further cleanup Trilinos and try some things (read up on opt-stuff)
+    - use std::unordered_set for row & column indices-vectors in trilinos => does the map need sorted indices?
+    - Function-Documentation
+    - Delete copy and assignment-constructors?
+'''
```

## KratosMultiphysics/MappingApplication/empire_mortar_mapper.py

 * *Ordering differences only*

```diff
@@ -1,342 +1,342 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KM
-
-# Mapping imports
-from KratosMultiphysics.MappingApplication import Mapper
-from KratosMultiphysics.MappingApplication.python_mapper import PythonMapper
-
-# other imports
-import os
-import ctypes as ctp
-
-def Create(model_part_origin, model_part_destination, mapper_settings):
-    return EmpireMortarMapper(model_part_origin, model_part_destination, mapper_settings)
-
-
-class EmpireMortarMapper(PythonMapper):
-    """Wrapper for the Mortar mapper of EMPIRE
-
-    Usage:
-    Empire needs to be compiled separately
-    It can then be used by either of the two ways:
-    - (default) use "startEMPIRE" to bring "EMPIRE_MAPPER_LIBSO_ON_MACHINE" to the environment
-    - use "path_mapper_lib" to sprecify the path to "libEMPIRE_MapperLib.so" (by default located in "EMPIRE-Core/lib/")
-    """
-
-    mapper_count = 0
-    instances = 0
-    mapper_lib = None
-
-    def __init__(self, model_part_origin, model_part_destination, mapper_settings):
-        super().__init__(model_part_origin, model_part_destination, mapper_settings)
-
-        if model_part_origin.IsDistributed() or model_part_destination.IsDistributed():
-            raise Exception('{} does not support mapping with distributed ModelParts!'.format(self._ClassName()))
-
-        if EmpireMortarMapper.mapper_lib:
-            KM.Logger.PrintInfo("EmpireMortarMapper", "Mapper lib is already loaded")
-        else:
-            KM.Logger.PrintInfo("EmpireMortarMapper", "Attempting to load mapper lib")
-            EmpireMortarMapper.mapper_lib = LoadEmpireMapperLib(self.mapper_settings["path_mapper_lib"].GetString())
-
-        self.mapper_name = "EmpireMortarMapper_"+str(EmpireMortarMapper.mapper_count)
-
-        self.mesh_name_origin = model_part_origin.FullName()+"_o_"+str(EmpireMortarMapper.mapper_count)
-        self.mesh_name_destination = model_part_destination.FullName()+"_d_"+str(EmpireMortarMapper.mapper_count)
-
-        self.__CreateEmpireFEMesh(self.model_part_origin, self.mesh_name_origin)
-        self.__CreateEmpireFEMesh(self.model_part_destination, self.mesh_name_destination)
-
-        self.__CreateMapper()
-
-        EmpireMortarMapper.mapper_count += 1 # required for identification purposes
-        EmpireMortarMapper.instances += 1
-        self.__inverse_mapper = None
-
-    def __del__(self):
-        if EmpireMortarMapper.mapper_lib.hasMapper(ConvertToChar(self.mapper_name)):
-            EmpireMortarMapper.mapper_lib.deleteMapper(ConvertToChar(self.mapper_name))
-
-        if EmpireMortarMapper.mapper_lib.hasMesh(ConvertToChar(self.mesh_name_origin)):
-            EmpireMortarMapper.mapper_lib.deleteMesh(ConvertToChar(self.mesh_name_origin))
-        if EmpireMortarMapper.mapper_lib.hasMesh(ConvertToChar(self.mesh_name_destination)):
-            EmpireMortarMapper.mapper_lib.deleteMesh(ConvertToChar(self.mesh_name_destination))
-
-        EmpireMortarMapper.instances -= 1
-        if EmpireMortarMapper.instances == 0: # last mapper was destoyed
-            if self.echo_level > 1:
-                KM.Logger.PrintInfo('EmpireMortarMapper', 'Destroying last instance, deleting all meshes & mappers')
-            #  delete everything to make sure nothing is left
-            EmpireMortarMapper.mapper_lib.deleteAllMappers()
-            EmpireMortarMapper.mapper_lib.deleteAllMeshes()
-
-    def UpdateInterface(self):
-        raise NotImplementedError('"UpdateInterface" is not yet implemented for "{}"!'.format(self._ClassName()))
-
-    # protected methods
-    def _MapInternal(self, variable_origin, variable_destination, mapper_flags):
-        if mapper_flags.Is(Mapper.USE_TRANSPOSE):
-            mapper_flags.Reset(Mapper.USE_TRANSPOSE)
-            mapper_flags.Set(KM.VISITED, True)
-            self.__GetInverseMapper().Map(variable_destination, variable_origin, mapper_flags)
-            return
-        elif mapper_flags.Is(KM.VISITED):
-            self.__MapInternalTranspose(variable_origin, variable_destination, mapper_flags)
-            return
-
-        self.__CheckMapperExists()
-
-        var_dim = GetVariableDimension(variable_origin)
-
-        origin_data_size = self.model_part_origin.NumberOfNodes()*var_dim
-        destination_data_size = self.model_part_destination.NumberOfNodes()*var_dim
-
-        c_origin_array = KratosFieldToCArray(self.model_part_origin.Nodes, variable_origin)
-        c_destination_array = (ctp.c_double * destination_data_size)(0.0)
-
-        EmpireMortarMapper.mapper_lib.doConsistentMapping(
-            ConvertToChar(self.mapper_name),
-            ctp.c_int(var_dim),
-            ctp.c_int(origin_data_size),
-            c_origin_array,
-            ctp.c_int(destination_data_size),
-            c_destination_array
-            )
-
-        CArrayToKratosField(
-            c_destination_array,
-            destination_data_size,
-            self.model_part_destination.Nodes,
-            variable_destination,
-            mapper_flags.Is(Mapper.ADD_VALUES), mapper_flags.Is(Mapper.SWAP_SIGN))
-
-    def _InverseMapInternal(self, variable_origin, variable_destination, mapper_flags):
-        if mapper_flags.Is(Mapper.USE_TRANSPOSE):
-            self.__MapInternalTranspose(variable_origin, variable_destination, mapper_flags)
-        else:
-            self.__GetInverseMapper().Map(variable_destination, variable_origin, mapper_flags)
-
-    @classmethod
-    def _GetDefaultParameters(cls):
-        this_defaults = KM.Parameters("""{
-            "path_mapper_lib"           : "",
-            "dual"                      : false,
-            "enforce_consistency"       : false,
-            "opposite_normals"          : false,
-            "use_initial_configuration" : false
-        }""")
-        this_defaults.AddMissingParameters(super()._GetDefaultParameters())
-        return this_defaults
-
-    # private methods
-    def __CreateEmpireFEMesh(self, model_part, mesh_name):
-        if model_part.NumberOfNodes() < 1:
-            raise Exception('No nodes exist in ModelPart "{}"!'.format(model_part.FullName()))
-
-        num_elements = model_part.NumberOfElements()
-        num_conditions = model_part.NumberOfConditions()
-
-        if num_elements > 0 and num_conditions > 0:
-            err_msg  = "Both Elements and Conditions are present which is not allowed!\n"
-            err_msg += "Name of ModelPart: {}\n".format(model_part.FullName())
-            err_msg += "Number of Elements: {}\n".format(num_elements)
-            err_msg += "Number of Conditions: {}".format(num_elements)
-            raise Exception(err_msg)
-
-        if num_elements + num_conditions == 0:
-            err_msg  = "No Elements and Conditions are present which is not allowed!\n"
-            err_msg += "Name of ModelPart: {}\n".format(model_part.FullName())
-            raise Exception(err_msg)
-
-        if num_conditions > 0:
-            entities_to_use = model_part.Conditions
-        else:
-            entities_to_use = model_part.Elements
-
-        for ent in entities_to_use:
-            if ent.GetGeometry().PointsNumber() not in [3,4]:
-                raise Exception("The EmpireMortarMapper only works with Triangles and Quadrilaterals")
-
-        c_mesh_name = ConvertToChar(mesh_name)
-
-        if EmpireMortarMapper.mapper_lib.hasMesh(c_mesh_name):
-            raise Exception('Mesh "{}" exists already in Empire!'.format(mesh_name))
-
-        c_num_nodes          = ctp.c_int(model_part.NumberOfNodes())
-        c_num_elems          = ctp.c_int(len(entities_to_use))
-        c_node_ids           = (ctp.c_int * c_num_nodes.value) (0)
-        c_node_coords        = (ctp.c_double * (3 * c_num_nodes.value))(0.0)
-        c_num_nodes_per_elem = (ctp.c_int * c_num_elems.value) (0)
-
-        if self.mapper_settings["use_initial_configuration"].GetBool():
-            for i_node, node in enumerate(model_part.Nodes):
-                c_node_ids[i_node] = node.Id
-                c_node_coords[i_node*3]   = node.X0
-                c_node_coords[i_node*3+1] = node.Y0
-                c_node_coords[i_node*3+2] = node.Z0
-
-        else:
-            for i_node, node in enumerate(model_part.Nodes):
-                c_node_ids[i_node] = node.Id
-                c_node_coords[i_node*3]   = node.X
-                c_node_coords[i_node*3+1] = node.Y
-                c_node_coords[i_node*3+2] = node.Z
-
-        elem_node_ctr = 0
-        for elem_ctr, elem in enumerate(entities_to_use):
-            c_num_nodes_per_elem[elem_ctr] = len(elem.GetNodes())
-            elem_node_ctr += c_num_nodes_per_elem[elem_ctr]
-
-        elem_index = 0
-        c_elems = (ctp.c_int * elem_node_ctr) (0)
-        for elem_ctr, elem in enumerate(entities_to_use):
-            for elem_node_ctr, elem_node in enumerate(elem.GetNodes()):
-                c_elems[elem_index + elem_node_ctr] = elem_node.Id
-            elem_index += len(elem.GetNodes())
-
-        triangulateAll = False
-        EmpireMortarMapper.mapper_lib.initFEMesh(c_mesh_name, c_num_nodes, c_num_elems, triangulateAll)
-        EmpireMortarMapper.mapper_lib.setNodesToFEMesh(c_mesh_name, c_node_ids, c_node_coords)
-        EmpireMortarMapper.mapper_lib.setElementsToFEMesh(c_mesh_name, c_num_nodes_per_elem, c_elems)
-
-        if self.echo_level > 1:
-            KM.Logger.PrintInfo('EmpireMortarMapper', 'Printing Mesh "{}"'.format(model_part.FullName()))
-            EmpireMortarMapper.mapper_lib.printMesh(c_mesh_name)
-
-    def __GetInverseMapper(self):
-        if not self.__inverse_mapper:
-            self.__inverse_mapper = self.__class__(self.model_part_destination, self.model_part_origin, self.mapper_settings)
-        return self.__inverse_mapper
-
-    def __CreateMapper(self):
-        dual               = int(self.mapper_settings["dual"].GetBool())
-        enforceConsistency = int(self.mapper_settings["enforce_consistency"].GetBool())
-        opposite_normals   = int(self.mapper_settings["opposite_normals"].GetBool())
-
-        EmpireMortarMapper.mapper_lib.initFEMMortarMapper(
-            ConvertToChar(self.mapper_name),
-            ConvertToChar(self.mesh_name_origin),
-            ConvertToChar(self.mesh_name_destination),
-            ctp.c_int(opposite_normals),
-            ctp.c_int(dual),
-            ctp.c_int(enforceConsistency)
-        )
-
-        self.__CheckMapperExists()
-
-        EmpireMortarMapper.mapper_lib.buildCouplingMatrices(ConvertToChar(self.mapper_name))
-
-    def __CheckMapperExists(self):
-        if not EmpireMortarMapper.mapper_lib.hasMapper(ConvertToChar(self.mapper_name)):
-            raise Exception('Mapper "{}" does not exist!'.format(self.mapper_name))
-
-    def __MapInternalTranspose(self, variable_origin, variable_destination, mapper_flags):
-        self.__CheckMapperExists()
-
-        var_dim = GetVariableDimension(variable_destination)
-
-        origin_data_size = self.model_part_origin.NumberOfNodes()*var_dim
-        destination_data_size = self.model_part_destination.NumberOfNodes()*var_dim
-
-        c_destination_array = KratosFieldToCArray(self.model_part_destination.Nodes, variable_destination)
-        c_origin_array = (ctp.c_double * origin_data_size)(0.0)
-
-        EmpireMortarMapper.mapper_lib.doConservativeMapping(
-            ConvertToChar(self.mapper_name),
-            ctp.c_int(var_dim),
-            ctp.c_int(destination_data_size),
-            c_destination_array,
-            ctp.c_int(origin_data_size),
-            c_origin_array
-            )
-
-        CArrayToKratosField(
-            c_origin_array,
-            origin_data_size,
-            self.model_part_origin.Nodes,
-            variable_origin,
-            mapper_flags.Is(Mapper.ADD_VALUES), mapper_flags.Is(Mapper.SWAP_SIGN))
-
-# Helper functions
-def GetVariableDimension(variable):
-    var_type = KM.KratosGlobals.GetVariableType(variable.Name())
-    if var_type == "Array":
-        return 3
-    elif var_type == "Double":
-        return 1
-    else:
-        raise Exception('Wrong variable type: "{}". Only "Array", "Double" and "Component" are allowed'.format(var_type))
-
-def ConvertToChar(string):
-    return ctp.c_char_p(string.encode(encoding='UTF-8'))
-
-def LoadEmpireMapperLib(path_mapper_lib):
-    KM.Logger.PrintInfo("EmpireMapperLibLoader", "Determining path to mapper lib")
-    # first try automatic detection using the environment that is set by Empire => startEMPIRE
-    if ('EMPIRE_MAPPER_LIBSO_ON_MACHINE' in os.environ):
-        KM.Logger.PrintInfo("EmpireMapperLibLoader", "EMPIRE_MAPPER_LIBSO_ON_MACHINE found in environment")
-        mapper_lib_path = os.environ['EMPIRE_MAPPER_LIBSO_ON_MACHINE']
-
-    else:
-        KM.Logger.PrintInfo("EmpireMapperLibLoader", "EMPIRE_MAPPER_LIBSO_ON_MACHINE NOT found in environment, using manually specified path to load the mapper lib")
-        mapper_lib_path = path_mapper_lib
-        if mapper_lib_path == "":
-            raise Exception('The automatic detection of the mapper lib failed, the path to the mapper lib has to be specified!')
-
-    KM.Logger.PrintInfo("EmpireMapperLibLoader", "Attempting to load the mapper lib")
-    # TODO check if still both are needed! (does the mapperlib link to MPI?)
-    try:
-        try: # OpenMPI
-            loaded_mapper_lib = ctp.CDLL(mapper_lib_path, ctp.RTLD_GLOBAL)
-            KM.Logger.PrintInfo('EmpireMapperLibLoader', 'Using standard OpenMPI')
-        except: # Intel MPI or OpenMPI compiled with "–disable-dlopen" option
-            loaded_mapper_lib = ctp.cdll.LoadLibrary(mapper_lib_path)
-            KM.Logger.PrintInfo('EmpireMapperLibLoader', 'Using Intel MPI or OpenMPI compiled with "–disable-dlopen" option')
-    except OSError:
-        raise Exception("Mapper lib could not be loaded!")
-
-    KM.Logger.PrintInfo("EmpireMapperLibLoader", 'Successfully loaded the mapper lib from "{}"'.format(mapper_lib_path))
-
-    return loaded_mapper_lib
-
-
-def SetSolutionStepValue(node, variable, value):
-    return node.SetSolutionStepValue(variable, 0, value)
-
-def KratosFieldToCArray(nodes, variable):
-    dim = GetVariableDimension(variable)
-    size = dim * len(nodes)
-    c_array = (ctp.c_double * size)(0.0)
-
-    if dim == 1:
-        for i_node, node in enumerate(nodes):
-            c_array[i_node] = node.GetSolutionStepValue(variable)
-    else:
-        for i_node, node in enumerate(nodes):
-            node_value = node.GetSolutionStepValue(variable)
-            for i_dim in range(dim):
-                c_array[i_node*dim + i_dim] = node_value[i_dim]
-
-    return c_array
-
-def CArrayToKratosField(c_array, c_array_size, nodes, variable, add_values, swap_sign):
-    dim = GetVariableDimension(variable)
-    if c_array_size != dim * len(nodes):
-        raise RuntimeError("Wrong size!")
-
-    if swap_sign:
-        for i in range(c_array_size):
-            c_array[i] *= (-1)
-
-    if add_values:
-        current_values = KratosFieldToCArray(nodes, variable)
-        for i in range(c_array_size):
-            c_array[i] += current_values[i]
-
-    if dim == 1:
-        for i_node, node in enumerate(nodes):
-            node.SetSolutionStepValue(variable, 0, c_array[i_node])
-    else:
-        for i_node, node in enumerate(nodes):
-            values = [c_array[i_node*dim], c_array[i_node*dim+1], c_array[i_node*dim+2]]
-            node.SetSolutionStepValue(variable, 0, values)
+# Importing the Kratos Library
+import KratosMultiphysics as KM
+
+# Mapping imports
+from KratosMultiphysics.MappingApplication import Mapper
+from KratosMultiphysics.MappingApplication.python_mapper import PythonMapper
+
+# other imports
+import os
+import ctypes as ctp
+
+def Create(model_part_origin, model_part_destination, mapper_settings):
+    return EmpireMortarMapper(model_part_origin, model_part_destination, mapper_settings)
+
+
+class EmpireMortarMapper(PythonMapper):
+    """Wrapper for the Mortar mapper of EMPIRE
+
+    Usage:
+    Empire needs to be compiled separately
+    It can then be used by either of the two ways:
+    - (default) use "startEMPIRE" to bring "EMPIRE_MAPPER_LIBSO_ON_MACHINE" to the environment
+    - use "path_mapper_lib" to sprecify the path to "libEMPIRE_MapperLib.so" (by default located in "EMPIRE-Core/lib/")
+    """
+
+    mapper_count = 0
+    instances = 0
+    mapper_lib = None
+
+    def __init__(self, model_part_origin, model_part_destination, mapper_settings):
+        super().__init__(model_part_origin, model_part_destination, mapper_settings)
+
+        if model_part_origin.IsDistributed() or model_part_destination.IsDistributed():
+            raise Exception('{} does not support mapping with distributed ModelParts!'.format(self._ClassName()))
+
+        if EmpireMortarMapper.mapper_lib:
+            KM.Logger.PrintInfo("EmpireMortarMapper", "Mapper lib is already loaded")
+        else:
+            KM.Logger.PrintInfo("EmpireMortarMapper", "Attempting to load mapper lib")
+            EmpireMortarMapper.mapper_lib = LoadEmpireMapperLib(self.mapper_settings["path_mapper_lib"].GetString())
+
+        self.mapper_name = "EmpireMortarMapper_"+str(EmpireMortarMapper.mapper_count)
+
+        self.mesh_name_origin = model_part_origin.FullName()+"_o_"+str(EmpireMortarMapper.mapper_count)
+        self.mesh_name_destination = model_part_destination.FullName()+"_d_"+str(EmpireMortarMapper.mapper_count)
+
+        self.__CreateEmpireFEMesh(self.model_part_origin, self.mesh_name_origin)
+        self.__CreateEmpireFEMesh(self.model_part_destination, self.mesh_name_destination)
+
+        self.__CreateMapper()
+
+        EmpireMortarMapper.mapper_count += 1 # required for identification purposes
+        EmpireMortarMapper.instances += 1
+        self.__inverse_mapper = None
+
+    def __del__(self):
+        if EmpireMortarMapper.mapper_lib.hasMapper(ConvertToChar(self.mapper_name)):
+            EmpireMortarMapper.mapper_lib.deleteMapper(ConvertToChar(self.mapper_name))
+
+        if EmpireMortarMapper.mapper_lib.hasMesh(ConvertToChar(self.mesh_name_origin)):
+            EmpireMortarMapper.mapper_lib.deleteMesh(ConvertToChar(self.mesh_name_origin))
+        if EmpireMortarMapper.mapper_lib.hasMesh(ConvertToChar(self.mesh_name_destination)):
+            EmpireMortarMapper.mapper_lib.deleteMesh(ConvertToChar(self.mesh_name_destination))
+
+        EmpireMortarMapper.instances -= 1
+        if EmpireMortarMapper.instances == 0: # last mapper was destoyed
+            if self.echo_level > 1:
+                KM.Logger.PrintInfo('EmpireMortarMapper', 'Destroying last instance, deleting all meshes & mappers')
+            #  delete everything to make sure nothing is left
+            EmpireMortarMapper.mapper_lib.deleteAllMappers()
+            EmpireMortarMapper.mapper_lib.deleteAllMeshes()
+
+    def UpdateInterface(self):
+        raise NotImplementedError('"UpdateInterface" is not yet implemented for "{}"!'.format(self._ClassName()))
+
+    # protected methods
+    def _MapInternal(self, variable_origin, variable_destination, mapper_flags):
+        if mapper_flags.Is(Mapper.USE_TRANSPOSE):
+            mapper_flags.Reset(Mapper.USE_TRANSPOSE)
+            mapper_flags.Set(KM.VISITED, True)
+            self.__GetInverseMapper().Map(variable_destination, variable_origin, mapper_flags)
+            return
+        elif mapper_flags.Is(KM.VISITED):
+            self.__MapInternalTranspose(variable_origin, variable_destination, mapper_flags)
+            return
+
+        self.__CheckMapperExists()
+
+        var_dim = GetVariableDimension(variable_origin)
+
+        origin_data_size = self.model_part_origin.NumberOfNodes()*var_dim
+        destination_data_size = self.model_part_destination.NumberOfNodes()*var_dim
+
+        c_origin_array = KratosFieldToCArray(self.model_part_origin.Nodes, variable_origin)
+        c_destination_array = (ctp.c_double * destination_data_size)(0.0)
+
+        EmpireMortarMapper.mapper_lib.doConsistentMapping(
+            ConvertToChar(self.mapper_name),
+            ctp.c_int(var_dim),
+            ctp.c_int(origin_data_size),
+            c_origin_array,
+            ctp.c_int(destination_data_size),
+            c_destination_array
+            )
+
+        CArrayToKratosField(
+            c_destination_array,
+            destination_data_size,
+            self.model_part_destination.Nodes,
+            variable_destination,
+            mapper_flags.Is(Mapper.ADD_VALUES), mapper_flags.Is(Mapper.SWAP_SIGN))
+
+    def _InverseMapInternal(self, variable_origin, variable_destination, mapper_flags):
+        if mapper_flags.Is(Mapper.USE_TRANSPOSE):
+            self.__MapInternalTranspose(variable_origin, variable_destination, mapper_flags)
+        else:
+            self.__GetInverseMapper().Map(variable_destination, variable_origin, mapper_flags)
+
+    @classmethod
+    def _GetDefaultParameters(cls):
+        this_defaults = KM.Parameters("""{
+            "path_mapper_lib"           : "",
+            "dual"                      : false,
+            "enforce_consistency"       : false,
+            "opposite_normals"          : false,
+            "use_initial_configuration" : false
+        }""")
+        this_defaults.AddMissingParameters(super()._GetDefaultParameters())
+        return this_defaults
+
+    # private methods
+    def __CreateEmpireFEMesh(self, model_part, mesh_name):
+        if model_part.NumberOfNodes() < 1:
+            raise Exception('No nodes exist in ModelPart "{}"!'.format(model_part.FullName()))
+
+        num_elements = model_part.NumberOfElements()
+        num_conditions = model_part.NumberOfConditions()
+
+        if num_elements > 0 and num_conditions > 0:
+            err_msg  = "Both Elements and Conditions are present which is not allowed!\n"
+            err_msg += "Name of ModelPart: {}\n".format(model_part.FullName())
+            err_msg += "Number of Elements: {}\n".format(num_elements)
+            err_msg += "Number of Conditions: {}".format(num_elements)
+            raise Exception(err_msg)
+
+        if num_elements + num_conditions == 0:
+            err_msg  = "No Elements and Conditions are present which is not allowed!\n"
+            err_msg += "Name of ModelPart: {}\n".format(model_part.FullName())
+            raise Exception(err_msg)
+
+        if num_conditions > 0:
+            entities_to_use = model_part.Conditions
+        else:
+            entities_to_use = model_part.Elements
+
+        for ent in entities_to_use:
+            if ent.GetGeometry().PointsNumber() not in [3,4]:
+                raise Exception("The EmpireMortarMapper only works with Triangles and Quadrilaterals")
+
+        c_mesh_name = ConvertToChar(mesh_name)
+
+        if EmpireMortarMapper.mapper_lib.hasMesh(c_mesh_name):
+            raise Exception('Mesh "{}" exists already in Empire!'.format(mesh_name))
+
+        c_num_nodes          = ctp.c_int(model_part.NumberOfNodes())
+        c_num_elems          = ctp.c_int(len(entities_to_use))
+        c_node_ids           = (ctp.c_int * c_num_nodes.value) (0)
+        c_node_coords        = (ctp.c_double * (3 * c_num_nodes.value))(0.0)
+        c_num_nodes_per_elem = (ctp.c_int * c_num_elems.value) (0)
+
+        if self.mapper_settings["use_initial_configuration"].GetBool():
+            for i_node, node in enumerate(model_part.Nodes):
+                c_node_ids[i_node] = node.Id
+                c_node_coords[i_node*3]   = node.X0
+                c_node_coords[i_node*3+1] = node.Y0
+                c_node_coords[i_node*3+2] = node.Z0
+
+        else:
+            for i_node, node in enumerate(model_part.Nodes):
+                c_node_ids[i_node] = node.Id
+                c_node_coords[i_node*3]   = node.X
+                c_node_coords[i_node*3+1] = node.Y
+                c_node_coords[i_node*3+2] = node.Z
+
+        elem_node_ctr = 0
+        for elem_ctr, elem in enumerate(entities_to_use):
+            c_num_nodes_per_elem[elem_ctr] = len(elem.GetNodes())
+            elem_node_ctr += c_num_nodes_per_elem[elem_ctr]
+
+        elem_index = 0
+        c_elems = (ctp.c_int * elem_node_ctr) (0)
+        for elem_ctr, elem in enumerate(entities_to_use):
+            for elem_node_ctr, elem_node in enumerate(elem.GetNodes()):
+                c_elems[elem_index + elem_node_ctr] = elem_node.Id
+            elem_index += len(elem.GetNodes())
+
+        triangulateAll = False
+        EmpireMortarMapper.mapper_lib.initFEMesh(c_mesh_name, c_num_nodes, c_num_elems, triangulateAll)
+        EmpireMortarMapper.mapper_lib.setNodesToFEMesh(c_mesh_name, c_node_ids, c_node_coords)
+        EmpireMortarMapper.mapper_lib.setElementsToFEMesh(c_mesh_name, c_num_nodes_per_elem, c_elems)
+
+        if self.echo_level > 1:
+            KM.Logger.PrintInfo('EmpireMortarMapper', 'Printing Mesh "{}"'.format(model_part.FullName()))
+            EmpireMortarMapper.mapper_lib.printMesh(c_mesh_name)
+
+    def __GetInverseMapper(self):
+        if not self.__inverse_mapper:
+            self.__inverse_mapper = self.__class__(self.model_part_destination, self.model_part_origin, self.mapper_settings)
+        return self.__inverse_mapper
+
+    def __CreateMapper(self):
+        dual               = int(self.mapper_settings["dual"].GetBool())
+        enforceConsistency = int(self.mapper_settings["enforce_consistency"].GetBool())
+        opposite_normals   = int(self.mapper_settings["opposite_normals"].GetBool())
+
+        EmpireMortarMapper.mapper_lib.initFEMMortarMapper(
+            ConvertToChar(self.mapper_name),
+            ConvertToChar(self.mesh_name_origin),
+            ConvertToChar(self.mesh_name_destination),
+            ctp.c_int(opposite_normals),
+            ctp.c_int(dual),
+            ctp.c_int(enforceConsistency)
+        )
+
+        self.__CheckMapperExists()
+
+        EmpireMortarMapper.mapper_lib.buildCouplingMatrices(ConvertToChar(self.mapper_name))
+
+    def __CheckMapperExists(self):
+        if not EmpireMortarMapper.mapper_lib.hasMapper(ConvertToChar(self.mapper_name)):
+            raise Exception('Mapper "{}" does not exist!'.format(self.mapper_name))
+
+    def __MapInternalTranspose(self, variable_origin, variable_destination, mapper_flags):
+        self.__CheckMapperExists()
+
+        var_dim = GetVariableDimension(variable_destination)
+
+        origin_data_size = self.model_part_origin.NumberOfNodes()*var_dim
+        destination_data_size = self.model_part_destination.NumberOfNodes()*var_dim
+
+        c_destination_array = KratosFieldToCArray(self.model_part_destination.Nodes, variable_destination)
+        c_origin_array = (ctp.c_double * origin_data_size)(0.0)
+
+        EmpireMortarMapper.mapper_lib.doConservativeMapping(
+            ConvertToChar(self.mapper_name),
+            ctp.c_int(var_dim),
+            ctp.c_int(destination_data_size),
+            c_destination_array,
+            ctp.c_int(origin_data_size),
+            c_origin_array
+            )
+
+        CArrayToKratosField(
+            c_origin_array,
+            origin_data_size,
+            self.model_part_origin.Nodes,
+            variable_origin,
+            mapper_flags.Is(Mapper.ADD_VALUES), mapper_flags.Is(Mapper.SWAP_SIGN))
+
+# Helper functions
+def GetVariableDimension(variable):
+    var_type = KM.KratosGlobals.GetVariableType(variable.Name())
+    if var_type == "Array":
+        return 3
+    elif var_type == "Double":
+        return 1
+    else:
+        raise Exception('Wrong variable type: "{}". Only "Array", "Double" and "Component" are allowed'.format(var_type))
+
+def ConvertToChar(string):
+    return ctp.c_char_p(string.encode(encoding='UTF-8'))
+
+def LoadEmpireMapperLib(path_mapper_lib):
+    KM.Logger.PrintInfo("EmpireMapperLibLoader", "Determining path to mapper lib")
+    # first try automatic detection using the environment that is set by Empire => startEMPIRE
+    if ('EMPIRE_MAPPER_LIBSO_ON_MACHINE' in os.environ):
+        KM.Logger.PrintInfo("EmpireMapperLibLoader", "EMPIRE_MAPPER_LIBSO_ON_MACHINE found in environment")
+        mapper_lib_path = os.environ['EMPIRE_MAPPER_LIBSO_ON_MACHINE']
+
+    else:
+        KM.Logger.PrintInfo("EmpireMapperLibLoader", "EMPIRE_MAPPER_LIBSO_ON_MACHINE NOT found in environment, using manually specified path to load the mapper lib")
+        mapper_lib_path = path_mapper_lib
+        if mapper_lib_path == "":
+            raise Exception('The automatic detection of the mapper lib failed, the path to the mapper lib has to be specified!')
+
+    KM.Logger.PrintInfo("EmpireMapperLibLoader", "Attempting to load the mapper lib")
+    # TODO check if still both are needed! (does the mapperlib link to MPI?)
+    try:
+        try: # OpenMPI
+            loaded_mapper_lib = ctp.CDLL(mapper_lib_path, ctp.RTLD_GLOBAL)
+            KM.Logger.PrintInfo('EmpireMapperLibLoader', 'Using standard OpenMPI')
+        except: # Intel MPI or OpenMPI compiled with "–disable-dlopen" option
+            loaded_mapper_lib = ctp.cdll.LoadLibrary(mapper_lib_path)
+            KM.Logger.PrintInfo('EmpireMapperLibLoader', 'Using Intel MPI or OpenMPI compiled with "–disable-dlopen" option')
+    except OSError:
+        raise Exception("Mapper lib could not be loaded!")
+
+    KM.Logger.PrintInfo("EmpireMapperLibLoader", 'Successfully loaded the mapper lib from "{}"'.format(mapper_lib_path))
+
+    return loaded_mapper_lib
+
+
+def SetSolutionStepValue(node, variable, value):
+    return node.SetSolutionStepValue(variable, 0, value)
+
+def KratosFieldToCArray(nodes, variable):
+    dim = GetVariableDimension(variable)
+    size = dim * len(nodes)
+    c_array = (ctp.c_double * size)(0.0)
+
+    if dim == 1:
+        for i_node, node in enumerate(nodes):
+            c_array[i_node] = node.GetSolutionStepValue(variable)
+    else:
+        for i_node, node in enumerate(nodes):
+            node_value = node.GetSolutionStepValue(variable)
+            for i_dim in range(dim):
+                c_array[i_node*dim + i_dim] = node_value[i_dim]
+
+    return c_array
+
+def CArrayToKratosField(c_array, c_array_size, nodes, variable, add_values, swap_sign):
+    dim = GetVariableDimension(variable)
+    if c_array_size != dim * len(nodes):
+        raise RuntimeError("Wrong size!")
+
+    if swap_sign:
+        for i in range(c_array_size):
+            c_array[i] *= (-1)
+
+    if add_values:
+        current_values = KratosFieldToCArray(nodes, variable)
+        for i in range(c_array_size):
+            c_array[i] += current_values[i]
+
+    if dim == 1:
+        for i_node, node in enumerate(nodes):
+            node.SetSolutionStepValue(variable, 0, c_array[i_node])
+    else:
+        for i_node, node in enumerate(nodes):
+            values = [c_array[i_node*dim], c_array[i_node*dim+1], c_array[i_node*dim+2]]
+            node.SetSolutionStepValue(variable, 0, values)
```

## KratosMultiphysics/MappingApplication/python_mapper.py

 * *Ordering differences only*

```diff
@@ -1,55 +1,55 @@
-# Importing the Kratos Library
-import KratosMultiphysics as KM
-
-# Other imports
-from abc import ABCMeta, abstractmethod
-
-class PythonMapper(metaclass=ABCMeta):
-    """Baseclass for python based mappers in Kratos
-    The inteface matches the C++ version ("custom_mappers/mapper.h")
-    The py-mappers are intentionally NOT derived from the c++ version.
-    Reasons:
-    - Doing so would require some special treatment of the pure virtual functions exposed to python
-    - They are more or less temporary until Kratos has more Mappers
-    """
-    def __init__(self, model_part_origin, model_part_destination, mapper_settings):
-        self.model_part_origin = model_part_origin
-        self.model_part_destination = model_part_destination
-
-        self.mapper_settings = mapper_settings
-        self.mapper_settings.ValidateAndAssignDefaults(self._GetDefaultParameters())
-
-        self.echo_level = self.mapper_settings["echo_level"].GetInt()
-
-    # public methods, same as in "custom_mappers/mapper.h"
-    def Map(self, variable_origin, variable_destination, mapper_flags=KM.Flags()):
-        CheckVariables(variable_origin, variable_destination)
-        self._MapInternal(variable_origin, variable_destination, mapper_flags)
-
-    def InverseMap(self, variable_origin, variable_destination, mapper_flags=KM.Flags()):
-        CheckVariables(variable_origin, variable_destination)
-        self._InverseMapInternal(variable_origin, variable_destination, mapper_flags)
-
-    @abstractmethod
-    def UpdateInterface(self): pass
-
-    # protected methods
-    @abstractmethod
-    def _MapInternal(self, variable_origin, variable_destination, mapper_flags): pass
-
-    @abstractmethod
-    def _InverseMapInternal(self, variable_origin, variable_destination, mapper_flags): pass
-
-    @classmethod
-    def _GetDefaultParameters(cls):
-        return KM.Parameters("""{
-            "mapper_type" : "",
-            "echo_level"  : 0
-        }""")
-
-    @classmethod
-    def _ClassName(cls):
-        return cls.__name__
-
-def CheckVariables(variable_origin, variable_destination):
+# Importing the Kratos Library
+import KratosMultiphysics as KM
+
+# Other imports
+from abc import ABCMeta, abstractmethod
+
+class PythonMapper(metaclass=ABCMeta):
+    """Baseclass for python based mappers in Kratos
+    The inteface matches the C++ version ("custom_mappers/mapper.h")
+    The py-mappers are intentionally NOT derived from the c++ version.
+    Reasons:
+    - Doing so would require some special treatment of the pure virtual functions exposed to python
+    - They are more or less temporary until Kratos has more Mappers
+    """
+    def __init__(self, model_part_origin, model_part_destination, mapper_settings):
+        self.model_part_origin = model_part_origin
+        self.model_part_destination = model_part_destination
+
+        self.mapper_settings = mapper_settings
+        self.mapper_settings.ValidateAndAssignDefaults(self._GetDefaultParameters())
+
+        self.echo_level = self.mapper_settings["echo_level"].GetInt()
+
+    # public methods, same as in "custom_mappers/mapper.h"
+    def Map(self, variable_origin, variable_destination, mapper_flags=KM.Flags()):
+        CheckVariables(variable_origin, variable_destination)
+        self._MapInternal(variable_origin, variable_destination, mapper_flags)
+
+    def InverseMap(self, variable_origin, variable_destination, mapper_flags=KM.Flags()):
+        CheckVariables(variable_origin, variable_destination)
+        self._InverseMapInternal(variable_origin, variable_destination, mapper_flags)
+
+    @abstractmethod
+    def UpdateInterface(self): pass
+
+    # protected methods
+    @abstractmethod
+    def _MapInternal(self, variable_origin, variable_destination, mapper_flags): pass
+
+    @abstractmethod
+    def _InverseMapInternal(self, variable_origin, variable_destination, mapper_flags): pass
+
+    @classmethod
+    def _GetDefaultParameters(cls):
+        return KM.Parameters("""{
+            "mapper_type" : "",
+            "echo_level"  : 0
+        }""")
+
+    @classmethod
+    def _ClassName(cls):
+        return cls.__name__
+
+def CheckVariables(variable_origin, variable_destination):
     pass
```

## KratosMultiphysics/MappingApplication/python_mapper_factory.py

 * *Ordering differences only*

```diff
@@ -1,39 +1,39 @@
-# Python factory for all the currently available Mappers in Kratos
-# The intention is to give the users a unique place to create Mappers
-# The goal is to implement the Mappers from the other Apps also in the
-# MappingApp (which inherently also work in MPI) and replace them in
-# the long run.
-# This way users won't notice / won't have to change their code
-
-import KratosMultiphysics as KM
-
-from importlib import import_module
-
-def _InternalCreateMapper(mapper_factory, err_info, model_part_origin, model_part_destination, mapper_settings):
-    if not isinstance(mapper_settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-
-    mapper_type = mapper_settings["mapper_type"].GetString()
-
-    # use the MappingApp if it has the requested mapper
-    if mapper_factory.HasMapper(mapper_type):
-        return mapper_factory.CreateMapper(model_part_origin, model_part_destination, mapper_settings)
-    else:
-        mapper_module = import_module(mapper_type)
-        return mapper_module.Create(model_part_origin, model_part_destination, mapper_settings)
-
-    list_avail_mappers = mapper_factory.GetRegisteredMapperNames()
-
-    err_msg  = 'The requested mapper "{}" is not available in {}\n'.format(mapper_type, err_info)
-    err_msg += 'The following mappers are available:'
-    for avail_mapper in list_avail_mappers:
-        err_msg += '\n\t{}'.format(avail_mapper)
-    raise Exception(err_msg)
-
-
-def CreateMapper(model_part_origin, model_part_destination, mapper_settings):
-    return _InternalCreateMapper(KM.MapperFactory, "serial (non-MPI)", model_part_origin, model_part_destination, mapper_settings)
-
-def CreateMPIMapper(model_part_origin, model_part_destination, mapper_settings):
-    from KratosMultiphysics.MappingApplication.MPIExtension import MPIMapperFactory
-    return _InternalCreateMapper(MPIMapperFactory, "MPI", model_part_origin, model_part_destination, mapper_settings)
+# Python factory for all the currently available Mappers in Kratos
+# The intention is to give the users a unique place to create Mappers
+# The goal is to implement the Mappers from the other Apps also in the
+# MappingApp (which inherently also work in MPI) and replace them in
+# the long run.
+# This way users won't notice / won't have to change their code
+
+import KratosMultiphysics as KM
+
+from importlib import import_module
+
+def _InternalCreateMapper(mapper_factory, err_info, model_part_origin, model_part_destination, mapper_settings):
+    if not isinstance(mapper_settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+
+    mapper_type = mapper_settings["mapper_type"].GetString()
+
+    # use the MappingApp if it has the requested mapper
+    if mapper_factory.HasMapper(mapper_type):
+        return mapper_factory.CreateMapper(model_part_origin, model_part_destination, mapper_settings)
+    else:
+        mapper_module = import_module(mapper_type)
+        return mapper_module.Create(model_part_origin, model_part_destination, mapper_settings)
+
+    list_avail_mappers = mapper_factory.GetRegisteredMapperNames()
+
+    err_msg  = 'The requested mapper "{}" is not available in {}\n'.format(mapper_type, err_info)
+    err_msg += 'The following mappers are available:'
+    for avail_mapper in list_avail_mappers:
+        err_msg += '\n\t{}'.format(avail_mapper)
+    raise Exception(err_msg)
+
+
+def CreateMapper(model_part_origin, model_part_destination, mapper_settings):
+    return _InternalCreateMapper(KM.MapperFactory, "serial (non-MPI)", model_part_origin, model_part_destination, mapper_settings)
+
+def CreateMPIMapper(model_part_origin, model_part_destination, mapper_settings):
+    from KratosMultiphysics.MappingApplication.MPIExtension import MPIMapperFactory
+    return _InternalCreateMapper(MPIMapperFactory, "MPI", model_part_origin, model_part_destination, mapper_settings)
```

## KratosMultiphysics/MappingApplication/serial_output_process.py

 * *Ordering differences only*

```diff
@@ -1,143 +1,143 @@
-import KratosMultiphysics as KM
-from KratosMultiphysics import MappingApplication # registering the mappers
-from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
-from KratosMultiphysics.process_factory import KratosProcessFactory
-
-def Factory(settings, model):
-    if not isinstance(settings, KM.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return SerialOutputProcess(model, settings["Parameters"])
-
-
-class SerialOutputProcess(KM.OutputProcess):
-    """This process is used in distributed simulations to do post-processing on one rank
-    For this first the results are mapped to a serial ModelPart, with which then postprocessing is done
-    This is not the most efficient approach by principle, but sometimes it is necessary to collect
-    all the results on one rank
-    """
-    def __init__(self, model, settings):
-        super().__init__()
-
-        self.settings = settings
-
-        default_settings = KM.Parameters('''{
-            "main_model_part_name_origin"      : "UNSPECIFIED",
-            "main_model_part_name_destination" : "UNSPECIFIED",
-            "mdpa_file_name_destination"  : "",
-            "historical_variables_destination" : [],
-            "destination_rank" : 0,
-            "mapper_settings" :  {},
-            "mapping_settings" : [],
-            "output_process_settings" : {}
-        }''')
-
-        settings.ValidateAndAssignDefaults(default_settings)
-
-        if len(settings["mapper_settings"].keys()) == 0:
-            raise Exception('no "mapper_settings" were specified!')
-
-        if settings["mapping_settings"].size() == 0:
-            raise Exception('no "mapping_settings" were specified!')
-
-        mdpa_file_name_destination = settings["mdpa_file_name_destination"].GetString()
-
-        model_part_origin = model.GetModelPart(settings["main_model_part_name_origin"].GetString())
-        if model_part_origin.IsSubModelPart():
-            raise Exception('Origin ModelPart cannot be a SubModelPart!')
-
-        self.model_part_destination = model.CreateModelPart(settings["main_model_part_name_destination"].GetString())
-        if self.model_part_destination.IsSubModelPart():
-            raise Exception('Destination ModelPart cannot be a SubModelPart!')
-
-        self.model_part_destination.ProcessInfo = model_part_origin.ProcessInfo # for detecting output writing
-
-        for var in GenerateVariableListFromInput(settings["historical_variables_destination"]):
-            self.model_part_destination.AddNodalSolutionStepVariable(var)
-
-        self.data_comm = model_part_origin.GetCommunicator().GetDataCommunicator()
-
-        self.destination_rank = settings["destination_rank"].GetInt()
-        if self.destination_rank >= self.data_comm.Size():
-            raise Exception("Destination rank %i larger than available size %i" %(self.destination_rank, self.data_comm.Size()))
-
-        # optionally read mdpa (only on one rank)
-        if mdpa_file_name_destination != "":
-            if self.data_comm.Rank() == self.destination_rank:
-                import_flags = KM.ModelPartIO.READ | KM.ModelPartIO.SKIP_TIMER
-                KM.ModelPartIO(mdpa_file_name_destination, import_flags).ReadModelPart(self.model_part_destination)
-
-            # properly initialize in MPI (on other ranks)
-            if model_part_origin.IsDistributed():
-                import KratosMultiphysics.mpi as KratosMPI
-
-                # initialize SubModelPartStructure on other ranks
-                KratosMPI.DistributedModelPartInitializer(self.model_part_destination, self.data_comm, self.destination_rank).CopySubModelPartStructure()
-
-                data_comm_destination = KratosMPI.DataCommunicatorFactory.CreateFromRanksAndRegister(
-                    self.data_comm,
-                    [self.destination_rank],
-                    "destination_mapping")
-
-                if self.data_comm.Rank() != self.destination_rank:
-                    KratosMPI.ModelPartCommunicatorUtilities.SetMPICommunicatorRecursively(self.model_part_destination, data_comm_destination)
-
-        # optionally create output process (only on one rank)
-        self.output_process = None
-        if len(settings["output_process_settings"].keys()) > 0 and self.data_comm.Rank() == self.destination_rank:
-            output_proc_params = KM.Parameters('''{ "dummy" : [] }''')
-            output_proc_params["dummy"].Append(settings["output_process_settings"])
-            self.output_process = KratosProcessFactory(model).ConstructListOfProcesses(output_proc_params["dummy"])[0]
-
-        # create mapper
-        if model_part_origin.IsDistributed():
-            from KratosMultiphysics.MappingApplication.MPIExtension import MPIMapperFactory
-
-            self.mapper = MPIMapperFactory.CreateMapper(
-                model_part_origin,
-                self.model_part_destination,
-                settings["mapper_settings"])
-        else:
-            self.mapper = KM.MapperFactory.CreateMapper(
-                model_part_origin,
-                self.model_part_destination,
-                settings["mapper_settings"])
-
-    def ExecuteFinalizeSolutionStep(self):
-        defaults = KM.Parameters('''{
-            "variable_origin"      : "UNSPECIFIED",
-            "variable_destination" : "UNSPECIFIED",
-            "mapping_options" : []
-        }''')
-
-        for mapping_params in self.settings["mapping_settings"]:
-            mapping_params.ValidateAndAssignDefaults(defaults)
-
-            variable_origin = KM.KratosGlobals.GetVariable(mapping_params["variable_origin"].GetString())
-            variable_destination = KM.KratosGlobals.GetVariable(mapping_params["variable_destination"].GetString())
-            mapper_flags = GetMapperFlags(mapping_params["mapping_options"])
-
-            self.mapper.Map(variable_origin, variable_destination, mapper_flags)
-
-    def IsOutputStep(self):
-        is_output_step = False
-        if self.data_comm.Rank() == self.destination_rank:
-            if self.output_process:
-                is_output_step = self.output_process.IsOutputStep()
-        return bool(self.data_comm.Broadcast(int(is_output_step), self.destination_rank))
-
-    def PrintOutput(self):
-        if self.data_comm.Rank() == self.destination_rank and self.output_process:
-            self.output_process.PrintOutput()
-
-
-def GetMapperFlags(settings):
-    mapper_flags_dict = {
-        "add_values"    : KM.Mapper.ADD_VALUES,
-        "swap_sign"     : KM.Mapper.SWAP_SIGN,
-        "use_transpose" : KM.Mapper.USE_TRANSPOSE
-    }
-    mapper_flags = KM.Flags()
-    for flag_name in settings.GetStringArray():
-        mapper_flags |= mapper_flags_dict[flag_name]
-
-    return mapper_flags
+import KratosMultiphysics as KM
+from KratosMultiphysics import MappingApplication # registering the mappers
+from KratosMultiphysics.kratos_utilities import GenerateVariableListFromInput
+from KratosMultiphysics.process_factory import KratosProcessFactory
+
+def Factory(settings, model):
+    if not isinstance(settings, KM.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return SerialOutputProcess(model, settings["Parameters"])
+
+
+class SerialOutputProcess(KM.OutputProcess):
+    """This process is used in distributed simulations to do post-processing on one rank
+    For this first the results are mapped to a serial ModelPart, with which then postprocessing is done
+    This is not the most efficient approach by principle, but sometimes it is necessary to collect
+    all the results on one rank
+    """
+    def __init__(self, model, settings):
+        super().__init__()
+
+        self.settings = settings
+
+        default_settings = KM.Parameters('''{
+            "main_model_part_name_origin"      : "UNSPECIFIED",
+            "main_model_part_name_destination" : "UNSPECIFIED",
+            "mdpa_file_name_destination"  : "",
+            "historical_variables_destination" : [],
+            "destination_rank" : 0,
+            "mapper_settings" :  {},
+            "mapping_settings" : [],
+            "output_process_settings" : {}
+        }''')
+
+        settings.ValidateAndAssignDefaults(default_settings)
+
+        if len(settings["mapper_settings"].keys()) == 0:
+            raise Exception('no "mapper_settings" were specified!')
+
+        if settings["mapping_settings"].size() == 0:
+            raise Exception('no "mapping_settings" were specified!')
+
+        mdpa_file_name_destination = settings["mdpa_file_name_destination"].GetString()
+
+        model_part_origin = model.GetModelPart(settings["main_model_part_name_origin"].GetString())
+        if model_part_origin.IsSubModelPart():
+            raise Exception('Origin ModelPart cannot be a SubModelPart!')
+
+        self.model_part_destination = model.CreateModelPart(settings["main_model_part_name_destination"].GetString())
+        if self.model_part_destination.IsSubModelPart():
+            raise Exception('Destination ModelPart cannot be a SubModelPart!')
+
+        self.model_part_destination.ProcessInfo = model_part_origin.ProcessInfo # for detecting output writing
+
+        for var in GenerateVariableListFromInput(settings["historical_variables_destination"]):
+            self.model_part_destination.AddNodalSolutionStepVariable(var)
+
+        self.data_comm = model_part_origin.GetCommunicator().GetDataCommunicator()
+
+        self.destination_rank = settings["destination_rank"].GetInt()
+        if self.destination_rank >= self.data_comm.Size():
+            raise Exception("Destination rank %i larger than available size %i" %(self.destination_rank, self.data_comm.Size()))
+
+        # optionally read mdpa (only on one rank)
+        if mdpa_file_name_destination != "":
+            if self.data_comm.Rank() == self.destination_rank:
+                import_flags = KM.ModelPartIO.READ | KM.ModelPartIO.SKIP_TIMER
+                KM.ModelPartIO(mdpa_file_name_destination, import_flags).ReadModelPart(self.model_part_destination)
+
+            # properly initialize in MPI (on other ranks)
+            if model_part_origin.IsDistributed():
+                import KratosMultiphysics.mpi as KratosMPI
+
+                # initialize SubModelPartStructure on other ranks
+                KratosMPI.DistributedModelPartInitializer(self.model_part_destination, self.data_comm, self.destination_rank).CopySubModelPartStructure()
+
+                data_comm_destination = KratosMPI.DataCommunicatorFactory.CreateFromRanksAndRegister(
+                    self.data_comm,
+                    [self.destination_rank],
+                    "destination_mapping")
+
+                if self.data_comm.Rank() != self.destination_rank:
+                    KratosMPI.ModelPartCommunicatorUtilities.SetMPICommunicatorRecursively(self.model_part_destination, data_comm_destination)
+
+        # optionally create output process (only on one rank)
+        self.output_process = None
+        if len(settings["output_process_settings"].keys()) > 0 and self.data_comm.Rank() == self.destination_rank:
+            output_proc_params = KM.Parameters('''{ "dummy" : [] }''')
+            output_proc_params["dummy"].Append(settings["output_process_settings"])
+            self.output_process = KratosProcessFactory(model).ConstructListOfProcesses(output_proc_params["dummy"])[0]
+
+        # create mapper
+        if model_part_origin.IsDistributed():
+            from KratosMultiphysics.MappingApplication.MPIExtension import MPIMapperFactory
+
+            self.mapper = MPIMapperFactory.CreateMapper(
+                model_part_origin,
+                self.model_part_destination,
+                settings["mapper_settings"])
+        else:
+            self.mapper = KM.MapperFactory.CreateMapper(
+                model_part_origin,
+                self.model_part_destination,
+                settings["mapper_settings"])
+
+    def ExecuteFinalizeSolutionStep(self):
+        defaults = KM.Parameters('''{
+            "variable_origin"      : "UNSPECIFIED",
+            "variable_destination" : "UNSPECIFIED",
+            "mapping_options" : []
+        }''')
+
+        for mapping_params in self.settings["mapping_settings"]:
+            mapping_params.ValidateAndAssignDefaults(defaults)
+
+            variable_origin = KM.KratosGlobals.GetVariable(mapping_params["variable_origin"].GetString())
+            variable_destination = KM.KratosGlobals.GetVariable(mapping_params["variable_destination"].GetString())
+            mapper_flags = GetMapperFlags(mapping_params["mapping_options"])
+
+            self.mapper.Map(variable_origin, variable_destination, mapper_flags)
+
+    def IsOutputStep(self):
+        is_output_step = False
+        if self.data_comm.Rank() == self.destination_rank:
+            if self.output_process:
+                is_output_step = self.output_process.IsOutputStep()
+        return bool(self.data_comm.Broadcast(int(is_output_step), self.destination_rank))
+
+    def PrintOutput(self):
+        if self.data_comm.Rank() == self.destination_rank and self.output_process:
+            self.output_process.PrintOutput()
+
+
+def GetMapperFlags(settings):
+    mapper_flags_dict = {
+        "add_values"    : KM.Mapper.ADD_VALUES,
+        "swap_sign"     : KM.Mapper.SWAP_SIGN,
+        "use_transpose" : KM.Mapper.USE_TRANSPOSE
+    }
+    mapper_flags = KM.Flags()
+    for flag_name in settings.GetStringArray():
+        mapper_flags |= mapper_flags_dict[flag_name]
+
+    return mapper_flags
```

## Comparing `KratosMappingApplication-9.4.6.dist-info/METADATA` & `KratosMappingApplication-9.5.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,420 +1,420 @@
-Metadata-Version: 2.1
-Name: KratosMappingApplication
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
-## Mapping Application
-
-The Mapping Application contains the core developments in mapping data between non matching grids. It works both in shared and distributed (**MPI**) memory environments as well as in 1D, 2D and 3D domains.
-
-### Overview
-
-- [List of features](#list-of-features)
-- [Dependencies](#dependencies)
-- [Mapping in CoSimulation](#Mapping-in-CoSimulation)
-- [Basic Usage](#basic-usage)
-- [Advanced Usage](#advanced-usage)
-- [Available Mappers](#available-mappers)
-- [When to use which Mapper?](#when-to-use-which-mapper)
-- [Using the Mapper for ModelParts that are not part of all ranks](#using-the-mapper-for-modelparts-that-are-not-part-of-all-ranks)
-- [Miscellaneous functionalities](#miscellaneous-functionalities)
-- [FAQ](#faq)
-
-### List of features
-
-- Parallelism:
-  - Serial (no parallelism)
-  - Shared memory (OpenMP)
-  - Distributed memory (MPI)
-- Domain sizes: 1D / 2D / 3D
-- Matching and non matching grids
-- Different mapping technologies (see [here](#available-mappers)):
-  - Nearest Neighbor
-  - Nearest Element
-  - Barycentric
-- Mapping operations (see [here](#customizing-the-behavior-of-the-mapping-with-flags))
-
-### Dependencies
-
-The serial / shared memory parallel compilation of the Mapping Application doesn't have any dependencies (except the `KratosCore`).
-
-The distributed compilation of the Mapping Application depends on the [Trilinos library](https://trilinos.github.io/). Also most of the MPI-solvers in Kratos depend on Trilinos, see the [Trilinos Application](../TrilinosApplication).
-
-### Mapping in CoSimulation
-
-The Mapping Application can be used for mapping within the [CoSimulation Application](../CoSimulationApplication). This can be done by using the  [KratosMappingDataTransferOperator](../CoSimulationApplication/python_scripts/data_transfer_operators/kratos_mapping.py).
-
-### Basic Usage
-
-The _Mapper_ maps nodal data from one _ModelPart_ to another. This means that the input for the _Mapper_ is two _ModelParts_, the **Origin** and the **Destination**. Furthermore settings in the form of _Kratos::Parameters_ are passed.
-
-The _Mapper_ is constructed using the _MapperFactory_. See the following basic example.
-
-```py
-# import the Kratos Core
-import KratosMultiphysics as KM
-# import the MappingApplication to load the mappers
-import KratosMultiphysics.MappingApplication as KratosMapping
-
-# create ModelParts
-# ...
-
-mapper_settings = KM.Parameters("""{
-    "mapper_type": "nearest_neighbor",
-    "echo_level" : 0
-}""")
-
-# creating a mapper for shared memory
-mapper = KM.MapperFactory.CreateMapper(
-    model_part_origin,
-    model_part_destination,
-    mapper_settings
-)
-```
-
-For constructing an _MPI-Mapper_ use the `MPIExtension` instead:
-
-```py
-# creating a mapper for distributed memory
-from KratosMultiphysics.MappingApplication import MPIExtension as MappingMPIExtension
-mpi_mapper = MappingMPIExtension.MPIMapperFactory.CreateMapper(
-    model_part_origin,
-    model_part_destination,
-    mapper_settings
-)
-```
-
-After constructing the _Mapper_ / _MPI-Mapper_ it can be used immediately to map any scalar and vector quantities, no further initialization is necessary.\
-The **Map** function is used to map values from the **Origin** to the **Destination**. For this the _Variables_ have to be specified. See the following example for mapping scalar quantities.
-
-```py
-# mapping scalar quantities
-# this maps the nodal quantities of TEMPERATURE on the origin-ModelPart
-# to the nodal quantities of AMBIENT_TEMPERATURE on the destination-ModelPart
-
-mapper.Map(KM.TEMPERATURE, KM.AMBIENT_TEMPERATURE)
-```
-
-The **Map** function is overloaded, this means that mapping vector quantities works in the same way as mapping scalar quantites.
-
-```py
-# mapping vector quantities
-# this maps the nodal quantities of VELOCITY on the origin-ModelPart
-# to the nodal quantities of MESH_VELOCITY on the destination-ModelPart.
-
-mapper.Map(KM.VELOCITY, KM.MESH_VELOCITY)
-```
-
-Mapping from **Destination** to **Origin** can be done using the **InverseMap** function which works in the same way as the **Map** function.
-
-```py
-# inverse mapping scalar quantities
-# this maps the nodal quantities of AMBIENT_TEMPERATURE on the destination-ModelPart
-# to the nodal quantities of TEMPERATURE on the origin-ModelPart
-
-mapper.InverseMap(KM.TEMPERATURE, KM.AMBIENT_TEMPERATURE)
-
-# inverse mapping vector quantities
-# this maps the nodal quantities of MESH_VELOCITY on the destination-ModelPart
-# to the nodal quantities of VELOCITY on the origin-ModelPart
-
-mapper.InverseMap(KM.VELOCITY, KM.MESH_VELOCITY)
-```
-
-### Advanced Usage
-
-The previous section introduced the basics of using the _MappingApplication_. The more advanced usage is explained in this section.
-
-#### Customizing the behavior of the mapping with Flags
-
-By default the mapping functions **Map** and **InverseMap** will overwrite the values where they map to. In order to add instead of overwrite the values the behavior can be customized by using _Kratos::Flags_. Consider in the following example that several forces are acting on a surface. Overwritting the values would cancel the previously applied forces.
-
-```py
-# Instead of overwriting, this will add the values to the existing ones
-
-mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.ADD_VALUES)
-```
-
-Sometimes it can be necessary to swap the signs of quantites that are to be mapped. This can be done with the following:
-
-```py
-# Swapping the sign, i.e. multiplying the values with (-1)
-
-mapper.Map(KM.DISPLACEMENT, KM.MESH_DISPLACEMENT, KM.Mapper.SWAP_SIGN)
-```
-
-The flags can also be combined:
-
-```py
-mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.ADD_VALUES | KM.Mapper.SWAP_SIGN)
-```
-
-Historical nodal values are used by default. Mapping to an from nonhistorical nodal values is also supported, the following examples show the usage:
-
-This maps the values from the origin (`REACTION`) as historical values to the destination (`FORCE`) as nonhistorical values:
-
-```py
-mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.TO_NON_HISTORICAL)
-```
-
-This maps the values from the origin (`REACTION`) as nonhistorical values to the destination (`FORCE`) as historical values:
-
-```py
-mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.FROM_NON_HISTORICAL)
-```
-
-This maps the values from the destination (`FORCE`) as historical values to the origin (`REACTION`) as nonhistorical values:
-
-```py
-mapper.InverseMap(KM.REACTION, KM.FORCE, KM.Mapper.TO_NON_HISTORICAL)
-```
-
-This maps the values from the destination (`FORCE`) as nonhistorical values to the origin (`REACTION`) as historical values:
-
-```py
-mapper.InverseMap(KM.REACTION, KM.FORCE, KM.Mapper.FROM_NON_HISTORICAL)
-```
-
-Of course it is possible to use both origin and destination nonhistorical. This maps the values from the origin (`REACTION`) as nonhistorical values to the destination (`FORCE`) as nonhistorical values:
-
-```py
-mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.FROM_NON_HISTORICAL | KM.Mapper.TO_NON_HISTORICAL)
-```
-
-Many _Mappers_ internally construct a mapping matrix. It is possible to use the transpose of this matrix for mapping with `USE_TRANSPOSE`. This is often used for conservative mapping of forces in FSI, when the virtual work on both interfaces should be preserved.
-
-```py
-mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.USE_TRANSPOSE)
-```
-
-#### Updating the Interface
-
-In case of moving interfaces (e.g. in a problem involving Contact between bodies) it can become necessary to update the _Mapper_ to take the new geometrical positions of the interfaces into account.\
-One way of doing this would be to construct a new _Mapper_, but this is not efficient and sometimes not even possible.
-
-Hence the _Mapper_ provides the **UpdateInterface** function for updating itseld with respect to the new geometrical positions of the interfaces.\
-Note that this is potentially an expensive operation due to searching the new geometrical neighbors on the interface.
-
-```py
-mapper.UpdateInterface()
-```
-
-#### Checking which mappers are available
-
-The following can be used to see which _Mappers_ are available:
-
-```py
-# available mappers for shared memory
-KM.MapperFactory.GetRegisteredMapperNames()
-
-# available mappers for distributed memory
-MappingMPIExtension.MPIMapperFactory.GetRegisteredMapperNames()
-
-# check if mapper for shared memory exists
-KM.MapperFactory.HasMapper("mapper_name")
-
-# check if mapper for distributed memory exists
-MappingMPIExtension.MPIMapperFactory.HasMapper("mapper_name")
-```
-
-#### Search settings
-The search of neighbors / partners on the other side of the interface is a crucial task when creating the mapper. Especially in distributed computations (MPI) this can be very expensive and time consuming. Hence the search of the mapper is very optimized to provide robust and fast results. For this the search works in several iterations where the search radius is increased in each iteration.
-The default settings of the search are working fine in most cases, but in some special cases it might still be necessary to tweak and optimize the settings. The following settings are available (as sub-parameter `search_settings` of the settings that are given to the mapper):
-
-| name | type | default| description |
-|---|---|---|---|
-| `search_radius`| `double` | computed | The search radius to start with in the first iteration. In each next iteration it will be increased by multiplying with `search_radius_increase_factor` (`search_radius *= search_radius_increase_factor`) |
-| `max_search_radius` | `double` | computed | The max search radius to use. |
-| `search_radius_increase_factor`| `double` | `2.0` | factor by which the search radius is increasing in each search iteration (see above). **Tuning this parameter is usually the best way to achieve a faster search**. In many cases decreasing it will speed up the search, especially for volumetric mapping, but it is case dependent. |
-| `max_num_search_iterations` | `int` | computed (min 3) | max number of search iterations that is conducted. If the search is successful before then it will terminate earlier. The more heterogeneous the mesh the larger this will be.
-
-It is recommended to set the `echo_level` to 2 or higher for getting useful information from the search. This will help to debug the search in case of problems.
-
-### Available Mappers
-
-This section explains the theory behind the mappers.
-
-#### Nearest Neighbor
-
-The _NearestNeighborMapper_ is a very simple/basic _Mapper_. Searches its closest neighbor (node) on the other interface. During mapping it gets/sets its value to the value of its closest neighbor.
-
-This mapper is best suited for problems where both interfaces have a similar discretization. Furthermore it is very robust and can be used for setting up problems when one does not (yet) want to deal with mapping.
-
-Internally it constructs the mapping matrix, hence it offers the usage of the transposed mapping matrix. When using this, for very inhomogenous interface discretizations it can come to oscillations in the mapped quantities.
-
-**Supported mesh topologies**: This mapper only works with nodes and hence supports any mesh topology
-
-#### Nearest Element
-
-The _NearestElementMapper_ projects nodes to the elements( or conditions) on other side of the inteface. Mapping is then done by interpolating the values of the nodes of the elements by using the shape functions at the projected position.
-
-This mapper is best suited for problems where the _NearestNeighborMapper_ cannot be used, i.e. for cases where the discretization on the interfaces is different. Note that it is less robust than the _NearestNeighborMapper_ due to the projections it performs. In case a projection fails, it uses an approximation that is similar to the approach of the _NearestNeighborMapper_. This can be disabled by setting `use_approximation` to `false` in the mapper-settings.
-
-Internally it constructs the mapping matrix, hence it offers the usage of the transposed mapping matrix. When using this, for very inhomogenous interface discretizations it can come to oscillations in the mapped quantities.
-
-**Supported mesh topologies**: Any mesh topology available in Kratos, which includes the most common linear and quadratic geometries, see [here](../../kratos/geometries).
-
-#### Barycentric
-
-The _BarycentricMapper_ uses the closest nodes to reconstructs a geometry. This geometry is used in the same way as the _NearestElementMapper_ for interpolating the values of the nodes using the shape functions.
-
-This mapper can be used when no geometries are available and interpolative properties of the mapper are required. E.g. for particle methods when only nodes or point-based entities are available. Overall it can be seen as combining the advantages of the _NearestNeighborMapper_ (which only requires points as input) with the advantages of the _NearestElementMapper_ (which has interpolative properties). The disadvantage is that the reconstruction of the geometry can cause problems in complex situations, hence it should only be used if the _NearestElementMapper_ cannot be used.
-
-Furthermore, the geometry type for the reconstruction/interpolation has to be chosen with the `interpolation_type` setting. The following types are available: `line`, `triangle` and `tetrahedra`
-
-Internally it constructs the mapping matrix, hence it offers the usage of the transposed mapping matrix. When using this, for very inhomogenous interface discretizations it can come to oscillations in the mapped quantities.
-
-**Supported mesh topologies**: This mapper only works with nodes and hence supports any mesh topology
-
-### When to use which Mapper?
-
-- **Matching Interface**\
-  For a matching interface the _NearestNeighborMapper_ is the best / fastes choice. Note that the ordering / numbering of the nodes doesn't matter.
-
-- **Interfaces with almost matching discretizations**\
-  In this case both the _NearestNeighborMapper_ and the _NearestElementMapper_ can yield good results.
-
-- **Interfaces with non matching discretizations**\
-  The _NearestElementMapper_ is recommended because it results in smoother mapping results due to the interpolation using the shape functions.
-
-- **Interfaces with non matching discretizations when no geometries are available for interpolation**\
-  The _NearestElementMapper_ cannot be used as it requires geometries for the ionterpolation. Here the _BarycentricMapper_ is recommended because it reconstructs geometries from the surrounding nodes and then uses it to interpolate.
-
-### Using the Mapper for ModelParts that are not part of all ranks
-
-In MPI parallel simulations usually all `ModelParts` are distributed across all ranks. However in some cases this does not hold, for example in FSI when the fluid runs on all ranks but the structure runs serial on one rank. In this case it is necessary to do the following:
-
-- Create a dummy-`ModelPart` on the ranks that do not have the original ModelPart.
-- **IMPORTANT**: This `ModelPart` must have a `DataCommunicator` that is not defined on the ranks that are not part of the original `ModelPart`.
-- Create and MPI-mapper as explained [above](#basic-usage), using the original and the dummy `ModelPart`s on the respective ranks.
-
-Check [this test](https://github.com/KratosMultiphysics/Kratos/blob/master/applications/MappingApplication/tests/blade_mapping_test.py) for more details and usage example.
-
-For an example the following assumptions are made:
-
-- Overall 4 MPI processes are used
-- `model_part_fluid` is distributed across all 4 ranks
-- `model_part_structure` is not distributed and exists only on rank 0
-
-```py
-import KratosMultiphysics as KM
-import KratosMultiphysics.mpi as KratosMPI
-
-# "model_part_fluid" was already read and exists on all ranks
-# "model_part_structure" was already read and exists only on rank 0
-
-
-# getting the DataCommunicator that wraps `MPI_COMM_WORLD` i.e. contains all ranks
-world_data_comm = KM.ParallelEnvironment.GetDataCommunicator("World)
-
-# define the ranks on which the structure ModelPart exists
-# structure can also be distributed across several (but not all) ranks
-structure_ranks = [0]
-
-# create a DataCommunicator containing only the structure ranks
-structure_ranks_data_comm_name = "structure_ranks"
-data_comm_all_structure_ranks = KratosMPI.DataCommunicatorFactory.CreateFromRanksAndRegister(
-    world_data_comm,
-    structure_ranks,
-    structure_ranks_data_comm_name)
-
-# create a dummy ModelPart on the ranks where the original ModelPart does not exist
-if world_data_comm.Rank() not in structure_ranks:
-    dummy_model = KM.Model()
-    model_part_structure = dummy_model.CreateModelPart("structure_dummy")
-
-    # Important: set the DataCommunicator so that the Mapper knows on which ranks the ModelPart is only a dummy
-    KratosMPI.ModelPartCommunicatorUtilities.SetMPICommunicator(model_part_structure, data_comm_all_structure_ranks)
-
-# now the Mapper can be created with the original and the dummy ModelParts
-mpi_mapper = MappingMPIExtension.MPIMapperFactory.CreateMapper(
-    model_part_fluid,
-    model_part_structure,
-    mapper_settings
-)
-```
-
-### Miscellaneous functionalities
-- [serial_output_process](https://github.com/KratosMultiphysics/Kratos/blob/master/applications/MappingApplication/python_scripts/serial_output_process.py): This process can be used to map results to one rank and then do postprocessing on this rank. This has two advantages:
-  - Some output formats write one file per rank in distributed simulations, which leads to many files when running with many cores. This process collects the results on one rank and can hence reduce the number of files significantly
-  - Different meshes can be used to do the postprocessing. This is in particular useful when the computational mesh is very fine, but a coarser mesh would be sufficient for postprocessing.
-
-  <ins>The following input parameters are used:</ins>
-  - `model_part_name_origin`: name of the origin ModelPart where the data comes from (is being mapped from)
-  - `model_part_name_destination`: name of destination ModelPart where the data is mapped to. This ModelPart is being read.
-  - `mdpa_file_name_destination`: name of the mdpa file containing the mesh that is used for the destination
-  - `historical_variables_destination` list of historical variables that are allocated on the destination ModelPart
-  - `destination_rank` rank on which the processing of the destination happens (i.e. the rank on which the destination ModelPart is read). Note that this increases the memory usage significantly, especially for large destination meshes. The default is rank 0, which in most distributed simulations acts as the master rank with already increased computational effort. Hence it can make sense to use another rank, preferably on another compute node, to optimize the memory and computational load balance
-  - `mapper_settings`: setting that are passed to the mapper, as explained above
-  - `mapping_settings`: list of mapping steps to be executed before the postprocessing is done. `variable_origin` and `variable_destination` must be specified, while `mapping_options` is optional and can contain the flags as explained above.
-  - `output_process_settings`: The settings for the output process (which will be only executed on the destination rank). **Important**: For mapping onto a serial ModelPart, the DataCommunicator is set as explained [here](#using-the-mapper-for-modelparts-that-are-not-part-of-all-ranks). This means that the destination ModelPart is not valid on other ranks and can hence not be used in the regular postprocessing (which happens also on the ranks where it is not valid and hence some MPI-functionalities would fail)
-  Example input:
-  ~~~js
-  "python_module" : "serial_output_process",
-  "kratos_module" : "KratosMultiphysics.MappingApplication",
-  "Parameters"    : {
-      "model_part_name_origin"      : "FluidModelPart",
-      "model_part_name_destination" : "PostProcessing",
-      "mdpa_file_name_destination"  : "coarse_mesh",
-      "historical_variables_destination" : ["REACTION", "DISPLACEMENT"],
-      "mapper_settings" :  {"mapper_type" : "nearest_neighbor"},
-      "mapping_settings" : [{
-          "variable_origin" : "REACTION",
-          "variable_destination" : "REACTION"
-      },{
-          "variable_origin" : "REACTION",
-          "variable_destination" : "REACTION",
-          "mapping_options" : ["add_values"]
-      },{
-          "variable_origin" : "MESH_DISPLACEMENT",
-          "variable_destination" : "DISPLACEMENT"
-      }],
-      "output_process_settings" : {
-          "python_module" : "vtk_output_process",
-          "kratos_module" : "KratosMultiphysics",
-          "Parameters"    : {
-              // ...
-          }
-      }
-  }
-  ~~~
-
-### FAQ
-
-- **Is mapping of elemental / conditional data or gauss-point values possible?**\
-  The mapper only supports mapping of nodal data. In order to map other quantities, those have to first be inter- / extrapolated to the nodes.
-
-- **Something is not working with the mapping. What should I do?**\
-  Problems with mapping can have many sources. The first thing in debugging what is happening is to increase the `echo_level` of the _Mapper_. Then in many times warnings are shown in case of some problems.
-
-- **I get oscillatory solutions when mapping with `USE_TRANSPOSE`**\
-  Research has shown that "simple" mappers like _NearestNeighbor_ and _NearestElement_ can have problems with mapping with the transpose (i.e. when using `USE_TRANSPOSE`) if the meshes are very different. Using the _MortarMapper_ technology can improve this situation. This _Mapper_ is currently under development.
-
-- **Projections find the wrong result**\
-  For complex geometries the projections can fail to find the correct result if many lines or surfaces are close. In those situations it helps to partition the mapping interface and construct multiple mappers with the smaller interfaces.
-
-- **Creation of the mapper takes very long**\
-  Often this is because of of unfit search settings. If the settings are not suitable for the problem then the mapper creation time can increase several magnitudes! Check [here](#search-settings) for an explanation of how to set the search settings in case the defaults are not working well.
+Metadata-Version: 2.1
+Name: KratosMappingApplication
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
+## Mapping Application
+
+The Mapping Application contains the core developments in mapping data between non matching grids. It works both in shared and distributed (**MPI**) memory environments as well as in 1D, 2D and 3D domains.
+
+### Overview
+
+- [List of features](#list-of-features)
+- [Dependencies](#dependencies)
+- [Mapping in CoSimulation](#Mapping-in-CoSimulation)
+- [Basic Usage](#basic-usage)
+- [Advanced Usage](#advanced-usage)
+- [Available Mappers](#available-mappers)
+- [When to use which Mapper?](#when-to-use-which-mapper)
+- [Using the Mapper for ModelParts that are not part of all ranks](#using-the-mapper-for-modelparts-that-are-not-part-of-all-ranks)
+- [Miscellaneous functionalities](#miscellaneous-functionalities)
+- [FAQ](#faq)
+
+### List of features
+
+- Parallelism:
+  - Serial (no parallelism)
+  - Shared memory (OpenMP)
+  - Distributed memory (MPI)
+- Domain sizes: 1D / 2D / 3D
+- Matching and non matching grids
+- Different mapping technologies (see [here](#available-mappers)):
+  - Nearest Neighbor
+  - Nearest Element
+  - Barycentric
+- Mapping operations (see [here](#customizing-the-behavior-of-the-mapping-with-flags))
+
+### Dependencies
+
+The serial / shared memory parallel compilation of the Mapping Application doesn't have any dependencies (except the `KratosCore`).
+
+The distributed compilation of the Mapping Application depends on the [Trilinos library](https://trilinos.github.io/). Also most of the MPI-solvers in Kratos depend on Trilinos, see the [Trilinos Application](../TrilinosApplication).
+
+### Mapping in CoSimulation
+
+The Mapping Application can be used for mapping within the [CoSimulation Application](../CoSimulationApplication). This can be done by using the  [KratosMappingDataTransferOperator](../CoSimulationApplication/python_scripts/data_transfer_operators/kratos_mapping.py).
+
+### Basic Usage
+
+The _Mapper_ maps nodal data from one _ModelPart_ to another. This means that the input for the _Mapper_ is two _ModelParts_, the **Origin** and the **Destination**. Furthermore settings in the form of _Kratos::Parameters_ are passed.
+
+The _Mapper_ is constructed using the _MapperFactory_. See the following basic example.
+
+```py
+# import the Kratos Core
+import KratosMultiphysics as KM
+# import the MappingApplication to load the mappers
+import KratosMultiphysics.MappingApplication as KratosMapping
+
+# create ModelParts
+# ...
+
+mapper_settings = KM.Parameters("""{
+    "mapper_type": "nearest_neighbor",
+    "echo_level" : 0
+}""")
+
+# creating a mapper for shared memory
+mapper = KM.MapperFactory.CreateMapper(
+    model_part_origin,
+    model_part_destination,
+    mapper_settings
+)
+```
+
+For constructing an _MPI-Mapper_ use the `MPIExtension` instead:
+
+```py
+# creating a mapper for distributed memory
+from KratosMultiphysics.MappingApplication import MPIExtension as MappingMPIExtension
+mpi_mapper = MappingMPIExtension.MPIMapperFactory.CreateMapper(
+    model_part_origin,
+    model_part_destination,
+    mapper_settings
+)
+```
+
+After constructing the _Mapper_ / _MPI-Mapper_ it can be used immediately to map any scalar and vector quantities, no further initialization is necessary.\
+The **Map** function is used to map values from the **Origin** to the **Destination**. For this the _Variables_ have to be specified. See the following example for mapping scalar quantities.
+
+```py
+# mapping scalar quantities
+# this maps the nodal quantities of TEMPERATURE on the origin-ModelPart
+# to the nodal quantities of AMBIENT_TEMPERATURE on the destination-ModelPart
+
+mapper.Map(KM.TEMPERATURE, KM.AMBIENT_TEMPERATURE)
+```
+
+The **Map** function is overloaded, this means that mapping vector quantities works in the same way as mapping scalar quantites.
+
+```py
+# mapping vector quantities
+# this maps the nodal quantities of VELOCITY on the origin-ModelPart
+# to the nodal quantities of MESH_VELOCITY on the destination-ModelPart.
+
+mapper.Map(KM.VELOCITY, KM.MESH_VELOCITY)
+```
+
+Mapping from **Destination** to **Origin** can be done using the **InverseMap** function which works in the same way as the **Map** function.
+
+```py
+# inverse mapping scalar quantities
+# this maps the nodal quantities of AMBIENT_TEMPERATURE on the destination-ModelPart
+# to the nodal quantities of TEMPERATURE on the origin-ModelPart
+
+mapper.InverseMap(KM.TEMPERATURE, KM.AMBIENT_TEMPERATURE)
+
+# inverse mapping vector quantities
+# this maps the nodal quantities of MESH_VELOCITY on the destination-ModelPart
+# to the nodal quantities of VELOCITY on the origin-ModelPart
+
+mapper.InverseMap(KM.VELOCITY, KM.MESH_VELOCITY)
+```
+
+### Advanced Usage
+
+The previous section introduced the basics of using the _MappingApplication_. The more advanced usage is explained in this section.
+
+#### Customizing the behavior of the mapping with Flags
+
+By default the mapping functions **Map** and **InverseMap** will overwrite the values where they map to. In order to add instead of overwrite the values the behavior can be customized by using _Kratos::Flags_. Consider in the following example that several forces are acting on a surface. Overwritting the values would cancel the previously applied forces.
+
+```py
+# Instead of overwriting, this will add the values to the existing ones
+
+mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.ADD_VALUES)
+```
+
+Sometimes it can be necessary to swap the signs of quantites that are to be mapped. This can be done with the following:
+
+```py
+# Swapping the sign, i.e. multiplying the values with (-1)
+
+mapper.Map(KM.DISPLACEMENT, KM.MESH_DISPLACEMENT, KM.Mapper.SWAP_SIGN)
+```
+
+The flags can also be combined:
+
+```py
+mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.ADD_VALUES | KM.Mapper.SWAP_SIGN)
+```
+
+Historical nodal values are used by default. Mapping to an from nonhistorical nodal values is also supported, the following examples show the usage:
+
+This maps the values from the origin (`REACTION`) as historical values to the destination (`FORCE`) as nonhistorical values:
+
+```py
+mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.TO_NON_HISTORICAL)
+```
+
+This maps the values from the origin (`REACTION`) as nonhistorical values to the destination (`FORCE`) as historical values:
+
+```py
+mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.FROM_NON_HISTORICAL)
+```
+
+This maps the values from the destination (`FORCE`) as historical values to the origin (`REACTION`) as nonhistorical values:
+
+```py
+mapper.InverseMap(KM.REACTION, KM.FORCE, KM.Mapper.TO_NON_HISTORICAL)
+```
+
+This maps the values from the destination (`FORCE`) as nonhistorical values to the origin (`REACTION`) as historical values:
+
+```py
+mapper.InverseMap(KM.REACTION, KM.FORCE, KM.Mapper.FROM_NON_HISTORICAL)
+```
+
+Of course it is possible to use both origin and destination nonhistorical. This maps the values from the origin (`REACTION`) as nonhistorical values to the destination (`FORCE`) as nonhistorical values:
+
+```py
+mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.FROM_NON_HISTORICAL | KM.Mapper.TO_NON_HISTORICAL)
+```
+
+Many _Mappers_ internally construct a mapping matrix. It is possible to use the transpose of this matrix for mapping with `USE_TRANSPOSE`. This is often used for conservative mapping of forces in FSI, when the virtual work on both interfaces should be preserved.
+
+```py
+mapper.Map(KM.REACTION, KM.FORCE, KM.Mapper.USE_TRANSPOSE)
+```
+
+#### Updating the Interface
+
+In case of moving interfaces (e.g. in a problem involving Contact between bodies) it can become necessary to update the _Mapper_ to take the new geometrical positions of the interfaces into account.\
+One way of doing this would be to construct a new _Mapper_, but this is not efficient and sometimes not even possible.
+
+Hence the _Mapper_ provides the **UpdateInterface** function for updating itseld with respect to the new geometrical positions of the interfaces.\
+Note that this is potentially an expensive operation due to searching the new geometrical neighbors on the interface.
+
+```py
+mapper.UpdateInterface()
+```
+
+#### Checking which mappers are available
+
+The following can be used to see which _Mappers_ are available:
+
+```py
+# available mappers for shared memory
+KM.MapperFactory.GetRegisteredMapperNames()
+
+# available mappers for distributed memory
+MappingMPIExtension.MPIMapperFactory.GetRegisteredMapperNames()
+
+# check if mapper for shared memory exists
+KM.MapperFactory.HasMapper("mapper_name")
+
+# check if mapper for distributed memory exists
+MappingMPIExtension.MPIMapperFactory.HasMapper("mapper_name")
+```
+
+#### Search settings
+The search of neighbors / partners on the other side of the interface is a crucial task when creating the mapper. Especially in distributed computations (MPI) this can be very expensive and time consuming. Hence the search of the mapper is very optimized to provide robust and fast results. For this the search works in several iterations where the search radius is increased in each iteration.
+The default settings of the search are working fine in most cases, but in some special cases it might still be necessary to tweak and optimize the settings. The following settings are available (as sub-parameter `search_settings` of the settings that are given to the mapper):
+
+| name | type | default| description |
+|---|---|---|---|
+| `search_radius`| `double` | computed | The search radius to start with in the first iteration. In each next iteration it will be increased by multiplying with `search_radius_increase_factor` (`search_radius *= search_radius_increase_factor`) |
+| `max_search_radius` | `double` | computed | The max search radius to use. |
+| `search_radius_increase_factor`| `double` | `2.0` | factor by which the search radius is increasing in each search iteration (see above). **Tuning this parameter is usually the best way to achieve a faster search**. In many cases decreasing it will speed up the search, especially for volumetric mapping, but it is case dependent. |
+| `max_num_search_iterations` | `int` | computed (min 3) | max number of search iterations that is conducted. If the search is successful before then it will terminate earlier. The more heterogeneous the mesh the larger this will be.
+
+It is recommended to set the `echo_level` to 2 or higher for getting useful information from the search. This will help to debug the search in case of problems.
+
+### Available Mappers
+
+This section explains the theory behind the mappers.
+
+#### Nearest Neighbor
+
+The _NearestNeighborMapper_ is a very simple/basic _Mapper_. Searches its closest neighbor (node) on the other interface. During mapping it gets/sets its value to the value of its closest neighbor.
+
+This mapper is best suited for problems where both interfaces have a similar discretization. Furthermore it is very robust and can be used for setting up problems when one does not (yet) want to deal with mapping.
+
+Internally it constructs the mapping matrix, hence it offers the usage of the transposed mapping matrix. When using this, for very inhomogenous interface discretizations it can come to oscillations in the mapped quantities.
+
+**Supported mesh topologies**: This mapper only works with nodes and hence supports any mesh topology
+
+#### Nearest Element
+
+The _NearestElementMapper_ projects nodes to the elements( or conditions) on other side of the inteface. Mapping is then done by interpolating the values of the nodes of the elements by using the shape functions at the projected position.
+
+This mapper is best suited for problems where the _NearestNeighborMapper_ cannot be used, i.e. for cases where the discretization on the interfaces is different. Note that it is less robust than the _NearestNeighborMapper_ due to the projections it performs. In case a projection fails, it uses an approximation that is similar to the approach of the _NearestNeighborMapper_. This can be disabled by setting `use_approximation` to `false` in the mapper-settings.
+
+Internally it constructs the mapping matrix, hence it offers the usage of the transposed mapping matrix. When using this, for very inhomogenous interface discretizations it can come to oscillations in the mapped quantities.
+
+**Supported mesh topologies**: Any mesh topology available in Kratos, which includes the most common linear and quadratic geometries, see [here](../../kratos/geometries).
+
+#### Barycentric
+
+The _BarycentricMapper_ uses the closest nodes to reconstructs a geometry. This geometry is used in the same way as the _NearestElementMapper_ for interpolating the values of the nodes using the shape functions.
+
+This mapper can be used when no geometries are available and interpolative properties of the mapper are required. E.g. for particle methods when only nodes or point-based entities are available. Overall it can be seen as combining the advantages of the _NearestNeighborMapper_ (which only requires points as input) with the advantages of the _NearestElementMapper_ (which has interpolative properties). The disadvantage is that the reconstruction of the geometry can cause problems in complex situations, hence it should only be used if the _NearestElementMapper_ cannot be used.
+
+Furthermore, the geometry type for the reconstruction/interpolation has to be chosen with the `interpolation_type` setting. The following types are available: `line`, `triangle` and `tetrahedra`
+
+Internally it constructs the mapping matrix, hence it offers the usage of the transposed mapping matrix. When using this, for very inhomogenous interface discretizations it can come to oscillations in the mapped quantities.
+
+**Supported mesh topologies**: This mapper only works with nodes and hence supports any mesh topology
+
+### When to use which Mapper?
+
+- **Matching Interface**\
+  For a matching interface the _NearestNeighborMapper_ is the best / fastes choice. Note that the ordering / numbering of the nodes doesn't matter.
+
+- **Interfaces with almost matching discretizations**\
+  In this case both the _NearestNeighborMapper_ and the _NearestElementMapper_ can yield good results.
+
+- **Interfaces with non matching discretizations**\
+  The _NearestElementMapper_ is recommended because it results in smoother mapping results due to the interpolation using the shape functions.
+
+- **Interfaces with non matching discretizations when no geometries are available for interpolation**\
+  The _NearestElementMapper_ cannot be used as it requires geometries for the ionterpolation. Here the _BarycentricMapper_ is recommended because it reconstructs geometries from the surrounding nodes and then uses it to interpolate.
+
+### Using the Mapper for ModelParts that are not part of all ranks
+
+In MPI parallel simulations usually all `ModelParts` are distributed across all ranks. However in some cases this does not hold, for example in FSI when the fluid runs on all ranks but the structure runs serial on one rank. In this case it is necessary to do the following:
+
+- Create a dummy-`ModelPart` on the ranks that do not have the original ModelPart.
+- **IMPORTANT**: This `ModelPart` must have a `DataCommunicator` that is not defined on the ranks that are not part of the original `ModelPart`.
+- Create and MPI-mapper as explained [above](#basic-usage), using the original and the dummy `ModelPart`s on the respective ranks.
+
+Check [this test](https://github.com/KratosMultiphysics/Kratos/blob/master/applications/MappingApplication/tests/blade_mapping_test.py) for more details and usage example.
+
+For an example the following assumptions are made:
+
+- Overall 4 MPI processes are used
+- `model_part_fluid` is distributed across all 4 ranks
+- `model_part_structure` is not distributed and exists only on rank 0
+
+```py
+import KratosMultiphysics as KM
+import KratosMultiphysics.mpi as KratosMPI
+
+# "model_part_fluid" was already read and exists on all ranks
+# "model_part_structure" was already read and exists only on rank 0
+
+
+# getting the DataCommunicator that wraps `MPI_COMM_WORLD` i.e. contains all ranks
+world_data_comm = KM.ParallelEnvironment.GetDataCommunicator("World)
+
+# define the ranks on which the structure ModelPart exists
+# structure can also be distributed across several (but not all) ranks
+structure_ranks = [0]
+
+# create a DataCommunicator containing only the structure ranks
+structure_ranks_data_comm_name = "structure_ranks"
+data_comm_all_structure_ranks = KratosMPI.DataCommunicatorFactory.CreateFromRanksAndRegister(
+    world_data_comm,
+    structure_ranks,
+    structure_ranks_data_comm_name)
+
+# create a dummy ModelPart on the ranks where the original ModelPart does not exist
+if world_data_comm.Rank() not in structure_ranks:
+    dummy_model = KM.Model()
+    model_part_structure = dummy_model.CreateModelPart("structure_dummy")
+
+    # Important: set the DataCommunicator so that the Mapper knows on which ranks the ModelPart is only a dummy
+    KratosMPI.ModelPartCommunicatorUtilities.SetMPICommunicator(model_part_structure, data_comm_all_structure_ranks)
+
+# now the Mapper can be created with the original and the dummy ModelParts
+mpi_mapper = MappingMPIExtension.MPIMapperFactory.CreateMapper(
+    model_part_fluid,
+    model_part_structure,
+    mapper_settings
+)
+```
+
+### Miscellaneous functionalities
+- [serial_output_process](https://github.com/KratosMultiphysics/Kratos/blob/master/applications/MappingApplication/python_scripts/serial_output_process.py): This process can be used to map results to one rank and then do postprocessing on this rank. This has two advantages:
+  - Some output formats write one file per rank in distributed simulations, which leads to many files when running with many cores. This process collects the results on one rank and can hence reduce the number of files significantly
+  - Different meshes can be used to do the postprocessing. This is in particular useful when the computational mesh is very fine, but a coarser mesh would be sufficient for postprocessing.
+
+  <ins>The following input parameters are used:</ins>
+  - `model_part_name_origin`: name of the origin ModelPart where the data comes from (is being mapped from)
+  - `model_part_name_destination`: name of destination ModelPart where the data is mapped to. This ModelPart is being read.
+  - `mdpa_file_name_destination`: name of the mdpa file containing the mesh that is used for the destination
+  - `historical_variables_destination` list of historical variables that are allocated on the destination ModelPart
+  - `destination_rank` rank on which the processing of the destination happens (i.e. the rank on which the destination ModelPart is read). Note that this increases the memory usage significantly, especially for large destination meshes. The default is rank 0, which in most distributed simulations acts as the master rank with already increased computational effort. Hence it can make sense to use another rank, preferably on another compute node, to optimize the memory and computational load balance
+  - `mapper_settings`: setting that are passed to the mapper, as explained above
+  - `mapping_settings`: list of mapping steps to be executed before the postprocessing is done. `variable_origin` and `variable_destination` must be specified, while `mapping_options` is optional and can contain the flags as explained above.
+  - `output_process_settings`: The settings for the output process (which will be only executed on the destination rank). **Important**: For mapping onto a serial ModelPart, the DataCommunicator is set as explained [here](#using-the-mapper-for-modelparts-that-are-not-part-of-all-ranks). This means that the destination ModelPart is not valid on other ranks and can hence not be used in the regular postprocessing (which happens also on the ranks where it is not valid and hence some MPI-functionalities would fail)
+  Example input:
+  ~~~js
+  "python_module" : "serial_output_process",
+  "kratos_module" : "KratosMultiphysics.MappingApplication",
+  "Parameters"    : {
+      "model_part_name_origin"      : "FluidModelPart",
+      "model_part_name_destination" : "PostProcessing",
+      "mdpa_file_name_destination"  : "coarse_mesh",
+      "historical_variables_destination" : ["REACTION", "DISPLACEMENT"],
+      "mapper_settings" :  {"mapper_type" : "nearest_neighbor"},
+      "mapping_settings" : [{
+          "variable_origin" : "REACTION",
+          "variable_destination" : "REACTION"
+      },{
+          "variable_origin" : "REACTION",
+          "variable_destination" : "REACTION",
+          "mapping_options" : ["add_values"]
+      },{
+          "variable_origin" : "MESH_DISPLACEMENT",
+          "variable_destination" : "DISPLACEMENT"
+      }],
+      "output_process_settings" : {
+          "python_module" : "vtk_output_process",
+          "kratos_module" : "KratosMultiphysics",
+          "Parameters"    : {
+              // ...
+          }
+      }
+  }
+  ~~~
+
+### FAQ
+
+- **Is mapping of elemental / conditional data or gauss-point values possible?**\
+  The mapper only supports mapping of nodal data. In order to map other quantities, those have to first be inter- / extrapolated to the nodes.
+
+- **Something is not working with the mapping. What should I do?**\
+  Problems with mapping can have many sources. The first thing in debugging what is happening is to increase the `echo_level` of the _Mapper_. Then in many times warnings are shown in case of some problems.
+
+- **I get oscillatory solutions when mapping with `USE_TRANSPOSE`**\
+  Research has shown that "simple" mappers like _NearestNeighbor_ and _NearestElement_ can have problems with mapping with the transpose (i.e. when using `USE_TRANSPOSE`) if the meshes are very different. Using the _MortarMapper_ technology can improve this situation. This _Mapper_ is currently under development.
+
+- **Projections find the wrong result**\
+  For complex geometries the projections can fail to find the correct result if many lines or surfaces are close. In those situations it helps to partition the mapping interface and construct multiple mappers with the smaller interfaces.
+
+- **Creation of the mapper takes very long**\
+  Often this is because of of unfit search settings. If the settings are not suitable for the problem then the mapper creation time can increase several magnitudes! Check [here](#search-settings) for an explanation of how to set the search settings in case the defaults are not working well.
```

## Comparing `KratosMappingApplication-9.4.6.dist-info/RECORD` & `KratosMappingApplication-9.5.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-KratosMultiphysics/.libs/KratosMappingApplication.pyd,sha256=fmaDmf0ifY9x_Pl9K6ZufBCbCry_M5Bh_68PTBaypqA,444416
-KratosMultiphysics/.libs/KratosMappingCore.dll,sha256=IJNqvq4YjH0sXuObKCPEy9NN394nNYn41qxW8D_9dwY,1862144
-KratosMultiphysics/.libs/KratosMappingCore.lib,sha256=9FWWLocFPExbChysLc4RU5RmvoyFEgznqZdx2t9D8Wo,545960
-KratosMultiphysics/MappingApplication/__init__.py,sha256=sFBx7bwd5cRBdr-rRdaobZgj_opsmLTdKhY-t-3NRxI,2597
-KratosMultiphysics/MappingApplication/empire_mortar_mapper.py,sha256=l9qDqVa64hmBHcSjlnRzRcK7SmicYTFawiNYxIMcYtQ,15467
-KratosMultiphysics/MappingApplication/python_mapper.py,sha256=11pTgIzae_y5AQ1fokBClJdR8El7C9apJmguLY_g3DA,2123
-KratosMultiphysics/MappingApplication/python_mapper_factory.py,sha256=aOLJUw-SM2hLCqMEhiN-Zvg5N_E6kZItu9OZM3c8fFQ,1998
-KratosMultiphysics/MappingApplication/serial_output_process.py,sha256=AEubUwO7QBxjXFf71SL6w5uuEfXTFTxqziU2w2Wc8AQ,6856
-KratosMappingApplication-9.4.6.dist-info/METADATA,sha256=xyG56cJRdUA3Az2pbuRqktSfIlGBL2QUOOlmv7Yw_8g,23923
-KratosMappingApplication-9.4.6.dist-info/WHEEL,sha256=GZFS91_ufm4WrNPBaFVPB9MvOXR6bMZQhPcZRRTN5YM,100
-KratosMappingApplication-9.4.6.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
-KratosMappingApplication-9.4.6.dist-info/RECORD,,
+KratosMappingApplication.libs/libKratosMappingCore-e2ac717d.so,sha256=GGWtns2nmSNbpNW8VsvVSJLpjXMEJt-mQCJWvMP5LoY,6392009
+KratosMultiphysics/MappingApplication/python_mapper.py,sha256=BOGmU4cWfDUIjLX8gi_ofSXbAKjbmsXUkIEeWbzK1yc,2069
+KratosMultiphysics/MappingApplication/empire_mortar_mapper.py,sha256=sYYlgKEsUo5D-XN0J9LZgynJHkj6Mcyd15L1ZoNZWZ0,15125
+KratosMultiphysics/MappingApplication/serial_output_process.py,sha256=xqkvP51m8rfHZ1IJcsPoM5f3y3vlr7AKV2WmaRCzMcA,6713
+KratosMultiphysics/MappingApplication/python_mapper_factory.py,sha256=i595t-6Zb-dGlV9vvUY-0f7mlvxa67HqTQMt-HsdRMQ,1959
+KratosMultiphysics/MappingApplication/__init__.py,sha256=7c09Lo9AkwNDNLhDYe-EKwtPQRsB_kaodgVUj6_vJlw,2546
+KratosMultiphysics/.libs/KratosMappingApplication.cpython-39-x86_64-linux-gnu.so,sha256=c3M_cmwVquJdpKWnvdB9RVVWMZeFHIlvfwNRShzUI5I,1580393
+KratosMultiphysics/.libs/libKratosMappingCore.so,sha256=WewDt9F4F4-6In3AmT4oltzjtJUCEexx3JXSB8ur81E,5958473
+KratosMappingApplication-9.5.dist-info/METADATA,sha256=SoaPDWJmRPGmannEJeUeJTWmFIZju1avitRdzHos-bY,23499
+KratosMappingApplication-9.5.dist-info/WHEEL,sha256=rY0Y6THYM7EImsHfF-zs67o8pQciAsMw9_YuSvftjrQ,148
+KratosMappingApplication-9.5.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
+KratosMappingApplication-9.5.dist-info/RECORD,,
```

