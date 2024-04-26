# Comparing `tmp/momonga-0.0.5-py3-none-any.whl.zip` & `tmp/momonga-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15388 bytes, number of entries: 11
+Zip file size: 15369 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      136 b- defN 24-Apr-20 08:49 momonga/__init__.py
--rw-rw-r--  2.0 unx    15159 b- defN 24-Apr-24 10:04 momonga/momonga.py
+-rw-rw-r--  2.0 unx    15034 b- defN 24-Apr-26 01:36 momonga/momonga.py
 -rw-rw-r--  2.0 unx      959 b- defN 24-Apr-23 04:16 momonga/momonga_exception.py
 -rw-rw-r--  2.0 unx     2698 b- defN 24-Apr-24 09:24 momonga/momonga_response.py
--rw-rw-r--  2.0 unx    11967 b- defN 24-Apr-24 09:20 momonga/momonga_session_manager.py
+-rw-rw-r--  2.0 unx    11915 b- defN 24-Apr-26 00:54 momonga/momonga_session_manager.py
 -rw-rw-r--  2.0 unx     9392 b- defN 24-Apr-24 09:23 momonga/momonga_sk_wrapper.py
--rw-rw-r--  2.0 unx     1061 b- defN 24-Apr-24 10:26 momonga-0.0.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx    10268 b- defN 24-Apr-24 10:26 momonga-0.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 10:26 momonga-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 24-Apr-24 10:26 momonga-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      883 b- defN 24-Apr-24 10:26 momonga-0.0.5.dist-info/RECORD
-11 files, 52623 bytes uncompressed, 13902 bytes compressed:  73.6%
+-rw-rw-r--  2.0 unx     1061 b- defN 24-Apr-26 01:38 momonga-0.0.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    10353 b- defN 24-Apr-26 01:38 momonga-0.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-26 01:38 momonga-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 24-Apr-26 01:38 momonga-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      883 b- defN 24-Apr-26 01:38 momonga-0.0.6.dist-info/RECORD
+11 files, 52531 bytes uncompressed, 13883 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: momonga/momonga_session_manager.py
 Comment: 
 
 Filename: momonga/momonga_sk_wrapper.py
 Comment: 
 
-Filename: momonga-0.0.5.dist-info/LICENSE
+Filename: momonga-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: momonga-0.0.5.dist-info/METADATA
+Filename: momonga-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: momonga-0.0.5.dist-info/WHEEL
+Filename: momonga-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: momonga-0.0.5.dist-info/top_level.txt
+Filename: momonga-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: momonga-0.0.5.dist-info/RECORD
+Filename: momonga-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## momonga/momonga.py

