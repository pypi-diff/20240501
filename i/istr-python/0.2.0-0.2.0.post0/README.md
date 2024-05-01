# Comparing `tmp/istr_python-0.2.0.tar.gz` & `tmp/istr_python-0.2.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.2.0.tar", last modified: Tue Apr 30 11:49:06 2024, max compression
+gzip compressed data, was "istr_python-0.2.0.post0.tar", last modified: Wed May  1 15:46:05 2024, max compression
```

## Comparing `istr_python-0.2.0.tar` & `istr_python-0.2.0.post0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 11:49:06.470996 istr_python-0.2.0/
--rw-rw-rw-   0        0        0    11703 2024-04-30 11:49:06.468918 istr_python-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    10764 2024-04-30 07:19:54.000000 istr_python-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 11:49:06.437441 istr_python-0.2.0/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.2.0/istr/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.2.0/istr/install istr.py
--rw-rw-rw-   0        0        0    20662 2024-04-30 11:44:48.000000 istr_python-0.2.0/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-04-30 11:49:06.465304 istr_python-0.2.0/istr_python.egg-info/
--rw-rw-rw-   0        0        0    11703 2024-04-30 11:49:06.000000 istr_python-0.2.0/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-30 11:49:06.000000 istr_python-0.2.0/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 11:49:06.000000 istr_python-0.2.0/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-30 11:49:06.000000 istr_python-0.2.0/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      658 2024-04-30 11:48:59.000000 istr_python-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 11:49:06.471994 istr_python-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 11:49:06.463308 istr_python-0.2.0/tests/
--rw-rw-rw-   0        0        0    13111 2024-04-30 11:45:24.000000 istr_python-0.2.0/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-05-01 15:46:05.685639 istr_python-0.2.0.post0/
+-rw-rw-rw-   0        0        0    13136 2024-05-01 15:46:05.683754 istr_python-0.2.0.post0/PKG-INFO
+-rw-rw-rw-   0        0        0    12151 2024-05-01 07:19:51.000000 istr_python-0.2.0.post0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 15:46:05.648793 istr_python-0.2.0.post0/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.2.0.post0/istr/__init__.py
+-rw-rw-rw-   0        0        0    20752 2024-05-01 06:41:58.000000 istr_python-0.2.0.post0/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-05-01 15:46:05.681995 istr_python-0.2.0.post0/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    13136 2024-05-01 15:46:05.000000 istr_python-0.2.0.post0/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-01 15:46:05.000000 istr_python-0.2.0.post0/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 15:46:05.000000 istr_python-0.2.0.post0/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-01 15:46:05.000000 istr_python-0.2.0.post0/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      660 2024-05-01 15:45:57.000000 istr_python-0.2.0.post0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 15:46:05.685639 istr_python-0.2.0.post0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 15:46:05.668731 istr_python-0.2.0.post0/tests/
+-rw-rw-rw-   0        0        0    13111 2024-04-30 11:45:24.000000 istr_python-0.2.0.post0/tests/test_istr.py
```

### Comparing `istr_python-0.2.0/PKG-INFO` & `istr_python-0.2.0.post0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.2.0
+Version: 0.2.0.post0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -15,33 +15,34 @@
 
 ## Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
 
-This can be very handy for solving puzzles, but also for other purposes. For instance the
+This can be very handy for solving puzzles, but also for other purposes.</br>
+For instance the
 famous send more money puzzle
 ```
   S E N D
   M O R E
 --------- +
 M O N E Y
 ```
 can be nicely, albeit not very efficient, coded as:
 ```
 import itertools
 from istr import istr
 
 for s, e, n, d, m, o, r, y in istr(itertools.permutations(range(10), 8)):
     if m and ((s|e|n|d) + (m|o|r|e) == (m|o|n|e|y)):
-        print(f" {s|e|n|d}")
-        print(f" {m|o|r|e}")
-        print("-----")
-        print(f"{m|o|n|e|y}")
+        print(f' {s|e|n|d}')
+        print(f' {m|o|r|e}')
+        print('-----')
+        print(f'{m|o|n|e|y}')
 ```
 
 And it is a nice demonstration of extending a class (str) with extra and changed functionality.
 
 ## Installation
 Installing istr with pip is easy.
 ```
@@ -60,34 +61,34 @@
 
 ```
 from istr import istr
 ```
 
 Now we can define some istrs:
 ```
-four = istr("4")
-five = istr("5")
+four = istr('4')
+five = istr('5')
 ```
 Then we can do
 ```
 x= four * five
 ```
-, after which x is `istr("20")`
+, after which x is `istr('20')`
 
 And now we can do
 ```
 print(x == 20)
-print(x == "20")
+print(x == '20')
 ```
 resulting in two times `True`. That's because istrs instances are treated as int, although they are strings.
 
 That means that we can also say
 ```
 print(x < 30)
-print(x >= "10")
+print(x >= '10')
 ```
 again resulting in two times `True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
@@ -111,108 +112,108 @@
 
 And the result is again an istr.
 
 That means that
 ```
 (four | five) / 3
 ```
-is `istr("9")`.
+is `istr('9')`.
 
 In order to repeat a string in the usual sense, you cannot use `3 * four`, as that woud be `12`. 
 
 We use the matrix multiplication operator (@) for this. So `3 @ four` is `444`. As is `four @ 3`.
 
 Also allowed are
 ```
 abs(four)
 -four 
 ```
 
 The bool operator works on the integer value of an istr. So
