# Comparing `tmp/kutil_jakubaugustyn-0.0.6.tar.gz` & `tmp/kutil_jakubaugustyn-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kutil_jakubaugustyn-0.0.6.tar", last modified: Sat Apr 20 12:58:30 2024, max compression
+gzip compressed data, was "kutil_jakubaugustyn-0.0.7.tar", last modified: Fri Apr 26 15:29:36 2024, max compression
```

## Comparing `kutil_jakubaugustyn-0.0.6.tar` & `kutil_jakubaugustyn-0.0.7.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.880808 kutil_jakubaugustyn-0.0.6/
--rw-rw-rw-   0        0        0     1093 2023-12-08 14:54:39.000000 kutil_jakubaugustyn-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1374 2024-04-20 12:58:30.880808 kutil_jakubaugustyn-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      810 2024-02-28 16:16:37.000000 kutil_jakubaugustyn-0.0.6/README.md
--rw-rw-rw-   0        0        0      824 2024-04-20 12:58:01.000000 kutil_jakubaugustyn-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-20 12:58:30.880808 kutil_jakubaugustyn-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:29.878123 kutil_jakubaugustyn-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.880808 kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/
--rw-rw-rw-   0        0        0     1374 2024-04-20 12:58:29.000000 kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3719 2024-04-20 12:58:29.000000 kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 12:58:29.000000 kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-20 12:58:29.000000 kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:29.915879 kutil_jakubaugustyn-0.0.6/src/kutil/
--rw-rw-rw-   0        0        0      302 2024-02-28 19:22:19.000000 kutil_jakubaugustyn-0.0.6/src/kutil/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:29.947132 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/
--rw-rw-rw-   0        0        0     2401 2023-12-18 18:55:31.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/BidirectionalByteArray.py
--rw-rw-rw-   0        0        0     4303 2024-03-25 17:59:57.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/ByteBuffer.py
--rw-rw-rw-   0        0        0     5333 2024-03-02 12:29:40.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/DataBuffer.py
--rw-rw-rw-   0        0        0      375 2024-01-07 13:46:13.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/Serializable.py
--rw-rw-rw-   0        0        0     1268 2023-12-18 18:20:16.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/TextOutput.py
--rw-rw-rw-   0        0        0      335 2024-03-02 12:31:14.000000 kutil_jakubaugustyn-0.0.6/src/kutil/buffer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:29.962756 kutil_jakubaugustyn-0.0.6/src/kutil/io/
--rw-rw-rw-   0        0        0      262 2024-04-16 09:37:01.000000 kutil_jakubaugustyn-0.0.6/src/kutil/io/__init__.py
--rw-rw-rw-   0        0        0     2983 2023-12-26 14:36:42.000000 kutil_jakubaugustyn-0.0.6/src/kutil/io/directory.py
--rw-rw-rw-   0        0        0     3568 2024-04-16 09:35:52.000000 kutil_jakubaugustyn-0.0.6/src/kutil/io/file.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.016150 kutil_jakubaugustyn-0.0.6/src/kutil/language/
--rw-rw-rw-   0        0        0     4560 2024-02-28 19:21:38.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/AST.py
--rw-rw-rw-   0        0        0     5769 2024-01-13 18:03:43.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/BytecodeFile.py
--rw-rw-rw-   0        0        0     1608 2024-01-16 14:45:31.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Compiler.py
--rw-rw-rw-   0        0        0      704 2024-01-13 11:58:11.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Error.py
--rw-rw-rw-   0        0        0     1601 2024-01-16 14:49:22.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Interpreter.py
--rw-rw-rw-   0        0        0     4116 2024-01-16 14:49:42.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Language.py
--rw-rw-rw-   0        0        0     1441 2024-01-16 15:20:00.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Lexer.py
--rw-rw-rw-   0        0        0     1797 2024-01-16 14:41:55.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Options.py
--rw-rw-rw-   0        0        0     1101 2024-01-16 17:36:44.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Parser.py
--rw-rw-rw-   0        0        0      625 2024-01-13 18:35:04.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Stack.py
--rw-rw-rw-   0        0        0     2020 2024-01-03 18:39:33.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/Token.py
--rw-rw-rw-   0        0        0      389 2024-01-14 18:53:04.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.031779 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/
--rw-rw-rw-   0        0        0     8372 2024-01-16 14:54:52.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/BrainFuck.py
--rw-rw-rw-   0        0        0      274 2024-01-14 19:45:36.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.078649 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/
--rw-rw-rw-   0        0        0    40883 2024-02-10 17:14:05.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSLexer.py
--rw-rw-rw-   0        0        0     1565 2024-01-22 17:04:30.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSOptions.py
--rw-rw-rw-   0        0        0   142027 2024-02-11 14:35:27.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSParser.py
--rw-rw-rw-   0        0        0     1210 2024-01-22 17:24:55.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/Javascript.py
--rw-rw-rw-   0        0        0     1669 2024-01-21 06:51:49.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/__init__.py
--rw-rw-rw-   0        0        0     5070 2024-01-25 20:00:28.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/character.py
--rw-rw-rw-   0        0        0     3458 2024-01-16 14:12:04.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/error_handler.py
--rw-rw-rw-   0        0        0     5801 2024-01-16 15:26:49.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/messages.py
--rw-rw-rw-   0        0        0    42770 2024-02-21 12:59:35.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/nodes.py
--rw-rw-rw-   0        0        0     5251 2024-01-21 17:55:38.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/syntax.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.116414 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/
--rw-rw-rw-   0        0        0     1074 2024-01-13 19:36:22.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/Canvas.py
--rw-rw-rw-   0        0        0     6901 2024-01-13 20:32:00.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/Employee.py
--rw-rw-rw-   0        0        0    11803 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTCompiler.py
--rw-rw-rw-   0        0        0     3559 2024-01-14 19:32:22.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTInterpreter.py
--rw-rw-rw-   0        0        0     6072 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTLexer.py
--rw-rw-rw-   0        0        0     6736 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTParser.py
--rw-rw-rw-   0        0        0      636 2024-01-13 14:35:10.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PaintTryhard.py
--rw-rw-rw-   0        0        0       65 2024-01-03 15:59:55.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.147670 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/
--rw-rw-rw-   0        0        0     1628 2024-01-13 18:57:59.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/__init__.py
--rw-rw-rw-   0        0        0     2954 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/boss.py
--rw-rw-rw-   0        0        0     2265 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py
--rw-rw-rw-   0        0        0     4943 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/painter.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.178915 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/
--rw-rw-rw-   0        0        0     1378 2024-03-02 14:21:02.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/AbstractProtocol.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.263549 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/
--rw-rw-rw-   0        0        0     1216 2024-03-02 10:37:15.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPHeaders.py
--rw-rw-rw-   0        0        0      310 2024-01-13 09:57:02.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPMethod.py
--rw-rw-rw-   0        0        0     3822 2024-03-02 10:54:44.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPRequest.py
--rw-rw-rw-   0        0        0     1806 2023-12-09 15:40:16.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPResponse.py
--rw-rw-rw-   0        0        0      306 2023-12-09 14:59:15.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/__init__.py
--rw-rw-rw-   0        0        0     1261 2024-03-02 13:51:31.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPConnection.py
--rw-rw-rw-   0        0        0    12459 2024-03-31 19:30:22.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPSConnection.py
--rw-rw-rw-   0        0        0     5991 2024-04-15 18:47:36.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPServer.py
--rw-rw-rw-   0        0        0     7923 2024-03-28 17:23:06.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/ProtocolConnection.py
--rw-rw-rw-   0        0        0     2589 2024-04-15 18:47:36.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/ProtocolServer.py
--rw-rw-rw-   0        0        0      944 2024-03-02 10:48:15.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TCPConnection.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.464097 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/
--rw-rw-rw-   0        0        0     2388 2024-03-28 17:36:36.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/AlertCause.py
--rw-rw-rw-   0        0        0     4694 2024-03-29 11:04:02.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/CipherSuite.py
--rw-rw-rw-   0        0        0     5969 2024-03-29 12:13:33.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/ConnectionState.py
--rw-rw-rw-   0        0        0     4200 2024-03-28 16:44:17.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/RawTLSRecord.py
--rw-rw-rw-   0        0        0       65 2024-03-02 10:25:01.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/__init__.py
--rw-rw-rw-   0        0        0     1851 2024-03-29 08:57:18.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/certificate_verifier.py
--rw-rw-rw-   0        0        0     6240 2024-03-28 06:30:56.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/extensions.py
--rw-rw-rw-   0        0        0    12644 2024-03-29 11:00:58.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/messages.py
--rw-rw-rw-   0        0        0     5135 2024-03-28 05:52:47.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/records.py
--rw-rw-rw-   0        0        0    13034 2024-03-28 11:30:36.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/tls_cryptography.py
--rw-rw-rw-   0        0        0      918 2024-04-15 18:08:31.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/URLSearchParams.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.464097 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/WS/
--rw-rw-rw-   0        0        0     4311 2024-01-13 09:57:02.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/WS/WSMessage.py
--rw-rw-rw-   0        0        0      136 2023-12-09 16:55:52.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/WS/__init__.py
--rw-rw-rw-   0        0        0     2753 2024-03-02 14:32:31.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/WSConnection.py
--rw-rw-rw-   0        0        0      628 2024-03-02 10:33:58.000000 kutil_jakubaugustyn-0.0.6/src/kutil/protocol/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.533115 kutil_jakubaugustyn-0.0.6/src/kutil/storage/
--rw-rw-rw-   0        0        0       97 2023-12-31 13:49:32.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/Cache.py
--rw-rw-rw-   0        0        0     6611 2024-03-01 16:41:47.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/Config.py
--rw-rw-rw-   0        0        0       65 2023-12-26 11:19:38.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.680264 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/
--rw-rw-rw-   0        0        0      250 2024-01-10 15:41:05.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/__init__.py
--rw-rw-rw-   0        0        0     2151 2024-02-21 16:56:37.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/bon.py
--rw-rw-rw-   0        0        0     2109 2024-01-10 17:02:50.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/converter.py
--rw-rw-rw-   0        0        0     5779 2024-02-21 16:53:13.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/decoder.py
--rw-rw-rw-   0        0        0     6588 2024-02-21 17:02:44.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/encoder.py
--rw-rw-rw-   0        0        0      761 2024-02-21 16:43:29.000000 kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/shared.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.764908 kutil_jakubaugustyn-0.0.6/src/kutil/threads/
--rw-rw-rw-   0        0        0     1721 2023-12-26 07:13:22.000000 kutil_jakubaugustyn-0.0.6/src/kutil/threads/ThreadWaiter.py
--rw-rw-rw-   0        0        0      120 2023-12-20 15:36:57.000000 kutil_jakubaugustyn-0.0.6/src/kutil/threads/__init__.py
--rw-rw-rw-   0        0        0    15510 2024-03-02 11:13:45.000000 kutil_jakubaugustyn-0.0.6/src/kutil/typing_help.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.818300 kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/
--rw-rw-rw-   0        0        0    27300 2024-04-20 12:54:07.000000 kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/MapyCZServer.py
--rw-rw-rw-   0        0        0     3167 2024-04-16 08:53:51.000000 kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/WebScraperServer.py
--rw-rw-rw-   0        0        0      187 2023-12-23 13:37:41.000000 kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 12:58:30.880808 kutil_jakubaugustyn-0.0.6/tests/
--rw-rw-rw-   0        0        0     1400 2024-02-21 17:02:14.000000 kutil_jakubaugustyn-0.0.6/tests/test_bon.py
--rw-rw-rw-   0        0        0      756 2024-03-02 10:48:38.000000 kutil_jakubaugustyn-0.0.6/tests/test_bytebuffer.py
--rw-rw-rw-   0        0        0     2174 2024-01-21 08:11:04.000000 kutil_jakubaugustyn-0.0.6/tests/test_js.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:36.286588 kutil_jakubaugustyn-0.0.7/
+-rw-rw-rw-   0        0        0     1093 2023-12-08 14:54:39.000000 kutil_jakubaugustyn-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1374 2024-04-26 15:29:36.286588 kutil_jakubaugustyn-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2024-02-28 16:16:37.000000 kutil_jakubaugustyn-0.0.7/README.md
+-rw-rw-rw-   0        0        0      824 2024-04-26 15:27:06.000000 kutil_jakubaugustyn-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 15:29:36.286588 kutil_jakubaugustyn-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:35.603762 kutil_jakubaugustyn-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:36.286588 kutil_jakubaugustyn-0.0.7/src/KUtil_jakubaugustyn.egg-info/
+-rw-rw-rw-   0        0        0     1374 2024-04-26 15:29:35.000000 kutil_jakubaugustyn-0.0.7/src/KUtil_jakubaugustyn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3719 2024-04-26 15:29:35.000000 kutil_jakubaugustyn-0.0.7/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 15:29:35.000000 kutil_jakubaugustyn-0.0.7/src/KUtil_jakubaugustyn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-26 15:29:35.000000 kutil_jakubaugustyn-0.0.7/src/KUtil_jakubaugustyn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:35.656289 kutil_jakubaugustyn-0.0.7/src/kutil/
+-rw-rw-rw-   0        0        0      302 2024-02-28 19:22:19.000000 kutil_jakubaugustyn-0.0.7/src/kutil/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:35.697296 kutil_jakubaugustyn-0.0.7/src/kutil/buffer/
+-rw-rw-rw-   0        0        0     2277 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/buffer/BidirectionalByteArray.py
+-rw-rw-rw-   0        0        0     5345 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/buffer/ByteBuffer.py
+-rw-rw-rw-   0        0        0     6151 2024-04-26 15:07:54.000000 kutil_jakubaugustyn-0.0.7/src/kutil/buffer/DataBuffer.py
+-rw-rw-rw-   0        0        0      375 2024-01-07 13:46:13.000000 kutil_jakubaugustyn-0.0.7/src/kutil/buffer/Serializable.py
+-rw-rw-rw-   0        0        0     1268 2023-12-18 18:20:16.000000 kutil_jakubaugustyn-0.0.7/src/kutil/buffer/TextOutput.py
+-rw-rw-rw-   0        0        0      335 2024-03-02 12:31:14.000000 kutil_jakubaugustyn-0.0.7/src/kutil/buffer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:35.707338 kutil_jakubaugustyn-0.0.7/src/kutil/io/
+-rw-rw-rw-   0        0        0      262 2024-04-16 09:37:01.000000 kutil_jakubaugustyn-0.0.7/src/kutil/io/__init__.py
+-rw-rw-rw-   0        0        0     2983 2023-12-26 14:36:42.000000 kutil_jakubaugustyn-0.0.7/src/kutil/io/directory.py
+-rw-rw-rw-   0        0        0     3568 2024-04-16 09:35:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/io/file.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:35.807528 kutil_jakubaugustyn-0.0.7/src/kutil/language/
+-rw-rw-rw-   0        0        0     4560 2024-02-28 19:21:38.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/AST.py
+-rw-rw-rw-   0        0        0     5772 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/BytecodeFile.py
+-rw-rw-rw-   0        0        0     1608 2024-01-16 14:45:31.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/Compiler.py
+-rw-rw-rw-   0        0        0      704 2024-01-13 11:58:11.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/Error.py
+-rw-rw-rw-   0        0        0     1601 2024-01-16 14:49:22.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/Interpreter.py
+-rw-rw-rw-   0        0        0     4116 2024-01-16 14:49:42.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/Language.py
+-rw-rw-rw-   0        0        0     1441 2024-01-16 15:20:00.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/Lexer.py
+-rw-rw-rw-   0        0        0     1797 2024-01-16 14:41:55.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/Options.py
+-rw-rw-rw-   0        0        0     1101 2024-01-16 17:36:44.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/Parser.py
+-rw-rw-rw-   0        0        0      625 2024-01-13 18:35:04.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/Stack.py
+-rw-rw-rw-   0        0        0     2020 2024-01-03 18:39:33.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/Token.py
+-rw-rw-rw-   0        0        0      389 2024-01-14 18:53:04.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:35.807528 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/
+-rw-rw-rw-   0        0        0     8372 2024-01-16 14:54:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/BrainFuck.py
+-rw-rw-rw-   0        0        0      274 2024-01-14 19:45:36.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:35.885649 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/
+-rw-rw-rw-   0        0        0    40883 2024-02-10 17:14:05.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/JSLexer.py
+-rw-rw-rw-   0        0        0     1578 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/JSOptions.py
+-rw-rw-rw-   0        0        0   142049 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/JSParser.py
+-rw-rw-rw-   0        0        0     1210 2024-01-22 17:24:55.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/Javascript.py
+-rw-rw-rw-   0        0        0     1669 2024-01-21 06:51:49.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/__init__.py
+-rw-rw-rw-   0        0        0     5070 2024-01-25 20:00:28.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/character.py
+-rw-rw-rw-   0        0        0     3458 2024-01-16 14:12:04.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/error_handler.py
+-rw-rw-rw-   0        0        0     5801 2024-01-16 15:26:49.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/messages.py
+-rw-rw-rw-   0        0        0    42792 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/nodes.py
+-rw-rw-rw-   0        0        0     5251 2024-01-21 17:55:38.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/syntax.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:35.916895 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/
+-rw-rw-rw-   0        0        0     1074 2024-01-13 19:36:22.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/Canvas.py
+-rw-rw-rw-   0        0        0     6901 2024-01-13 20:32:00.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/Employee.py
+-rw-rw-rw-   0        0        0    11806 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/PTCompiler.py
+-rw-rw-rw-   0        0        0     3559 2024-01-14 19:32:22.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/PTInterpreter.py
+-rw-rw-rw-   0        0        0     6072 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/PTLexer.py
+-rw-rw-rw-   0        0        0     6736 2024-01-16 14:57:34.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/PTParser.py
+-rw-rw-rw-   0        0        0      636 2024-01-13 14:35:10.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/PaintTryhard.py
+-rw-rw-rw-   0        0        0       65 2024-01-03 15:59:55.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:35.974553 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/jobs/
+-rw-rw-rw-   0        0        0     1628 2024-01-13 18:57:59.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/jobs/__init__.py
+-rw-rw-rw-   0        0        0     2954 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/jobs/boss.py
+-rw-rw-rw-   0        0        0     2265 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py
+-rw-rw-rw-   0        0        0     4943 2024-01-13 20:30:06.000000 kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/jobs/painter.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:36.037151 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/
+-rw-rw-rw-   0        0        0     1378 2024-03-02 14:21:02.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/AbstractProtocol.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:36.057713 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTP/
+-rw-rw-rw-   0        0        0     1216 2024-03-02 10:37:15.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTP/HTTPHeaders.py
+-rw-rw-rw-   0        0        0      310 2024-01-13 09:57:02.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTP/HTTPMethod.py
+-rw-rw-rw-   0        0        0     3822 2024-03-02 10:54:44.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTP/HTTPRequest.py
+-rw-rw-rw-   0        0        0     1806 2023-12-09 15:40:16.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTP/HTTPResponse.py
+-rw-rw-rw-   0        0        0      306 2023-12-09 14:59:15.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTP/__init__.py
+-rw-rw-rw-   0        0        0     1261 2024-03-02 13:51:31.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTPConnection.py
+-rw-rw-rw-   0        0        0    12462 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTPSConnection.py
+-rw-rw-rw-   0        0        0     6010 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTPServer.py
+-rw-rw-rw-   0        0        0     7954 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/ProtocolConnection.py
+-rw-rw-rw-   0        0        0     2605 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/ProtocolServer.py
+-rw-rw-rw-   0        0        0      944 2024-03-02 10:48:15.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TCPConnection.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:36.191443 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/
+-rw-rw-rw-   0        0        0     2388 2024-03-28 17:36:36.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/AlertCause.py
+-rw-rw-rw-   0        0        0     4694 2024-03-29 11:04:02.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/CipherSuite.py
+-rw-rw-rw-   0        0        0     6003 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/ConnectionState.py
+-rw-rw-rw-   0        0        0     4228 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/RawTLSRecord.py
+-rw-rw-rw-   0        0        0       65 2024-03-02 10:25:01.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/__init__.py
+-rw-rw-rw-   0        0        0     1888 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/certificate_verifier.py
+-rw-rw-rw-   0        0        0     6262 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/extensions.py
+-rw-rw-rw-   0        0        0    12733 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/messages.py
+-rw-rw-rw-   0        0        0     5172 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/records.py
+-rw-rw-rw-   0        0        0    13047 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/tls_cryptography.py
+-rw-rw-rw-   0        0        0      918 2024-04-15 18:08:31.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/URLSearchParams.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:36.204437 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/WS/
+-rw-rw-rw-   0        0        0     4311 2024-01-13 09:57:02.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/WS/WSMessage.py
+-rw-rw-rw-   0        0        0      136 2023-12-09 16:55:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/WS/__init__.py
+-rw-rw-rw-   0        0        0     2766 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/WSConnection.py
+-rw-rw-rw-   0        0        0      628 2024-03-02 10:33:58.000000 kutil_jakubaugustyn-0.0.7/src/kutil/protocol/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:36.208468 kutil_jakubaugustyn-0.0.7/src/kutil/storage/
+-rw-rw-rw-   0        0        0       97 2023-12-31 13:49:32.000000 kutil_jakubaugustyn-0.0.7/src/kutil/storage/Cache.py
+-rw-rw-rw-   0        0        0     6611 2024-03-01 16:41:47.000000 kutil_jakubaugustyn-0.0.7/src/kutil/storage/Config.py
+-rw-rw-rw-   0        0        0       65 2023-12-26 11:19:38.000000 kutil_jakubaugustyn-0.0.7/src/kutil/storage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:36.239717 kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/
+-rw-rw-rw-   0        0        0      250 2024-01-10 15:41:05.000000 kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/__init__.py
+-rw-rw-rw-   0        0        0     2151 2024-02-21 16:56:37.000000 kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/bon.py
+-rw-rw-rw-   0        0        0     2109 2024-01-10 17:02:50.000000 kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/converter.py
+-rw-rw-rw-   0        0        0     5779 2024-02-21 16:53:13.000000 kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/decoder.py
+-rw-rw-rw-   0        0        0     6588 2024-02-21 17:02:44.000000 kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/encoder.py
+-rw-rw-rw-   0        0        0      761 2024-02-21 16:43:29.000000 kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/shared.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:36.239717 kutil_jakubaugustyn-0.0.7/src/kutil/threads/
+-rw-rw-rw-   0        0        0     1753 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/threads/ThreadWaiter.py
+-rw-rw-rw-   0        0        0      120 2023-12-20 15:36:57.000000 kutil_jakubaugustyn-0.0.7/src/kutil/threads/__init__.py
+-rw-rw-rw-   0        0        0    15537 2024-04-26 13:56:26.000000 kutil_jakubaugustyn-0.0.7/src/kutil/typing_help.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:36.255340 kutil_jakubaugustyn-0.0.7/src/kutil/webscraper/
+-rw-rw-rw-   0        0        0    27306 2024-04-26 15:26:52.000000 kutil_jakubaugustyn-0.0.7/src/kutil/webscraper/MapyCZServer.py
+-rw-rw-rw-   0        0        0     3167 2024-04-16 08:53:51.000000 kutil_jakubaugustyn-0.0.7/src/kutil/webscraper/WebScraperServer.py
+-rw-rw-rw-   0        0        0      187 2023-12-23 13:37:41.000000 kutil_jakubaugustyn-0.0.7/src/kutil/webscraper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 15:29:36.270964 kutil_jakubaugustyn-0.0.7/tests/
+-rw-rw-rw-   0        0        0     1400 2024-02-21 17:02:14.000000 kutil_jakubaugustyn-0.0.7/tests/test_bon.py
+-rw-rw-rw-   0        0        0      756 2024-03-02 10:48:38.000000 kutil_jakubaugustyn-0.0.7/tests/test_bytebuffer.py
+-rw-rw-rw-   0        0        0     2174 2024-01-21 08:11:04.000000 kutil_jakubaugustyn-0.0.7/tests/test_js.py
```

### Comparing `kutil_jakubaugustyn-0.0.6/LICENSE` & `kutil_jakubaugustyn-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/PKG-INFO` & `kutil_jakubaugustyn-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KUtil-jakubaugustyn
-Version: 0.0.6
+Version: 0.0.7
 Summary: Kuba's Python Utilities
 Author-email: Jakub Augustýn <kubik.augustyn@post.cz>, Radek Augustýn <raugustyn@post.cz>
 Project-URL: Homepage, https://github.com/kubikaugustyn/KUtil
 Project-URL: Issues, https://github.com/kubikaugustyn/KUtil/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kutil_jakubaugustyn-0.0.6/README.md` & `kutil_jakubaugustyn-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/pyproject.toml` & `kutil_jakubaugustyn-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copied that from https://github.com/Kronuz/esprima-python/blob/master/pyproject.toml
 requires = ["setuptools>=61.0", "wheel", "setuptools_scm[toml]>=8.0"]
 build-backend = "setuptools.build_meta"
 [tool.setuptools_scm]
 
 [project]
 name = "KUtil-jakubaugustyn"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "Jakub Augustýn", email = "kubik.augustyn@post.cz" },
     { name = "Radek Augustýn", email = "raugustyn@post.cz" },
 ]
 description = "Kuba's Python Utilities"
 readme = "README.md"
 requires-python = ">=3.12"
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/PKG-INFO` & `kutil_jakubaugustyn-0.0.7/src/KUtil_jakubaugustyn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KUtil-jakubaugustyn
-Version: 0.0.6
+Version: 0.0.7
 Summary: Kuba's Python Utilities
 Author-email: Jakub Augustýn <kubik.augustyn@post.cz>, Radek Augustýn <raugustyn@post.cz>
 Project-URL: Homepage, https://github.com/kubikaugustyn/KUtil
 Project-URL: Issues, https://github.com/kubikaugustyn/KUtil/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt` & `kutil_jakubaugustyn-0.0.7/src/KUtil_jakubaugustyn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/buffer/BidirectionalByteArray.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/buffer/BidirectionalByteArray.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