```diff
@@ -61,15 +61,15 @@
         logger.info('Momonga is closed.')
 
     def __build_request_payload(self,
                                 tid: int,
                                 epc: int,
                                 edt: bytes = b'',
                                ) -> bytes:
-        ehd  = b'\x10\x81'     # econet lite edata format 1
+        ehd  = b'\x10\x81'     # echonet lite edata format 1
         tid  = tid.to_bytes(4, 'big')[-2:]
         seoj = b'\x05\xFF\x01' # controller class
         deoj = b'\x02\x88\x01' # low-voltage smart electric energy meter class
         opc  = b'\x01'
         if edt:
             esv = b'\x61' # setc
         else:
@@ -81,34 +81,38 @@
 
     def __extract_response_payload(self,
                                    data: bytes,
                                    tid: int,
                                    epc: int,
                                   ):
         ehd = data[0:2]
-        if  ehd != b'\x10\x81': # econet lite edata format 1
-            raise MomongaResponseNotExpected('The data format is not Econet Lite EDATA format 1')
+        if  ehd != b'\x10\x81': # echonet lite edata format 1
+            raise MomongaResponseNotExpected('The data format is not ECHONET Lite EDATA format 1')
 
         if int.from_bytes(data[2:4], 'big') != tid:
             raise MomongaResponseNotExpected('The transaction ID does not match.')
 
         seoj = data[4:7]
         if seoj != b'\x02\x88\x01': # low-voltage smart electric energy meter class
             raise MomongaResponseNotExpected('The source is not a smart meter.')
 
         deoj = data[7:10]
         if deoj != b'\x05\xFF\x01': # controller class
             raise MomongaResponseNotExpected('The destination is not a controller.')
 
+        if data[12] != epc:
+            raise MomongaResponseNotExpected('The property code does not match. EPC: %X' % epc)
+
         esv = data[10]
         if 0x50 <= esv <= 0x5F:
             raise MomongaResponseNotPossible('The target smart meter could not respond. ESV: %X' % esv)
+
         opc = data[11]
         assert opc == 1, 'Unexpected packet format. OPC is expected 1 but %d was set.' % opc
-        epc = data[12]
+
         pdc = data[13]
         if pdc == 0:
             edt = None
         else:
             edt = data[14:14+pdc]
 
         return {'ehd': ehd, 'tid': tid, 'seoj': seoj, 'deoj': deoj, 'esv': esv,
@@ -138,18 +142,18 @@
                     if param == '00':
                         logger.info('Successfully transmitted a packet for "%X" request.' % (epc))
                         continue
                     elif param == '01':
                         logger.warning('Retransmitting the packet for "%X" request.' % (epc))
                         break # to rexmit
                     elif param == '02':
-                        logger.warning('Automatically retrying to transmit the packet for "%X" request.' % (epc))
+                        logger.warning('Transmitting neighbor solicitation packets.' % (epc))
                         continue
                 elif res.startswith('EVENT 02'):
-                    logger.info('Successfully retransmitted the packet for "%X" request.' % (epc))
+                    logger.info('Received a neighbor advertisement packet.' % (epc))
                     continue
                 elif res.startswith('ERXUDP'):
                     udp_pkt = SkEventRxUdp([res])
                     if not (udp_pkt.src_port == udp_pkt.dst_port == 0x0E1A):
                         continue
                     elif udp_pkt.side != 0:
                         continue
@@ -231,15 +235,15 @@
         return unit_map.get(unit_index)
 
     def get_historical_cumulative_energy_1(self,
                                            day: int = 0,
                                            reverse: bool = False,
                                           ) -> list:
         self.__prepare_to_get_cumulative_energy()
-        self.set_day_for_which_to_retrieve_historical_data_1(day)
+        self.set_day_for_historical_data_1(day)
 
         if reverse is False:
             epc = 0xE2
         else:
             epc = 0xE4
 
         res = self.__request(epc)
@@ -259,20 +263,20 @@
             else:
                 cumulative_energy *= self.energy_coefficient
                 cumulative_energy *= self.energy_unit 
             historical_cumulative_energy.append({'timestamp': timestamp, 'cumulative energy': cumulative_energy})
             timestamp += datetime.timedelta(minutes=30)
         return historical_cumulative_energy
  
-    def set_day_for_which_to_retrieve_historical_data_1(self,
-                                                        day: int = 0,
-                                                       ) -> None:
+    def set_day_for_historical_data_1(self,
+                                      day: int = 0,
+                                     ) -> None:
         self.__request(0xE5, day.to_bytes(1, 'big'))
 
-    def get_day_for_which_to_retrieve_historical_data_1(self) -> int:
+    def get_day_for_historical_data_1(self) -> int:
         res = self.__request(0xE5)
         day = int.from_bytes(res.get('edt'), 'big')
         return day
  
     def get_instantaneous_power(self) -> float:
         res = self.__request(0xE7)
         power = int.from_bytes(res.get('edt'), 'big', signed=True)
@@ -312,15 +316,15 @@
                                            timestamp: datetime.datetime = None,
                                            num_of_data_points: int = 12,
                                           ) -> list:
         if timestamp is None:
             timestamp = datetime.datetime.now()
 
         self.__prepare_to_get_cumulative_energy()
-        self.set_time_for_which_to_retrieve_historical_data_2(timestamp, num_of_data_points)
+        self.set_time_for_historical_data_2(timestamp, num_of_data_points)
 
         res = self.__request(0xEC)
         edt = res.get('edt')
         year = int.from_bytes(edt[0:2], 'big')
         num_of_data_points = edt[6]
         energy_data_points = edt[7:]
 
@@ -345,33 +349,33 @@
             historical_cumulative_energy.append(
                 {'timestamp': timestamp,
                  'cumulative energy': {'normal direction': normal_direction_energy,
                                        'reverse direction': reverse_direction_energy}})
             timestamp -= datetime.timedelta(minutes=30)
         return historical_cumulative_energy
  
-    def set_time_for_which_to_retrieve_historical_data_2(self,
-                                                         timestamp: datetime.datetime,
-                                                         num_of_data_points: int = 12,
-                                                        ) -> None:
+    def set_time_for_historical_data_2(self,
+                                       timestamp: datetime.datetime,
+                                       num_of_data_points: int = 12,
+                                      ) -> None:
         year = timestamp.year.to_bytes(2, 'big')
         month = timestamp.month.to_bytes(1, 'big')
         day = timestamp.day.to_bytes(1, 'big')
         hour = timestamp.hour.to_bytes(1, 'big')
 
         if 0 <= timestamp.minute < 30:
             minute = 0
         else:
             minute = 30
 
         minute = minute.to_bytes(1, 'big')
         num_of_data_points = num_of_data_points.to_bytes(1, 'big')
         self.__request(0xED, year + month + day + hour + minute + num_of_data_points)
 
-    def get_time_for_which_to_retrieve_historical_data_2(self) -> dict:
+    def get_time_for_historical_data_2(self) -> dict:
         res = self.__request(0xED)
         edt = res.get('edt')
         year = int.from_bytes(edt[0:2], 'big')
         if year == 0xFFFF:
             timestamp = None
         else:
             timestamp = datetime.datetime(year, edt[2], edt[3], edt[4], edt[5])
```