-`bool("0")` ==> `False`
-`bool("1")` ==> `True`
+`bool(istr('0'))` ==> `False`
+`bool(istr('1'))` ==> `True`
 The code
 ```
-if istr("0"):
-    print("True")
+if istr('0'):
+    print('True')
 else:
-    print("False")
+    print('False')
 ```
 will print `False`
 
 For the in operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
 ```
-"34" in istr(1234)
+'34' in istr(1234)
 34 in istr(1234)
 ```
 On the left hand side an istr is always treated as a string:
 ```
-istr(1234) in "01234566890ABCDEF"
+istr(1234) in '01234566890ABCDEF'
 ```
 
 Note that all calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
 Also divisions are always floor divisions!
 
-There's a special case for `istr("")`. This is a proper empty string, but also represents the value of 0.
-That is to allow for `istr("").join(i for i in "01234)"`, resulting in `istr("01234")`.
+There's a special case for `istr('')`. This is a proper empty string, but also represents the value of 0.
+That is to allow for `istr('').join(i for i in '01234)'`, resulting in `istr('01234')`.
 
 Sorting a list of istrs is based on the integer value, not the string. So
 
-`" ".join(sorted("1 3 2 4 5 6 11 7 9 8 10 12 0".split()))`
+`' '.join(sorted('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))`
 
 is
 
-`"0 1 10 11 2 3 4 5 6 7 8 9"`
+`'0 1 10 11 2 3 4 5 6 7 8 9'`
 
 ,whereas
 
-`" ".join(sorted(istr("1 3 2 4 5 6 11 7 9 8 10 12 0".split())))`
+`' '.join(sorted(istr('1 3 2 4 5 6 11 7 9 8 10 12 0'.split())))`
 
 is 
 
-`"0 1 2 3 4 5 6 7 8 9 10 11"`
+`'0 1 2 3 4 5 6 7 8 9 10 11'`
 
 ## Using other values for istr than numeric value or str
 Apart from with simple numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
 - if a dict (or subtype of dict), the same type dict will be returned with all values istr'ed
 
-    `istr({0: 0, 1: 1, 2: 4})` ==> `{0: istr("0"), 1: istr("1"), 2: istr("4")}`
+    `istr({0: 0, 1: 1, 2: 4})` ==> `{0: istr('0'), 1: istr('1'), 2: istr('4')}`
 
 - if an iterator, the iterator will be mapped with istr
 
     `istr(i * i for i in range(3))` ==> `<map object>`
 
-    `list(istr(i * i for i in range(3)))` ==> `[istr("0"), istr("1"), istr("4")]`
+    `list(istr(i * i for i in range(3)))` ==> `[istr('0'), istr('1'), istr('4')]`
 
 - if an iterable, the same type will be returned with all elements istr'ed
 
-    `istr([0, 1, 4])` ==> `[istr("0"), istr("1"), istr("4")]`
+    `istr([0, 1, 4])` ==> `[istr('0'), istr('1'), istr('4')]`
 
-    `istr((0, 1, 4))` ==> `(istr("0"), istr("1"), istr("4"))`
+    `istr((0, 1, 4))` ==> `(istr('0'), istr('1'), istr('4'))`
 
-    `istr({0, 1, 4})` ==> `{istr("4"), istr("0"), istr("1")} ## or similar`
+    `istr({0, 1, 4})` ==> `{istr('4'), istr('0'), istr('1')} ## or similar`
 
 - if a range, an istr.range instance will be returned
     
     `istr(range(3))` ==> `istr.range(3)`
 
-    `list(istr(range(3)))` ==> `[istr("0"), istr("1"), istr("2")]`
+    `list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]`
 
     `len(istr(range(3)))` ==> `3`
 
 - if an istr.range instance, the same istr.range will be returned
 
 ## More than one parameter for istr
 It is possible to give more than one parameter, in which case a tuple
 of the istrs of the parameters will be returned, which can be handy
 to unpack multiple values, e.g.
 
-`a, b, c = istr(5, 6, 7)` ==> `a=istr("5") , b=istr("6"), c=istr("7")`
+`a, b, c = istr(5, 6, 7)` ==> `a=istr('5') , b=istr('6'), c=istr('7')`
 
 ## test for even/odd
 It is possible to test for even/odd with the
 
 `is_even` and `is_odd` method, e.g.
 
 ```
@@ -221,35 +222,35 @@
 ```
 This will print `True` twice.
 
 ## reverse an istr
 The method `istr.reversed()` will return the an istr with the reversed content:
 ```
 print(repr(istr(456).reversed()))
-print(repr(istr("0456").reversed()))
+print(repr(istr('0456').reversed()))
 ```
 result:
 ```
-istr("654")
-istr("6540")
+istr('654')
+istr('6540')
 ```
 The same can -of course- be achieved with
 ```
 print(repr(istr(456)[::-1]))
-print(repr(istr("0456")[::-1]))
+print(repr(istr('0456')[::-1]))
 ```
 Note that is impossible to reverse a negative istr.
 
 ## enumerate with istrs
 
 The `istr.enumerate` method can be used just as the builtin enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
 ```
-    for i,c in istr.enumerate("abc"):
-        print(f"{repr(i)} {c}")
+    for i,c in istr.enumerate('abc'):
+        print(f'{repr(i)} {c}')
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
 ```
@@ -259,14 +260,44 @@
 The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
 `list(istr.concat(((1,2),(3,4)))` ==> `istr([12,34])`
 
 `list(istr.concat(itertools.permutations(range(3),2)))` ==> `[istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')]` 
 
