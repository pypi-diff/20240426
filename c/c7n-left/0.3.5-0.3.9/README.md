# Comparing `tmp/c7n_left-0.3.5-py3-none-any.whl.zip` & `tmp/c7n_left-0.3.9-py3-none-any.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                     38299 (000000000000959Bh)
-  Actual end-cent-dir record offset:         38277 (0000000000009585h)
-  Expected end-cent-dir record offset:       38277 (0000000000009585h)
+  Zip archive file size:                     38733 (000000000000974Dh)
+  Actual end-cent-dir record offset:         38711 (0000000000009737h)
+  Expected end-cent-dir record offset:       38711 (0000000000009737h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
   central directory contains 19 entries.
-  The central directory is 1433 (0000000000000599h) bytes long,
+  The central directory is 1409 (0000000000000581h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 36844 (0000000000008FECh).
+  is 37302 (00000000000091B6h).
 
 
 Central directory entry #1:
 ---------------------------
 
   c7n_left/cli.py
 
@@ -27,17 +27,17 @@
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  32-bit CRC value (hex):                         51ef7d9f
-  compressed size:                                1409 bytes
-  uncompressed size:                              4726 bytes
+  32-bit CRC value (hex):                         7acca64a
+  compressed size:                                1513 bytes
+  uncompressed size:                              5101 bytes
   length of filename:                             15 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -45,16 +45,16 @@
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
   c7n_left/core.py
 
-  offset of local header from start of archive:   1454
-                                                  (00000000000005AEh) bytes
+  offset of local header from start of archive:   1558
+                                                  (0000000000000616h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -74,16 +74,16 @@
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
   c7n_left/data/taggable.json
 
-  offset of local header from start of archive:   4842
-                                                  (00000000000012EAh) bytes
+  offset of local header from start of archive:   4946
+                                                  (0000000000001352h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -103,16 +103,16 @@
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
   c7n_left/entry.py
 
-  offset of local header from start of archive:   15046
-                                                  (0000000000003AC6h) bytes
+  offset of local header from start of archive:   15150
+                                                  (0000000000003B2Eh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -132,16 +132,16 @@
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
   c7n_left/filters.py
 
-  offset of local header from start of archive:   15202
-                                                  (0000000000003B62h) bytes
+  offset of local header from start of archive:   15306
+                                                  (0000000000003BCAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -161,28 +161,28 @@
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
   c7n_left/output.py
 
-  offset of local header from start of archive:   16667
-                                                  (000000000000411Bh) bytes
+  offset of local header from start of archive:   16771
+                                                  (0000000000004183h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  32-bit CRC value (hex):                         2aea4fa7
-  compressed size:                                5323 bytes
-  uncompressed size:                              21504 bytes
+  32-bit CRC value (hex):                         7755e0c6
+  compressed size:                                5326 bytes
+  uncompressed size:                              21548 bytes
   length of filename:                             18 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
@@ -190,16 +190,16 @@
   There is no file comment.
 
 Central directory entry #7:
 ---------------------------
 
   c7n_left/policy.py
 
-  offset of local header from start of archive:   22038
-                                                  (0000000000005616h) bytes
+  offset of local header from start of archive:   22145
+                                                  (0000000000005681h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -219,16 +219,16 @@
   There is no file comment.
 
 Central directory entry #8:
 ---------------------------
 
   c7n_left/providers/terraform/__init__.py
 
-  offset of local header from start of archive:   22661
-                                                  (0000000000005885h) bytes
+  offset of local header from start of archive:   22768
+                                                  (00000000000058F0h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -248,16 +248,16 @@
   There is no file comment.
 
 Central directory entry #9:
 ---------------------------
 
   c7n_left/providers/terraform/filters.py
 
-  offset of local header from start of archive:   22841
-                                                  (0000000000005939h) bytes
+  offset of local header from start of archive:   22948
+                                                  (00000000000059A4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -277,16 +277,16 @@
   There is no file comment.
 
 Central directory entry #10:
 ---------------------------
 
   c7n_left/providers/terraform/graph.py
 
-  offset of local header from start of archive:   23419
-                                                  (0000000000005B7Bh) bytes
+  offset of local header from start of archive:   23526
+                                                  (0000000000005BE6h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -306,16 +306,16 @@
   There is no file comment.
 
 Central directory entry #11:
 ---------------------------
 
   c7n_left/providers/terraform/provider.py
 
-  offset of local header from start of archive:   24616
-                                                  (0000000000006028h) bytes
+  offset of local header from start of archive:   24723
+                                                  (0000000000006093h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -335,16 +335,16 @@
   There is no file comment.
 
 Central directory entry #12:
 ---------------------------
 
   c7n_left/providers/terraform/resource.py
 
-  offset of local header from start of archive:   26223
-                                                  (000000000000666Fh) bytes
+  offset of local header from start of archive:   26330
+                                                  (00000000000066DAh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -364,16 +364,16 @@
   There is no file comment.
 
 Central directory entry #13:
 ---------------------------
 
   c7n_left/providers/terraform/variables.py
 
-  offset of local header from start of archive:   26714
-                                                  (000000000000685Ah) bytes
+  offset of local header from start of archive:   26821
+                                                  (00000000000068C5h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -393,16 +393,16 @@
   There is no file comment.
 
 Central directory entry #14:
 ---------------------------
 
   c7n_left/test.py
 
-  offset of local header from start of archive:   28920
-                                                  (00000000000070F8h) bytes
+  offset of local header from start of archive:   29027
+                                                  (0000000000007163h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -422,16 +422,16 @@
   There is no file comment.
 
 Central directory entry #15:
 ---------------------------
 
   c7n_left/utils.py
 
-  offset of local header from start of archive:   30948
-                                                  (00000000000078E4h) bytes
+  offset of local header from start of archive:   31055
+                                                  (000000000000794Fh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
@@ -449,128 +449,120 @@
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #16:
 ---------------------------
 
-  c7n_left-0.3.5.dist-info/METADATA
+  c7n_left-0.3.9.dist-info/WHEEL
 
-  offset of local header from start of archive:   31143
-                                                  (00000000000079A7h) bytes
+  offset of local header from start of archive:   31250
+                                                  (0000000000007A12h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Sep 29 13:44:02
-  file last modified on (UT extra field modtime): 2023 Sep 29 17:44:02 local
-  file last modified on (UT extra field modtime): 2023 Sep 29 17:44:02 UTC
-  32-bit CRC value (hex):                         8e2339c3
-  compressed size:                                4384 bytes
-  uncompressed size:                              12304 bytes
-  length of filename:                             33 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
+  32-bit CRC value (hex):                         194415e5
+  compressed size:                                86 bytes
+  uncompressed size:                              88 bytes
+  length of filename:                             30 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 f5 01 00 00 04 14 00 00 00.
-
   There is no file comment.
 
 Central directory entry #17:
 ---------------------------
 
-  c7n_left-0.3.5.dist-info/WHEEL
+  c7n_left-0.3.9.dist-info/entry_points.txt
 
-  offset of local header from start of archive:   35618
-                                                  (0000000000008B22h) bytes
+  offset of local header from start of archive:   31396
+                                                  (0000000000007AA4h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
   file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  32-bit CRC value (hex):                         9255a969
-  compressed size:                                85 bytes
-  uncompressed size:                              88 bytes
-  length of filename:                             30 characters
+  32-bit CRC value (hex):                         4c64f7f0
+  compressed size:                                42 bytes
+  uncompressed size:                              45 bytes
+  length of filename:                             41 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #18:
 ---------------------------
 
-  c7n_left-0.3.5.dist-info/entry_points.txt
+  c7n_left-0.3.9.dist-info/METADATA
 
-  offset of local header from start of archive:   35763
-                                                  (0000000000008BB3h) bytes
+  offset of local header from start of archive:   31509
+                                                  (0000000000007B15h) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          1980 Jan 1 00:00:00
-  32-bit CRC value (hex):                         4c64f7f0
-  compressed size:                                42 bytes
-  uncompressed size:                              45 bytes
-  length of filename:                             41 characters
+  file last modified on (DOS date/time):          2016 Jan 1 00:00:00
+  32-bit CRC value (hex):                         bf0c7f8f
+  compressed size:                                4761 bytes
+  uncompressed size:                              15097 bytes
+  length of filename:                             33 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100644 octal):            -rw-r--r--
+  Unix file attributes (000644 octal):            ?rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #19:
 ---------------------------
 
-  c7n_left-0.3.5.dist-info/RECORD
+  c7n_left-0.3.9.dist-info/RECORD
 
-  offset of local header from start of archive:   35876
-                                                  (0000000000008C24h) bytes
+  offset of local header from start of archive:   36333
+                                                  (0000000000008DEDh) bytes
   file system or operating system of origin:      Unix
   version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2016 Jan 1 00:00:00
-  32-bit CRC value (hex):                         b9e5e879
-  compressed size:                                907 bytes
+  file last modified on (DOS date/time):          2023 Oct 3 15:25:58
+  32-bit CRC value (hex):                         3d08f222
+  compressed size:                                908 bytes
   uncompressed size:                              1561 bytes
   length of filename:                             31 characters
   length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (000644 octal):            ?rw-r--r--
+  Unix file attributes (000600 octal):            ?rw-------
   MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: c7n_left/test.py
 Comment: 
 
 Filename: c7n_left/utils.py
 Comment: 
 
-Filename: c7n_left-0.3.5.dist-info/METADATA
+Filename: c7n_left-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_left-0.3.5.dist-info/WHEEL
+Filename: c7n_left-0.3.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: c7n_left-0.3.5.dist-info/entry_points.txt
+Filename: c7n_left-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: c7n_left-0.3.5.dist-info/RECORD
+Filename: c7n_left-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## c7n_left/cli.py

```diff
@@ -43,20 +43,19 @@
 @click.option(
     "--output-query",
     default=None,
     help="Use a jmespath expression to filter json output",
 )
 def dump(directory, var_file, output_file, output_query):
     """Dump the parsed resource graph or subset"""
-
-    config = Config.empty(
-        source_dir=Path(directory),
+    config = get_config(
+        directory,
         output="jsongraph",
         output_file=output_file,
-        var_files=var_file,
+        var_file=var_file,
         output_query=output_query,
     )
     reporter = get_reporter(config)
     config["reporter"] = reporter
     provider = get_provider(config.source_dir)
     provider.initialize(config)
     graph = provider.parse(config.source_dir, config.var_files)
@@ -101,67 +100,84 @@
     directory,
     output,
     output_file,
     var_file,
     output_query,
     summary,
     filters,
+    reporter=None,
 ):
     """evaluate policies against IaC sources.
 
     c7n-left -p policy_dir -d terraform_root --filters "severity=HIGH"
 
 
     WARNING - CLI interface subject to change.
     """
-    config = Config.empty(
-        source_dir=Path(directory),
-        policy_dir=Path(policy_dir),
+    config = get_config(
+        directory,
+        policy_dir,
         output=output,
         output_file=output_file,
-        var_files=var_file,
         output_query=output_query,
+        var_file=var_file,
         summary=summary,
         filters=filters,
     )
-
-    exec_filter = ExecutionFilter.parse(config)
-    config["exec_filter"] = exec_filter
-    policies = exec_filter.filter_policies(load_policies(policy_dir, config))
+    policies = config.exec_filter.filter_policies(load_policies(policy_dir, config))
     if not policies:
         log.warning("no policies found")
         sys.exit(1)
-    reporter = get_reporter(config)
+    if reporter is None:
+        reporter = get_reporter(config)
     config["reporter"] = reporter
     runner = CollectionRunner(policies, config, reporter)
     sys.exit(int(runner.run()))
 
 
 @cli.command()
 @click.option("-p", "--policy-dir", type=click.Path(), required=True)
 @click.option("--filters", help="filter policies or resources as k=v pairs with globbing")
 def test(policy_dir, filters):
     """Run policy tests."""
     policy_dir = Path(policy_dir)
     source_dir = policy_dir / "tests"
 
+    config = get_config(source_dir, policy_dir, output_file=sys.stdout, filters=filters)
+    reporter = TestReporter(None, config)
+    policies = config.exec_filter.filter_policies(load_policies(policy_dir, config))
+    runner = TestRunner(policies, config, reporter)
+    sys.exit(int(runner.run()))
+
+
+def get_config(
+    directory=None,
+    policy_dir=None,
+    output=None,
+    output_file=None,
+    var_file=(),
+    output_query=None,
+    summary=None,
+    filters=None,
+    format='terraform',
+):
     config = Config.empty(
-        source_dir=source_dir,
-        policy_dir=policy_dir,
-        output_file=sys.stdout,
+        source_dir=directory and Path(directory),
+        policy_dir=policy_dir and Path(policy_dir),
+        output=output,
+        output_file=output_file,
+        var_files=var_file,
+        output_query=output_query,
+        summary=summary,
         filters=filters,
-        var_files=(),
+        format=format,
     )
-
-    reporter = TestReporter(None, config)
     exec_filter = ExecutionFilter.parse(config)
     config["exec_filter"] = exec_filter
-    policies = exec_filter.filter_policies(load_policies(policy_dir, config))
-    runner = TestRunner(policies, config, reporter)
-    sys.exit(int(runner.run()))
+    return config
 
 
 if __name__ == "__main__":  # pragma: no cover
     try:
         cli()
     except Exception:
         import pdb, traceback
```

## c7n_left/output.py

```diff
@@ -153,15 +153,16 @@
         policy_resources = Counter()
         type_counts = Counter()
         type_policies = Counter()
 
         resource_count = 0
 
         for rtype, resources in graph.get_resources_by_type():
-            resources = self.config.exec_filter.filter_resources(rtype, resources)
+            if self.config.exec_filter:
+                resources = self.config.exec_filter.filter_resources(rtype, resources)
             if "_" not in rtype:
                 continue
             if not resources:
                 continue
 
             resource_count += len(resources)
             type_counts[rtype] = len(resources)
```

