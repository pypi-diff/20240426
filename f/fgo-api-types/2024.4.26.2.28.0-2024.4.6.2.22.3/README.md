# Comparing `tmp/fgo_api_types-2024.4.26.2.28.0.tar.gz` & `tmp/fgo_api_types-2024.4.6.2.22.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2024.4.26.2.28.0.tar", max compression
+gzip compressed data, was "fgo_api_types-2024.4.6.2.22.3.tar", max compression
```

## Comparing `fgo_api_types-2024.4.26.2.28.0.tar` & `fgo_api_types-2024.4.6.2.22.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2024-04-26 02:27:45.580986 fgo_api_types-2024.4.26.2.28.0/LICENSE
--rw-r--r--   0        0        0      449 2024-04-26 02:27:45.580986 fgo_api_types-2024.4.26.2.28.0/README.md
--rw-r--r--   0        0        0        0 2024-04-26 02:28:00.932926 fgo_api_types-2024.4.26.2.28.0/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2024-04-26 02:28:00.932926 fgo_api_types-2024.4.26.2.28.0/fgo_api_types/base.py
--rw-r--r--   0        0        0     4368 2024-04-26 02:28:00.932926 fgo_api_types-2024.4.26.2.28.0/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3762 2024-04-26 02:28:00.932926 fgo_api_types-2024.4.26.2.28.0/fgo_api_types/common.py
--rw-r--r--   0        0        0    40935 2024-04-26 02:28:00.932926 fgo_api_types-2024.4.26.2.28.0/fgo_api_types/enums.py
--rw-r--r--   0        0        0   178091 2024-04-26 02:28:00.932926 fgo_api_types-2024.4.26.2.28.0/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    85943 2024-04-26 02:28:00.932926 fgo_api_types-2024.4.26.2.28.0/fgo_api_types/nice.py
--rw-r--r--   0        0        0    59051 2024-04-26 02:28:00.932926 fgo_api_types-2024.4.26.2.28.0/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4518 2024-04-26 02:28:00.932926 fgo_api_types-2024.4.26.2.28.0/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    19285 2024-04-26 02:28:00.932926 fgo_api_types-2024.4.26.2.28.0/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2024-04-26 02:28:01.248925 fgo_api_types-2024.4.26.2.28.0/pyproject.toml
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 fgo_api_types-2024.4.26.2.28.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-06 02:21:48.273692 fgo_api_types-2024.4.6.2.22.3/LICENSE
+-rw-r--r--   0        0        0      449 2024-04-06 02:21:48.273692 fgo_api_types-2024.4.6.2.22.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4368 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3762 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/common.py
+-rw-r--r--   0        0        0    40655 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   176026 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    85618 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    59051 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4518 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    19285 2024-04-06 02:22:03.377702 fgo_api_types-2024.4.6.2.22.3/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2024-04-06 02:22:03.705703 fgo_api_types-2024.4.6.2.22.3/pyproject.toml
+-rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 fgo_api_types-2024.4.6.2.22.3/PKG-INFO
```

### Comparing `fgo_api_types-2024.4.26.2.28.0/LICENSE` & `fgo_api_types-2024.4.6.2.22.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.26.2.28.0/fgo_api_types/basic.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.26.2.28.0/fgo_api_types/common.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.26.2.28.0/fgo_api_types/enums.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,17 +356,14 @@
     salemAbby = "salemAbby"
     uOlgaMarie = "uOlgaMarie"
     uOlgaMarieAlienGod = "uOlgaMarieAlienGod"
     beast = "beast"
     beastVI = "beastVI"
     beastVIBoss = "beastVIBoss"
     uOlgaMarieFlare = "uOlgaMarieFlare"
-    uOlgaMarieAqua = "uOlgaMarieAqua"
-    uOlgaMarieFlareCollection = "uOlgaMarieFlareCollection"
-    uOlgaMarieAquaCollection = "uOlgaMarieAquaCollection"
     atlasUnmappedClass = "atlasUnmappedClass"
     # OTHER = "OTHER"
     ALL = "ALL"
     # EXTRA = "EXTRA"
     # MIX = "MIX"
 
 
@@ -403,31 +400,28 @@
     30: SvtClass.beastILost,
     31: SvtClass.uOlgaMarieAlienGod,
     32: SvtClass.uOlgaMarie,
     33: SvtClass.beast,
     34: SvtClass.beastVI,
     35: SvtClass.beastVIBoss,
     36: SvtClass.uOlgaMarieFlare,
-    37: SvtClass.uOlgaMarieAqua,
     97: SvtClass.unknown,
     # 98
     # 99
     # 100
     107: SvtClass.agarthaPenth,
     124: SvtClass.cccFinaleEmiyaAlter,
     125: SvtClass.salemAbby,
     # 1000: SvtClass.OTHER,
     # For Support List
     1001: SvtClass.ALL,
     # 1002: SvtClass.EXTRA,
     # 1003: SvtClass.MIX,
     # 1004: SvtClass.EXTRA1,
     # 1005: SvtClass.EXTRA2,