+## generate istr with digits
+
+The class method `digits` can be used to return an istr of digits according to a given specification.
+The method takes either no or a number of arguments.
+
+If no arguments are given, the result will be istr('0123456789').
+
+The given argument(s) result in a range of digits.
+
+- `<n>` ==> n
+- `<n-m> ==> n, n+1, ..., m
+- `-n>` ==> 0, 1, ... n
+- `n->` ==> n, n+1, ..., 9
+- `''` ==> 0, 1, ..., 9
+
+(n and m must be digit between 0 and 9)
+
+The final result is an istr composed of the given range(s).
+
+Here are some examples:
+
+- `istr.digits()` ==> `istr('0123456789')`
+- `istr.digits('')` ==> `istr('0123456789')`
+- `istr.digits('1')` ==> `istr('1')`
+- `istr.digits('3-')` ==> `istr('3456789')`
+- `istr.digits('-3')` ==> `istr('0123')`
+- `istr('1-4', '6', '8-9')` ==> `istr('1234689')`
+- `istr('1', '1-2', '1-3')` ==> `istr('11213')`
+
+
 ## Subclassing istr
 When a class is derived from istr, all methods will return that newly derived class. 
 
 E.g.
 ```
 class jstr(istr):
     ...
@@ -279,36 +310,36 @@
 
 It is possible to control the way an `istr` instance will be repr'ed.
 
 By default, the `istr('5')` is represented as `istr('5')`.
 
 With the istr.repr_mode() context manager, that can be changed:
 ```
-with istr.repr_mode("str"):
+with istr.repr_mode('str'):
     five = istr('5')
     print(repr(five))
-with istr.repr_mode("int"):
+with istr.repr_mode('int'):
     five = istr('5')
     print(repr(five))
-with istr.repr_mode("istr"):
+with istr.repr_mode('istr'):
     five = istr('5')
     print(repr(five))
 ```
 This will print
 ```
 '5'
 5
 istr('5')
 ```
 Note that the way an `istr` is represented is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 
 ```
-istr.repr_mode("str")
+istr.repr_mode('str')
 five = istr('5')
 print(repr(five))
 ```
 This will print
 ```
 '5'
 ```
@@ -326,15 +357,15 @@
 
 Note that the integer is always stored in base 10 mode, but the string
 representation will reflect the chosen base (at time of initialization).
 
 Some examples:
 ```
 with istr.base(16):
-    a = istr("7fff")
+    a = istr('7fff')
     print(int(a))
 
     b = istr(15)
     print(repr(b))
 ```
 This will result in
 ```
@@ -344,15 +375,15 @@
 All calculations are done in the decimal 10 system.
 
 Note that the way an `istr` is interpreted is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 ```
 istr.base(16)
-print(int(istr("7fff")))
+print(int(istr('7fff')))
 ```
 This will print
 ```
 32767
 ```
 Finally, the current base can be queried with `istr.base()`, so upon start:
 ```
@@ -374,70 +405,79 @@
 
 `repr(4))` ==> `istr('4')`
 
 With the `istr.format()` context manager this behavior can be changed.
 If the format specifier is a number, most likely a single digit, that
 will be the minimum number of characters in the string:
 ```
-with istr.format("3"):
+with istr.format('3'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('  1')
 istr(' 12')
 istr('123')
 istr('1234')
 ```
 If the string starts with a `0`, the string will be zero filled:
 ```
-with istr.format("03"):
+with istr.format('03'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('001')
 istr('012')
 istr('123')
 istr('1234')
 ```
 Note that if a format other than the default `''` is used, the string will reformatted even if the `istr` is specified with a string:
 ```
-with istr.format("03"):
-    print(repr(istr("  12 ")))
+with istr.format('03'):
+    print(repr(istr('  12 ')))
 ```
 will result in `istr('0012')`
 
 Remark: For bases other than 10, the string will never be reformatted!
 
 ## Operations
 ----------------------------
+```
+The table below shows whether the string or the int version of istr is applied.
+
 operator/function   int  str  Example
 ----------------------------
 +                    x        istr(20) + 3 ==> istr('23')
 _                    x        istr(20) - 3 ==> istr('17')
 *                    x        istr(20) * 3 ==> istr('60')
 /                    x        istr(20) / 3 ==> istr('6')
 //                   x        istr(20) // 3 ==> istr('6')
 %                    x        istr(20) % 3 ==> istr('2')
+divmod               x        divmod(istr(20), 3) ==> (istr('6'), istr('2'))
 **                   x        istr(2) ** 3 ==> istr('8')
 @                         x   istr(20) @ 3 ==> istr('202020')
 ==                   x    x   istr(20) == 20 ==> True | istr(20) == '20' ==> True
 |                         x   istr(20) | 5 ==> istr('205')
-abs                  x
+abs                  x        abs(istr(-20)) ==> istr('20')
+bool                 x        bool(istr(' 0 ')) ==> False
 <=, <, >, >=         x        istr('100') > istr('2') ==> True
 slicing              x        istr(12345)[1:3] ==> istr('23')
+iterate                   x   [x for x in istr(20)] ==> [istr('2'), istr('0')
+len                       x   len(istr(' 20 ')) ==> 4
+count                     x   istr(100),count('0') ==> 2
+index                     x   istr(' 100 ').index('0') ==> 2
 ----------------------------
-
+```
 ## Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used.
 
 ## Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
```

### Comparing `istr_python-0.2.0/README.md` & `istr_python-0.2.0.post0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 
 ## Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
 
-This can be very handy for solving puzzles, but also for other purposes. For instance the
+This can be very handy for solving puzzles, but also for other purposes.</br>
+For instance the
 famous send more money puzzle
 ```
   S E N D
   M O R E
 --------- +
 M O N E Y
 ```
 can be nicely, albeit not very efficient, coded as:
 ```
 import itertools
 from istr import istr
 
 for s, e, n, d, m, o, r, y in istr(itertools.permutations(range(10), 8)):
     if m and ((s|e|n|d) + (m|o|r|e) == (m|o|n|e|y)):
-        print(f" {s|e|n|d}")
-        print(f" {m|o|r|e}")
-        print("-----")
-        print(f"{m|o|n|e|y}")
+        print(f' {s|e|n|d}')
+        print(f' {m|o|r|e}')
+        print('-----')
+        print(f'{m|o|n|e|y}')
 ```
 
 And it is a nice demonstration of extending a class (str) with extra and changed functionality.
 
 ## Installation
 Installing istr with pip is easy.
 ```
@@ -47,34 +48,34 @@
 
 ```
 from istr import istr
 ```
 
 Now we can define some istrs:
 ```
