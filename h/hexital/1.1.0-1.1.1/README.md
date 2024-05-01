# Comparing `tmp/hexital-1.1.0.tar.gz` & `tmp/hexital-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexital-1.1.0.tar", max compression
+gzip compressed data, was "hexital-1.1.1.tar", max compression
```

## Comparing `hexital-1.1.0.tar` & `hexital-1.1.1.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0     5503 2024-04-21 16:16:53.425528 hexital-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1067 2024-04-21 16:16:53.425528 hexital-1.1.0/LICENSE
--rw-r--r--   0        0        0    12974 2024-04-21 16:16:53.425528 hexital-1.1.0/README.md
--rw-r--r--   0        0        0      249 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/__init__.py
--rw-r--r--   0        0        0      835 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/analysis/__init__.py
--rw-r--r--   0        0        0    12246 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/analysis/movement.py
--rw-r--r--   0        0        0     3921 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/analysis/patterns.py
--rw-r--r--   0        0        0     6102 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/analysis/utils.py
--rw-r--r--   0        0        0       80 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/candlesticks/__init__.py
--rw-r--r--   0        0        0      719 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/candlesticks/heikinashi.py
--rw-r--r--   0        0        0        0 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/__init__.py
--rw-r--r--   0        0        0     5636 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/candle.py
--rw-r--r--   0        0        0     7806 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/candle_manager.py
--rw-r--r--   0        0        0      958 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/candlestick_type.py
--rw-r--r--   0        0        0     9691 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/hexital.py
--rw-r--r--   0        0        0    12456 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/core/indicator.py
--rw-r--r--   0        0        0      632 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/exceptions.py
--rw-r--r--   0        0        0     1084 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/__init__.py
--rw-r--r--   0        0        0     3476 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/adx.py
--rw-r--r--   0        0        0     2188 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/amorph.py
--rw-r--r--   0        0        0     1447 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/aroon.py
--rw-r--r--   0        0        0     1049 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/atr.py
--rw-r--r--   0        0        0     1307 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/bbands.py
--rw-r--r--   0        0        0     1102 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/counter.py
--rw-r--r--   0        0        0     1147 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/donchian.py
--rw-r--r--   0        0        0     1295 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/ema.py
--rw-r--r--   0        0        0      426 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/hla.py
--rw-r--r--   0        0        0     1500 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/hma.py
--rw-r--r--   0        0        0     1602 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/kc.py
--rw-r--r--   0        0        0     2818 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/macd.py
--rw-r--r--   0        0        0      818 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/obv.py
--rw-r--r--   0        0        0     1413 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/rma.py
--rw-r--r--   0        0        0      676 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/roc.py
--rw-r--r--   0        0        0     2550 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/rsi.py
--rw-r--r--   0        0        0     1168 2024-04-21 16:16:53.425528 hexital-1.1.0/hexital/indicators/sma.py
--rw-r--r--   0        0        0     1672 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/stdev.py
--rw-r--r--   0        0        0     2900 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/stoch.py
--rw-r--r--   0        0        0     2366 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/supertrend.py
--rw-r--r--   0        0        0      824 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/tr.py
--rw-r--r--   0        0        0     2782 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/tsi.py
--rw-r--r--   0        0        0     1363 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/vwap.py
--rw-r--r--   0        0        0      906 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/vwma.py
--rw-r--r--   0        0        0      962 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/indicators/wma.py
--rw-r--r--   0        0        0       89 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/utils/__init__.py
--rw-r--r--   0        0        0     2960 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/utils/candles.py
--rw-r--r--   0        0        0      585 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/utils/candlesticks.py
--rw-r--r--   0        0        0     1088 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/utils/indexing.py
--rw-r--r--   0        0        0     2792 2024-04-21 16:16:53.429529 hexital-1.1.0/hexital/utils/timeframe.py
--rw-r--r--   0        0        0     1534 2024-04-21 16:16:53.429529 hexital-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    13985 1970-01-01 00:00:00.000000 hexital-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5954 2024-05-01 16:43:32.128182 hexital-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1067 2024-05-01 16:43:32.128182 hexital-1.1.1/LICENSE
+-rw-r--r--   0        0        0    12974 2024-05-01 16:43:32.128182 hexital-1.1.1/README.md
+-rw-r--r--   0        0        0      249 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/__init__.py
+-rw-r--r--   0        0        0      835 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/analysis/__init__.py
+-rw-r--r--   0        0        0    12357 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/analysis/movement.py
+-rw-r--r--   0        0        0     3921 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/analysis/patterns.py
+-rw-r--r--   0        0        0     6102 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/analysis/utils.py
+-rw-r--r--   0        0        0       80 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/candlesticks/__init__.py
+-rw-r--r--   0        0        0      719 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/candlesticks/heikinashi.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/__init__.py
+-rw-r--r--   0        0        0     5636 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/candle.py
+-rw-r--r--   0        0        0     7806 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/candle_manager.py
+-rw-r--r--   0        0        0      958 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/candlestick_type.py
+-rw-r--r--   0        0        0     9721 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/hexital.py
+-rw-r--r--   0        0        0    12456 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/core/indicator.py
+-rw-r--r--   0        0        0      632 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/exceptions.py
+-rw-r--r--   0        0        0     1272 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/__init__.py
+-rw-r--r--   0        0        0     3476 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/adx.py
+-rw-r--r--   0        0        0     2188 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/amorph.py
+-rw-r--r--   0        0        0     1182 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/aroon.py
+-rw-r--r--   0        0        0     1049 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/atr.py
+-rw-r--r--   0        0        0     1391 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/bbands.py
+-rw-r--r--   0        0        0     1102 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/counter.py
+-rw-r--r--   0        0        0     1169 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/donchian.py
+-rw-r--r--   0        0        0     1295 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/ema.py
+-rw-r--r--   0        0        0      714 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/highest_lowest.py
+-rw-r--r--   0        0        0      426 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/hla.py
+-rw-r--r--   0        0        0     1708 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/hma.py
+-rw-r--r--   0        0        0     1602 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/kc.py
+-rw-r--r--   0        0        0     2818 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/macd.py
+-rw-r--r--   0        0        0      818 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/obv.py
+-rw-r--r--   0        0        0     1370 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/rma.py
+-rw-r--r--   0        0        0      685 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/roc.py
+-rw-r--r--   0        0        0     2550 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/rsi.py
+-rw-r--r--   0        0        0     1168 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/sma.py
+-rw-r--r--   0        0        0     1760 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/stdev.py
+-rw-r--r--   0        0        0     1188 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/stdevthres.py
+-rw-r--r--   0        0        0     2852 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/stoch.py
+-rw-r--r--   0        0        0     2366 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/supertrend.py
+-rw-r--r--   0        0        0      824 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/tr.py
+-rw-r--r--   0        0        0     2782 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/tsi.py
+-rw-r--r--   0        0        0     1363 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/vwap.py
+-rw-r--r--   0        0        0      906 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/vwma.py
+-rw-r--r--   0        0        0      962 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/indicators/wma.py
+-rw-r--r--   0        0        0       89 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/utils/__init__.py
+-rw-r--r--   0        0        0     2960 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/utils/candles.py
+-rw-r--r--   0        0        0      585 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/utils/candlesticks.py
+-rw-r--r--   0        0        0     1088 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/utils/indexing.py
+-rw-r--r--   0        0        0     2792 2024-05-01 16:43:32.128182 hexital-1.1.1/hexital/utils/timeframe.py
+-rw-r--r--   0        0        0     1534 2024-05-01 16:43:32.128182 hexital-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    13985 1970-01-01 00:00:00.000000 hexital-1.1.1/PKG-INFO
```

### Comparing `hexital-1.1.0/CHANGELOG.md` & `hexital-1.1.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.1.1 - 2024-05-01
+- Changed Movement rising/falling default length from 4 to 1
+- Added better exceptions to Hexital verifying dict indicators
+- Mass Indicator clean up to fix, unused/unended input_value's and unused sub indicators
+- Fixed minor donchian error
+- Fixed Highest and Lowest movement methods from returning bool False instead of None
+- Added Indicators
+  - Added HighestLowest (HL)
+  - Added Standard Deviation Threshold (STDEVTHRES)
+
 ## 1.1.0 - 2024-04-21
 
 - Removed Movement/Patterns from Hexital/Indicator
 - Removed get_indicator from Hexital as indicator already exists
 - Renamed candles_all to get_candles
 - Updated prev_exists to accept optional Indicator to be more useful
 - Altered Indicator name reading, to avoid issue's such as "TR" in "ATR"