-    9001: SvtClass.uOlgaMarieFlareCollection,
-    9002: SvtClass.uOlgaMarieAquaCollection,
 }
 
 
 def get_class_name(class_id: int) -> SvtClass | str:
     if class_id in CLASS_NAME:
         return CLASS_NAME[class_id]
     else:
```

### Comparing `fgo_api_types-2024.4.26.2.28.0/fgo_api_types/gameenums.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/gameenums.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,16 +258,14 @@
     SUB_FIELD_BUFF = 131
     EVENT_FORTIFICATION_POINT_UP = 132
     GAIN_NP_INDIVIDUAL_SUM = 133
     SET_QUEST_ROUTE_FLAG = 134
     LAST_USE_PLAYER_SKILL_COPY = 135
     CHANGE_ENEMY_MASTER_FACE = 136
     DAMAGE_VALUE_SAFE_ONCE = 137
-    ADD_BATTLE_VALUE = 138
-    SET_BATTLE_VALUE = 139
 
 
 class NiceFuncType(StrEnum):
     """Function Type Enum"""
 
     none = "none"
     addState = "addState"
@@ -366,16 +364,14 @@
     subFieldBuff = "subFieldBuff"
     eventFortificationPointUp = "eventFortificationPointUp"
     gainNpIndividualSum = "gainNpIndividualSum"
     setQuestRouteFlag = "setQuestRouteFlag"
     lastUsePlayerSkillCopy = "lastUsePlayerSkillCopy"
     changeEnemyMasterFace = "changeEnemyMasterFace"
     damageValueSafeOnce = "damageValueSafeOnce"
-    addBattleValue = "addBattleValue"
-    setBattleValue = "setBattleValue"
 
 
 FUNC_TYPE_NAME: dict[int, NiceFuncType] = {
     0: NiceFuncType.none,
     1: NiceFuncType.addState,
     2: NiceFuncType.subState,
     3: NiceFuncType.damage,
@@ -472,16 +468,14 @@
     131: NiceFuncType.subFieldBuff,
     132: NiceFuncType.eventFortificationPointUp,
     133: NiceFuncType.gainNpIndividualSum,
     134: NiceFuncType.setQuestRouteFlag,
     135: NiceFuncType.lastUsePlayerSkillCopy,
     136: NiceFuncType.changeEnemyMasterFace,
     137: NiceFuncType.damageValueSafeOnce,
-    138: NiceFuncType.addBattleValue,
-    139: NiceFuncType.setBattleValue,
 }
 
 
 class FuncTargetType(IntEnum):
     SELF = 0
     PT_ONE = 1
     PT_ANOTHER = 2
@@ -657,15 +651,15 @@
     SUB_MAXHP = 82
     BATTLESTART_FUNCTION = 83
     WAVESTART_FUNCTION = 84
     SELFTURNEND_FUNCTION = 85
     DAMAGE_FUNCTION = 86
     UP_GIVEGAIN_HP = 87
     DOWN_GIVEGAIN_HP = 88
-    COMMANDATTACK_AFTER_FUNCTION = 89
+    COMMANDATTACK_FUNCTION = 89
     DEADATTACK_FUNCTION = 90
     UP_SPECIALDEFENCE = 91
     DOWN_SPECIALDEFENCE = 92
     UP_DAMAGEDROPNP = 93
     DOWN_DAMAGEDROPNP = 94
     ENTRY_FUNCTION = 95
     UP_CHAGETD = 96
@@ -696,25 +690,25 @@
     PIERCE_DEFENCE = 121
     UP_GUTS_HP = 122
     DOWN_GUTS_HP = 123
     UP_FUNCGAIN_NP = 124
     DOWN_FUNCGAIN_NP = 125
     UP_FUNC_HP_REDUCE = 126
     DOWN_FUNC_HP_REDUCE = 127
-    UP_DEFENCE_COMMANDDAMAGE = 128
-    DOWN_DEFENCE_COMMANDDAMAGE = 129
+    UP_DEFENCECOMMAN_DAMAGE = 128
+    DOWN_DEFENCECOMMAN_DAMAGE = 129
     NPATTACK_PREV_BUFF = 130
     FIX_COMMANDCARD = 131
     DONOT_GAINNP = 132
     FIELD_INDIVIDUALITY = 133
     DONOT_ACT_COMMANDTYPE = 134
     UP_DAMAGE_EVENT_POINT = 135
     UP_DAMAGE_SPECIAL = 136