## momonga/momonga_session_manager.py

```diff
@@ -102,15 +102,15 @@
             # to set a pan id.
             self.skw.sksreg('S3', self.pan_id)
             # to establish a pana session.
             try:
                 self.skw.skjoin(self.smart_meter_addr)
                 self.session_established = True
                 logger.info('A PANA session has been established.')
-            except MomongaSkJoinFailure as e:
+            except MomongaSkJoinFailure:
                 logger.error('Gave up to establish a PANA session. Check the Route-B ID and password. Then try again.')
                 raise MomongaSkJoinFailure('Gave up to establish a PANA session. Check the Route-B ID and password. Then try again.')
 
             while not self.pkt_sbsc_q.empty():
                 self.pkt_sbsc_q.get()
             while not self.recv_q.empty():
                 self.recv_q.get()
@@ -122,41 +122,40 @@
             self.skw.subscribers.update({'pkt_sbsc_q': self.pkt_sbsc_q})
 
             self.receiver_th.start()
 
             logger.info('A Momonga session is open.')
             return self
         except Exception as e:
-            logger.error('Could not open a Momonga session. %s: %s' % (type(e).__name__, str(e)))
+            logger.error('Could not open a Momonga session. %s: %s' % (type(e).__name__, e))
             self.close()
             raise e
 
     def close(self) -> None:
         logger.info('Closing the Momonga session...')
-        for _ in range(3):
-            self.rejoin_lock.acquire(timeout=200)
 
-            if self.session_established is True:
-                try:
-                    self.session_established = False
-                    logger.info('Terminating the PANA session...')
-                    self.skw.skterm()
-                    break
-                except MomongaSkCommandFailedToExecute:
-                    logger.warning('Failed to terminate the PANA session.')
-                finally:
-                    self.rejoin_lock.release()
-            else:
+        if self.rejoin_lock.acquire(timeout=120) is False:
+            logger.warning('Failed to acquire "rejoin_lock".')
+
+        if self.session_established is True:
+            try:
+                self.session_established = False
+                logger.info('Terminating the PANA session...')
+                self.skw.skterm()
+            except Exception as e:
+                logger.warning('Failed to terminate the PANA session. %s: %s' % (type(e).__name__, e))
+            finally:
                 self.rejoin_lock.release()
-                break
-            time.sleep(3)
+        else:
+            self.rejoin_lock.release()
 
-        if self.receiver_th is not None and self.receiver_th.is_alive():
-            self.pkt_sbsc_q.put('__CLOSE__') # to close the receiver thread.
-            self.receiver_th.join()
+        if self.receiver_th is not None:
+            if self.receiver_th.is_alive():
+                self.pkt_sbsc_q.put('__CLOSE__') # to close the receiver thread.
+                self.receiver_th.join()
             self.receiver_th = None
 
         if self.skw.subscribers.get('pkt_sbsc_q') is not None:
             self.skw.subscribers.pop('pkt_sbsc_q')
 
         self.unrestrict_to_xmit(force=True)
 
@@ -189,14 +188,16 @@
                         try:
                             self.skw.skjoin(self.smart_meter_addr)
                         except MomongaSkJoinFailure as e:
                             logger.error('%s Close Momonga and open it again.' % e)
                             raise MomongaNeedToReopen('%s Close Momonga and open it again.' % e)
                         finally:
                             self.rejoin_lock.release()
+                    else:
+                        self.rejoin_lock.release()
                 elif res.startswith('EVENT 25'):
                     logger.debug('Successfully rejoined the PAN.')
                     self.session_established = True
                     self.unrestrict_to_xmit()
                 elif res.startswith('EVENT 32'):
                     logger.warning('The transmission rate limit has been exceeded.')
                     self.restrict_to_xmit()
@@ -218,70 +219,71 @@
             self.receiver_exception = e
 
         logger.debug('The packet receiver has been stopped.')
 
     def xmitter(self,
                 data: bytes,
                ) -> None:
-        logger.debug('Trying to acquire "rejoin_lock".')
-        if self.rejoin_lock.acquire(timeout=600) is False: # waiting for rejoining the PAN
-            logger.error('Rejoining a PANA session may fail. Close Momonga and open it again.')
-            raise MomongaNeedToReopen('Rejoining a PANA session may fail. Close Momonga and open it again.')
-        logger.debug('Acquired "rejoin_lock".')
-        self.rejoin_lock.release()
-        if self.receiver_exception is not None:
-            logger.error('Got an exception from the packet receiver. %s: %s' % (type(self.receiver_exception).__name__, str(e)))
-            raise self.receiver_exception
-
         xmitted = False
         for _ in range(3):
             logger.debug('Trying to acquire "xmit_lock".')
-            if self.xmit_lock.acquire(timeout=3600) is False: 
+            for _ in range(30):
+                unlocked =  self.xmit_lock.acquire(timeout=120) 
+                if unlocked is False: 
+                    logger.warning('Could not acquire "xmit_lock".')
+                    if self.receiver_exception is not None:
+                        logger.error('Got an exception from the receiver thread. %s: %s' % (type(self.receiver_exception).__name__, self.receiver_exception))
+                        raise MomongaNeedToReopen('Got an exception from the receiver thread. %s: %s' % (type(self.receiver_exception).__name__, self.receiver_exception))
+                else:
+                    break
+
+            if unlocked is False: 
                 logger.error('Transmission rights could not be acquired. Close Momonga and open it again.')
                 raise MomongaNeedToReopen('Transmission rights could not be acquired. Close Momonga and open it again.')
-            logger.debug('Acquired "xmit_lock".')
+            else:
+                logger.debug('Acquired "xmit_lock".')
 
             assert self.session_established is not False, 'Tried to transmit a packet, but no PANA session was established.'
 
             try:
                 self.skw.sksendto(self.smart_meter_addr, data)
                 xmitted = True
                 break
             except MomongaSkCommandExecutionFailure as e:
-                logger.warning('Failed to transmit a packet: %s' % str(e))
+                logger.warning('Failed to transmit a packet: %s' % e)
             except Exception as e:
-                logger.warning('An error occurred to transmit a packet. %s: %s' % (type(e).__name__, str(e)))
+                logger.warning('An error occurred to transmit a packet. %s: %s' % (type(e).__name__, e))
             finally:
                 self.xmit_lock.release()
             time.sleep(3)
         if xmitted is False:
             logger.error('Could not transmit a packet. Close Momonga and open it again.')
             raise MomongaNeedToReopen('Could not transmit a packet. Close Momonga and open it again.')
 
     def restrict_to_xmit(self) -> None:
         self.xmit_restriction_cnt += 1
         logger.debug('The counter for the restriction was incremented: %d' % (self.xmit_restriction_cnt))
 
-        assert self.xmit_restriction_cnt <= 2, 'The critical section counter for data transmission is inconsistent: The value is set too large for the counter.'
+        assert self.xmit_restriction_cnt <= 2, 'The critical section counter for data transmission is inconsistent: Too big than expected.'
 
         if self.xmit_restriction_cnt == 1:
             logger.debug('Trying to restrict data transmission.')
             self.xmit_lock.acquire()
             logger.debug('Data transmission is being restricted.')
 
     def unrestrict_to_xmit(self, force=False) -> None:
         if force is True:
             self.xmit_restriction_cnt = 0
             logger.debug('The counter for the restriction was forcibly set to zero.')
         else:
             self.xmit_restriction_cnt -= 1
             logger.debug('The counter for the restriction was decremented: %d' % (self.xmit_restriction_cnt))
 
-        assert self.xmit_restriction_cnt >= 0, 'The critical section counter for data transmit is inconsistent: The counter is set to a value that is a too small.'
+        assert self.xmit_restriction_cnt >= 0, 'The critical section counter for data transmit is inconsistent: Too small than expected.'
 
         if self.xmit_restriction_cnt == 0:
             try:
                 self.xmit_lock.release()
             except RuntimeError as e:
-                #logger.warning('Could not release "xmit_lock": %s' % str(e))
+                #logger.warning('Could not release "xmit_lock": %s' % e)
                 pass
             logger.debug('Data transmission is being unrestricted.')
```

