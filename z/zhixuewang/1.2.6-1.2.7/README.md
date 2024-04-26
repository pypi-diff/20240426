# Comparing `tmp/zhixuewang-1.2.6-py3-none-any.whl.zip` & `tmp/zhixuewang-1.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 22042 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat      617 b- defN 24-Apr-05 14:07 zhixuewang/__init__.py
+Zip file size: 22605 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat      626 b- defN 24-Apr-26 08:35 zhixuewang/__init__.py
 -rw-rw-rw-  2.0 fat     5015 b- defN 23-Oct-05 01:21 zhixuewang/account.py
 -rw-rw-rw-  2.0 fat      941 b- defN 23-Oct-05 01:21 zhixuewang/exceptions.py
--rw-rw-rw-  2.0 fat     8837 b- defN 23-Oct-06 11:45 zhixuewang/models.py
+-rw-rw-rw-  2.0 fat     9430 b- defN 24-Apr-26 08:34 zhixuewang/models.py
 -rw-rw-rw-  2.0 fat     4578 b- defN 23-Dec-09 15:07 zhixuewang/session.py
 -rw-rw-rw-  2.0 fat      377 b- defN 23-Oct-05 01:21 zhixuewang/urls.py
 -rw-rw-rw-  2.0 fat       87 b- defN 23-Jul-06 13:22 zhixuewang/student/__init__.py
--rw-rw-rw-  2.0 fat    26124 b- defN 24-Apr-05 14:06 zhixuewang/student/student.py
+-rw-rw-rw-  2.0 fat    28879 b- defN 24-Apr-26 08:34 zhixuewang/student/student.py
 -rw-rw-rw-  2.0 fat     2056 b- defN 23-Oct-08 14:27 zhixuewang/student/urls.py
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Oct-05 01:21 zhixuewang/teacher/__init__.py
 -rw-rw-rw-  2.0 fat     1390 b- defN 23-Oct-06 11:43 zhixuewang/teacher/models.py
 -rw-rw-rw-  2.0 fat    13633 b- defN 24-Apr-05 14:06 zhixuewang/teacher/teacher.py
 -rw-rw-rw-  2.0 fat     1357 b- defN 23-Oct-05 02:06 zhixuewang/teacher/urls.py
 -rw-rw-rw-  2.0 fat       96 b- defN 23-Oct-05 01:21 zhixuewang/tools/__init__.py
 -rw-rw-rw-  2.0 fat      433 b- defN 20-Aug-05 14:04 zhixuewang/tools/datetime_tool.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-05 14:08 zhixuewang-1.2.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      280 b- defN 24-Apr-05 14:08 zhixuewang-1.2.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-05 14:08 zhixuewang-1.2.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-05 14:08 zhixuewang-1.2.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1632 b- defN 24-Apr-05 14:08 zhixuewang-1.2.6.dist-info/RECORD
-20 files, 68739 bytes uncompressed, 19382 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-26 08:35 zhixuewang-1.2.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      288 b- defN 24-Apr-26 08:35 zhixuewang-1.2.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-26 08:35 zhixuewang-1.2.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-26 08:35 zhixuewang-1.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1632 b- defN 24-Apr-26 08:35 zhixuewang-1.2.7.dist-info/RECORD
+20 files, 72104 bytes uncompressed, 19945 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: zhixuewang/tools/__init__.py
 Comment: 
 
 Filename: zhixuewang/tools/datetime_tool.py
 Comment: 
 
-Filename: zhixuewang-1.2.6.dist-info/LICENSE
+Filename: zhixuewang-1.2.7.dist-info/LICENSE
 Comment: 
 
-Filename: zhixuewang-1.2.6.dist-info/METADATA
+Filename: zhixuewang-1.2.7.dist-info/METADATA
 Comment: 
 
-Filename: zhixuewang-1.2.6.dist-info/WHEEL
+Filename: zhixuewang-1.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: zhixuewang-1.2.6.dist-info/top_level.txt
+Filename: zhixuewang-1.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: zhixuewang-1.2.6.dist-info/RECORD
+Filename: zhixuewang-1.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zhixuewang/__init__.py

```diff
@@ -1,10 +1,10 @@
-__author__ = "anwenhu,MasterYuan418,immoses648"
-__date__ = "2024/4/5 22:10"
-__version__ = "1.2.6"
+__author__ = "anwenhu,MasterYuan418,immoses648,krn1pnc"
+__date__ = "2024/4/26 16:40"
+__version__ = "1.2.7"
 
 from zhixuewang.account import (login, login_id, rewrite_str, login_student, login_teacher,
                                 login_student_id, login_teacher_id, load_account)
 from zhixuewang.session import get_session, get_session_id
 
 VERSION = tuple(map(int, __version__.split('.')))
 __all__ = [
```