-    ATTACK_AFTER_FUNCTION = 137
-    COMMANDCODEATTACK_BEFORE_FUNCTION = 138
+    ATTACK_FUNCTION = 137
+    COMMANDCODEATTACK_FUNCTION = 138
     DONOT_NOBLE_COND_MISMATCH = 139
     DONOT_SELECT_COMMANDCARD = 140
     DONOT_REPLACE = 141
     SHORTEN_USER_EQUIP_SKILL = 142
     TD_TYPE_CHANGE = 143
     OVERWRITE_CLASS_RELATION = 144
     TD_TYPE_CHANGE_ARTS = 145
@@ -840,15 +834,15 @@
     subMaxhp = "subMaxhp"
     battlestartFunction = "battlestartFunction"
     wavestartFunction = "wavestartFunction"
     selfturnendFunction = "selfturnendFunction"
     damageFunction = "damageFunction"
     upGivegainHp = "upGivegainHp"
     downGivegainHp = "downGivegainHp"
-    commandattackAfterFunction = "commandattackAfterFunction"
+    commandattackFunction = "commandattackFunction"
     deadattackFunction = "deadattackFunction"
     upSpecialdefence = "upSpecialdefence"
     downSpecialdefence = "downSpecialdefence"
     upDamagedropnp = "upDamagedropnp"
     downDamagedropnp = "downDamagedropnp"
     entryFunction = "entryFunction"
     upChagetd = "upChagetd"
@@ -879,25 +873,25 @@
     pierceDefence = "pierceDefence"
     upGutsHp = "upGutsHp"
     downGutsHp = "downGutsHp"
     upFuncgainNp = "upFuncgainNp"
     downFuncgainNp = "downFuncgainNp"
     upFuncHpReduce = "upFuncHpReduce"
     downFuncHpReduce = "downFuncHpReduce"
-    upDefenceCommanddamage = "upDefenceCommanddamage"
-    downDefenceCommanddamage = "downDefenceCommanddamage"
+    upDefencecommanDamage = "upDefencecommanDamage"
+    downDefencecommanDamage = "downDefencecommanDamage"
     npattackPrevBuff = "npattackPrevBuff"
     fixCommandcard = "fixCommandcard"
     donotGainnp = "donotGainnp"
     fieldIndividuality = "fieldIndividuality"
     donotActCommandtype = "donotActCommandtype"
     upDamageEventPoint = "upDamageEventPoint"
     upDamageSpecial = "upDamageSpecial"
-    attackAfterFunction = "attackAfterFunction"
-    commandcodeattackBeforeFunction = "commandcodeattackBeforeFunction"
+    attackFunction = "attackFunction"
+    commandcodeattackFunction = "commandcodeattackFunction"
     donotNobleCondMismatch = "donotNobleCondMismatch"
     donotSelectCommandcard = "donotSelectCommandcard"
     donotReplace = "donotReplace"
     shortenUserEquipSkill = "shortenUserEquipSkill"
     tdTypeChange = "tdTypeChange"
     overwriteClassRelation = "overwriteClassRelation"
     tdTypeChangeArts = "tdTypeChangeArts"
@@ -1021,15 +1015,15 @@
     82: NiceBuffType.subMaxhp,
     83: NiceBuffType.battlestartFunction,
     84: NiceBuffType.wavestartFunction,
     85: NiceBuffType.selfturnendFunction,
     86: NiceBuffType.damageFunction,
     87: NiceBuffType.upGivegainHp,
     88: NiceBuffType.downGivegainHp,
-    89: NiceBuffType.commandattackAfterFunction,
+    89: NiceBuffType.commandattackFunction,
     90: NiceBuffType.deadattackFunction,
     91: NiceBuffType.upSpecialdefence,
     92: NiceBuffType.downSpecialdefence,
     93: NiceBuffType.upDamagedropnp,
     94: NiceBuffType.downDamagedropnp,
     95: NiceBuffType.entryFunction,
     96: NiceBuffType.upChagetd,
@@ -1060,25 +1054,25 @@
     121: NiceBuffType.pierceDefence,
     122: NiceBuffType.upGutsHp,
     123: NiceBuffType.downGutsHp,
     124: NiceBuffType.upFuncgainNp,
     125: NiceBuffType.downFuncgainNp,
     126: NiceBuffType.upFuncHpReduce,
     127: NiceBuffType.downFuncHpReduce,
-    128: NiceBuffType.upDefenceCommanddamage,
-    129: NiceBuffType.downDefenceCommanddamage,
+    128: NiceBuffType.upDefencecommanDamage,
+    129: NiceBuffType.downDefencecommanDamage,
     130: NiceBuffType.npattackPrevBuff,
     131: NiceBuffType.fixCommandcard,
     132: NiceBuffType.donotGainnp,
     133: NiceBuffType.fieldIndividuality,
     134: NiceBuffType.donotActCommandtype,
     135: NiceBuffType.upDamageEventPoint,
     136: NiceBuffType.upDamageSpecial,
