# Comparing `tmp/ygoutil-0.1.0.tar.gz` & `tmp/ygoutil-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygoutil-0.1.0.tar", last modified: Sat Apr 27 21:30:56 2024, max compression
+gzip compressed data, was "ygoutil-0.2.0.tar", last modified: Wed May  1 20:08:21 2024, max compression
```

## Comparing `ygoutil-0.1.0.tar` & `ygoutil-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,33 @@
--rw-r--r--   0        0        0     1064 2024-04-27 21:30:40.337932 ygoutil-0.1.0/LICENSE
--rw-r--r--   0        0        0      115 2024-04-27 21:30:40.337932 ygoutil-0.1.0/README.md
--rw-r--r--   0        0        0      760 2024-04-27 21:30:56.834227 ygoutil-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       51 2024-04-27 21:30:40.337932 ygoutil-0.1.0/src/ygoutil/__init__.py
--rw-r--r--   0        0        0       22 2024-04-27 21:30:40.337932 ygoutil-0.1.0/src/ygoutil/__version__.py
--rw-r--r--   0        0        0     8740 2024-04-27 21:30:40.337932 ygoutil-0.1.0/src/ygoutil/card.py
--rw-r--r--   0        0        0     6686 2024-04-27 21:30:40.337932 ygoutil-0.1.0/src/ygoutil/constant.py
--rw-r--r--   0        0        0     7128 2024-04-27 21:30:40.337932 ygoutil-0.1.0/src/ygoutil/dataloader.py
--rw-r--r--   0        0        0      114 2024-04-27 21:30:40.337932 ygoutil-0.1.0/src/ygoutil/source/__init__.py
--rw-r--r--   0        0        0     8763 2024-04-27 21:30:40.337932 ygoutil-0.1.0/src/ygoutil/source/baige.py
--rw-r--r--   0        0        0     8709 2024-04-27 21:30:40.337932 ygoutil-0.1.0/src/ygoutil/source/ourocg.py
--rw-r--r--   0        0        0    13394 2024-04-27 21:30:40.337932 ygoutil-0.1.0/src/ygoutil/sqlbuilder.py
--rw-r--r--   0        0        0     6377 2024-04-27 21:30:40.337932 ygoutil-0.1.0/src/ygoutil/ygoRoom.py
--rw-r--r--   0        0        0        0 2024-04-27 21:30:40.337932 ygoutil-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      157 2024-04-27 21:30:40.337932 ygoutil-0.1.0/tests/test_card.py
--rw-r--r--   0        0        0     1929 2024-04-27 21:30:40.337932 ygoutil-0.1.0/tests/test_cdb.py
--rw-r--r--   0        0        0      223 2024-04-27 21:30:40.337932 ygoutil-0.1.0/tests/test_source/test_baige.py
--rw-r--r--   0        0        0      231 2024-04-27 21:30:40.337932 ygoutil-0.1.0/tests/test_source/test_ourocg.py
--rw-r--r--   0        0        0     1049 2024-04-27 21:30:40.337932 ygoutil-0.1.0/tests/test_sql.py
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 ygoutil-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-01 20:08:06.550142 ygoutil-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1156 2024-05-01 20:08:06.550142 ygoutil-0.2.0/README.md
+-rw-r--r--   0        0        0      760 2024-05-01 20:08:21.654206 ygoutil-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       51 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/__version__.py
+-rw-r--r--   0        0        0      314 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/__init__.py
+-rw-r--r--   0        0        0     5167 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/card.py
+-rw-r--r--   0        0        0     8321 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/constant.py
+-rw-r--r--   0        0        0      420 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/ids.py
+-rw-r--r--   0        0        0      277 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/misc.py
+-rw-r--r--   0        0        0    10640 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/card/unit.py
+-rw-r--r--   0        0        0     7128 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/dataloader.py
+-rw-r--r--   0        0        0        0 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/legacy/__init__.py
+-rw-r--r--   0        0        0     8786 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/legacy/card.py
+-rw-r--r--   0        0        0      138 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/__init__.py
+-rw-r--r--   0        0        0      259 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/baige/__init__.py
+-rw-r--r--   0        0        0     2856 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/baige/api.py
+-rw-r--r--   0        0        0     3607 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/baige/misc.py
+-rw-r--r--   0        0        0    12674 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/baige/page.py
+-rw-r--r--   0        0        0     1953 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/base.py
+-rw-r--r--   0        0        0        0 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/cdb/__init__.py
+-rw-r--r--   0        0        0     3556 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/cdb/misc.py
+-rw-r--r--   0        0        0     1370 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/misc.py
+-rw-r--r--   0        0        0    17833 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/source/ourocg.py
+-rw-r--r--   0        0        0    13403 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/sqlbuilder.py
+-rw-r--r--   0        0        0     6377 2024-05-01 20:08:06.550142 ygoutil-0.2.0/src/ygoutil/ygoRoom.py
+-rw-r--r--   0        0        0        0 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/test_card.py
+-rw-r--r--   0        0        0     1929 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/test_cdb.py
+-rw-r--r--   0        0        0     2447 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/test_source/test_baige.py
+-rw-r--r--   0        0        0     1687 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/test_source/test_ourocg.py
+-rw-r--r--   0        0        0     1054 2024-05-01 20:08:06.550142 ygoutil-0.2.0/tests/test_sql.py
+-rw-r--r--   0        0        0     1524 1970-01-01 00:00:00.000000 ygoutil-0.2.0/PKG-INFO
```

### Comparing `ygoutil-0.1.0/LICENSE` & `ygoutil-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ygoutil-0.1.0/pyproject.toml` & `ygoutil-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "beautifulsoup4>=4.12.3",
     "lxml>=5.2.1",
     "tomli>=2.0.1",
     "tomli-w>=1.0.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `ygoutil-0.1.0/src/ygoutil/card.py` & `ygoutil-0.2.0/src/ygoutil/legacy/card.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from typing import Iterable
 from functools import partialmethod
 