-four = istr("4")
-five = istr("5")
+four = istr('4')
+five = istr('5')
 ```
 Then we can do
 ```
 x= four * five
 ```
-, after which x is `istr("20")`
+, after which x is `istr('20')`
 
 And now we can do
 ```
 print(x == 20)
-print(x == "20")
+print(x == '20')
 ```
 resulting in two times `True`. That's because istrs instances are treated as int, although they are strings.
 
 That means that we can also say
 ```
 print(x < 30)
-print(x >= "10")
+print(x >= '10')
 ```
 again resulting in two times `True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
@@ -98,108 +99,108 @@
 
 And the result is again an istr.
 
 That means that
 ```
 (four | five) / 3
 ```
-is `istr("9")`.
+is `istr('9')`.
 
 In order to repeat a string in the usual sense, you cannot use `3 * four`, as that woud be `12`. 
 
 We use the matrix multiplication operator (@) for this. So `3 @ four` is `444`. As is `four @ 3`.
 
 Also allowed are
 ```
 abs(four)
 -four 
 ```
 
 The bool operator works on the integer value of an istr. So
-`bool("0")` ==> `False`
-`bool("1")` ==> `True`
+`bool(istr('0'))` ==> `False`
+`bool(istr('1'))` ==> `True`
 The code
 ```
-if istr("0"):
-    print("True")
+if istr('0'):
+    print('True')
 else:
-    print("False")
+    print('False')
 ```
 will print `False`
 
 For the in operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
 ```
-"34" in istr(1234)
+'34' in istr(1234)
 34 in istr(1234)
 ```
 On the left hand side an istr is always treated as a string:
 ```
-istr(1234) in "01234566890ABCDEF"
+istr(1234) in '01234566890ABCDEF'
 ```
 
 Note that all calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
 Also divisions are always floor divisions!
 
-There's a special case for `istr("")`. This is a proper empty string, but also represents the value of 0.
-That is to allow for `istr("").join(i for i in "01234)"`, resulting in `istr("01234")`.
+There's a special case for `istr('')`. This is a proper empty string, but also represents the value of 0.
+That is to allow for `istr('').join(i for i in '01234)'`, resulting in `istr('01234')`.
 
 Sorting a list of istrs is based on the integer value, not the string. So
 
-`" ".join(sorted("1 3 2 4 5 6 11 7 9 8 10 12 0".split()))`
+`' '.join(sorted('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))`
 
 is
 
-`"0 1 10 11 2 3 4 5 6 7 8 9"`
+`'0 1 10 11 2 3 4 5 6 7 8 9'`
 
 ,whereas
 
-`" ".join(sorted(istr("1 3 2 4 5 6 11 7 9 8 10 12 0".split())))`
+`' '.join(sorted(istr('1 3 2 4 5 6 11 7 9 8 10 12 0'.split())))`
 
 is 
 
-`"0 1 2 3 4 5 6 7 8 9 10 11"`
+`'0 1 2 3 4 5 6 7 8 9 10 11'`
 
 ## Using other values for istr than numeric value or str
 Apart from with simple numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
 - if a dict (or subtype of dict), the same type dict will be returned with all values istr'ed
 
-    `istr({0: 0, 1: 1, 2: 4})` ==> `{0: istr("0"), 1: istr("1"), 2: istr("4")}`
+    `istr({0: 0, 1: 1, 2: 4})` ==> `{0: istr('0'), 1: istr('1'), 2: istr('4')}`
 
 - if an iterator, the iterator will be mapped with istr
 
     `istr(i * i for i in range(3))` ==> `<map object>`
 
-    `list(istr(i * i for i in range(3)))` ==> `[istr("0"), istr("1"), istr("4")]`
+    `list(istr(i * i for i in range(3)))` ==> `[istr('0'), istr('1'), istr('4')]`
 
 - if an iterable, the same type will be returned with all elements istr'ed
 
-    `istr([0, 1, 4])` ==> `[istr("0"), istr("1"), istr("4")]`
+    `istr([0, 1, 4])` ==> `[istr('0'), istr('1'), istr('4')]`
 
-    `istr((0, 1, 4))` ==> `(istr("0"), istr("1"), istr("4"))`
+    `istr((0, 1, 4))` ==> `(istr('0'), istr('1'), istr('4'))`
 
-    `istr({0, 1, 4})` ==> `{istr("4"), istr("0"), istr("1")} ## or similar`
+    `istr({0, 1, 4})` ==> `{istr('4'), istr('0'), istr('1')} ## or similar`
 
 - if a range, an istr.range instance will be returned
     
     `istr(range(3))` ==> `istr.range(3)`
 
-    `list(istr(range(3)))` ==> `[istr("0"), istr("1"), istr("2")]`
+    `list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]`
 
     `len(istr(range(3)))` ==> `3`
 
 - if an istr.range instance, the same istr.range will be returned
 
 ## More than one parameter for istr
 It is possible to give more than one parameter, in which case a tuple
 of the istrs of the parameters will be returned, which can be handy
 to unpack multiple values, e.g.
 