-    137: NiceBuffType.attackAfterFunction,
-    138: NiceBuffType.commandcodeattackBeforeFunction,
+    137: NiceBuffType.attackFunction,
+    138: NiceBuffType.commandcodeattackFunction,
     139: NiceBuffType.donotNobleCondMismatch,
     140: NiceBuffType.donotSelectCommandcard,
     141: NiceBuffType.donotReplace,
     142: NiceBuffType.shortenUserEquipSkill,
     143: NiceBuffType.tdTypeChange,
     144: NiceBuffType.overwriteClassRelation,
     145: NiceBuffType.tdTypeChangeArts,
@@ -1186,15 +1180,15 @@
     REGAIN_NP_USED_NOBLE = 50
     FUNCTION_DEAD = 51
     MAXHP_RATE = 52
     MAXHP_VALUE = 53
     FUNCTION_WAVESTART = 54
     FUNCTION_SELFTURNEND = 55
     GIVE_GAIN_HP = 56
-    FUNCTION_COMMANDATTACK_AFTER = 57
+    FUNCTION_COMMANDATTACK = 57
     FUNCTION_DEADATTACK = 58
     FUNCTION_ENTRY = 59
     CHAGETD = 60
     GRANT_SUBSTATE = 61
     TOLERANCE_SUBSTATE = 62
     GRANT_INSTANTDEATH = 63
     FUNCTION_DAMAGE = 64
@@ -1209,16 +1203,16 @@
     FUNCTION_NPATTACK = 73
     FIX_COMMANDCARD = 74
     DONOT_GAINNP = 75
     FIELD_INDIVIDUALITY = 76
     DONOT_ACT_COMMANDTYPE = 77
     DAMAGE_EVENT_POINT = 78
     DAMAGE_SPECIAL = 79
-    FUNCTION_ATTACK_AFTER = 80
-    FUNCTION_COMMANDCODEATTACK_BEFORE = 81
+    FUNCTION_ATTACK = 80
+    FUNCTION_COMMANDCODEATTACK = 81
     DONOT_NOBLE_COND_MISMATCH = 82
     DONOT_SELECT_COMMANDCARD = 83
     DONOT_REPLACE = 84
     SHORTEN_USER_EQUIP_SKILL = 85
     TD_TYPE_CHANGE = 86
     OVERWRITE_CLASS_RELATION = 87
     FUNCTION_COMMANDATTACK_BEFORE = 88
@@ -1320,15 +1314,15 @@
     regainNpUsedNoble = "regainNpUsedNoble"
     functionDead = "functionDead"
     maxhpRate = "maxhpRate"
     maxhpValue = "maxhpValue"
     functionWavestart = "functionWavestart"
     functionSelfturnend = "functionSelfturnend"
     giveGainHp = "giveGainHp"
-    functionCommandattackAfter = "functionCommandattackAfter"
+    functionCommandattack = "functionCommandattack"
     functionDeadattack = "functionDeadattack"
     functionEntry = "functionEntry"
     chagetd = "chagetd"
     grantSubstate = "grantSubstate"
     toleranceSubstate = "toleranceSubstate"
     grantInstantdeath = "grantInstantdeath"
     functionDamage = "functionDamage"
@@ -1343,16 +1337,16 @@
     functionNpattack = "functionNpattack"
     fixCommandcard = "fixCommandcard"
     donotGainnp = "donotGainnp"
     fieldIndividuality = "fieldIndividuality"
     donotActCommandtype = "donotActCommandtype"
     damageEventPoint = "damageEventPoint"
     damageSpecial = "damageSpecial"
-    functionAttackAfter = "functionAttackAfter"
-    functionCommandcodeattackBefore = "functionCommandcodeattackBefore"
+    functionAttack = "functionAttack"
+    functionCommandcodeattack = "functionCommandcodeattack"
     donotNobleCondMismatch = "donotNobleCondMismatch"
     donotSelectCommandcard = "donotSelectCommandcard"
     donotReplace = "donotReplace"
     shortenUserEquipSkill = "shortenUserEquipSkill"
     tdTypeChange = "tdTypeChange"
     overwriteClassRelation = "overwriteClassRelation"
     functionCommandattackBefore = "functionCommandattackBefore"
@@ -1452,15 +1446,15 @@
     50: NiceBuffAction.regainNpUsedNoble,
     51: NiceBuffAction.functionDead,
     52: NiceBuffAction.maxhpRate,
     53: NiceBuffAction.maxhpValue,
     54: NiceBuffAction.functionWavestart,
     55: NiceBuffAction.functionSelfturnend,
     56: NiceBuffAction.giveGainHp,