```

### Comparing `hexital-1.1.0/LICENSE` & `hexital-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/README.md` & `hexital-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/analysis/__init__.py` & `hexital-1.1.1/hexital/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/analysis/movement.py` & `hexital-1.1.1/hexital/analysis/movement.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         return None
 
     readings = _get_clean_readings(candles, indicator, length, index_, True)
 
     return abs(min(readings) - max(readings))
 
 
-def rising(candles: List[Candle], indicator: str, length: int = 4, index: int = -1) -> bool:
+def rising(candles: List[Candle], indicator: str, length: int = 1, index: int = -1) -> bool:
     """True if current `indicator` is greater than all previous `indicator`
     for `length` bars back, False otherwise.
     Length `excludes` latest"""
     index_ = absindex(index, len(candles))
     if index_ is None:
         return False
 
@@ -108,15 +108,15 @@
         return False
 
     readings = _get_clean_readings(candles, indicator, length, index_)
 
     return all(reading < latest_reading for reading in readings)
 
 
-def falling(candles: List[Candle], indicator: str, length: int = 4, index: int = -1) -> bool:
+def falling(candles: List[Candle], indicator: str, length: int = 1, index: int = -1) -> bool:
     """True if current `indicator` reading is less than all previous `indicator`
     reading for `length` bars back, False otherwise.
     Length `excludes` latest"""
     index_ = absindex(index, len(candles))
     if index_ is None:
         return False
 