-from typing import Iterable, TypeVar, Iterator
-
-TBidirectionalByteArray = TypeVar("TBidirectionalByteArray", bound="BidirectionalByteArray")
+from typing import Iterable, Iterator, Self, Optional
 
 
 class BidirectionalByteArray:
     data: bytearray
     dataNegative: bytearray
 
     def __init__(self):
@@ -23,29 +21,29 @@
             return self.data[pos]
         else:
             return self.dataNegative[abs(pos) - 1]
 
     def __len__(self) -> int:
         return len(self.data) + len(self.dataNegative)
 
-    def writeByte(self, byte: int, pos: int) -> TBidirectionalByteArray:
+    def writeByte(self, byte: int, pos: int) -> Self:
         self.extendTo(pos)
         if pos >= 0:
             self.data[pos] = byte
         else:
             self.dataNegative[abs(pos) - 1] = byte
         return self
 
     def export(self) -> bytes:
         return bytes(self.dataNegative) + bytes(self.data)
 
     def getOffset(self) -> int:
         return -len(self.dataNegative)
 
-    def reset(self, data: Iterable[int] | None = None, offset: int = 0) -> TBidirectionalByteArray:
+    def reset(self, data: Optional[Iterable[int]] = None, offset: int = 0) -> Self:
         self.data.clear()
         assert data is None
         # if data is not None:
         #     self.data.extend(data)
         return self
 
     def has(self, pos: int) -> bool:
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/buffer/ByteBuffer.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/WS/WSMessage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,138 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
-import copy
-from typing import Iterable, Self
-
-
-class OutOfBoundsReadError(BaseException):
-    pass
-
+from enum import Enum, unique
+from kutil import ByteBuffer
+from kutil.buffer.Serializable import Serializable
+
+@unique
+class WSOpcode(Enum):
+    CONTINUATION_FRAME = 0x0
+    TEXT_FRAME = 0x1
+    BINARY_FRAME = 0x2
+    CONNECTION_CLOSE = 0x8
+    PING = 0x9
+    PONG = 0xA
+
+
+class WSData:
+    isBinary: bool
+    __raw: bytes
+
+    def __init__(self, data: bytes | bytearray | str | None = None):
+        if data is None:
+            data = b''
+        self.isBinary = isinstance(data, bytes) or isinstance(data, bytearray)
+        if self.isBinary:
+            self.raw = bytes(data)
+        else:
+            self.text = data
 