-    57: NiceBuffAction.functionCommandattackAfter,
+    57: NiceBuffAction.functionCommandattack,
     58: NiceBuffAction.functionDeadattack,
     59: NiceBuffAction.functionEntry,
     60: NiceBuffAction.chagetd,
     61: NiceBuffAction.grantSubstate,
     62: NiceBuffAction.toleranceSubstate,
     63: NiceBuffAction.grantInstantdeath,
     64: NiceBuffAction.functionDamage,
@@ -1475,16 +1469,16 @@
     73: NiceBuffAction.functionNpattack,
     74: NiceBuffAction.fixCommandcard,
     75: NiceBuffAction.donotGainnp,
     76: NiceBuffAction.fieldIndividuality,
     77: NiceBuffAction.donotActCommandtype,
     78: NiceBuffAction.damageEventPoint,
     79: NiceBuffAction.damageSpecial,
-    80: NiceBuffAction.functionAttackAfter,
-    81: NiceBuffAction.functionCommandcodeattackBefore,
+    80: NiceBuffAction.functionAttack,
+    81: NiceBuffAction.functionCommandcodeattack,
     82: NiceBuffAction.donotNobleCondMismatch,
     83: NiceBuffAction.donotSelectCommandcard,
     84: NiceBuffAction.donotReplace,
     85: NiceBuffAction.shortenUserEquipSkill,
     86: NiceBuffAction.tdTypeChange,
     87: NiceBuffAction.overwriteClassRelation,
     88: NiceBuffAction.functionCommandattackBefore,
@@ -1760,15 +1754,14 @@
     EUQIP_SKILL_USE_ITEM = 28
     SVT_COIN = 29
     FRIENDSHIP_UP_ITEM = 30
     PP = 31
     TRADE_AP = 32
     RI = 33
     STORMPOD = 34
-    BATTLE_ITEM = 35
 
 
 class NiceItemType(StrEnum):
     """Item Type Enum"""
 
     qp = "qp"
     stone = "stone"
@@ -1800,15 +1793,14 @@
     euqipSkillUseItem = "euqipSkillUseItem"
     svtCoin = "svtCoin"
     friendshipUpItem = "friendshipUpItem"
     pp = "pp"
     tradeAp = "tradeAp"
     ri = "ri"
     stormpod = "stormpod"
-    battleItem = "battleItem"
 
 
 ITEM_TYPE_NAME: dict[int, NiceItemType] = {
     1: NiceItemType.qp,
     2: NiceItemType.stone,
     3: NiceItemType.apRecover,
     4: NiceItemType.apAdd,
@@ -1838,15 +1830,14 @@
     28: NiceItemType.euqipSkillUseItem,
     29: NiceItemType.svtCoin,
     30: NiceItemType.friendshipUpItem,
     31: NiceItemType.pp,
     32: NiceItemType.tradeAp,
     33: NiceItemType.ri,
     34: NiceItemType.stormpod,
-    35: NiceItemType.battleItem,
 }
 
 
 class GiftType(IntEnum):
     SERVANT = 1
     ITEM = 2
     FRIENDSHIP = 3
@@ -1858,15 +1849,14 @@
     COSTUME_RELEASE = 9
     COSTUME_GET = 10
     COMMAND_CODE = 11
     EVENT_POINT_BUFF = 12
     EVENT_BOARD_GAME_TOKEN = 13
     EVENT_COMMAND_ASSIST = 14
     EVENT_HEEL_PORTRAIT = 15
-    BATTLE_ITEM = 16
 
 
 class NiceGiftType(StrEnum):
     """Gift Type Enum"""
 
     servant = "servant"
     item = "item"
@@ -1879,15 +1869,14 @@
     costumeRelease = "costumeRelease"
     costumeGet = "costumeGet"
     commandCode = "commandCode"
     eventPointBuff = "eventPointBuff"
     eventBoardGameToken = "eventBoardGameToken"
     eventCommandAssist = "eventCommandAssist"
     eventHeelPortrait = "eventHeelPortrait"
-    battleItem = "battleItem"
 
 
 GIFT_TYPE_NAME: dict[int, NiceGiftType] = {
     1: NiceGiftType.servant,
     2: NiceGiftType.item,
     3: NiceGiftType.friendship,
     4: NiceGiftType.userExp,
@@ -1898,15 +1887,14 @@
     9: NiceGiftType.costumeRelease,
     10: NiceGiftType.costumeGet,
     11: NiceGiftType.commandCode,
     12: NiceGiftType.eventPointBuff,
     13: NiceGiftType.eventBoardGameToken,
     14: NiceGiftType.eventCommandAssist,
     15: NiceGiftType.eventHeelPortrait,
-    16: NiceGiftType.battleItem,
 }
 
 
 class ShopType(IntEnum):
     NONE = 0
     EVENT_ITEM = 1
     MANA = 2