@@ -185,48 +185,51 @@
 
     mean = sum(reading for reading in readings) / length
     return round(mean, 2) > latest_reading
 
 
 def highest(
     candles: List[Candle], indicator: str, length: int = 4, index: int = -1
-) -> float | bool:
+) -> float | None:
     """Highest reading for a given number of bars back.
     Returns:
         Highest reading in the series.
     """
     index_ = absindex(index, len(candles))
     if index_ is None:
         return False
 
     if not reading_period(candles, length, indicator, index_):
         length = reading_count(candles, indicator) - 1
 
     readings = _get_clean_readings(candles, indicator, length, index_, True)
 
-    return max([reading for reading in readings], default=False)
+    max_reading = max([reading for reading in readings], default=False)
+    return max_reading if max_reading else None
 
 
 def lowest(
     candles: List[Candle], indicator: str, length: int = 4, index: int = -1
-) -> float | bool:
+) -> float | None:
     """Lowest reading for a given number of bars back.
     Returns:
         Lowest reading in the series.
     """
     index_ = absindex(index, len(candles))
     if index_ is None:
         return False
 
     if not reading_period(candles, length, indicator):
         length = reading_count(candles, indicator) - 1
 
     readings = _get_clean_readings(candles, indicator, length, index_, True)
 
-    return min([reading for reading in readings], default=False)
+    min_reading = min([reading for reading in readings], default=False)
+
+    return min_reading if min_reading else None
 
 
 def highestbar(
     candles: List[Candle], indicator: str, length: int = 4, index: int = -1
 ) -> int | None:
     """Highest reading offset for a given number of bars back.
     Returns:
```

### Comparing `hexital-1.1.0/hexital/analysis/patterns.py` & `hexital-1.1.1/hexital/analysis/patterns.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/analysis/utils.py` & `hexital-1.1.1/hexital/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/candlesticks/heikinashi.py` & `hexital-1.1.1/hexital/candlesticks/heikinashi.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/core/candle.py` & `hexital-1.1.1/hexital/core/candle.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/core/candle_manager.py` & `hexital-1.1.1/hexital/core/candle_manager.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/core/candlestick_type.py` & `hexital-1.1.1/hexital/core/candlestick_type.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/core/hexital.py` & `hexital-1.1.1/hexital/core/hexital.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,36 +99,37 @@
                 indicator.candle_manager = self._candles[manager.name]
 
         return valid_indicators
 
     def _build_indicator(self, raw_indicator: dict) -> Indicator:
         analysis_map = PATTERN_MAP | MOVEMENT_MAP
         amorph_class = INDICATOR_MAP["Amorph"]
+        indicator = deepcopy(raw_indicator)
 
-        if raw_indicator.get("indicator"):
-            indicator_name = raw_indicator.pop("indicator")
+        if indicator.get("indicator"):
+            indicator_name = indicator.pop("indicator")
 
             if INDICATOR_MAP.get(indicator_name):
                 indicator_class = INDICATOR_MAP[indicator_name]
-                return indicator_class(**raw_indicator)
+                return indicator_class(**indicator)
             else:
-                raise InvalidIndicator(f"Indicator {indicator_name} does not exist")
+                raise InvalidIndicator(f"Indicator {indicator_name} does not exist. [{indicator}]")
 
-        elif raw_indicator.get("analysis") and isinstance(raw_indicator.get("analysis"), str):
-            analysis_name = raw_indicator.pop("analysis")
+        elif indicator.get("analysis") and isinstance(indicator.get("analysis"), str):
+            analysis_name = indicator.pop("analysis")
             if not analysis_map.get(analysis_name):
                 raise InvalidAnalysis(
-                    f"analysis {analysis_name} does not exist in patterns or movements"
+                    f"analysis {analysis_name} does not exist in patterns or movements. [{indicator}]"
                 )
 
-            return amorph_class(analysis=analysis_map[analysis_name], **raw_indicator)
+            return amorph_class(analysis=analysis_map[analysis_name], **indicator)
 
-        elif raw_indicator.get("analysis") and callable(raw_indicator.get("analysis")):
-            method_name = raw_indicator.pop("analysis")
-            return amorph_class(analysis=method_name, **raw_indicator)
+        elif indicator.get("analysis") and callable(indicator.get("analysis")):
+            method_name = indicator.pop("analysis")
+            return amorph_class(analysis=method_name, **indicator)
         else:
             raise InvalidAnalysis(
                 f"Dict Indicator missing 'indicator' or 'analysis' name, not: {raw_indicator}"
             )
 
     def candles(self, timeframe: Optional[str] = None) -> List[Candle]:
         if timeframe and self._candles.get(timeframe, False):
```

### Comparing `hexital-1.1.0/hexital/core/indicator.py` & `hexital-1.1.1/hexital/core/indicator.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/exceptions.py` & `hexital-1.1.1/hexital/exceptions.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/__init__.py` & `hexital-1.1.1/hexital/indicators/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 from .amorph import Amorph
 from .aroon import AROON
 from .atr import ATR
 from .bbands import BBANDS
 from .counter import Counter
 from .donchian import Donchian
 from .ema import EMA
+from .highest_lowest import HighestLowest
 from .hla import HighLowAverage
 from .hma import HMA
 from .kc import KC
 from .macd import MACD
 from .obv import OBV
 from .rma import RMA
 from .roc import ROC
 from .rsi import RSI
 from .sma import SMA
-from .stdev import STDEV
+from .stdev import StandardDeviation
+from .stdevthres import StandardDeviationThreshold
 from .stoch import STOCH
 from .supertrend import Supertrend
 from .tr import TR
 from .tsi import TSI
 from .vwap import VWAP
 from .vwma import VWMA
 from .wma import WMA
@@ -29,24 +31,26 @@
     "Counter": Counter,
     "aroon": AROON,
     "ADX": ADX,
     "ATR": ATR,
     "BBANDS": BBANDS,
     "donchian": Donchian,
     "EMA": EMA,
+    "HL": HighestLowest,
     "HLA": HighLowAverage,
     "HMA": HMA,
     "KC": KC,
     "MACD": MACD,
     "OBV": OBV,
     "RMA": RMA,
     "ROC": ROC,
     "RSI": RSI,
     "SMA": SMA,
-    "STDEV": STDEV,
+    "STDEV": StandardDeviation,
+    "STDEVTHRES": StandardDeviationThreshold,
     "STOCH": STOCH,
     "Supertrend": Supertrend,
     "TR": TR,
     "TSI": TSI,
     "VWAP": VWAP,
     "VWMA": VWMA,
     "WMA": WMA,
```

### Comparing `hexital-1.1.0/hexital/indicators/adx.py` & `hexital-1.1.1/hexital/indicators/adx.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/amorph.py` & `hexital-1.1.1/hexital/indicators/amorph.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/aroon.py` & `hexital-1.1.1/hexital/indicators/aroon.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 from dataclasses import dataclass, field
 
 from hexital.analysis import movement
 from hexital.core.indicator import Indicator
-from hexital.indicators.sma import SMA
-from hexital.indicators.stdev import STDEV
 
 
 @dataclass(kw_only=True)
 class AROON(Indicator):
     """Aroon (aroon)
     Source: https://www.fidelity.com/learning-center/trading-investing/technical-analysis/technical-indicator-guide/aroon-indicator
     """
 
     _name: str = field(init=False, default="AROON")
     period: int = 14
-    input_value: str = "close"
 
     def _generate_name(self) -> str:
         return f"{self._name}_{self.period}"
 
-    def _initialise(self):
-        self.add_sub_indicator(STDEV(period=self.period))
-        self.add_sub_indicator(SMA(period=self.period))
-
     def _calculate_reading(self, index: int) -> float | dict | None:
         aroon = {
             "AROONU": None,
             "AROOND": None,
             "AROONOSC": None,
         }
-        if self.reading_period(self.period + 1, self.input_value):
+        if self.reading_period(self.period + 1, "high"):
             aroon["AROONU"] = (
                 (self.period - movement.highestbar(self.candles, "high", self.period + 1, index))
                 / self.period
             ) * 100
             aroon["AROOND"] = (
                 (self.period - movement.lowestbar(self.candles, "low", self.period + 1, index))
                 / self.period
```

### Comparing `hexital-1.1.0/hexital/indicators/atr.py` & `hexital-1.1.1/hexital/indicators/atr.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/counter.py` & `hexital-1.1.1/hexital/indicators/counter.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/donchian.py` & `hexital-1.1.1/hexital/indicators/donchian.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,21 +17,22 @@
         period (int) Default: 20
 
 
     """
 
     _name: str = field(init=False, default="DONCHIAN")
     period: int = 20