-from ygoutil.constant import CardType, CardRace, CardAttribute, LinkMark, linkMark2str, CardCategory
+from ygoutil.card.constant import CardType, CardRace, CardAttribute, LinkMark, LinkMarkStyle, CardCategory
 
 class Card:
     """YGO 卡片"""
 
     def __init__(self, types: Iterable[CardType | str] = None):
         self.id = None  # 卡号
         self.name: str | None = None  # 卡名（中文）
@@ -67,15 +67,15 @@
     @property
     def isLink(self):
         """ 是连接 """
         return CardType.Link in self.cardType
 
     def fillCardType(self, *types: CardType | str):
         for t in types:
-            if isinstance(t, str) and (ct := CardType.fromStr(t)):
+            if isinstance(t, str) and (ct := CardType.from_str(t)):
                 self.cardType.add(ct)
             else:
                 self.cardType.add(t)
 
     def initMonster(self):
         if self.isMonster:
             self.attack = None  # 攻击力
@@ -106,25 +106,26 @@
         if self.isRD:
             yield "RUSH DUEL  "
         else:
             yield self._checkAndFill(self.id, "{}  ")
         yield self._checkAndFill(self.limit, "{}")  # 禁限
         yield self._checkAndFill(self.ot, "  {}\n", "\n")  # O/T
         if self.set:  # 卡片字段
-            yield f"系列 {' '.join(self.set)}\n"
+            yield f"{' '.join(self.set)}\n"
         if self.isMonster:
             yield self._checkAndFill(str(self.race), "{}族")
             yield self._checkAndFill(str(self.attribute), "  {}属性")
             if self.isXyz:
                 yield self._checkAndFill(self.rank, "  {}阶\n")
             if self.isLink:
                 yield self._checkAndFill(self.linknum, "  LINK-{}\n")
                 # result+=self._checkAndFill(self.attack,"攻击力 {}\n")
                 yield self._checkAndFill(self.attack, "{}/-\n")