-class OutOfBoundsUndoError(BaseException):
-    pass
-
-
-class ByteBuffer(Iterable[int]):
-    data: bytearray
-    pointer: int
-
-    def __init__(self, dataOrLength: Iterable[int] | int = 0):
-        self.data = bytearray(dataOrLength) if isinstance(dataOrLength, int) else bytearray(
-            dataOrLength)
-        self.pointer = 0
-
-    def readByte(self) -> int:
-        self.assertHas(1)
-        self.pointer += 1
-        return self.data[self.pointer - 1]
-
-    def readLastByte(self) -> int:
-        assert len(self.data) > 0
-        return self.data[-1]
-
-    def read(self, amount: int) -> bytearray:
-        if amount == 0:
-            return bytearray()
-        self.assertHas(amount)
-        self.pointer += amount
-        return self.data[self.pointer - amount:self.pointer]
-
-    def readLine(self, newLine: bytes = b"\r\n") -> bytearray:
-        amount: int = self.index(newLine)
-        data: bytearray = self.read(amount) if amount > 0 else bytearray()
-        self.skip(len(newLine))
-        return data
-
-    def index(self, seq: bytes) -> int:
-        self.assertHas(len(seq))
-        for i in range(len(self) - len(seq) + 1):
-            if self.data[self.pointer + i:self.pointer + i + len(seq)] == seq:
-                return i
-        raise IndexError
-
-    def skip(self, amount: int):
-        assert amount > 0
-        self.assertHas(amount)
-        self.pointer += amount
-
-    def back(self, amount: int):
-        assert amount > 0
-        self.assertHas(-amount)
-        self.pointer -= amount
+    @property
+    def superSecretRawAccess(self) -> bytes:
+        """Lol. Just don't use this if you don't know what are you doing."""
+        return self.__raw
+
+    @property
+    def raw(self) -> bytes:
+        assert self.isBinary
+        return self.__raw
+
+    @raw.setter
+    def raw(self, newBytes: bytes):
+        assert self.isBinary
+        self.__raw = newBytes
+
+    @property
+    def text(self) -> str:
+        assert not self.isBinary
+        return self.__raw.decode("utf-8")
+
+    @text.setter
+    def text(self, newText: str):
+        assert not self.isBinary
+        self.__raw = newText.encode("utf-8")
+
+    @property
+    def lenBytes(self) -> int:
+        if len(self.__raw) <= 125:
+            return 1
+        if len(self.__raw) <= 0xFFFF:
+            return 2
+        assert len(self.__raw) <= 0xFFFFFFFFFFFFFFFF
+        return 8
 
     def __len__(self) -> int:
-        return len(self.data) - self.pointer
+        return len(self.__raw)
 
-    def readRest(self) -> bytearray:
-        if len(self) == 0:
-            return bytearray(0)
-        self.assertHas(1)
-        amount = len(self)
-        self.pointer += amount
-        return self.data[self.pointer - amount:self.pointer]
-
-    def writeByte(self, byte: int, i: int = -1) -> Self:
-        if i == -1:
-            self.data.append(byte)
-        else:
-            self.data.insert(i, byte)
-        return self
-
-    def write(self, data: Iterable[int], i: int = -1) -> Self:
-        if i == -1:
-            self.data.extend(data)
-        else:
-            for byteI, byte in enumerate(data):
-                self.writeByte(byte, i + byteI)
-        return self
-
-    def export(self) -> bytes:
-        return bytes(self.data)
-
-    def reset(self, data: Iterable[int] | None = None) -> Self:
-        self.resetPointer()
-        self.data.clear()
-        if data is not None:
-            self.data.extend(data)
-        return self
-
-    def resetBeforePointer(self) -> Self:
-        self.data = self.data[self.pointer:]
-        self.resetPointer()
-        return self
-
-    def resetPointer(self) -> Self:
-        self.pointer = 0
-        return self
-
-    def assertHas(self, amount: int) -> bool:
-        if amount == 0:
-            raise ValueError("Invalid amount")
-        bytesLeft: int = len(self.data) - self.pointer
-        if amount < 0:
-            if -amount > self.pointer:
-                raise OutOfBoundsUndoError(
-                    f"Not enough bytes (going back by {-amount}, but {self.pointer} had been read)")
-        else:
-            if len(self.data) < self.pointer + amount:
-                raise OutOfBoundsReadError(
-                    f"Not enough bytes (reading {amount}, but {bytesLeft} are available)")
-        return True
-
-    def has(self, amount: int) -> bool:
-        if amount == 0:
-            return True
-        if amount < 0:
-            if -amount > self.pointer:
-                return False
-        else:
-            if len(self.data) < self.pointer + amount:
-                return False
-        return True
-
-    def copy(self) -> Self:
-        copyBuff = ByteBuffer()
-        copyBuff.data = copy.copy(self.data)
-        copyBuff.pointer = self.pointer
-        return copyBuff
-
-    def __iter__(self):
-        """Iterates over all bytes of the buffer, ignoring and not mutating the pointer."""
-        for byte in self.data:
-            yield byte
+    def mask(self, maskingKey: bytes):
+        assert len(maskingKey) == 4
+        masked: bytearray = bytearray(self.__raw)
+        for i, byte in enumerate(self.__raw):
+            masked[i] = byte ^ maskingKey[i % 4]
+        self.__raw = bytes(masked)
+
+
+class WSMessage(Serializable):
+    isFin: bool
+    # rsv: int - not used, we don't use any extension
+    opcode: WSOpcode
+    maskingKey: bytes | None
+    payload: WSData
+
+    def __init__(self):
+        super().__init__()
+        self.isFin = True
+        # self.rsv = 0
+        self.opcode = WSOpcode.TEXT_FRAME
+        self.maskingKey = None
+        self.payload = WSData()
+
+    def read(self, buff: ByteBuffer):
+        # https://en.wikipedia.org/wiki/WebSocket#Base_Framing_Protocol
+        byte: int = buff.readByte()
+        self.isFin = bool(byte & 0b10000000)
+        self.opcode = WSOpcode(byte & 0x0F)
+        byte: int = buff.readByte()
+        isMasked = bool(byte & 0b10000000)
+        payloadLength: int = byte & 0b01111111
+        if payloadLength == 126:
+            raise ValueError("Unknown endianness - big or little?")
+            # payloadLength = int.from_bytes(buff.read(2), "big", signed=False)
+        elif payloadLength == 127:
+            raise ValueError("Unknown endianness - big or little?")
+            # payloadLength = int.from_bytes(buff.read(8), "big", signed=False)
+        self.maskingKey = buff.read(4) if isMasked else None
+        self.payload = WSData(bytes(buff.read(payloadLength)))
+        self.payload.isBinary = self.opcode != WSOpcode.TEXT_FRAME
+        if isMasked:
+            self.payload.mask(self.maskingKey)
+
+    def write(self, buff: ByteBuffer):
+        byte: int = 0
+        if self.isFin:
+            byte |= 0b10000000
+        byte |= self.opcode.value
+        buff.writeByte(byte)
+        byte: int = 0
+        if self.isMasked:
+            byte |= 0b10000000
+        payloadBytes = self.payload.lenBytes
+        if payloadBytes == 1:
+            byte |= len(self.payload)
+        elif payloadBytes == 2:
+            byte |= 126
+        elif payloadBytes == 8:
+            byte |= 127
+        buff.writeByte(byte)
+        if payloadBytes > 1:
+            raise ValueError("Unknown endianness - big or little?")
+            # buff.write(len(self.payload).to_bytes(payloadBytes, "big", signed=False))
+        if self.isMasked:
+            assert len(self.maskingKey) == 4
+            buff.write(self.maskingKey)
+        buff.write(self.payload.superSecretRawAccess)
+
+    @property
+    def isMasked(self) -> bool:
+        return self.maskingKey is not None
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/buffer/TextOutput.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/buffer/TextOutput.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/io/directory.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/io/directory.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/io/file.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/io/file.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/AST.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/AST.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/BytecodeFile.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/BytecodeFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     @abstractmethod
     def write(self, buffer: ByteBuffer) -> None:
         """This is the method that should write the bytecode etc. into an ArrayBuffer,
          reading the data from self."""
         pass
 
     @abstractmethod