-    input_value: str = "close"
 
     def _generate_name(self) -> str:
         return f"{self._name}_{self.period}"
 
     def _calculate_reading(self, index: int) -> float | dict | None:
         donchian = {"DCL": None, "DCM": None, "DCU": None}
 
-        if self.prev_exists() or self.reading_period(self.period, "high", index):
+        if self.prev_reading(f"{self.name}.DCU") is not None or self.reading_period(
+            self.period, "high", index
+        ):
             donchian["DCU"] = movement.highest(self.candles, "high", self.period - 1, index)
             donchian["DCL"] = movement.lowest(self.candles, "low", self.period - 1, index)
             donchian["DCM"] = (donchian["DCU"] + donchian["DCL"]) / 2
 
         return donchian
```

### Comparing `hexital-1.1.0/hexital/indicators/ema.py` & `hexital-1.1.1/hexital/indicators/ema.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/hma.py` & `hexital-1.1.1/hexital/indicators/hma.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,17 +18,27 @@
     period: int = 10
     input_value: str = "close"
 
     def _generate_name(self) -> str:
         return f"{self._name}_{self.period}"
 
     def _initialise(self):
-        self.add_sub_indicator(WMA(period=self.period, fullname_override=f"{self.name}_WMA"))
         self.add_sub_indicator(
-            WMA(period=int(self.period / 2), fullname_override=f"{self.name}_WMAh")
+            WMA(
+                input_value=self.input_value,
+                period=self.period,
+                fullname_override=f"{self.name}_WMA",
+            )
+        )
+        self.add_sub_indicator(
+            WMA(
+                input_value=self.input_value,
+                period=int(self.period / 2),
+                fullname_override=f"{self.name}_WMAh",
+            )
         )
 
         self.add_managed_indicator("raw_HMA", Managed(fullname_override=f"{self.name}_HMAr"))
         self.managed_indicators["raw_HMA"].add_sub_indicator(
             WMA(
                 input_value=f"{self.name}_HMAr",
                 period=int(math.sqrt(self.period)),
```

### Comparing `hexital-1.1.0/hexital/indicators/kc.py` & `hexital-1.1.1/hexital/indicators/kc.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/macd.py` & `hexital-1.1.1/hexital/indicators/macd.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/obv.py` & `hexital-1.1.1/hexital/indicators/obv.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/rma.py` & `hexital-1.1.1/hexital/indicators/rma.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,14 @@
     _name: str = field(init=False, default="RMA")
     period: int = 10
     input_value: str = "close"
 
     def _generate_name(self) -> str:
         return f"{self._name}_{self.period}"
 
-    def _initialise(self):
-        return
-
     def _calculate_reading(self, index: int) -> float | dict | None:
         alpha = float(1.0 / self.period)
 
         if self.prev_exists():
             return float(
                 (alpha * self.reading(self.input_value)) + ((1.0 - alpha) * self.prev_reading())
             )
```

### Comparing `hexital-1.1.0/hexital/indicators/roc.py` & `hexital-1.1.1/hexital/indicators/roc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,12 +11,12 @@
     period: int = 10
     input_value: str = "close"
 
     def _generate_name(self) -> str:
         return f"{self._name}"
 
     def _calculate_reading(self, index: int) -> float | dict | None:
-        if self.prev_exists() or self.reading_period(self.period + 1, "close"):
+        if self.prev_exists() or self.reading_period(self.period + 1, self.input_value):
             period_n_back = self.reading(self.input_value, index - self.period)
 
             return ((self.reading(self.input_value) - period_n_back) / period_n_back) * 100
         return None
```

### Comparing `hexital-1.1.0/hexital/indicators/rsi.py` & `hexital-1.1.1/hexital/indicators/rsi.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/sma.py` & `hexital-1.1.1/hexital/indicators/sma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/stdev.py` & `hexital-1.1.1/hexital/indicators/stdev.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass, field
 from math import sqrt
 
 from hexital.core.indicator import Indicator, Managed
 
 
 @dataclass(kw_only=True)
-class STDEV(Indicator):
+class StandardDeviation(Indicator):
     """Rolling Standard Deviation
 
     https://jonisalonen.com/2014/efficient-and-accurate-rolling-standard-deviation/
     """
 
     _name: str = field(init=False, default="STDEV")
     period: int = 30
@@ -23,14 +23,17 @@
 
     def _calculate_reading(self, index: int) -> float | dict | None:
         old_mean = 0
         variance = 0
         removed_val = 0
         in_calc_range = False
 
+        if self.reading(self.input_value) is None:
+            return None
+
         if self.reading_period(self.period + 1, self.input_value, index):
             removed_val = self.reading(self.input_value, index - self.period)
             in_calc_range = True
 
         if self.prev_exists(f"{self.name}_data.mean"):
             old_mean = self.prev_reading(f"{self.name}_data.mean")
```

### Comparing `hexital-1.1.0/hexital/indicators/stoch.py` & `hexital-1.1.1/hexital/indicators/stoch.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,14 @@
     slow_period: int = 3
     smoothing_k: int = 3
     input_value: str = "close"
 
     def _generate_name(self) -> str:
         return f"{self._name}_{self.period}"
 
-    def _validate_fields(self):
-        return
-
     def _initialise(self):
         self.add_managed_indicator("STOCH_data", Managed(fullname_override=f"{self.name}_data"))
         self.managed_indicators["STOCH_data"].add_sub_indicator(
             SMA(
                 input_value=f"{self.name}_data.stoch",
                 period=self.smoothing_k,
                 fullname_override=f"{self.name}_k",
```

### Comparing `hexital-1.1.0/hexital/indicators/supertrend.py` & `hexital-1.1.1/hexital/indicators/supertrend.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/tr.py` & `hexital-1.1.1/hexital/indicators/tr.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/tsi.py` & `hexital-1.1.1/hexital/indicators/tsi.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/vwap.py` & `hexital-1.1.1/hexital/indicators/vwap.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/vwma.py` & `hexital-1.1.1/hexital/indicators/vwma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/indicators/wma.py` & `hexital-1.1.1/hexital/indicators/wma.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/utils/candles.py` & `hexital-1.1.1/hexital/utils/candles.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/utils/candlesticks.py` & `hexital-1.1.1/hexital/utils/candlesticks.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/utils/indexing.py` & `hexital-1.1.1/hexital/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/hexital/utils/timeframe.py` & `hexital-1.1.1/hexital/utils/timeframe.py`

 * *Files identical despite different names*

### Comparing `hexital-1.1.0/pyproject.toml` & `hexital-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hexital"
-version = "1.1.0"
+version = "1.1.1"
 description = "Hex Incremental Technical Analysis Library"
 readme = "README.md"
 license = "MIT"
 authors = ["Merlin Roe <merlin.roe@hotmail.co.uk>"]
 homepage = "https://github.com/MerlinR/Hexital"
 repository = "https://github.com/MerlinR/Hexital"
 documentation = "https://github.com/MerlinR/Hexital"
```

### Comparing `hexital-1.1.0/PKG-INFO` & `hexital-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexital
-Version: 1.1.0
+Version: 1.1.1
 Summary: Hex Incremental Technical Analysis Library
 Home-page: https://github.com/MerlinR/Hexital
 License: MIT
 Keywords: trading,quant,indicators
 Author: Merlin Roe
 Author-email: merlin.roe@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
```