-`a, b, c = istr(5, 6, 7)` ==> `a=istr("5") , b=istr("6"), c=istr("7")`
+`a, b, c = istr(5, 6, 7)` ==> `a=istr('5') , b=istr('6'), c=istr('7')`
 
 ## test for even/odd
 It is possible to test for even/odd with the
 
 `is_even` and `is_odd` method, e.g.
 
 ```
@@ -208,35 +209,35 @@
 ```
 This will print `True` twice.
 
 ## reverse an istr
 The method `istr.reversed()` will return the an istr with the reversed content:
 ```
 print(repr(istr(456).reversed()))
-print(repr(istr("0456").reversed()))
+print(repr(istr('0456').reversed()))
 ```
 result:
 ```
-istr("654")
-istr("6540")
+istr('654')
+istr('6540')
 ```
 The same can -of course- be achieved with
 ```
 print(repr(istr(456)[::-1]))
-print(repr(istr("0456")[::-1]))
+print(repr(istr('0456')[::-1]))
 ```
 Note that is impossible to reverse a negative istr.
 
 ## enumerate with istrs
 
 The `istr.enumerate` method can be used just as the builtin enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
 ```
-    for i,c in istr.enumerate("abc"):
-        print(f"{repr(i)} {c}")
+    for i,c in istr.enumerate('abc'):
+        print(f'{repr(i)} {c}')
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
 ```
@@ -246,14 +247,44 @@
 The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
 `list(istr.concat(((1,2),(3,4)))` ==> `istr([12,34])`
 
 `list(istr.concat(itertools.permutations(range(3),2)))` ==> `[istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')]` 
 
+## generate istr with digits
+
+The class method `digits` can be used to return an istr of digits according to a given specification.
+The method takes either no or a number of arguments.
+
+If no arguments are given, the result will be istr('0123456789').
+
+The given argument(s) result in a range of digits.
+
+- `<n>` ==> n
+- `<n-m> ==> n, n+1, ..., m
+- `-n>` ==> 0, 1, ... n
+- `n->` ==> n, n+1, ..., 9
+- `''` ==> 0, 1, ..., 9
+
+(n and m must be digit between 0 and 9)
+
+The final result is an istr composed of the given range(s).
+
+Here are some examples:
+
+- `istr.digits()` ==> `istr('0123456789')`
+- `istr.digits('')` ==> `istr('0123456789')`
+- `istr.digits('1')` ==> `istr('1')`
+- `istr.digits('3-')` ==> `istr('3456789')`
+- `istr.digits('-3')` ==> `istr('0123')`
+- `istr('1-4', '6', '8-9')` ==> `istr('1234689')`
+- `istr('1', '1-2', '1-3')` ==> `istr('11213')`
+
+
 ## Subclassing istr
 When a class is derived from istr, all methods will return that newly derived class. 
 
 E.g.
 ```
 class jstr(istr):
     ...
@@ -266,36 +297,36 @@
 
 It is possible to control the way an `istr` instance will be repr'ed.
 
 By default, the `istr('5')` is represented as `istr('5')`.
 
 With the istr.repr_mode() context manager, that can be changed:
 ```
-with istr.repr_mode("str"):
+with istr.repr_mode('str'):
     five = istr('5')
     print(repr(five))
-with istr.repr_mode("int"):
+with istr.repr_mode('int'):
     five = istr('5')
     print(repr(five))
-with istr.repr_mode("istr"):
+with istr.repr_mode('istr'):
     five = istr('5')
     print(repr(five))
 ```
 This will print
 ```
 '5'
 5
 istr('5')
 ```
 Note that the way an `istr` is represented is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 
 ```
-istr.repr_mode("str")
+istr.repr_mode('str')
 five = istr('5')
 print(repr(five))
 ```
 This will print
 ```
 '5'
 ```
@@ -313,15 +344,15 @@
 
 Note that the integer is always stored in base 10 mode, but the string
 representation will reflect the chosen base (at time of initialization).
 
 Some examples:
 ```
 with istr.base(16):
-    a = istr("7fff")
+    a = istr('7fff')
     print(int(a))
 
     b = istr(15)
     print(repr(b))
 ```
 This will result in
 ```
@@ -331,15 +362,15 @@
 All calculations are done in the decimal 10 system.
 
 Note that the way an `istr` is interpreted is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 ```
 istr.base(16)
-print(int(istr("7fff")))
+print(int(istr('7fff')))
 ```
 This will print
 ```
 32767
 ```
 Finally, the current base can be queried with `istr.base()`, so upon start:
 ```
@@ -361,70 +392,79 @@
 
 `repr(4))` ==> `istr('4')`
 
 With the `istr.format()` context manager this behavior can be changed.
 If the format specifier is a number, most likely a single digit, that
 will be the minimum number of characters in the string:
 ```
-with istr.format("3"):
+with istr.format('3'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('  1')
 istr(' 12')
 istr('123')
 istr('1234')
 ```
 If the string starts with a `0`, the string will be zero filled:
 ```
-with istr.format("03"):
+with istr.format('03'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('001')
 istr('012')
 istr('123')
 istr('1234')
 ```
 Note that if a format other than the default `''` is used, the string will reformatted even if the `istr` is specified with a string:
 ```
-with istr.format("03"):
-    print(repr(istr("  12 ")))
+with istr.format('03'):
+    print(repr(istr('  12 ')))
 ```
 will result in `istr('0012')`
 
 Remark: For bases other than 10, the string will never be reformatted!
 
 ## Operations
 ----------------------------