-    def read(self, buffer: ByteBuffer, compareCrc32Data: bytes | None) -> None:
+    def read(self, buffer: ByteBuffer, compareCrc32Data: Optional[bytes]) -> None:
         """This is the method that should read the bytecode etc. from an ArrayBuffer,
         storing the data in self.
 
         If compareCrc32Data is provided and mismatches the crc32 data of the file,
         an error is raised to let the programmer know new version of the bytecode file
         must be created (by compiling the code). The implementation depends on the subclass."""
         pass
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/Compiler.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/Compiler.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/Error.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/Error.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/Interpreter.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/Interpreter.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/Language.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/Language.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/Lexer.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/Lexer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/Options.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/Options.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/Parser.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/Parser.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/Stack.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/Stack.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/Token.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/Token.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/BrainFuck.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/BrainFuck.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSLexer.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/JSLexer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSOptions.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/JSOptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 from enum import Enum, unique
-from typing import Callable
+from typing import Callable, Optional
 
 from kutil.language.Options import UnifiedOptions
 from kutil.language.languages.javascript.error_handler import ErrorHandler
 
 
 class JSOptions(UnifiedOptions):
     ignoreComments: bool
@@ -14,15 +14,15 @@
     errorHandlerParser: ErrorHandler
     lexer: object  # JSLexer
     delegate: Callable
     module: bool
 
     range: bool
     loc: bool
-    source: str | None
+    source: Optional[str]
     tokens: bool
     comment: bool
     tolerant: bool
     classProperties: bool
 
     def __init__(self, range=False, loc=False, source=None, tokens=False, comment=False,
                  tolerant=False, classProperties=True, **options):
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/JSParser.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/JSParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 from enum import Enum, unique
-from typing import Callable, Any, overload
+from typing import Callable, Any, overload, Optional
 
 from kutil.language.languages.javascript.JSLexer import JSLexer, RawToken, SourceLocation, \
     Position, RegExp
 from kutil.language.languages.javascript.JSOptions import JSOptions
 from kutil.language.languages.javascript.error_handler import ErrorHandler
 from kutil.language.languages.javascript.messages import Messages
 from kutil.language.languages.javascript.syntax import JSNode, JSToken, TokenName
@@ -79,15 +79,15 @@
     def __init__(self, type: JSNode, value: Any, regex=None, range=None, loc=None):
         super().__init__(type, value)
         self.regex = regex
         self.range = range
         self.loc = loc
 
 
-type DelegateType = Callable[[nodes.Node, SourceLocation], nodes.Node | None]
+type DelegateType = Callable[[nodes.Node, SourceLocation], Optional[nodes.Node]]
 type GrammarParseFunctionReturn = Any
 type GrammarParseFunction = Callable[[], GrammarParseFunctionReturn]
 
 
 class JSParser(OneUseParser):
     config: Config
     errorHandler: ErrorHandler
@@ -208,15 +208,15 @@
         index = self.lastMarker.index
         line = self.scanner.lineNumber
         column = self.lastMarker.column + 1
         self.errorHandler.tolerateError(index, line, column, msg)
 
     # Throw an exception because of the token.
 
-    def unexpectedTokenError(self, token: RawToken, message: str | None = None):
+    def unexpectedTokenError(self, token: RawToken, message: Optional[str] = None):
         msg = message or Messages.UnexpectedToken
         if token:
             if not message:
                 typ = token.kind
                 if typ is JSToken.EOF:
                     msg = Messages.UnexpectedEOS
                 elif typ is JSToken.Identifier:
@@ -249,15 +249,15 @@
             return self.errorHandler.createError(index, line, column, msg)
         else:
             index = self.lastMarker.index
             line = self.lastMarker.line
             column = self.lastMarker.column + 1
             return self.errorHandler.createError(index, line, column, msg)
 
-    def throwUnexpectedToken(self, token: RawToken | None = None, message: str | None = None):
+    def throwUnexpectedToken(self, token: Optional[RawToken] = None, message: Optional[str] = None):
         """
         Always throws an exception.
         :param token: The token that caused the error
         :param message: The message with further information
         :raise JSParserError: Always
         :return:
         """
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/Javascript.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/Javascript.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/__init__.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/character.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/character.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/error_handler.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/error_handler.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/messages.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/messages.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/nodes.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 import json
 from abc import abstractmethod, ABC
-from typing import Literal as TypingLiteral, Any, Self
+from typing import Literal as TypingLiteral, Any, Self, Optional
 
 from kutil import NL
 from .character import TABULATOR
 from .syntax import JSNode
 from .JSLexer import RegExp
 from kutil.language.AST import ASTNode, AST
 
@@ -765,18 +765,18 @@
         super().__init__(properties)
         self.type = JSNode.ObjectPattern
 
 
 class Property(StaticNode):
     key: int
     computed: bool
-    value: int | None
+    value: Optional[int]
     kind: TypingLiteral["init", "get", "set"]
-    method: int | None
-    shorthand: int | None
+    method: Optional[int]
+    shorthand: Optional[int]
 
     def __init__(self, kind, key, computed, value, method, shorthand):
         super().__init__(JSNode.Property, (kind, key, computed, value, method, shorthand))
         self.key = key
         self.computed = computed
         self.value = value
         self.kind = kind
@@ -1114,15 +1114,15 @@
                 content += NL
 
         return content
 
 
 class VariableDeclarator(Node):
     id: int
-    init: int | None
+    init: Optional[int]
 
     def __init__(self, id, init):
         super().__init__(JSNode.VariableDeclarator, (id, init))
         self.id = id
         self.init = init
 
     def toString(self, ast: AST, offset: str = "", startOffset: bool = True) -> str:
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/javascript/syntax.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/javascript/syntax.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/Canvas.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/Canvas.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/Employee.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/Employee.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTCompiler.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/PTCompiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     def getContracts(self) -> Iterator[tuple[ContractInfo, PTBytecode]]:
         for contractBuff, bytecode in self.contracts:
             info: ContractInfo = ContractInfo()
             info.read(contractBuff)
             yield info, bytecode
 
-    def read(self, buffer: ByteBuffer, compareCrc32Data: bytes | None = None) -> None:
+    def read(self, buffer: ByteBuffer, compareCrc32Data: Optional[bytes] = None) -> None:
         dBuff: DataBuffer = DataBuffer(buffer)
 
         self.crc32 = dBuff.readUInt32()
         if compareCrc32Data is not None:
             buffer.back(4)
             if not dBuff.readAndCompareCRC32(compareCrc32Data):
                 raise CRC32MismatchError
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTInterpreter.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/PTInterpreter.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTLexer.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/PTLexer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PTParser.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/PTParser.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/PaintTryhard.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/PaintTryhard.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/__init__.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/boss.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/jobs/boss.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/jobs/mathematician.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/language/languages/paint_tryhard/jobs/painter.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/language/languages/paint_tryhard/jobs/painter.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/AbstractProtocol.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/AbstractProtocol.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPHeaders.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTP/HTTPHeaders.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPRequest.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTP/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTP/HTTPResponse.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTP/HTTPResponse.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPConnection.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTPConnection.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPSConnection.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTPSConnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         super().__init__(address, [TCPProtocol(self), TLSProtocol(self), HTTPProtocol(self)],
                          onData, onEstablished)
 
         self.state.setServerDomainName(address[0])
         self._sendHello()
 
     def onDataInner(self, data: Any, stoppedUnpacking: bool = False,
-                    layer: AbstractProtocol | None = None) -> bool | Any:
+                    layer: Optional[AbstractProtocol] = None) -> bool | Any:
         if not stoppedUnpacking:
             return True
         assert isinstance(layer, TLSProtocol)
         assert isinstance(data, RawTLSRecord)
 
         if isinstance(data, records.AlertRecord):
             # TODO Deal with the non-fatal errors too
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/HTTPServer.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/HTTPServer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
-from typing import Callable, Any, Self
+from typing import Callable, Any, Self, Optional
 
 from kutil.typing_help import neverCall
 
 from kutil.protocol.AbstractProtocol import AbstractProtocol, NeedMoreDataError
 from kutil.buffer.ByteBuffer import ByteBuffer
 from kutil.protocol.ProtocolConnection import ProtocolConnection
 from kutil.protocol.ProtocolServer import ProtocolServer
@@ -50,16 +50,16 @@
 
 
 class HTTPServerConnection(ProtocolConnection):
     # Note that editing the __init__ method might break the whole thing
     onData: Callable[[Self, HTTPRequest | WSMessage], None]
     didUpgradeToWS: bool
     acceptWSChecker: AcceptWSChecker
-    onWebsocketEstablishment: Callable[[Any], None] | None
-    wsConn: WSConnection | None
+    onWebsocketEstablishment: Optional[Callable[[Any], None]]
+    wsConn: Optional[WSConnection]
 
     def init(self):
         self.didUpgradeToWS = False
         self.acceptWSChecker = lambda x, y: False
         self.onWebsocketEstablishment = None  # Change if wanted, called with self as the argument
         self.wsConn = None
 