@@ -3831,20 +3819,14 @@
     COUNT_PLAYER_SKILL_EQUAL_INCLUDE_MASTER_SKILL = 190
     TOTAL_TURN_HIGHER = 191
     TOTAL_TURN_LOWER = 192
     TOTAL_TURN_EQUAL = 193
     CHECK_WAR_BOARD_SQUARE_INDIVIDUALITY = 194
     CHECK_PT_HIGHER_NPGAUGE = 195
     CHECK_SELF_HIGHER_NPGAUGE = 196
-    CHECK_BATTLE_VALUE_ABOVE = 197
-    CHECK_BATTLE_VALUE_EQUAL = 198
-    CHECK_BATTLE_VALUE_NOT_EQUAL = 199
-    CHECK_BATTLE_VALUE_BELOW = 200
-    CHECK_BATTLE_VALUE_BETWEEN = 201
-    CHECK_BATTLE_VALUE_NOT_BETWEEN = 202
 
 
 class NiceAiCond(StrEnum):
     """AI Cond Enum"""
 
     none = "none"
     hpHigher = "hpHigher"
@@ -4015,20 +3997,14 @@
     countPlayerSkillEqualIncludeMasterSkill = "countPlayerSkillEqualIncludeMasterSkill"
     totalTurnHigher = "totalTurnHigher"
     totalTurnLower = "totalTurnLower"
     totalTurnEqual = "totalTurnEqual"
     checkWarBoardSquareIndividuality = "checkWarBoardSquareIndividuality"
     checkPtHigherNpgauge = "checkPtHigherNpgauge"
     checkSelfHigherNpgauge = "checkSelfHigherNpgauge"
-    checkBattleValueAbove = "checkBattleValueAbove"
-    checkBattleValueEqual = "checkBattleValueEqual"
-    checkBattleValueNotEqual = "checkBattleValueNotEqual"
-    checkBattleValueBelow = "checkBattleValueBelow"
-    checkBattleValueBetween = "checkBattleValueBetween"
-    checkBattleValueNotBetween = "checkBattleValueNotBetween"
 
 
 AI_COND_NAME: dict[int, NiceAiCond] = {
     0: NiceAiCond.none,
     10: NiceAiCond.hpHigher,
     11: NiceAiCond.hpLower,
     20: NiceAiCond.actcount,
@@ -4181,20 +4157,14 @@
     190: NiceAiCond.countPlayerSkillEqualIncludeMasterSkill,
     191: NiceAiCond.totalTurnHigher,
     192: NiceAiCond.totalTurnLower,
     193: NiceAiCond.totalTurnEqual,
     194: NiceAiCond.checkWarBoardSquareIndividuality,
     195: NiceAiCond.checkPtHigherNpgauge,
     196: NiceAiCond.checkSelfHigherNpgauge,
-    197: NiceAiCond.checkBattleValueAbove,
-    198: NiceAiCond.checkBattleValueEqual,
-    199: NiceAiCond.checkBattleValueNotEqual,
-    200: NiceAiCond.checkBattleValueBelow,
-    201: NiceAiCond.checkBattleValueBetween,
-    202: NiceAiCond.checkBattleValueNotBetween,
 }
 
 
 class AiActType(IntEnum):
     NONE = 0
     RANDOM = 1
     ATTACK = 2
@@ -4696,15 +4666,14 @@
     CHECK_TARGET_SKILL_THISTURN = 34
     CHECK_SELECT_CHAIN = 35
     COUNT_PLAYER_NP = 36
     COUNT_PLAYER_SKILL = 37
     COUNT_PLAYER_SKILL_INCLUDE_MASTER_SKILL = 38
     TOTAL_TURN = 39
     WAR_BOARD_SQUARE_INDIVIDUALITY = 40
-    CHECK_BATTLE_VALUE = 41
 
 
 class NiceAiCondParameter(StrEnum):
     """Ai Condition Parameter"""
 
     none = "none"
     turn = "turn"
@@ -4743,15 +4712,14 @@
     checkTargetSkillThisturn = "checkTargetSkillThisturn"
     checkSelectChain = "checkSelectChain"
     countPlayerNp = "countPlayerNp"
     countPlayerSkill = "countPlayerSkill"
     countPlayerSkillIncludeMasterSkill = "countPlayerSkillIncludeMasterSkill"
     totalTurn = "totalTurn"
     warBoardSquareIndividuality = "warBoardSquareIndividuality"