+```
+The table below shows whether the string or the int version of istr is applied.
+
 operator/function   int  str  Example
 ----------------------------
 +                    x        istr(20) + 3 ==> istr('23')
 _                    x        istr(20) - 3 ==> istr('17')
 *                    x        istr(20) * 3 ==> istr('60')
 /                    x        istr(20) / 3 ==> istr('6')
 //                   x        istr(20) // 3 ==> istr('6')
 %                    x        istr(20) % 3 ==> istr('2')
+divmod               x        divmod(istr(20), 3) ==> (istr('6'), istr('2'))
 **                   x        istr(2) ** 3 ==> istr('8')
 @                         x   istr(20) @ 3 ==> istr('202020')
 ==                   x    x   istr(20) == 20 ==> True | istr(20) == '20' ==> True
 |                         x   istr(20) | 5 ==> istr('205')
-abs                  x
+abs                  x        abs(istr(-20)) ==> istr('20')
+bool                 x        bool(istr(' 0 ')) ==> False
 <=, <, >, >=         x        istr('100') > istr('2') ==> True
 slicing              x        istr(12345)[1:3] ==> istr('23')
+iterate                   x   [x for x in istr(20)] ==> [istr('2'), istr('0')
+len                       x   len(istr(' 20 ')) ==> 4
+count                     x   istr(100),count('0') ==> 2
+index                     x   istr(' 100 ').index('0') ==> 2
 ----------------------------
-
+```
 ## Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used.
 
 ## Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
```

### Comparing `istr_python-0.2.0/istr/istr.py` & `istr_python-0.2.0.post0/istr/istr.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 Added __iter__ method__ .
     So now,
         for c in istr('123'):
             ...
         results in c values that are istrs 
 
 Added istr.digits method:
-    Examples
-    --------
-    istr.digits() ==> istr('0123456789')
-    istr.digits('') ==> istr('0123456789')
-    istr.digits('1') ==> istr('1')
-    istr.digits('3-') ==> istr('3456789')
-    istr.digits('-3') ==> istr('0123')
-    istr('1-4', '6', '8-9') ==> istr('1234689')
-    istr.digits('1', '1-2', '1-3') ==> istr('11213')
+Examples
+--------
+istr.digits() ==> istr('0123456789')
+istr.digits('') ==> istr('0123456789')
+istr.digits('1') ==> istr('1')
+istr.digits('3-') ==> istr('3456789')
+istr.digits('-3') ==> istr('0123')
+istr('1-4', '6', '8-9') ==> istr('1234689')
+istr.digits('1', '1-2', '1-3') ==> istr('112123')
+
+    Note that a digit can occur more than once.
 
 version 0.1.2  2024-04-26  
 -------------------------
 Added all relevant string methods to return istrs or data structures with istrs.
 Added corresponding tests.
 
 version 0.1.0  2024-04-22  
@@ -532,14 +534,19 @@
         istr.digits() ==> istr('0123456789')
         istr.digits('') ==> istr('0123456789')
         istr.digits('1') ==> istr('1')
         istr.digits('3-') ==> istr('3456789')
         istr.digits('-3') ==> istr('0123')
         istr('1-4', '6', '8-9') ==> istr('1234689')
         istr('1', '1-2', '1-3') ==> istr('11213')