@@ -69,15 +69,15 @@
         else:
             resp: HTTPResponse = HTTPResponse(400, "Bad request", HTTPHeaders(),
                                               b'Invalid key header or version != 13 selected')
         self.sendData(resp)
         self.close(WebSocketNotAllowed())
 
     def onDataInner(self, data: HTTPRequest | WSMessage, stoppedUnpacking: bool = False,
-                    layer: AbstractProtocol | None = None) -> bool:
+                    layer: Optional[AbstractProtocol] = None) -> bool:
         assert isinstance(data, HTTPRequest) if not self.didUpgradeToWS else isinstance(data,
                                                                                         WSMessage)
         if not self.didUpgradeToWS:
             if data.headers.get("Upgrade") == "websocket" and data.headers.get(
                     "Connection") == "Upgrade":
                 if not self.acceptWSChecker(self, data):
                     # Cancel the connection if we aren't allowed to establish a WS connection
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/ProtocolConnection.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/ProtocolConnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 from threading import Thread
-from typing import Callable, Any
+from typing import Callable, Any, Optional
 from socket import socket, AF_INET, SOCK_STREAM
 from kutil.protocol.AbstractProtocol import AbstractProtocol, NeedMoreDataError, StopUnpacking
 from kutil.buffer.ByteBuffer import ByteBuffer
 
 type OnDataListener = Callable[[ProtocolConnection, Any], None]
 type OnEstablishedListener = Callable[[ProtocolEstablishedConnection], None]
-type OnCloseListener = Callable[[ProtocolConnection, Exception | None], None]
+type OnCloseListener = Callable[[ProtocolConnection, Optional[Exception]], None]
 
 
 class ConnectionClosed(Exception):
     pass
 
 
 class ProtocolConnection:
@@ -22,16 +22,16 @@
     onData: OnDataListener
     onCloseListeners: list[OnCloseListener]
     receiverThread: Thread
     closed: bool
     sock: socket
 
     def __init__(self, address: tuple[str, int], layers: list[AbstractProtocol],
-                 onData: OnDataListener, sock: socket | None = None,
-                 onClose: list[OnCloseListener] | None = None):
+                 onData: OnDataListener, sock: Optional[socket] = None,
+                 onClose: Optional[list[OnCloseListener]] = None):
         self.layers = layers
         self.onData = onData
         self.onCloseListeners = onClose if onClose is not None else []
         self.receiverThread = Thread(target=self.receive)
         self.closed = False
         if sock is None:  # If we are a client connection
             self.connect(address)
@@ -41,15 +41,15 @@
             # Note that you need to manually call startRecv()
         self.init()
 
     def init(self):
         pass  # Subclasses will overwrite this
 
     def onDataInner(self, data: Any, stoppedUnpacking: bool = False,
-                    layer: AbstractProtocol | None = None) -> bool | Any:
+                    layer: Optional[AbstractProtocol] = None) -> bool | Any:
         return True  # Subclasses will overwrite this, return whether you want to call the onData handler
 
     def startRecv(self):
         self.receiverThread.start()
 
     def connect(self, address: tuple[str, int]):
         self.sock = socket(AF_INET, SOCK_STREAM)
@@ -63,15 +63,15 @@
         assert isinstance(protocol, AbstractProtocol)
         self.layers.append(protocol)
 
     def removeProtocol(self, protocol: AbstractProtocol):
         """Removes a protocol and it's contained protocols"""
         self.layers = self.layers[:self.layers.index(protocol)]
 
-    def close(self, cause: Exception | None = None):
+    def close(self, cause: Optional[Exception] = None):
         self.closed = True
         # try:
         self.sock.close()
         # except OSError:
         #     pass
 
         for listener in self.onCloseListeners:
@@ -175,15 +175,15 @@
 
 class ProtocolEstablishedConnection(ProtocolConnection):
     _established: bool
     onEstablished: OnEstablishedListener
 
     def __init__(self, address: tuple[str, int], layers: list[AbstractProtocol],
                  onData: OnDataListener, onEstablished: OnEstablishedListener,
-                 sock: socket | None = None, onClose: list[OnCloseListener] | None = None):
+                 sock: Optional[socket] = None, onClose: Optional[list[OnCloseListener]] = None):
         self._established = False
         self.onEstablished = onEstablished
         super().__init__(address, layers, onData, sock, onClose)
 
     def markEstablished(self):
         if self._established:
             raise ValueError("Cannot re-establish an already established connection")
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/ProtocolServer.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/ProtocolServer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 from socket import socket, AF_INET, SOCK_STREAM
-from typing import Callable, Any
+from typing import Callable, Any, Optional
 
 from kutil.typing_help import neverCall
 
 from kutil.protocol.AbstractProtocol import AbstractProtocol
 from kutil.protocol.ProtocolConnection import ProtocolConnection
 
 type OnConnectionListener = Callable[
@@ -29,15 +29,15 @@
         self.layersGetter = layersGetter
         self.onConnection = onConnection
         self.closed = True
         self.connections = []
 
         self.sock.bind(address)
 
-    def listen(self, maxAmount: int | None = None):
+    def listen(self, maxAmount: Optional[int] = None):
         if maxAmount is None:
             self.sock.listen()
         else:
             self.sock.listen(maxAmount)
         self.closed = False
         i = 0
         while (i < maxAmount) if maxAmount is not None else True:
@@ -51,15 +51,15 @@
             if not self.onConnectionInner(connection):
                 continue
             connection.onData = self.onConnection(connection)
             connection.onCloseListeners.append(self.__onConnectionClose)
             self.connections.append(connection)
             connection.startRecv()
 
-    def __onConnectionClose(self, connection: ProtocolConnection, cause: Exception | None) -> None:
+    def __onConnectionClose(self, connection: ProtocolConnection, cause: Optional[Exception]) -> None:
         if connection not in self.connections:
             return
         self.connections.remove(connection)
 
     def onConnectionInner(self, conn: ProtocolConnection) -> bool:
         return True  # Rewritten by subclasses, returns whether the connection should be kept
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TCPConnection.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TCPConnection.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/AlertCause.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/AlertCause.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/CipherSuite.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/CipherSuite.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/ConnectionState.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/ConnectionState.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import os
 
 import urllib3.util
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import dh
 from enum import Enum, unique, IntEnum, auto
-from typing import Self
+from typing import Self, Optional
 
 from kutil.protocol.TLS.extensions import NamedGroup, KeyShareEntry
 from kutil.protocol.TLS.CipherSuite import CipherSuite
 from kutil.protocol.TLS.tls_cryptography import Certificate, generateKeypair
 
 
 @unique
@@ -69,20 +69,20 @@
     FINISHED_SENT = auto()
     CHANGE_CIPHER_RECEIVED = auto()
     APPLICATION_DATA = auto()
 
 
 class ConnectionState:
     state: ConnectionStateType
-    mac: MACType | None
-    keyExchangeAlgorithm: KeyExchangeAlgorithm | None
-    rootCertificate: Certificate | None
+    mac: Optional[MACType]
+    keyExchangeAlgorithm: Optional[KeyExchangeAlgorithm]
+    rootCertificate: Optional[Certificate]
     certificates: list[Certificate]
-    verifiedCertificateChain: list[Certificate] | None
-    _version: TLSVersion | None
+    verifiedCertificateChain: Optional[list[Certificate]]
+    _version: Optional[TLSVersion]
     supportedCipherSuites: list[CipherSuite] = list(CipherSuite)  # Well, lets lie to the server...
     supportedGroups: list[NamedGroup] = [
         # TODO Order and implement them all properly
         # Finite Field Groups(DHE)
         NamedGroup.ffdhe8192,
         NamedGroup.ffdhe6144,
         NamedGroup.ffdhe4096,
@@ -93,18 +93,18 @@
         NamedGroup.secp384r1,
         NamedGroup.secp521r1,
         NamedGroup.x25519,
         NamedGroup.x448
     ]
     clientSharedKeys: list[KeyShareEntry]
     _privateKeys: dict[NamedGroup, dh.DHPrivateKey]
-    pendingCipher: CipherSuite | None
-    _selectedCipher: CipherSuite | None
+    pendingCipher: Optional[CipherSuite]
+    _selectedCipher: Optional[CipherSuite]
     sessionID: bytes
-    serverDomainName: str | None
+    serverDomainName: Optional[str]
 
     def __init__(self):
         self.state = ConnectionStateType.INIT
         self.mac = None
         self.keyExchangeAlgorithm = None
         self.rootCertificate = None
         self.certificates = []
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/RawTLSRecord.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/RawTLSRecord.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 from enum import IntEnum, unique, Enum
-from typing import Final, Self
+from typing import Final, Self, Optional
 
 from kutil.protocol.AbstractProtocol import NeedMoreDataError
 
 from kutil.protocol.TLS.ConnectionState import ConnectionState, ConnectionStateType, TLSVersion
 
 from kutil.protocol.TLS.AlertCause import AlertCause
 
@@ -29,21 +29,21 @@
 class RawTLSRecordNeedMoreDataError(NeedMoreDataError):
     pass
 
 
 class RawTLSRecord(Serializable):
     connectionState: ConnectionState
     contentType: TLSRecordType
-    payload: bytes | None
-    mac: bytes | None
-    padding: bytes | None
+    payload: Optional[bytes]
+    mac: Optional[bytes]
+    padding: Optional[bytes]
 
     def __init__(self, contentType: TLSRecordType, connectionState: ConnectionState,
-                 payload: bytes | None = None, mac: bytes | None = None,
-                 padding: bytes | None = None) -> None:
+                 payload: Optional[bytes] = None, mac: Optional[bytes] = None,
+                 padding: Optional[bytes] = None) -> None:
         self.connectionState = connectionState
         self.contentType = contentType
         self.payload = payload
         self.mac = mac
         self.padding = padding
 
     def write(self, buff: ByteBuffer):
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/certificate_verifier.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/certificate_verifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 #  -*- coding: utf-8 -*-
 """
 This is the crucial point of the connection. If you find any bugs that could lead to auth bypass,
 create an issue on GitHub here: https://github.com/kubikaugustyn/KUtil/issues/new
 """
 __author__ = "kubik.augustyn@post.cz"
 
