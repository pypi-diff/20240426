# Comparing `tmp/correpy-0.3.0.tar.gz` & `tmp/correpy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "correpy-0.3.0.tar", max compression
+gzip compressed data, was "correpy-0.4.1.tar", max compression
```

## Comparing `correpy-0.3.0.tar` & `correpy-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2024-01-13 21:08:27.367544 correpy-0.3.0/LICENSE
--rw-r--r--   0        0        0     4822 2024-01-13 21:08:27.367544 correpy-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/__init__.py
--rw-r--r--   0        0        0        0 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/domain/entities/__init__.py
--rw-r--r--   0        0        0     2241 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/domain/entities/brokerage_note.py
--rw-r--r--   0        0        0     1406 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/domain/entities/security.py
--rw-r--r--   0        0        0      703 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/domain/entities/transaction.py
--rw-r--r--   0        0        0      596 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/domain/enums.py
--rw-r--r--   0        0        0       64 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/domain/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/parsers/__init__.py
--rw-r--r--   0        0        0        0 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/parsers/brokerage_notes/__init__.py
--rw-r--r--   0        0        0        0 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/parsers/brokerage_notes/b3_parser/__init__.py
--rw-r--r--   0        0        0     9844 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/parsers/brokerage_notes/b3_parser/b3_parser.py
--rw-r--r--   0        0        0     2119 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/parsers/brokerage_notes/b3_parser/nuinvest.py
--rw-r--r--   0        0        0     5930 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/parsers/brokerage_notes/base_parser.py
--rw-r--r--   0        0        0      908 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/parsers/brokerage_notes/brokerage_note_section.py
--rw-r--r--   0        0        0      108 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/parsers/brokerage_notes/word_rectangle.py
--rw-r--r--   0        0        0      118 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/parsers/exceptions.py
--rw-r--r--   0        0        0     2575 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/parsers/fitz_parser.py
--rw-r--r--   0        0        0        0 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/py.typed
--rw-r--r--   0        0        0      653 2024-01-13 21:08:27.367544 correpy-0.3.0/correpy/utils.py
--rw-r--r--   0        0        0     2164 2024-01-13 21:08:27.371544 correpy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5778 1970-01-01 00:00:00.000000 correpy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-26 20:11:58.518864 correpy-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5010 2024-04-26 20:11:58.518864 correpy-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/entities/__init__.py
+-rw-r--r--   0        0        0     2263 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/entities/brokerage_note.py
+-rw-r--r--   0        0        0     1405 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/entities/security.py
+-rw-r--r--   0        0        0      703 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/entities/transaction.py
+-rw-r--r--   0        0        0      596 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/enums.py
+-rw-r--r--   0        0        0       64 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/domain/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/b3_parser/__init__.py
+-rw-r--r--   0        0        0    11260 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/b3_parser/b3_parser.py
+-rw-r--r--   0        0        0     2012 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/b3_parser/nuinvest.py
+-rw-r--r--   0        0        0     5988 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/base_parser.py
+-rw-r--r--   0        0        0      908 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/brokerage_note_section.py
+-rw-r--r--   0        0        0      108 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/brokerage_notes/word_rectangle.py
+-rw-r--r--   0        0        0      118 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/exceptions.py
+-rw-r--r--   0        0        0     2567 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/parsers/fitz_parser.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/py.typed
+-rw-r--r--   0        0        0     1123 2024-04-26 20:11:58.518864 correpy-0.4.1/correpy/utils.py
+-rw-r--r--   0        0        0     2164 2024-04-26 20:11:58.518864 correpy-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5966 1970-01-01 00:00:00.000000 correpy-0.4.1/PKG-INFO
```

### Comparing `correpy-0.3.0/LICENSE` & `correpy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `correpy-0.3.0/README.md` & `correpy-0.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -76,28 +76,30 @@
 ```
 
 ### Descrição das entidades
 Abaixo você pode encontrar a descrição de cada um dos campos retornados. 
 
 #### Brokerage Note
 