## zhixuewang/models.py

```diff
@@ -1,12 +1,13 @@
 import base64
 from enum import Enum
 import os
 import pickle
 from typing import List, Callable, Union, TypeVar
+from datetime import datetime
 from dataclasses import dataclass, field
 from zhixuewang.session import get_basic_session, get_session
 from zhixuewang.tools.datetime_tool import get_property
 from zhixuewang.urls import Url
 
 
 class Role(Enum):
@@ -264,14 +265,45 @@
             return msg[:-1]
 
     def __str__(self):
         return self.__repr__()
 
 
 @dataclass
+class MarkingRecord:
+    """批改记录"""
+
+    time: datetime
+    score: float
+    teacher_name: str
+
+
+@dataclass
+class SubTopicRecord:
+    """小题得分详情"""
+
+    score: float
+    marking_records: Union[None, ExtendedList[MarkingRecord]]
+
+
+@dataclass
+class TopicRecord:
+    """题目得分详情"""
+
+    title: str
+    score: float
+    standard_score: float
+    subtopic_records: Union[None, ExtendedList[SubTopicRecord]]
+
+
+class AnswerRecord(ExtendedList[TopicRecord]):
+    """一场考试的得分详情"""
+
+
+@dataclass
 class HwType:
     """作业类型, eg: 105 自由出题"""
 
     name: str
     code: int
```

## zhixuewang/student/student.py

```diff
@@ -8,14 +8,18 @@
     ErrorBookTopic,
     ExtendedList,
     Exam,
     HwResource,
     HwType,
     HwAnswer,
     Mark,
+    MarkingRecord,
+    SubTopicRecord,
+    TopicRecord,
+    AnswerRecord,
     Role,
     StuHomework,
     Subject,
     SubjectScore,
     StuClass,
     School,
     Sex,
@@ -23,14 +27,15 @@
     StuPerson
 )
 from zhixuewang.exceptions import (
     UserDefunctError,
     PageConnectionError,
 )
 from zhixuewang.student.urls import Url
+from datetime import datetime
 
 
 def _check_is_uuid(msg: str):
     """判断msg是否为uuid"""
     return (
             len(msg) == 36
             and msg[14] == "4"
@@ -380,14 +385,73 @@
         if not exam:
             return []
         subject = self.get_subject(subject_data, exam)
         if not subject:
             return []
         return self.__get_original(subject.id, exam.id)
 
+    def __get_answer_records(self, topic_set_id: str, exam_id: str):
+        self.update_login_status()
+        r = self._session.get(
+            Url.GET_ORIGINAL_URL,
+            params={
+                "examId": exam_id,
+                "paperId": topic_set_id,
+            },
+            headers=self.get_auth_header(),
+        )
+        if not r.ok:
+            raise PageConnectionError(f"__get_answer_records出错 \n {r.text}")
+        elif not r.json()["result"]:
+            raise PageConnectionError(f"__get_answer_records出错 \n {r.json()}")
+        json_data = json.loads(r.json()["result"]["sheetDatas"])
+        records = AnswerRecord()
+        for topic in json_data["userAnswerRecordDTO"]["answerRecordDetails"]:
+            topic_records = TopicRecord(
+                title=topic["dispTitle"],
+                score=topic["score"],
+                standard_score=topic["standardScore"],
+                subtopic_records=None
+            )
+            if "subTopics" in topic:
+                topic_records.subtopic_records = []
+                for subtopic in topic["subTopics"]:
+                    subtopic_record = SubTopicRecord(
+                        score=subtopic["score"], marking_records=None)
+                    if "teacherMarkingRecords" in subtopic:
+                        subtopic_record.marking_records = [
+                            MarkingRecord(
+                                time=datetime.fromtimestamp(marking["markingTime"] / 1e3),
+                                score=marking["score"],
+                                teacher_name=marking["teacherName"]
+                            )
+                            for marking in subtopic["teacherMarkingRecords"]
+                        ]
+                    topic_records.subtopic_records.append(subtopic_record)
+            records.append(topic_records)
+        return records
+
+    def get_answer_records(self, subject_data: Union[Subject, str], exam_data: Union[Exam, str] = "") -> AnswerRecord:
+        """获得指定考试学科的得分详情
+
+        Args:
+            subject_data (Union[Subject, str]): 学科id 或 学科名称 或 Subject实例
+            exam_data (Union[Exam, str]): 考试id 或 考试名称, 默认为最新考试
+
+        Returns:
+            AnswerRecord: 得分详情
+        """
+        exam = self.get_exam(exam_data)
+        if not exam:
+            return AnswerRecord()
+        subject = self.get_subject(subject_data, exam)
+        if not subject:
+            return AnswerRecord()
+        return self.__get_answer_records(subject.id, exam.id)
+
     def get_clazzs(self) -> ExtendedList[StuClass]:
         """获取当前年级所有班级"""
         clazzs: ExtendedList[StuClass] = ExtendedList()
         r = self._session.get(Url.GET_CLAZZS_URL, params={"d": int(time.time())})
         if not r.ok:
             raise PageConnectionError(f"get_clazzs出错 \n {r.text}")
         json_data = r.json()
```