-    checkBattleValue = "checkBattleValue"
 
 
 AI_COND_PARAMETER_NAME: dict[int, NiceAiCondParameter] = {
     0: NiceAiCondParameter.none,
     1: NiceAiCondParameter.turn,
     2: NiceAiCondParameter.space,
     3: NiceAiCondParameter.prevActid,
@@ -4788,15 +4756,14 @@
     34: NiceAiCondParameter.checkTargetSkillThisturn,
     35: NiceAiCondParameter.checkSelectChain,
     36: NiceAiCondParameter.countPlayerNp,
     37: NiceAiCondParameter.countPlayerSkill,
     38: NiceAiCondParameter.countPlayerSkillIncludeMasterSkill,
     39: NiceAiCondParameter.totalTurn,
     40: NiceAiCondParameter.warBoardSquareIndividuality,
-    41: NiceAiCondParameter.checkBattleValue,
 }
 
 
 class AiRefineTarget(IntEnum):
     ANY = 0
     ALL = 1
     HIGHER = 2
@@ -4827,42 +4794,36 @@
     NONE = 0
     EQUAL = 1
     EQUAL_NOT = 2
     HIGHER = 3
     LOWER = 4
     MULTIPLE = 5
     EXIST = 6
-    BETWEEN = 7
-    BETWEEN_NOT = 8
 
 
 class NiceAiCondCheck(StrEnum):
     """Ai Condition Check"""
 
     none = "none"
     equal = "equal"
     equalNot = "equalNot"
     higher = "higher"
     lower_ = "lower"
     multiple = "multiple"
     exist = "exist"
-    between = "between"
-    betweenNot = "betweenNot"
 
 
 AI_COND_CHECK_NAME: dict[int, NiceAiCondCheck] = {
     0: NiceAiCondCheck.none,
     1: NiceAiCondCheck.equal,
     2: NiceAiCondCheck.equalNot,
     3: NiceAiCondCheck.higher,
     4: NiceAiCondCheck.lower_,
     5: NiceAiCondCheck.multiple,
     6: NiceAiCondCheck.exist,
-    7: NiceAiCondCheck.between,
-    8: NiceAiCondCheck.betweenNot,
 }
 
 
 class TreasureDeviceEffectFlag(IntEnum):
     SUPPORT = -1
     ATTACK_ENEMY_ALL = 1
     ATTACK_ENEMY_ONE = 2
@@ -5585,31 +5546,7 @@
     1: NiceSvtDeadType.escape,
     2: NiceSvtDeadType.stand,
     3: NiceSvtDeadType.effect,
     4: NiceSvtDeadType.wait,
     5: NiceSvtDeadType.energy,
     6: NiceSvtDeadType.crystal,
 }
-
-
-class AiAllocationSvtFlag(IntEnum):
-    ALL = 0
-    OWN = 1
-    FRIEND = 2
-    NPC = 4
-
-
-class NiceAiAllocationSvtFlag(StrEnum):
-    """AI Allocation Svt Flag"""
-
-    all = "all"
-    own = "own"
-    friend = "friend"
-    npc = "npc"
-
-
-AI_ALLOCATION_SVT_FLAG_NAME: dict[int, NiceAiAllocationSvtFlag] = {
-    0: NiceAiAllocationSvtFlag.all,
-    1: NiceAiAllocationSvtFlag.own,
-    2: NiceAiAllocationSvtFlag.friend,
-    4: NiceAiAllocationSvtFlag.npc,
-}
```

### Comparing `fgo_api_types-2024.4.26.2.28.0/fgo_api_types/nice.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/nice.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     StageLimitActType,
     SvtClass,
 )
 from .gameenums import (
     NiceAiActNum,
     NiceAiActTarget,
     NiceAiActType,
-    NiceAiAllocationSvtFlag,
     NiceAiCond,
     NiceBattleFieldEnvironmentGrantType,
     NiceBuffType,
     NiceCardType,
     NiceClassBoardSkillType,
     NiceClassBoardSquareFlag,
     NiceCombineAdjustTarget,
@@ -350,15 +349,15 @@
         default=None,
         description="The buff with this dataVal is removed if the linked buff is removed.",
     )
     AllowSubBgmPlaying: int | None = None
     NotAccompanyWhenLinkedTargetMoveState: int | None = None
     NotTargetSkillIdArray: list[int] | None = None
     ShortTurn: int | None = None
-    FieldIndividuality: list[int] | None = None
+    FieldIndividuality: int | None = None
     BGId: int | None = None
     BGType: int | None = None
     BgmId: int | None = None
     TakeOverFieldState: int | None = None
     TakeOverNextWaveBGAndBGM: int | None = None
     RemoveFieldBuffActorDeath: int | None = None
     FieldBuffGrantType: int | None = None
@@ -1771,14 +1770,15 @@
     condGroup: int
     condType: NiceCondType
     targetIds: list[int]
     targetNum: int
     conditionMessage: str
     closedMessage: str
     flag: int