+from typing import Optional
+
 from cryptography.x509 import DNSName, load_pem_x509_certificates
 from cryptography.x509.verification import PolicyBuilder, Store, VerificationError
 import certifi
 from datetime import datetime
 
 from kutil.protocol.TLS.ConnectionState import ConnectionState
 
-_STORE: Store | None = None
+_STORE: Optional[Store] = None
 
 
 def getStore() -> Store:
     global _STORE
     if _STORE is not None:
         return _STORE
     with open(certifi.where(), "rb") as pemCerts:
         _STORE = Store(load_pem_x509_certificates(pemCerts.read()))
     return _STORE
 
 
 # https://datatracker.ietf.org/doc/html/rfc5280
 # https://cryptography.io/en/latest/x509/verification/
 # This is the crucial point of the connection - is the certificate valid?
-def verifyPeerCertificates(state: ConnectionState) -> tuple[int, Exception | None]:
+def verifyPeerCertificates(state: ConnectionState) -> tuple[int, Optional[Exception]]:
     """
     Verifies the provided certificate's validity.
     :param state: Connection state containing certificates to check
     :return: [error code + cause] or [-1 and None] if no error occurred
     """
     state.verifiedCertificateChain = None
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/extensions.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/extensions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 from enum import IntEnum, unique
-from typing import Final
+from typing import Final, Optional
 
 from kutil.buffer.DataBuffer import DataBuffer
 from kutil.buffer.ByteBuffer import ByteBuffer
 
 from kutil.buffer.Serializable import Serializable
 
 
@@ -37,15 +37,15 @@
     KEY_SHARE = 51
 
 
 class Extension(Serializable):
     extensionType: ExtensionType
     payload: bytes
 
-    def __init__(self, extensionType: ExtensionType | None, payload: bytes | None = None):
+    def __init__(self, extensionType: Optional[ExtensionType], payload: Optional[bytes] = None):
         self.extensionType = extensionType
         self.payload = payload if payload is not None else b''
 
     def write(self, buff: ByteBuffer):
         dBuff = DataBuffer(buff)
         dBuff.writeUInt16(self.extensionType.value)
         dBuff.writeUInt16(len(self.payload))
@@ -90,15 +90,15 @@
 ECDHE_GROUPS: Final[set[NamedGroup]] = {NamedGroup.secp256r1, NamedGroup.secp384r1,
                                         NamedGroup.secp521r1}
 
 
 class SupportedGroupsExtension(Extension):
     namedGroups: list[NamedGroup]
 
-    def __init__(self, namedGroups: list[NamedGroup] | None = None):
+    def __init__(self, namedGroups: Optional[list[NamedGroup]] = None):
         self.namedGroups = namedGroups if namedGroups is not None else []
         super().__init__(ExtensionType.SUPPORTED_GROUPS)
 
     def write(self, buff: ByteBuffer):
         b = DataBuffer()
         assert len(self.namedGroups) > 0
         b.writeUInt16(len(self.namedGroups) * 2)
@@ -132,15 +132,15 @@
         assert length > 0
         self.keyExchange = buff.read(length)
 
 
 class KeyShareExtension(Extension):
     clientShares: list[KeyShareEntry]
 
-    def __init__(self, clientShares: list[KeyShareEntry] | None = None):
+    def __init__(self, clientShares: Optional[list[KeyShareEntry]] = None):
         self.clientShares = clientShares if clientShares is not None else []
         super().__init__(ExtensionType.KEY_SHARE)
 
     def write(self, buff: ByteBuffer):
         # TODO Don't use 2 buffers
         payloadBuff = ByteBuffer()
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/messages.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 import os
 import sys
 from enum import IntEnum, unique
+from typing import Optional
 
 from kutil.protocol.TLS.extensions import Extension, readExtension, readExtensions, writeExtensions, \
     NamedGroup
 
 from kutil.protocol.TLS.CipherSuite import CipherSuite, CERTIFICATE_SUITES, SRP_ALL_SUITES, \
     DH_ALL_SUITES, ECDH_ALL_SUITES
 
@@ -38,15 +39,15 @@
     Finished = 20
 
 
 class Message(Serializable):
     messageType: MessageType
     payload: bytes
 
-    def __init__(self, messageType: MessageType | None = None, payload: bytes | None = None):
+    def __init__(self, messageType: Optional[MessageType] = None, payload: Optional[bytes] = None):
         self.messageType = messageType
         self.payload = payload
 
     @staticmethod
     def readType(dBuff: DataBuffer, rollback: bool = False) -> MessageType:
         msgType: MessageType = MessageType(dBuff.readUInt8())
         if rollback:
@@ -77,18 +78,18 @@
     protocolVersion: TLSVersion
     random: bytes
     sessionID: bytes
     cipherSuites: list[CipherSuite]
     compressionMethods: bytes
     extensions: list[Extension]
 
-    def __init__(self, protocolVersion: TLSVersion, random: bytes | None = None,
-                 sessionID: bytes | None = None, cipherSuites: list[CipherSuite] | None = None,
-                 compressionMethods: bytes | None = None,
-                 extensions: list[Extension] | None = None):
+    def __init__(self, protocolVersion: TLSVersion, random: Optional[bytes] = None,
+                 sessionID: Optional[bytes] = None, cipherSuites: Optional[list[CipherSuite]] = None,
+                 compressionMethods: Optional[bytes] = None,
+                 extensions: Optional[list[Extension]] = None):
         self.protocolVersion = protocolVersion
         self.random = random if random is not None else os.urandom(32)
         self.sessionID = sessionID if sessionID is not None else b''
         self.cipherSuites = cipherSuites if cipherSuites is not None else []
         self.compressionMethods = compressionMethods if \
             compressionMethods is not None else b''
         self.extensions = extensions if extensions is not None else []
@@ -122,17 +123,17 @@
     protocolVersion: TLSVersion
     random: bytes
     sessionIDEcho: bytes
     cipherSuite: CipherSuite
     compressionMethod: int
     extensions: list[Extension]
 
-    def __init__(self, protocolVersion: TLSVersion | None = None, random: bytes | None = None,
-                 sessionIDEcho: bytes | None = None, cipherSuite: CipherSuite | None = None,
-                 compressionMethod: int | None = None, extensions: list[Extension] | None = None):
+    def __init__(self, protocolVersion: Optional[TLSVersion] = None, random: Optional[bytes] = None,
+                 sessionIDEcho: Optional[bytes] = None, cipherSuite: Optional[CipherSuite] = None,
+                 compressionMethod: Optional[int] = None, extensions: Optional[list[Extension]] = None):
         self.protocolVersion = protocolVersion
         self.random = random if random is not None else os.urandom(32)
         self.sessionIDEcho = sessionIDEcho if sessionIDEcho is not None else b''
         self.cipherSuite = cipherSuite if cipherSuite is not None else None
         self.compressionMethod = compressionMethod if compressionMethod is not None else None
         self.extensions = extensions if extensions is not None else []
 
@@ -168,16 +169,16 @@
     RawPublicKey = 2
 
 
 class CertificateMessage(Message):
     certRequestCtx: bytes  # certificate_request_context
     certificates: list[Certificate | AnyPublicKey]
 
-    def __init__(self, certRequestCtx: bytes | None = None,
-                 certificates: list[Certificate | AnyPublicKey] | None = None):
+    def __init__(self, certRequestCtx: Optional[bytes] = None,
+                 certificates: Optional[list[Certificate | AnyPublicKey]] = None):
         self.certRequestCtx = certRequestCtx or b''
         self.certificates = certificates or []
         super().__init__(MessageType.Certificate, b'')
 
     def read(self, buff: ByteBuffer):
         super().read(buff)
         b = ByteBuffer(self.payload)
@@ -209,15 +210,15 @@
 
 
 # https://datatracker.ietf.org/doc/html/rfc8446#section-4.4.4
 class FinishedMessage(Message):
     macSize: int
     verifyData: bytes
 
-    def __init__(self, macSize: int, verifyData: bytes | None = None):
+    def __init__(self, macSize: int, verifyData: Optional[bytes] = None):
         self.macSize = macSize
         self.verifyData = verifyData if verifyData else b''
         super().__init__(MessageType.Finished, b'')
 
     def read(self, buff: ByteBuffer):
         super().read(buff)
         assert len(self.payload) == self.macSize
@@ -235,17 +236,17 @@
     version: TLSVersion
 
     srp_A: int
     dh_Yc: int
     ecdh_Yc: bytes
     encryptedPreMasterSecret: bytes
 