-                middle = linkMark2str[len(linkMark2str) // 2]
+                # middle = linkMark2str[len(linkMark2str) // 2]
+                middle = LinkMarkStyle.middle()
                 # marklist=["   "]*8
                 # marklist=[middle]*8
                 marklist = [
                     str(lm) if lm in self.linkmark else middle for lm in LinkMark
                 ]
                 marklines = [
                     f"{marklist[5]}{marklist[6]}{marklist[7]}\n",
@@ -182,15 +183,15 @@
                 self.defence = Card.dealAtkDef(t[8])
             if self.isXyz:
                 self.rank = self.level
             if self.isP:
                 self.Pmark = Card.getPmark(t[9])
             self.race = Card.bit2Race(t[10])
             self.attribute = Card.bit2Attribute(t[11])
-            self.category = Card.bit2Category(t[12])
+        self.category = Card.bit2Category(t[12])
 
     @staticmethod
     def dealAtkDef(val):
         return val if val >= 0 else "?"
 
     @staticmethod
     def dealLevel(val):
```

### Comparing `ygoutil-0.1.0/src/ygoutil/constant.py` & `ygoutil-0.2.0/src/ygoutil/card/constant.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 
 from typing import TYPE_CHECKING, Any
-from enum import Enum, IntFlag
+from enum import IntFlag, IntEnum
 
 def _repr(self: IntFlag):
     return f"{self.name or self.__class__.__name__}({hex(self.value)})"
 
 if TYPE_CHECKING:
     def _repr(self: Any) -> str:
         raise NotImplementedError
+    
 
 class CardType(IntFlag):
     """ 卡片种类 """
+    Unknown = 0x0
+
     Monster = 0x1
     Spell = 0x2
     Trap = 0x4
     # N/A=0x8
     Normal = 0x10  # 通常（怪兽）
     Effect = 0x20
     Fusion = 0x40
@@ -41,19 +44,21 @@
 
     def __str__(self):
         return cardType2str.get(self) or super().__str__()
 
     __repr__ = _repr
 
     @staticmethod
-    def fromStr(text: str):
+    def from_str(text: str):
         return str2cardType.get(text)
 
 
 cardType2str = {
+    CardType.Unknown: "未知",
+
     CardType.Monster: "怪兽",
     CardType.Normal: "通常",
     CardType.Effect: "效果",
     CardType.Tuner: "调整",
     CardType.Gemini: "二重",
     CardType.Flip: "反转",
     CardType.Union: "同盟",
@@ -75,51 +80,59 @@
     CardType.Equip: "装备",
     CardType.Field: "场地",
     CardType.Counter: "反击",
 }
 
 str2cardType = {v: k for k, v in cardType2str.items()}
 str2cardType["XYZ"] = CardType.Xyz
+str2cardType["P"] = CardType.Pendulum
+str2cardType["link"] = CardType.Link
 
 
 class CardAttribute(IntFlag):
     """ 卡片属性 """
+    Unknown = 0x00
+
     Earth = 0x01
     Water = 0x02
     Fire = 0x04
     Wind = 0x08
     Light = 0x10
     Dark = 0x20
     Divine = 0x40  # 神属性
 
     def __str__(self):
         return cardAttribute2str.get(self) or super().__str__()
 
     __repr__ = _repr
 
     @staticmethod
-    def fromStr(text: str):
+    def from_str(text: str):
         return str2cardAttribute.get(text)
 
 
 cardAttribute2str = {
+    CardAttribute.Unknown: "未知",
+
     CardAttribute.Earth: "地",
     CardAttribute.Water: "水",
     CardAttribute.Fire: "炎",
     CardAttribute.Wind: "风",
     CardAttribute.Light: "光",
     CardAttribute.Dark: "暗",
     CardAttribute.Divine: "神",
 }
 
 str2cardAttribute = {v: k for k, v in cardAttribute2str.items()}
 
 
 class CardRace(IntFlag):
     """ 卡片种族 """
+    Unknown = 0x0
+
     Warrior = 0x1
     Spellcaster = 0x2
     Fairy = 0x4
     Fiend = 0x8
     Zombie = 0x10
     Machine = 0x20
     Aqua = 0x40
@@ -145,19 +158,21 @@
 
     def __str__(self):
         return cardRace2str.get(self) or super().__str__()
 
     __repr__ = _repr
 
     @staticmethod
-    def fromStr(text: str):
+    def from_str(text: str):
         return str2cardRace.get(text)
 
 
 cardRace2str = {
+    CardRace.Unknown: "未知",
+
     CardRace.Warrior: "战士",
     CardRace.Spellcaster: "魔法师",
     CardRace.Fairy: "天使",
     CardRace.Fiend: "恶魔",
     CardRace.Zombie: "不死",
     CardRace.Machine: "机械",
     CardRace.Aqua: "水",
@@ -184,48 +199,73 @@
 
 str2cardRace = {v: k for k, v in cardRace2str.items()}
 str2cardRace["爬虫"] = CardRace.Reptile
 
 
 class LinkMark(IntFlag):
     """ 连接标记 """
+    Unknown = 0x000
+
     BottomLeft = 0x001
     Bottom = 0x002
     BottomRight = 0x004
     Left = 0x008
     # Middle=0x010
     Right = 0x020
     TopLeft = 0x040
     Top = 0x080
     TopRight = 0x100
 
-    def toNumber(self):  # 1-9
+    def to_number(self):  # 1-9
         binstr = bin(self.value)[2:]  # "0b01" => "01"  len("01")=2
         return len(binstr)
 
     def __str__(self):
-        return linkMark2str[self.toNumber() - 1]
+        return LinkMarkStyle.to(self.to_number() - 1)
 
     __repr__ = _repr
 
     @staticmethod
-    def fromNumber(num, withMid=False):  # num: 1-9
-        if withMid and num > 4:
+    def from_number(num: int, with_mid=False):  # num: 1-9
+        if with_mid and num > 4:
             num -= 1
         # return number2linkMark[num-1]
-        return list(LinkMark)[num - 1]
+        # return list(LinkMark)[num - 1]
+        return LinkMark(1 << (num - 1))
+
+class LinkMarkStyle:
+
+    _style = ("↙️", "⬇️", "↘️", "⬅️", "⬜", "➡️", "↖️", "⬆️", "↗️")
 
+    @classmethod
+    def style(cls, num: int):
+        cls._style = (
+            ("↙️", "⬇️", "↘️", "⬅️", "⬜", "➡️", "↖️", "⬆️", "↗️"),
+            ("↙", "⬇", "↘", "⬅", "    ", "➡", "↖", "⬆", "↗"),
+            (" ◣", " ↓ ", "◢ ", "←", "   ", "→", " ◤", " ↑ ", "◥ "),
+            # ("↙", "↓", "↘", "←", "   ", "→", "↖", "↑", "↗"),
+        )[num]
+        return cls._style
+
+    @classmethod
+    def to(cls, num: int):
+        return cls._style[num]
+    
+    @classmethod
+    def middle(cls):
+        return cls._style[4]
 
 # number2linkMark=[lm for lm in LinkMark]
 # linkMark2str=[" ◣"," ↓ ","◢ ","←","   ","→"," ◤"," ↑ ","◥ "]
-linkMark2str = ["↙", "⬇", "↘", "⬅", "    ", "➡", "↖", "⬆", "↗"]  # "⏺"
+# linkMark2str = ["↙", "⬇", "↘", "⬅", "    ", "➡", "↖", "⬆", "↗"]  # "⏺"
 
-
-class CardCategory(Enum):
+class CardCategory(IntFlag):
     """ 效果分类 """
+    未知 = 0x00
+
     魔陷破坏 = 0x01  # SpellTrapDestroy=0x01
     怪兽破坏 = 0x02  # MonsterDestroy=0x02
     除外 = 0x04  # Remove=0x04
     送去墓地 = 0x08  # ToGrave=0x08
     返回手卡 = 0x10  # ToHand=0x10
     返回卡组 = 0x20  # ToDeck=0x20
     手卡破坏 = 0x40  # DiscardHand=0x40
@@ -256,12 +296,43 @@
     效果无效 = 0x80000000
 
     def __str__(self):
         return self.name
 
     __repr__ = _repr
 
+class CardOT(IntFlag):
+    """ 卡片所属规则 """
+    Unknown = 0x0
+
+    OCG = 0b01
+    TCG = 0b10
+    # OCG_TCG = 0b11
+    Custom = 0b100
+    SC = 0b1000
+    # SC_OCG = 0b1001
+    # SC_TCG = 0b1010
+    # SC_OCG_TCG = 0b1011
+
+    __repr__ = _repr
+
+class CardLF(IntEnum):
+    """ 卡片禁限 """
+    禁止 = 0
+    限制 = 1
+    准限制 = 2
+    无限制 = 3
+
+    def __str__(self):
+        return self.name
+    
+    @staticmethod
+    def from_str(text: str):
+        try:
+            return CardLF[text]
+        except KeyError:
+            return None
 
 if __name__ == "__main__":
     print(CardType.Token)
     print(list(CardType))
     print(CardType.Xyz | CardType.Pendulum)
```

### Comparing `ygoutil-0.1.0/src/ygoutil/dataloader.py` & `ygoutil-0.2.0/src/ygoutil/dataloader.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.1.0/src/ygoutil/sqlbuilder.py` & `ygoutil-0.2.0/src/ygoutil/sqlbuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ygoutil.constant import CardType, CardRace, CardAttribute
+from ygoutil.card.constant import CardType, CardRace, CardAttribute
 
 def _ensureCardType(cardType: CardType):
         def deco(func):
             def wrapper(self: "SQLBuilder", *args):
                 raw = func(self, *args)
                 if self._checkHas("cardType", cardType):
                     return raw  # 原 SQL 条件
@@ -53,33 +53,33 @@
     def dealKeyword(text: str) -> str:  # 占位 暂不处理
         return text
 
     @staticmethod
     def dealRace(text: str) -> CardRace | None:
         if text.endswith("族"):
             text = text[:-1]
-        return CardRace.fromStr(text)
+        return CardRace.from_str(text)
 
     @staticmethod
     def dealAttribute(text: str) -> CardAttribute | None:
         if text.endswith("属性"):
             text = text[:-2]
-        return CardAttribute.fromStr(text)
+        return CardAttribute.from_str(text)
 
     @staticmethod
     def dealCardType(text: str) -> CardType | None:
         if text.endswith("卡"):
             text = text[:-1]
         base = text[-2:]
         baseType = None
         # if (text.endswith("怪兽") and text!="怪兽") or (text.endswith("魔法") and text!="魔法") or (text.endswith("陷阱") and text!="陷阱"):
         if base in ("怪兽", "魔法", "陷阱") and text != base:
             text = text[:-2]
-            baseType = CardType.fromStr(base)
-        textType = CardType.fromStr(text)
+            baseType = CardType.from_str(base)
+        textType = CardType.from_str(text)
         if baseType is not None and textType is not None:
             textType |= baseType
         return textType
 
     @staticmethod
     def _dealAD(text: str) -> int | None:
         if text.isdigit() and len(text) < 5:  # 4 位及以下的数
```

### Comparing `ygoutil-0.1.0/src/ygoutil/ygoRoom.py` & `ygoutil-0.2.0/src/ygoutil/ygoRoom.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.1.0/tests/test_cdb.py` & `ygoutil-0.2.0/tests/test_cdb.py`

 * *Files identical despite different names*

### Comparing `ygoutil-0.1.0/tests/test_sql.py` & `ygoutil-0.2.0/tests/test_sql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import pytest
 
 from ygoutil.sqlbuilder import SQLBuilder
-from ygoutil.constant import CardType
+from ygoutil.card.constant import CardType
 
 @pytest.fixture
 def builder():
     return SQLBuilder()
 
 def test_sql_builder(builder: SQLBuilder):
     # assert not builder.params
```