## Comparing `zhixuewang-1.2.6.dist-info/LICENSE` & `zhixuewang-1.2.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zhixuewang-1.2.6.dist-info/RECORD` & `zhixuewang-1.2.7.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-zhixuewang/__init__.py,sha256=z-zYJ5qQQrB8xDpnIK2K1tCHiR9163xNUFe9L6CpXZA,617
+zhixuewang/__init__.py,sha256=fqeOTN1hvn1soIqvYm6DYCZ1dK3fXS9PKklY6iSaZwQ,626
 zhixuewang/account.py,sha256=3VKn7kYy5Ytw2JGWp8Bapaic-W8qCJY_5gDUTmLkNbQ,5015
 zhixuewang/exceptions.py,sha256=p_mnjq_FIZIwzks3QZsk5xKdGL7Dbbcsdf-OtvoRbVk,941
-zhixuewang/models.py,sha256=gneTnzGhUsUX1WIuDKD1rFgYjT81x4K-oGwwNx-1eb4,8837
+zhixuewang/models.py,sha256=gkcAnNZvWn4pSNo4Ioz3Bx0-st8cuniWetqSrWRZLAA,9430
 zhixuewang/session.py,sha256=Jp5qX379TqFCCSZvRrNN1ZUOub8cGTojzVgQ006hb_M,4578
 zhixuewang/urls.py,sha256=JzGiCpbgnLximLXPFBeoTJgCcZoNbceZcyPVv4_-I_o,377
 zhixuewang/student/__init__.py,sha256=1hZ_-EeFM4l7wF8D56jIMigTQ5b7o7sCCTR9_YRjsj0,87
-zhixuewang/student/student.py,sha256=QVyHb5iHZV9_fCoOqMu2tbbbPlE3WliQ5CanAOsc-f8,26124
+zhixuewang/student/student.py,sha256=6IyUoS9QskOXXKFdIF-XSnPUfzAlmlzVE4Mo9RMFXYI,28879
 zhixuewang/student/urls.py,sha256=92qXQSUzVC-IZSs1-I7eCdjjJnBgTPgzEdwon0ybyy8,2056
 zhixuewang/teacher/__init__.py,sha256=HQ02UJM7lhCgtamRCYcSuFOUTA_cWXNV2jyc9a_q4Sc,98
 zhixuewang/teacher/models.py,sha256=R8c7zljypjGOTYW60A6zss0h01xVslkoMHhk5SW_UJo,1390
 zhixuewang/teacher/teacher.py,sha256=Uso50QkKDUd7vNX35supGXheOPlshs4lpmBUeobNxJg,13633
 zhixuewang/teacher/urls.py,sha256=sAZpTI4ajOoTdvimVEq0OyiHuf80D-EJi_-09YzzmuQ,1357
 zhixuewang/tools/__init__.py,sha256=apzJbuBykdNmJaeellyr4NRPtAqCtSjMFuevsMEudkM,96
 zhixuewang/tools/datetime_tool.py,sha256=mCsCA0TK27ku4GCQY7ghyruhAeIeN6360jSZZ3XQNqw,433
-zhixuewang-1.2.6.dist-info/LICENSE,sha256=xfB-JOtu13adc_d9NLglK9fKvZZlHEDoKKpYliTvaQA,1085
-zhixuewang-1.2.6.dist-info/METADATA,sha256=4FbJMvYqr8gVW2N092e-jSk5oEuG2f9y-6eK2cvgHQ8,280
-zhixuewang-1.2.6.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-zhixuewang-1.2.6.dist-info/top_level.txt,sha256=ufrDrdhelpFTIliZw7eEvOtIK_zyIv4UssZNpQqV-Jw,11
-zhixuewang-1.2.6.dist-info/RECORD,,
+zhixuewang-1.2.7.dist-info/LICENSE,sha256=xfB-JOtu13adc_d9NLglK9fKvZZlHEDoKKpYliTvaQA,1085
+zhixuewang-1.2.7.dist-info/METADATA,sha256=f46CBeJWi1MPFVqAkHR_kH6Zap2GJRUf7w_4aVdwokU,288
+zhixuewang-1.2.7.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+zhixuewang-1.2.7.dist-info/top_level.txt,sha256=ufrDrdhelpFTIliZw7eEvOtIK_zyIv4UssZNpQqV-Jw,11
+zhixuewang-1.2.7.dist-info/RECORD,,
```