## Comparing `momonga-0.0.5.dist-info/LICENSE` & `momonga-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `momonga-0.0.5.dist-info/METADATA` & `momonga-0.0.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momonga
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Route B Library: A Communicator for Low-voltage Smart Electric Energy Meters
 Home-page: https://github.com/nbtk/momonga
 Author: nbtk
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,23 +28,25 @@
 ```
 
 # Simple Example
 下記のコードはPANAセッションを確立し、瞬時電力計測値を取得して表示します。PANのスキャンは最大で約２分、セッション確立は最大で約１分かかります。
 BルートID、パスワード、デバイスファイルへのパスは適宜変更してください。
 ```python3
 import momonga
-
+import time
 
 rbid = 'SET A ROUTE B ID'
 pwd  = 'SET A ROUTE B PASSWORD'
 dev  = '/dev/ttyUSB0' # in a case of RaspberryPi OS
 
 with momonga.Momonga(rbid, pwd, dev) as mo:
-    res = momonga.get_instantaneous_power()
-    print('%0.1fW' % res)
+    while True:
+        res = mo.get_instantaneous_power()
+        print('%0.1fW' % res)
+        time.sleep(60)
 ```
 
 ### Arguments
 - rbid: BルートID
 - pwd: Bルートパスワード
 - dev: Wi-SUNモジュールのデバイスファイルへのパス
 - baudrate: シリアル通信のボーレート(デフォルト: 11520)
@@ -63,17 +65,17 @@
 
 ## momonga.sk_wrapper_logger
 Wi-SUNモジュールとの通信ログ
 
 ## ログを有効にした例
 ```python3
 import momonga