-    def __init__(self, cipherSuite: CipherSuite, version: TLSVersion, srp_A: int | None = None,
-                 dh_Yc: int | None = None, ecdh_Yc: bytes | None = None,
-                 encryptedPreMasterSecret: bytes | None = None):
+    def __init__(self, cipherSuite: CipherSuite, version: TLSVersion, srp_A: Optional[int] = None,
+                 dh_Yc: Optional[int] = None, ecdh_Yc: Optional[bytes] = None,
+                 encryptedPreMasterSecret: Optional[bytes] = None):
         self.cipherSuite = cipherSuite
         self.version = version
 
         self.srp_A = srp_A or 0
         self.dh_Yc = dh_Yc or 0
         self.ecdh_Yc = ecdh_Yc or b''
         self.encryptedPreMasterSecret = encryptedPreMasterSecret or b''
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/records.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/records.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
+from typing import Optional
+
 from kutil.protocol.TLS import messages
 
 from kutil.protocol.TLS.ConnectionState import ConnectionState, ConnectionStateType
 
 from kutil import DataBuffer, ByteBuffer
 from kutil.protocol.TLS.RawTLSRecord import RawTLSRecord, TLSRecordType
 from kutil.protocol.TLS.AlertCause import AlertFatality, FATAL, WARNING_FATAL, WARNING, alertErrors
@@ -12,15 +14,15 @@
 
 
 # https://en.wikipedia.org/wiki/Transport_Layer_Security#Handshake_protocol
 class HandshakeRecord(RawTLSRecord):
     messages: list[Message]
 
     def __init__(self, connectionState: ConnectionState,
-                 messages: list[Message] | None = None) -> None:
+                 messages: Optional[list[Message]] = None) -> None:
         self.messages = messages if messages is not None else []
         super().__init__(TLSRecordType.Handshake, connectionState)
 
     def write(self, buff: ByteBuffer):
         payloadBuff: DataBuffer = DataBuffer()
 
         for msg in self.messages:
@@ -144,10 +146,10 @@
         if newProtocolType != 1:
             raise ValueError(f"Invalid protocol type: {newProtocolType}")
         self._protocolType = newProtocolType
 
 
 # https://en.wikipedia.org/wiki/Transport_Layer_Security#Application_protocol
 class ApplicationRecord(RawTLSRecord):
-    def __init__(self, connectionState: ConnectionState, payload: bytes | None = None) -> None:
+    def __init__(self, connectionState: ConnectionState, payload: Optional[bytes] = None) -> None:
         assert connectionState.state == ConnectionStateType.APPLICATION_DATA
         super().__init__(TLSRecordType.Application, connectionState, payload)
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/TLS/tls_cryptography.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/TLS/tls_cryptography.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 import math
 import re
-from typing import Final
+from typing import Final, Optional
 
 from cryptography.x509 import load_der_x509_certificate, Certificate
 from cryptography.hazmat.primitives.asymmetric import dh, ec, x25519, x448
 from cryptography.hazmat.primitives.serialization import load_der_public_key
 
 from kutil.protocol.TLS.extensions import NamedGroup, DHE_GROUPS, ECDHE_GROUPS
 
@@ -254,15 +254,15 @@
 ###################################
 #            Combined             #
 ###################################
 type AnyPrivateKey = dh.DHPrivateKey | ec.EllipticCurvePrivateKey | x25519.X25519PrivateKey | x448.X448PrivateKey
 type AnyPublicKey = dh.DHPublicKey | ec.EllipticCurvePublicKey | x25519.X25519PublicKey | x448.X448PublicKey
 
 
-def generateKeypair(group: NamedGroup) -> tuple[AnyPrivateKey, dh.DHPublicKey | None]:
+def generateKeypair(group: NamedGroup) -> tuple[AnyPrivateKey, Optional[dh.DHPublicKey]]:
     if group in DHE_GROUPS:
         return generateDHEKeypair(group)
     elif group in ECDHE_GROUPS:
         return generateECDHEPrivateKey(group), None
     elif group is NamedGroup.x25519:
         return generateX25519PrivateKey(), None
     elif group is NamedGroup.x448:
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/URLSearchParams.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/URLSearchParams.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/WSConnection.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/WSConnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 from base64 import b64encode
 from hashlib import sha1
-from typing import Any
+from typing import Any, Optional
 
 from kutil.protocol.AbstractProtocol import AbstractProtocol, NeedMoreDataError
 from kutil.buffer.ByteBuffer import ByteBuffer
 from kutil.protocol.ProtocolConnection import ProtocolConnection, ConnectionClosed
 from kutil.protocol.WS import WSMessage, WSOpcode, WSData
 
 
@@ -52,15 +52,15 @@
 class WSConnection(ProtocolConnection):
     dataBuffer: ByteBuffer
 
     def init(self):
         self.dataBuffer = ByteBuffer()
 
     def onDataInner(self, data: WSMessage, stoppedUnpacking: bool = False,
-                    layer: AbstractProtocol | None = None) -> bool | WSData:
+                    layer: Optional[AbstractProtocol] = None) -> bool | WSData:
         if data.opcode in (WSOpcode.BINARY_FRAME, WSOpcode.TEXT_FRAME):
             self.dataBuffer.write(data.payload.superSecretRawAccess)
             if data.isFin:
                 message: WSData = WSData(self.dataBuffer.export())
                 message.isBinary = data.opcode == WSOpcode.BINARY_FRAME
                 return message
             return False
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/protocol/__init__.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/storage/Config.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/storage/Config.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/bon.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/bon.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/converter.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/converter.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/decoder.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/decoder.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/encoder.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/encoder.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/storage/bon/shared.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/storage/bon/shared.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/threads/ThreadWaiter.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/threads/ThreadWaiter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #  -*- coding: utf-8 -*-
 __author__ = "kubik.augustyn@post.cz"
 
 from threading import Semaphore
+from typing import Optional
 
 
 class ThreadWaiter:
     canBeWaiting: bool
     waitingThreadCount: int
     semaphore: Semaphore
 
     def __init__(self):
         self.canBeWaiting = True
         self.waitingThreadCount = 0
         self.semaphore = Semaphore(0)
 
-    def wait(self, maxTime: float | None = None) -> bool:
+    def wait(self, maxTime: Optional[float] = None) -> bool:
         """
         Blocks the caller thread until the release() method is called. If it was called before the wait call,
         the thread execution will immediately continue.
         :param maxTime: The maximum time the thread can be blocked for, otherwise times out
         :return: Whether the wait completed successfully (True) or timed out (False)
         """
         if not self.canBeWaiting:
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/typing_help.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/typing_help.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import inspect
 import sys
 from typing import *
 
 # Exported things
 from frozenlist import FrozenList
 from itertools import chain
+from copy import deepcopy
 
 
 # Class decorators
 def singleton(cls):
     """
     A decorator, making a class be able to only have one instance. If you try to instantiate it
     multiple times, the same instance will be returned.
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/MapyCZServer.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/webscraper/MapyCZServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
         uri: str = f"https://api.mapy.cz/v1/maptiles/{mapSet.value}/tiles.json?apikey=API&lang={lang}"
         r = self.__authorizedGetRequest(uri)
         return r.content
 
     def __scrape(self, x: int, y: int, zoom: int, tileSize: str, mapSet: MapSet, lang: str,
                  canScrapeAround: bool = True) -> bytes:
         # print(f'X: {x}, Y: {y}, Zoom: {zoom}, tile size: {tileSize}, kind: {mapSet.name}, language: {lang}')
-        cachedValue: bytes | None = self.__obtainFromCache(x, y, zoom, tileSize, mapSet, lang)
+        cachedValue: Optional[bytes] = self.__obtainFromCache(x, y, zoom, tileSize, mapSet, lang)
         if cachedValue is not None:
             return cachedValue
         # https://api.mapy.cz/v1/maptiles/outdoor/tiles.json?apikey=virtual-
         # https://api.mapy.cz/v1/docs/maptiles/#/
         # uri: str = f"https://api.mapy.cz/v1/maptiles/outdoor/256@2x/{zoom}/{x}/{y}?apikey=API"
         uri: str = f"https://api.mapy.cz/v1/maptiles/{mapSet.value}/{tileSize}/{zoom}/{x}/{y}?apikey=API&lang={lang}"
         r = self.__authorizedGetRequest(uri)
@@ -450,15 +450,15 @@
         if self.__cachePath is None:
             return
         self.__cacheSizeLimiterWaiter.release()
         with open(self.__getCacheFilePath(x, y, zoom, tileSize, mapSet, lang), "wb+") as f:
             f.write(data)
 
     def __obtainFromCache(self, x: int, y: int, zoom: int, tileSize: str, mapSet: MapSet,
-                          lang: str) -> bytes | None:
+                          lang: str) -> Optional[bytes]:
         if self.__cachePath is None:
             return None
         path = self.__getCacheFilePath(x, y, zoom, tileSize, mapSet, lang)
         if not os.path.exists(path):
             return None
         with open(path, "rb") as f:
             return f.read()
```

### Comparing `kutil_jakubaugustyn-0.0.6/src/kutil/webscraper/WebScraperServer.py` & `kutil_jakubaugustyn-0.0.7/src/kutil/webscraper/WebScraperServer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/tests/test_bon.py` & `kutil_jakubaugustyn-0.0.7/tests/test_bon.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/tests/test_bytebuffer.py` & `kutil_jakubaugustyn-0.0.7/tests/test_bytebuffer.py`

 * *Files identical despite different names*

### Comparing `kutil_jakubaugustyn-0.0.6/tests/test_js.py` & `kutil_jakubaugustyn-0.0.7/tests/test_js.py`

 * *Files identical despite different names*