+    detail: Optional[NiceEventMissionConditionDetail] = None
     details: list[NiceEventMissionConditionDetail] | None = None
 
 
 class NiceEventMission(BaseModelORJson):
     id: int
     flag: int
     type: NiceMissionType
@@ -1871,21 +1871,23 @@
 class NiceEventTreasureBox(BaseModelORJson):
     slot: int
     id: int
     idx: int
     treasureBoxGifts: list[NiceEventTreasureBoxGift]
     maxDrawNumOnce: int
     extraGifts: list[NiceGift]
+    commonConsume: NiceCommonConsume
     consumes: list[NiceCommonConsume]
 
 
 class NiceEventDiggingBlock(BaseModelORJson):
     id: int
     eventId: int
     image: HttpUrl
+    commonConsume: NiceCommonConsume
     consumes: list[NiceCommonConsume]
     objectId: int
     diggingEventPoint: int
     blockNum: int
 
 
 class NiceEventDiggingReward(BaseModelORJson):
@@ -1905,14 +1907,15 @@
     rewards: list[NiceEventDiggingReward]
 
 
 class NiceEventCooltimeReward(BaseModelORJson):
     spotId: int
     lv: int
     name: str
+    commonRelease: NiceCommonRelease
     releaseConditions: list[NiceCommonRelease]
     cooltime: int
     addEventPointRate: int
     gifts: list[NiceGift]
     upperLimitGiftNum: int
 
 
@@ -2462,20 +2465,14 @@
     id: int
     type: NiceBattleFieldEnvironmentGrantType
     priority: int
     individuality: list[NiceTrait]
     imageId: int
 
 
-class NiceAiAllocation(BaseModelORJson):
-    aiIds: list[int]
-    individuality: NiceTrait
-    applySvtType: list[NiceAiAllocationSvtFlag]
-
-
 class NiceStage(BaseModelORJson):
     wave: int
     bgm: NiceBgm
     startEffectId: int
     fieldAis: list[FieldAi] = []
     call: list[int] = Field([], title="Summon these NPC IDs")
     enemyFieldPosCount: int | None = None
@@ -2484,15 +2481,14 @@
     limitAct: StageLimitActType | None = Field(
         None, title="Action after turn countdown is over"
     )
     battleBg: NiceBattleBg | None = None
     NoEntryIds: list[int] | None = None
     waveStartMovies: list[NiceStageStartMovie] = []
     cutin: NiceStageCutIn | None = None
-    aiAllocations: list[NiceAiAllocation] | None = None
     originalScript: dict[str, Any]
     enemies: list[QuestEnemy] = []
 
 
 class NiceQuestMessage(BaseModelORJson):
     idx: int
     message: str
@@ -2596,35 +2592,30 @@
     detail: QuestEnemy | None = None
     aiIds: list[int]
 
 
 class NiceQuestPhaseOverwriteEquipSkill(BaseModelORJson):
     lv: int
     id: int
-    condId: int | None = None
 
 
 class NiceQuestPhaseOverwriteEquipSkills(BaseModelORJson):
-    iconId: int | None = None
-    cutInView: int | None = None  # 1: ShowMasterSkillCutIn
-    notDispEquipSkillIconSplit: int | None = None
+    iconId: int
     skills: list[NiceQuestPhaseOverwriteEquipSkill]
 
 
 class NiceQuestPhaseExtraDetail(BaseModelORJson):
     questSelect: list[int] | None = None
     singleForceSvtId: int | None = None
     hintTitle: str | None = None
     hintMessage: str | None = None
     aiNpc: NiceQuestPhaseAiNpc | None = None
     aiMultiNpc: list[NiceQuestPhaseAiNpc] | None = None
     overwriteEquipSkills: NiceQuestPhaseOverwriteEquipSkills | None = None
-    addEquipSkills: NiceQuestPhaseOverwriteEquipSkills | None = None
     waveSetup: int | None = None  # U Olga Marie Quest
-    interruptibleQuest: int | None = None
     masterImageId: int | None = None
 
 
 class NiceRestriction(BaseModelORJson):
     id: int
     name: str
     type: NiceRestrictionType
```

### Comparing `fgo_api_types-2024.4.26.2.28.0/fgo_api_types/raw.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.26.2.28.0/fgo_api_types/rayshift.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.26.2.28.0/fgo_api_types/search.py` & `fgo_api_types-2024.4.6.2.22.3/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.4.26.2.28.0/pyproject.toml` & `fgo_api_types-2024.4.6.2.22.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2024.04.26.02.28.00"
+version = "2024.04.06.02.22.03"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2024.4.26.2.28.0/PKG-INFO` & `fgo_api_types-2024.4.6.2.22.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2024.4.26.2.28.0
+Version: 2024.4.6.2.22.3
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