+import time
 import logging
 
-
 log_fmt = logging.Formatter('%(asctime)s | %(levelname)s | %(name)s - %(message)s')
 log_hnd = logging.StreamHandler()
 log_hnd.setFormatter(log_fmt)
 momonga.logger.addHandler(log_hnd)
 momonga.logger.setLevel(logging.DEBUG)
 momonga.session_manager_logger.addHandler(log_hnd)
 momonga.session_manager_logger.setLevel(logging.DEBUG)
@@ -81,16 +83,18 @@
 momonga.sk_wrapper_logger.setLevel(logging.DEBUG)
 
 rbid = 'SET A ROUTE B ID'
 pwd  = 'SET A ROUTE B PASSWORD'
 dev  = '/dev/ttyUSB0' # in a case of RaspberryPi OS
 
 with momonga.Momonga(rbid, pwd, dev) as mo:
-    res = momonga.get_instantaneous_power()
-    print('%0.1fW' % res)
+    while True:
+        res = mo.get_instantaneous_power()
+        print('%0.1fW' % res)
+        time.sleep(60)
 ```
 
 # Exception
 主な例外は下記です。
 
 ## momonga.MomongaSkScanFailure
 PANをスキャンしたが見つからなかったときに送出される。スマートメーターと通信できるロケーションか、またBルートIDが正しく設定されているかを確認し、再試行すること。
@@ -100,27 +104,28 @@
 
 ## momonga.MomongaNeedToReopen
 スマートメーターに対してコマンドを送信できなかったなどの理由で、スマートメーターに再接続が必要なときに送出される。
 
 ## 例外を捕捉する例
 ```python3
 import momonga
+import time
 import sys
 
-
 rbid = 'SET A ROUTE B ID'
 pwd  = 'SET A ROUTE B PASSWORD'
 dev  = '/dev/ttyUSB0' # in a case of RaspberryPi OS
 
 while True:
     try:
         with momonga.Momonga(rbid, pwd, dev) as mo:
-            res = momonga.get_instantaneous_power()
-            print('%0.1fW' % res)
-            break
+            while True:
+                res = mo.get_instantaneous_power()
+                print('%0.1fW' % res)
+                time.sleep(60)
     except (momonga.MomongaSkScanFailure,
             momonga.MomongaSkJoinFailure,
             momonga.MomongaNeedToReopen) as e:
         print('%s: %s' % (type(e).__name__, e), file=sys.stderr)
         continue
 ```
 
@@ -203,22 +208,22 @@
 e.g.
 ```python3
 [{'timestamp': datetime.datetime,
   'cumulative energy': float}]
 ```
 注意: 収集日時はスマートメーター側で設定されたものではなくMomonga自身が設定しているため、実行中に日を跨ぐと収集日時に齟齬が生じる可能性がある。
 
-## momonga.set_day_for_which_to_retrieve_historical_data_1(day: int = 0)
+## momonga.set_day_for_historical_data_1(day: int = 0)
 積算履歴収集日1を設定する。
 ### Arguments
 - day: 積算履歴収集日(0:当日、1~:前日の日数)
 ### Return Value
 - None
 
-## momonga.get_day_for_which_to_retrieve_historical_data_1()
+## momonga.get_day_for_historical_data_1()
 積算履歴収集日1を設定する。
 ### Arguments
 - Void
 ### Return Value
 - int: 積算履歴収集日1
 
 ## momonga.get_instantaneous_power()
@@ -265,23 +270,23 @@
 e.g.
 ```python3
 [{'timestamp': datetime.datetime,
   'cumulative energy': {'normal direction': float,
                         'reverse direction': float}}]
 ```
 
-## momonga.set_time_for_which_to_retrieve_historical_data_2(timestamp: datetime.datetime, num_of_data_points: int = 12)
+## momonga.set_time_for_historical_data_2(timestamp: datetime.datetime, num_of_data_points: int = 12)
 積算履歴収集日時ならびに収集コマ数を設定する。
 ### Arguments
 - timestamp: 収集日時
 - num_of_data_points: 収集コマ数
 ### Return Value
 - None
 
-## momonga.get_time_for_which_to_retrieve_historical_data_2()
+## momonga.get_time_for_historical_data_2()
 積算履歴収集日時ならびに収集コマ数を取得する。
 ### Arguments
 - Void
 ### Return Value
 - dict: 収集日時と収集コマ数
 
 e.g.
```

## Comparing `momonga-0.0.5.dist-info/RECORD` & `momonga-0.0.6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 momonga/__init__.py,sha256=iWnaMiIWmYho2GfBZJiZ82rlo4znFfQlqNXkGwNXhLg,136
-momonga/momonga.py,sha256=rufLe-sknKiyg4apyaifir_uEvQavcMDYjxUGSRxZzc,15159
+momonga/momonga.py,sha256=7pLTNyIQNfSsK8D-GLF2IZTdlKq3i1UMh85tAoAf0vw,15034
 momonga/momonga_exception.py,sha256=IPcOVNU7mpm-upYTLLo6gIxFHzjCXxs-YwzhIej8PMU,959
 momonga/momonga_response.py,sha256=_t_aaA6z5cpZVGWIkir7J_fgwYabPSNrpBAiS36Ro7c,2698
-momonga/momonga_session_manager.py,sha256=UV6BqWxuRx6D1TgKtFIpcoX7avOetVQ5J6eSpqD-t4I,11967
+momonga/momonga_session_manager.py,sha256=jcOgnpXPdXvzqifyEBDsWMrjyAmuFTPlVaNi1vHbgvY,11915
 momonga/momonga_sk_wrapper.py,sha256=xaffyj3D3Mt84LljroJ07j-GHJTpsXTMp695vztZbz4,9392
-momonga-0.0.5.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
-momonga-0.0.5.dist-info/METADATA,sha256=X_TKp-K1MUYpCxy00Gb9Cv5_qKoUMwxwd5m08D0e3ZU,10268
-momonga-0.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-momonga-0.0.5.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
-momonga-0.0.5.dist-info/RECORD,,
+momonga-0.0.6.dist-info/LICENSE,sha256=pOXywwG9IIlOPHodSe52gNYGQZymYppp-BeVhAjPDME,1061
+momonga-0.0.6.dist-info/METADATA,sha256=c1S___K6HrTZSqHm5GkprsanPaPL9ZNDPHLf4sgoAX0,10353
+momonga-0.0.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+momonga-0.0.6.dist-info/top_level.txt,sha256=wB9RSzcUXuE3oWO6vYrP1GBIbDG-FM6juEp8yztPzbM,8
+momonga-0.0.6.dist-info/RECORD,,
```