-| BrokerageNote    |                                     |
-|------------------|-------------------------------------|
-| reference_date   | Data do pregão                      |
-| settlement_fee   | Taxa de liquidação                  |
-| registration_fee | Taxa de registro                    |
-| term_fee         | Taxa de termo/opções                |
-| ana_fee          | Taxa A.N.A                          |
-| emoluments       | Emolumentos                         |
-| operational_fee  | Taxa Operacional                    |
-| execution        | Execução                            |
-| custody_fee      | Taxa de custódia                    |
-| taxes            | Impostos                            |
-| others           | Outros                              |
-| transactions     | Lista de [transações](#transaction) |
+| BrokerageNote         |                                     |
+|-----------------------|-------------------------------------|
+| reference_id          | Número da nota                      |
+| reference_date        | Data do pregão                      |
+| settlement_fee        | Taxa de liquidação                  |
+| registration_fee      | Taxa de registro                    |
+| term_fee              | Taxa de termo/opções                |
+| ana_fee               | Taxa A.N.A                          |
+| emoluments            | Emolumentos                         |
+| operational_fee       | Taxa Operacional                    |
+| execution             | Execução                            |
+| custody_fee           | Taxa de custódia                    |
+| source_withheld_taxes | IRRF                    |
+| taxes                 | Impostos                            |
+| others                | Outros                              |
+| transactions          | Lista de [transações](#transaction) |
 
 #### Transaction
 
 | Transaction          |                                                            |
 |----------------------|------------------------------------------------------------|
 | transaction_type     | Enum com o tipo de transação (BUY - compra, SELL - venda)  |
 | amount               | Quantidade                                                 |
@@ -117,8 +119,8 @@
 Este projeto ainda está em evolução e qualquer PR é bem vindo. Algumas ferramentas estão sendo utilizadas para melhorar a qualidade do código:
 
 1. MyPy para checagem estática de tipos
 2. PyLint
 3. Black
 4. isort
 
-Para verificar se o seu código continua de acordo com os critérios definidos, basta rodar `./pipeline/lint.sh`.
+Para verificar se o seu código continua de acordo com os critérios definidos, basta rodar `./pipeline/lint.sh`.
```

### Comparing `correpy-0.3.0/correpy/domain/entities/brokerage_note.py` & `correpy-0.4.1/correpy/domain/entities/brokerage_note.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from correpy.domain.entities.transaction import Transaction
 from correpy.domain.enums import BrokerageNoteFeeType
 from correpy.domain.exceptions import InvalidBrokerageNoteFeeTypeException
 
 
 @dataclass
 class BrokerageNote:  # pylint:disable=too-many-instance-attributes
+    reference_id: int
     reference_date: date
     settlement_fee: Decimal = Decimal(0)
     registration_fee: Decimal = Decimal(0)
     term_fee: Decimal = Decimal(0)
     ana_fee: Decimal = Decimal(0)
     emoluments: Decimal = Decimal(0)
     operational_fee: Decimal = Decimal(0)
```

### Comparing `correpy-0.3.0/correpy/domain/entities/security.py` & `correpy-0.4.1/correpy/domain/entities/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 
 # 3	Ordinárias / VALE3
 # 4	Preferenciais / GGBR4
 # 5	Preferenciais Classe A / USIM5
 # 6	Preferenciais Classe B / ELET6
 # 11 BDRs, ETs e Units / BOVA11
 
-BASIC_TICKER_PATTERN = "([A-Z-0-9]{4})(2|3|4|5|6|11|12)(F|B)?"  # Format XXXXY or XXXXYF or XXXXYB where Y can be 3, 4, 11
-BDR_TICKER_PATTERN = "([A-Z-0-9]{4})(31|32|33|34|35|36|39)"  # Format XXXXYY where YY can be 31, 32, 33, 34, 35, 36, 39
+# Format XXXXY or XXXXYF or XXXXYB where Y can be 3, 4, 11
+BASIC_TICKER_PATTERN = "([A-Z-0-9]{4})(2|3|4|5|6|11|12)(F|B)?"
+
+# Format XXXXYY where YY can be 31, 32, 33, 34, 35, 36, 39
+BDR_TICKER_PATTERN = "([A-Z-0-9]{4})(31|32|33|34|35|36|39)"
 
 
 @dataclass
 class Security:
     name: str
     ticker: Optional[str] = None
```

### Comparing `correpy-0.3.0/correpy/domain/entities/transaction.py` & `correpy-0.4.1/correpy/domain/entities/transaction.py`

 * *Files identical despite different names*

### Comparing `correpy-0.3.0/correpy/domain/enums.py` & `correpy-0.4.1/correpy/domain/enums.py`

 * *Files identical despite different names*

### Comparing `correpy-0.3.0/correpy/parsers/brokerage_notes/b3_parser/b3_parser.py` & `correpy-0.4.1/correpy/parsers/brokerage_notes/b3_parser/b3_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 from fitz import TextPage
 
 from correpy.domain.entities.brokerage_note import BrokerageNote
 from correpy.domain.enums import BrokerageNoteFeeType
 from correpy.parsers.brokerage_notes.base_parser import BaseBrokerageNoteParser
 from correpy.parsers.brokerage_notes.brokerage_note_section import BrokerageNoteSection
 from correpy.parsers.exceptions import ProblemParsingBrokerageNoteException
-from correpy.utils import extract_date_from_line, extract_value_from_line
+from correpy.utils import extract_date_from_line, extract_value_from_line, extract_id_from_line
 
 
 class B3Parser(BaseBrokerageNoteParser):
     BROKERAGE_NOTE_X_AXIS_START_COORDINATE = 0
     BROKERAGE_NOTE_X_AXIS_END_COORDINATE = 601
     BROKERAGE_NOTE_FINANCIAL_SUMMARY_Y_AXIS_END = 842
     TRANSACTIONS_SECTION_TITLE = "Negócios realizados"
     TRANSACTIONS_SUMMARY_TITLE = "Resumo dos Negócios"
     FINANCIAL_SUMMARY_TITLE = "Resumo Financeiro"
     REFERENCE_DATE_TITLE = "Data pregão"
+    REFERENCE_NOTE_ID = "Nr. nota"
     CI_TITLE = "C.I"
     NET_VALUE_SECTION_TITLE = "Líquido para"
 
     buy_transaction_indicator_on_brokerage_note = "C"
     sell_transaction_indicator_on_brokerage_note = "V"
     first_column_transactions = "Q"
     transaction_columns_index = {
@@ -50,14 +51,19 @@
     }
     last_transaction_item = "Resumo dos Negócios"
 
     @classmethod
     def __get_reference_date_from_section(cls, brokerage_note_section: BrokerageNoteSection) -> date:
         return extract_date_from_line(line=brokerage_note_section.full_text)
 
+    @classmethod
+    def __get_reference_id_from_section(cls, brokerage_note_section: BrokerageNoteSection) -> int:
+        """Extrai e retorna o número da nota 'ID'"""
+        return extract_id_from_line(line=brokerage_note_section.text_by_lines[1])
+
     def __build_full_width_rectangle(self, *, y_axis_start: int, y_axis_end: int) -> fitz.Rect:
         return fitz.Rect(
             self.BROKERAGE_NOTE_X_AXIS_START_COORDINATE,
             y_axis_start,
             self.BROKERAGE_NOTE_X_AXIS_END_COORDINATE,
             y_axis_end,
         )
@@ -83,50 +89,69 @@
 
             if self._is_transactions_header_line(line_text=transaction_full_line):
                 can_include_transactions = True
 
         return transaction_lines_text
 
     def _get_or_create_brokerage_note_by_page(self, page: TextPage, page_number: int) -> BrokerageNote:
-        reference_date_rect = self.fitz_parser.search_and_extract_rectangle_from_text(
-            page=page, text=self.REFERENCE_DATE_TITLE
+        reference_id_rect = self.fitz_parser.search_and_extract_rectangle_from_text(
+            page=page, text=self.REFERENCE_NOTE_ID
         )
-        ci_rect = self.fitz_parser.search_and_extract_rectangle_from_text(page=page, text=self.CI_TITLE)
+        try:
+            ci_rect = self.fitz_parser.search_and_extract_rectangle_from_text(page=page, text=self.CI_TITLE)
+        except ProblemParsingBrokerageNoteException:
+            # From the initial text to 1/4 of the end of the page. It is this way because
+            # the final text (CI_TITLE) is not always available (multiple pages).
+            ci_rect = fitz.Rect(
+                reference_id_rect.x0, reference_id_rect.y0,
+                page.rect.width, page.rect.height * 0.25
+            )
         brokerage_note_summary_section = self._build_brokerage_note_section_from_two_rectangles(
-            first_rectangle=reference_date_rect, second_rectangle=ci_rect, page_number=page_number
+            first_rectangle=reference_id_rect, second_rectangle=ci_rect, page_number=page_number
+        )
+        current_reference_id = self.__get_reference_id_from_section(
+            brokerage_note_section=brokerage_note_summary_section
         )
         current_reference_date = self.__get_reference_date_from_section(
             brokerage_note_section=brokerage_note_summary_section
         )
-        if current_reference_date not in self.brokerage_notes:
-            brokerage_note = BrokerageNote(reference_date=current_reference_date)
-            self.brokerage_notes[current_reference_date] = brokerage_note
-        return self.brokerage_notes[current_reference_date]
+        note_key = (current_reference_id, current_reference_date)
+        if (brokerage_note := self.brokerage_notes.get(note_key)) is None:
+            brokerage_note = BrokerageNote(reference_id=current_reference_id,
+                                           reference_date=current_reference_date)
+            self.brokerage_notes[note_key] = brokerage_note
+        return brokerage_note
 
     def set_brokerage_note_transactions(self) -> None:
         for page_document in self.fitz_parser.document:  # type:ignore[union-attr]
             page = page_document.get_textpage()
             page_number = page_document.number
             try:
                 brokerage_note = self._get_or_create_brokerage_note_by_page(page=page, page_number=page_number)
                 transactions_title_rectangle = self.fitz_parser.search_and_extract_rectangle_from_text(
                     page=page, text=self.TRANSACTIONS_SECTION_TITLE
                 )
-                transactions_summary_title_rectangle = self.fitz_parser.search_and_extract_rectangle_from_text(
-                    page=page, text=self.TRANSACTIONS_SUMMARY_TITLE
-                )
-
                 rectangle_before_transactions = self.__build_full_width_rectangle(
                     y_axis_start=transactions_title_rectangle.y0,  # pylint:disable=no-member
                     y_axis_end=transactions_title_rectangle.y1,  # pylint:disable=no-member
                 )
-                rectangle_after_transactions = self.__build_full_width_rectangle(
-                    y_axis_start=transactions_summary_title_rectangle.y0,  # pylint:disable=no-member
-                    y_axis_end=transactions_summary_title_rectangle.y1,  # pylint:disable=no-member
-                )
+                try:
+                    transactions_summary_title_rectangle = self.fitz_parser.search_and_extract_rectangle_from_text(
+                        page=page, text=self.TRANSACTIONS_SUMMARY_TITLE
+                    )
+                    rectangle_after_transactions = self.__build_full_width_rectangle(
+                        y_axis_start=transactions_summary_title_rectangle.y0,  # pylint:disable=no-member
+                        y_axis_end=transactions_summary_title_rectangle.y1,  # pylint:disable=no-member
+                    )
+                except ProblemParsingBrokerageNoteException:
+                    # From the text rectangle 'rectangle_before_transactions' to the end of the page.
+                    rectangle_after_transactions = fitz.Rect(
+                        transactions_title_rectangle.x0, transactions_title_rectangle.y0,
+                        page.rect.width, page.rect.height
+                    )
                 transactions_brokerage_note_section = self._build_brokerage_note_section_from_two_rectangles(
                     first_rectangle=rectangle_before_transactions,
                     second_rectangle=rectangle_after_transactions,
                     page_number=page_number,
                 )
                 transactions = self._get_transaction_lines_text_from_words(
                     transactions_brokerage_note_section=transactions_brokerage_note_section
@@ -168,15 +193,15 @@
 
                 self.__set_brokerage_note_fees(
                     financial_summary_brokerage_note_section=financial_summary_brokerage_note_section,
                     page=page,
                     page_number=page_number,
                 )
 
-            except ProblemParsingBrokerageNoteException:
+            except ProblemParsingBrokerageNoteException as exc:
                 continue
 
     def __set_brokerage_note_fees(
         self, financial_summary_brokerage_note_section: BrokerageNoteSection, page: fitz.TextPage, page_number: int
     ) -> None:
         for line in financial_summary_brokerage_note_section.text_by_lines:
             self.__parse_brokerage_note_fee_from_summary_line(
```

### Comparing `correpy-0.3.0/correpy/parsers/brokerage_notes/b3_parser/nuinvest.py` & `correpy-0.4.1/correpy/parsers/brokerage_notes/b3_parser/nuinvest.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,18 @@
 
 from correpy.domain.enums import BrokerageNoteFeeType
 from correpy.parsers.brokerage_notes.b3_parser.b3_parser import B3Parser
 from correpy.parsers.brokerage_notes.brokerage_note_section import BrokerageNoteSection
 
 
 class NunInvestParser(B3Parser):
-	CI_TITLE = "Pav. 14, 15 - Torre A2 Jequitibá - Condomínio Parque da Cidade"
+	REFERENCE_NOTE_ID = "Número da nota"
+	CI_TITLE = "Valor/Ajuste D/C"
 	TRANSACTIONS_SECTION_TITLE = 'Nome do Cliente'
-	TRANSACTIONS_SUMMARY_TITLE = (
-		# sigle page
-		"Resumo dos Negócios",
-		# multipage: end of page
-		"Ouvidoria NuInvest Corretora de Valores S.A"
-	)
+	TRANSACTIONS_SUMMARY_TITLE = "Resumo dos Negócios"
 	first_column_transactions = "Mercado"
 	last_transaction_item = "BOVESPA"
 
 	financial_summary_header_mapper = {
 		"Taxa de Liquidação": BrokerageNoteFeeType.SETTLEMENT_FEE,
 		"Taxa de Registro": BrokerageNoteFeeType.REGISTRATION_FE,
 		"Taxa de Termo / Opções": BrokerageNoteFeeType.TERM_FEE,
```

### Comparing `correpy-0.3.0/correpy/parsers/brokerage_notes/base_parser.py` & `correpy-0.4.1/correpy/parsers/brokerage_notes/base_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 from correpy.domain.entities.brokerage_note import BrokerageNote
 from correpy.domain.entities.security import Security
 from correpy.domain.entities.transaction import Transaction
 from correpy.domain.enums import BrokerageNoteFeeType, TransactionType
 from correpy.parsers.brokerage_notes.brokerage_note_section import BrokerageNoteSection
 from correpy.parsers.brokerage_notes.word_rectangle import WordRectangle
 from correpy.parsers.fitz_parser import FitzParser
-from correpy.utils import extract_value_from_line
+from correpy.utils import extract_value_from_line, extract_amount_from_line
+
+NoteKey = tuple[int, date]
 
 
 class BaseBrokerageNoteParser(ABC):
     def __init__(self, brokerage_note: io.BytesIO, password: Optional[str] = None) -> None:
         self.fitz_parser = FitzParser(file=brokerage_note, password=password)
-        self.brokerage_notes: Dict[date, BrokerageNote] = {}
+        self.brokerage_notes: Dict[NoteKey, BrokerageNote] = {}
 
     @property
     @abstractmethod
     def buy_transaction_indicator_on_brokerage_note(self) -> str:
         ...
 
     @property
@@ -96,15 +98,15 @@
 
     def __parse_transaction_unit_price(self, *, line_array: List[str]) -> Decimal:
         unit_value_string = line_array[self.transaction_columns_index["unit_value"]]
         return extract_value_from_line(line=unit_value_string)
 
     def __parse_transaction_amount(self, *, line_array: List[str]) -> Decimal:
         amount_string = line_array[self.transaction_columns_index["amount"]]
-        return extract_value_from_line(line=amount_string)
+        return extract_amount_from_line(line=amount_string)
 
     def _create_transaction(self, *, line: str) -> Transaction:
         line_array = line.split(" ")
         transaction_type = self.__parse_transaction_type(line_array=line_array)
         security_name = self.__parse_security_name(line_array=line_array)
         unit_price = self.__parse_transaction_unit_price(line_array=line_array)
         amount = self.__parse_transaction_amount(line_array=line_array)
```

### Comparing `correpy-0.3.0/correpy/parsers/brokerage_notes/brokerage_note_section.py` & `correpy-0.4.1/correpy/parsers/brokerage_notes/brokerage_note_section.py`

 * *Files identical despite different names*

### Comparing `correpy-0.3.0/correpy/parsers/fitz_parser.py` & `correpy-0.4.1/correpy/parsers/fitz_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,16 @@
     def is_word_in_rectangle(cls, *, rectangle: fitz.Rect, word: WordRectangle) -> bool:
         return typing.cast(bool, fitz.Rect(word.x0, word.y0, word.x1, word.y1).intersects(rectangle))
 
     @classmethod
     def search_and_extract_rectangle_from_text(cls, *, page: TextPage, text: Union[str, List[str]]) -> fitz.Rect:
         if isinstance(text, str):
             text = [text]
-        for text in text:
-            # multitext search
-            if quadrilateral_position := page.search(text):
+        for value in text:  # multi-text search
+            if quadrilateral_position := page.search(value):
                 break
         else:
             quadrilateral_position = None
         if not quadrilateral_position:
             raise ProblemParsingBrokerageNoteException
         return quadrilateral_position[0].rect
```

### Comparing `correpy-0.3.0/pyproject.toml` & `correpy-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "correpy"
-version = "0.3.0"
+version = "0.4.1"
 description = "CorrePy (Corretagem Python) é uma lib responsável por parsear notas de corretagem no padrão B3 (Sinacor) e retornar os dados no formato JSON."
 authors = ["Thiago  Salvatore <thiago.salvatore@gmail.com>"]
 license = "Apache License 2.0"
 keywords = ["corretagem", "parser", "b3", "nota de corretagem", "imposto de renda"]
 readme = "README.md"
 homepage = "https://github.com/thiagosalvatore/correpy"
 repository = "https://github.com/thiagosalvatore/correpy"
```

### Comparing `correpy-0.3.0/PKG-INFO` & `correpy-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: correpy
-Version: 0.3.0
+Version: 0.4.1
 Summary: CorrePy (Corretagem Python) é uma lib responsável por parsear notas de corretagem no padrão B3 (Sinacor) e retornar os dados no formato JSON.
 Home-page: https://github.com/thiagosalvatore/correpy
 License: Apache-2.0
 Keywords: corretagem,parser,b3,nota de corretagem,imposto de renda
 Author: Thiago  Salvatore
 Author-email: thiago.salvatore@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -97,28 +97,30 @@
 ```
 
 ### Descrição das entidades
 Abaixo você pode encontrar a descrição de cada um dos campos retornados. 
 
 #### Brokerage Note
 
-| BrokerageNote    |                                     |
-|------------------|-------------------------------------|
-| reference_date   | Data do pregão                      |
-| settlement_fee   | Taxa de liquidação                  |
-| registration_fee | Taxa de registro                    |
-| term_fee         | Taxa de termo/opções                |
-| ana_fee          | Taxa A.N.A                          |
-| emoluments       | Emolumentos                         |
-| operational_fee  | Taxa Operacional                    |
-| execution        | Execução                            |
-| custody_fee      | Taxa de custódia                    |
-| taxes            | Impostos                            |
-| others           | Outros                              |
-| transactions     | Lista de [transações](#transaction) |
+| BrokerageNote         |                                     |
+|-----------------------|-------------------------------------|
+| reference_id          | Número da nota                      |
+| reference_date        | Data do pregão                      |
+| settlement_fee        | Taxa de liquidação                  |
+| registration_fee      | Taxa de registro                    |
+| term_fee              | Taxa de termo/opções                |
+| ana_fee               | Taxa A.N.A                          |
+| emoluments            | Emolumentos                         |
+| operational_fee       | Taxa Operacional                    |
+| execution             | Execução                            |
+| custody_fee           | Taxa de custódia                    |
+| source_withheld_taxes | IRRF                    |
+| taxes                 | Impostos                            |
+| others                | Outros                              |
+| transactions          | Lista de [transações](#transaction) |
 
 #### Transaction
 
 | Transaction          |                                                            |
 |----------------------|------------------------------------------------------------|
 | transaction_type     | Enum com o tipo de transação (BUY - compra, SELL - venda)  |
 | amount               | Quantidade                                                 |
@@ -139,7 +141,8 @@
 
 1. MyPy para checagem estática de tipos
 2. PyLint
 3. Black
 4. isort
 
 Para verificar se o seu código continua de acordo com os critérios definidos, basta rodar `./pipeline/lint.sh`.
+
```