+
+        Note
+        ----
+        A digit can occur more than once.
+
         '''
         result=[]
         if not args:
             args=['0-9']
         for arg in args:
             if arg.strip()=='':
                 arg='0-9'
@@ -642,12 +649,12 @@
     print(repr(istr.digits()))
     print(istr.digits('1-9'))
     print(istr.digits('1'))
     print(istr.digits('1-2', '6'))    
     print(istr.digits('1-5', '7-9'))        
     print(istr.digits('-5'))   
     print(istr.digits('3-'))   
-    a=istr('1-4', '6', '8-9')
+    print(repr(divmod(istr(20),3)))
 
 if __name__ == "__main__":
     main()
```

### Comparing `istr_python-0.2.0/istr_python.egg-info/PKG-INFO` & `istr_python-0.2.0.post0/istr_python.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.2.0
+Version: 0.2.0.post0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -15,33 +15,34 @@
 
 ## Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
 
-This can be very handy for solving puzzles, but also for other purposes. For instance the
+This can be very handy for solving puzzles, but also for other purposes.</br>
+For instance the
 famous send more money puzzle
 ```
   S E N D
   M O R E
 --------- +
 M O N E Y
 ```
 can be nicely, albeit not very efficient, coded as:
 ```
 import itertools
 from istr import istr
 
 for s, e, n, d, m, o, r, y in istr(itertools.permutations(range(10), 8)):
     if m and ((s|e|n|d) + (m|o|r|e) == (m|o|n|e|y)):
-        print(f" {s|e|n|d}")
-        print(f" {m|o|r|e}")
-        print("-----")
-        print(f"{m|o|n|e|y}")
+        print(f' {s|e|n|d}')
+        print(f' {m|o|r|e}')
+        print('-----')
+        print(f'{m|o|n|e|y}')
 ```
 
 And it is a nice demonstration of extending a class (str) with extra and changed functionality.
 
 ## Installation
 Installing istr with pip is easy.
 ```
@@ -60,34 +61,34 @@
 
 ```
 from istr import istr
 ```
 
 Now we can define some istrs:
 ```
-four = istr("4")
-five = istr("5")
+four = istr('4')
+five = istr('5')
 ```
 Then we can do
 ```
 x= four * five
 ```
-, after which x is `istr("20")`
+, after which x is `istr('20')`
 
 And now we can do
 ```
 print(x == 20)
-print(x == "20")
+print(x == '20')
 ```
 resulting in two times `True`. That's because istrs instances are treated as int, although they are strings.
 
 That means that we can also say
 ```
 print(x < 30)
-print(x >= "10")
+print(x >= '10')
 ```
 again resulting in two times `True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
@@ -111,108 +112,108 @@
 
 And the result is again an istr.
 
 That means that
 ```
 (four | five) / 3
 ```
-is `istr("9")`.
+is `istr('9')`.
 
 In order to repeat a string in the usual sense, you cannot use `3 * four`, as that woud be `12`. 
 
 We use the matrix multiplication operator (@) for this. So `3 @ four` is `444`. As is `four @ 3`.
 
 Also allowed are
 ```
 abs(four)
 -four 
 ```
 
 The bool operator works on the integer value of an istr. So
-`bool("0")` ==> `False`
-`bool("1")` ==> `True`
+`bool(istr('0'))` ==> `False`
+`bool(istr('1'))` ==> `True`
 The code
 ```
-if istr("0"):
-    print("True")
+if istr('0'):
+    print('True')
 else:
-    print("False")
+    print('False')
 ```
 will print `False`
 
 For the in operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
 ```
-"34" in istr(1234)
+'34' in istr(1234)
 34 in istr(1234)
 ```
 On the left hand side an istr is always treated as a string:
 ```
-istr(1234) in "01234566890ABCDEF"
+istr(1234) in '01234566890ABCDEF'
 ```
 
 Note that all calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
 Also divisions are always floor divisions!
 
-There's a special case for `istr("")`. This is a proper empty string, but also represents the value of 0.
-That is to allow for `istr("").join(i for i in "01234)"`, resulting in `istr("01234")`.
+There's a special case for `istr('')`. This is a proper empty string, but also represents the value of 0.
+That is to allow for `istr('').join(i for i in '01234)'`, resulting in `istr('01234')`.
 
 Sorting a list of istrs is based on the integer value, not the string. So
 
-`" ".join(sorted("1 3 2 4 5 6 11 7 9 8 10 12 0".split()))`
+`' '.join(sorted('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))`
 
 is
 
-`"0 1 10 11 2 3 4 5 6 7 8 9"`
+`'0 1 10 11 2 3 4 5 6 7 8 9'`
 
 ,whereas
 
-`" ".join(sorted(istr("1 3 2 4 5 6 11 7 9 8 10 12 0".split())))`
+`' '.join(sorted(istr('1 3 2 4 5 6 11 7 9 8 10 12 0'.split())))`
 
 is 
 
-`"0 1 2 3 4 5 6 7 8 9 10 11"`
+`'0 1 2 3 4 5 6 7 8 9 10 11'`
 
 ## Using other values for istr than numeric value or str
 Apart from with simple numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
 - if a dict (or subtype of dict), the same type dict will be returned with all values istr'ed
 
-    `istr({0: 0, 1: 1, 2: 4})` ==> `{0: istr("0"), 1: istr("1"), 2: istr("4")}`
+    `istr({0: 0, 1: 1, 2: 4})` ==> `{0: istr('0'), 1: istr('1'), 2: istr('4')}`
 
 - if an iterator, the iterator will be mapped with istr
 
     `istr(i * i for i in range(3))` ==> `<map object>`
 
-    `list(istr(i * i for i in range(3)))` ==> `[istr("0"), istr("1"), istr("4")]`
+    `list(istr(i * i for i in range(3)))` ==> `[istr('0'), istr('1'), istr('4')]`
 
 - if an iterable, the same type will be returned with all elements istr'ed
 
-    `istr([0, 1, 4])` ==> `[istr("0"), istr("1"), istr("4")]`
+    `istr([0, 1, 4])` ==> `[istr('0'), istr('1'), istr('4')]`
 
-    `istr((0, 1, 4))` ==> `(istr("0"), istr("1"), istr("4"))`
+    `istr((0, 1, 4))` ==> `(istr('0'), istr('1'), istr('4'))`
 
-    `istr({0, 1, 4})` ==> `{istr("4"), istr("0"), istr("1")} ## or similar`
+    `istr({0, 1, 4})` ==> `{istr('4'), istr('0'), istr('1')} ## or similar`
 
 - if a range, an istr.range instance will be returned
     
     `istr(range(3))` ==> `istr.range(3)`
 
-    `list(istr(range(3)))` ==> `[istr("0"), istr("1"), istr("2")]`
+    `list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]`
 
     `len(istr(range(3)))` ==> `3`
 
 - if an istr.range instance, the same istr.range will be returned
 
 ## More than one parameter for istr
 It is possible to give more than one parameter, in which case a tuple
 of the istrs of the parameters will be returned, which can be handy
 to unpack multiple values, e.g.
 
-`a, b, c = istr(5, 6, 7)` ==> `a=istr("5") , b=istr("6"), c=istr("7")`
+`a, b, c = istr(5, 6, 7)` ==> `a=istr('5') , b=istr('6'), c=istr('7')`
 
 ## test for even/odd
 It is possible to test for even/odd with the
 
 `is_even` and `is_odd` method, e.g.
 
 ```
@@ -221,35 +222,35 @@
 ```
 This will print `True` twice.
 
 ## reverse an istr
 The method `istr.reversed()` will return the an istr with the reversed content:
 ```
 print(repr(istr(456).reversed()))
-print(repr(istr("0456").reversed()))
+print(repr(istr('0456').reversed()))
 ```
 result:
 ```
-istr("654")
-istr("6540")
+istr('654')
+istr('6540')
 ```
 The same can -of course- be achieved with
 ```
 print(repr(istr(456)[::-1]))
-print(repr(istr("0456")[::-1]))
+print(repr(istr('0456')[::-1]))
 ```
 Note that is impossible to reverse a negative istr.
 
 ## enumerate with istrs
 
 The `istr.enumerate` method can be used just as the builtin enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
 ```
-    for i,c in istr.enumerate("abc"):
-        print(f"{repr(i)} {c}")
+    for i,c in istr.enumerate('abc'):
+        print(f'{repr(i)} {c}')
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
 ```
@@ -259,14 +260,44 @@
 The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
 `list(istr.concat(((1,2),(3,4)))` ==> `istr([12,34])`
 
 `list(istr.concat(itertools.permutations(range(3),2)))` ==> `[istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')]` 
 
+## generate istr with digits
+
+The class method `digits` can be used to return an istr of digits according to a given specification.
+The method takes either no or a number of arguments.
+
+If no arguments are given, the result will be istr('0123456789').
+
+The given argument(s) result in a range of digits.
+
+- `<n>` ==> n
+- `<n-m> ==> n, n+1, ..., m
+- `-n>` ==> 0, 1, ... n
+- `n->` ==> n, n+1, ..., 9
+- `''` ==> 0, 1, ..., 9
+
+(n and m must be digit between 0 and 9)
+
+The final result is an istr composed of the given range(s).
+
+Here are some examples:
+
+- `istr.digits()` ==> `istr('0123456789')`
+- `istr.digits('')` ==> `istr('0123456789')`
+- `istr.digits('1')` ==> `istr('1')`
+- `istr.digits('3-')` ==> `istr('3456789')`
+- `istr.digits('-3')` ==> `istr('0123')`
+- `istr('1-4', '6', '8-9')` ==> `istr('1234689')`
+- `istr('1', '1-2', '1-3')` ==> `istr('11213')`
+
+
 ## Subclassing istr
 When a class is derived from istr, all methods will return that newly derived class. 
 
 E.g.
 ```
 class jstr(istr):
     ...
@@ -279,36 +310,36 @@
 
 It is possible to control the way an `istr` instance will be repr'ed.
 
 By default, the `istr('5')` is represented as `istr('5')`.
 
 With the istr.repr_mode() context manager, that can be changed:
 ```
-with istr.repr_mode("str"):
+with istr.repr_mode('str'):
     five = istr('5')
     print(repr(five))
-with istr.repr_mode("int"):
+with istr.repr_mode('int'):
     five = istr('5')
     print(repr(five))
-with istr.repr_mode("istr"):
+with istr.repr_mode('istr'):
     five = istr('5')
     print(repr(five))
 ```
 This will print
 ```
 '5'
 5
 istr('5')
 ```
 Note that the way an `istr` is represented is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 
 ```
-istr.repr_mode("str")
+istr.repr_mode('str')
 five = istr('5')
 print(repr(five))
 ```
 This will print
 ```
 '5'
 ```
@@ -326,15 +357,15 @@
 
 Note that the integer is always stored in base 10 mode, but the string
 representation will reflect the chosen base (at time of initialization).
 
 Some examples:
 ```
 with istr.base(16):
-    a = istr("7fff")
+    a = istr('7fff')
     print(int(a))
 
     b = istr(15)
     print(repr(b))
 ```
 This will result in
 ```
@@ -344,15 +375,15 @@
 All calculations are done in the decimal 10 system.
 
 Note that the way an `istr` is interpreted is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 ```
 istr.base(16)
-print(int(istr("7fff")))
+print(int(istr('7fff')))
 ```
 This will print
 ```
 32767
 ```
 Finally, the current base can be queried with `istr.base()`, so upon start:
 ```
@@ -374,70 +405,79 @@
 
 `repr(4))` ==> `istr('4')`
 
 With the `istr.format()` context manager this behavior can be changed.
 If the format specifier is a number, most likely a single digit, that
 will be the minimum number of characters in the string:
 ```
-with istr.format("3"):
+with istr.format('3'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('  1')
 istr(' 12')
 istr('123')
 istr('1234')
 ```
 If the string starts with a `0`, the string will be zero filled:
 ```
-with istr.format("03"):
+with istr.format('03'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('001')
 istr('012')
 istr('123')
 istr('1234')
 ```
 Note that if a format other than the default `''` is used, the string will reformatted even if the `istr` is specified with a string:
 ```
-with istr.format("03"):
-    print(repr(istr("  12 ")))
+with istr.format('03'):
+    print(repr(istr('  12 ')))
 ```
 will result in `istr('0012')`
 
 Remark: For bases other than 10, the string will never be reformatted!
 
 ## Operations
 ----------------------------
+```
+The table below shows whether the string or the int version of istr is applied.
+
 operator/function   int  str  Example
 ----------------------------
 +                    x        istr(20) + 3 ==> istr('23')
 _                    x        istr(20) - 3 ==> istr('17')
 *                    x        istr(20) * 3 ==> istr('60')
 /                    x        istr(20) / 3 ==> istr('6')
 //                   x        istr(20) // 3 ==> istr('6')
 %                    x        istr(20) % 3 ==> istr('2')
+divmod               x        divmod(istr(20), 3) ==> (istr('6'), istr('2'))
 **                   x        istr(2) ** 3 ==> istr('8')
 @                         x   istr(20) @ 3 ==> istr('202020')
 ==                   x    x   istr(20) == 20 ==> True | istr(20) == '20' ==> True
 |                         x   istr(20) | 5 ==> istr('205')
-abs                  x
+abs                  x        abs(istr(-20)) ==> istr('20')
+bool                 x        bool(istr(' 0 ')) ==> False
 <=, <, >, >=         x        istr('100') > istr('2') ==> True
 slicing              x        istr(12345)[1:3] ==> istr('23')
+iterate                   x   [x for x in istr(20)] ==> [istr('2'), istr('0')
+len                       x   len(istr(' 20 ')) ==> 4
+count                     x   istr(100),count('0') ==> 2
+index                     x   istr(' 100 ').index('0') ==> 2
 ----------------------------
-
+```
 ## Test script
 There's an extensive pytest script in the `\tests` directory.
 
 This script also shows clearly the ways istr can be used.
 
 ## Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
```

### Comparing `istr_python-0.2.0/pyproject.toml` & `istr_python-0.2.0.post0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "0.2.0"
+version = "0.2.0-0"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `istr_python-0.2.0/tests/test_istr.py` & `istr_python-0.2.0.post0/tests/test_istr.py`

 * *Files identical despite different names*

