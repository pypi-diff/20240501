# Comparing `tmp/GlobalKit-1.6.tar.gz` & `tmp/globalkit-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GlobalKit-1.6.tar", last modified: Fri Nov  3 12:20:22 2023, max compression
+gzip compressed data, was "globalkit-1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `GlobalKit-1.6.tar` & `globalkit-1.7.tar`

### file list

```diff
@@ -1,15 +1,11 @@
-drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-11-03 12:20:22.775775 GlobalKit-1.6/
-drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-11-03 12:20:22.774643 GlobalKit-1.6/GlobalKit/
--rw-r--r--   0 artemkarpenko   (501) staff       (20)       50 2023-10-01 12:54:46.000000 GlobalKit-1.6/GlobalKit/__init__.py
--rw-r--r--   0 artemkarpenko   (501) staff       (20)     1862 2023-11-03 12:11:36.000000 GlobalKit-1.6/GlobalKit/alphabets.py
--rw-r--r--   0 artemkarpenko   (501) staff       (20)     1944 2023-11-03 10:29:58.000000 GlobalKit-1.6/GlobalKit/extra.py
--rw-r--r--   0 artemkarpenko   (501) staff       (20)     2533 2023-11-03 12:11:36.000000 GlobalKit-1.6/GlobalKit/functions.py
-drwxr-xr-x   0 artemkarpenko   (501) staff       (20)        0 2023-11-03 12:20:22.775373 GlobalKit-1.6/GlobalKit.egg-info/
--rw-r--r--   0 artemkarpenko   (501) staff       (20)     2609 2023-11-03 12:20:22.000000 GlobalKit-1.6/GlobalKit.egg-info/PKG-INFO
--rw-r--r--   0 artemkarpenko   (501) staff       (20)      237 2023-11-03 12:20:22.000000 GlobalKit-1.6/GlobalKit.egg-info/SOURCES.txt
--rw-r--r--   0 artemkarpenko   (501) staff       (20)        1 2023-11-03 12:20:22.000000 GlobalKit-1.6/GlobalKit.egg-info/dependency_links.txt
--rw-r--r--   0 artemkarpenko   (501) staff       (20)       10 2023-11-03 12:20:22.000000 GlobalKit-1.6/GlobalKit.egg-info/top_level.txt
--rw-r--r--   0 artemkarpenko   (501) staff       (20)     2609 2023-11-03 12:20:22.775610 GlobalKit-1.6/PKG-INFO
--rw-r--r--   0 artemkarpenko   (501) staff       (20)     2309 2023-11-03 12:20:10.000000 GlobalKit-1.6/README.md
--rw-r--r--   0 artemkarpenko   (501) staff       (20)       38 2023-11-03 12:20:22.775828 GlobalKit-1.6/setup.cfg
--rw-r--r--   0 artemkarpenko   (501) staff       (20)      563 2023-11-03 12:11:36.000000 GlobalKit-1.6/setup.py
+-rw-r--r--   0        0        0      158 2024-02-08 20:59:00.023277 globalkit-1.7/.editorconfig
+-rw-r--r--   0        0        0      195 2024-01-09 22:53:50.256838 globalkit-1.7/.gitignore
+-rw-r--r--   0        0        0      607 2024-01-13 22:18:47.215489 globalkit-1.7/GlobalKit/__init__.py
+-rw-r--r--   0        0        0     1465 2024-05-01 17:17:01.870336 globalkit-1.7/GlobalKit/alphabet.py
+-rw-r--r--   0        0        0     2189 2024-03-16 14:25:15.718263 globalkit-1.7/GlobalKit/functions.py
+-rw-r--r--   0        0        0     2132 2024-05-01 17:17:01.863641 globalkit-1.7/GlobalKit/main.py
+-rw-r--r--   0        0        0     3451 2024-05-01 17:17:01.867133 globalkit-1.7/README.md
+-rw-r--r--   0        0        0     1070 2024-05-01 17:17:01.857689 globalkit-1.7/license.txt
+-rw-r--r--   0        0        0      844 2024-02-08 20:52:06.435388 globalkit-1.7/pyproject.toml
+-rw-r--r--   0        0        0     1322 2024-05-01 17:17:01.874674 globalkit-1.7/tests/test_functions.py
+-rw-r--r--   0        0        0     4136 1970-01-01 00:00:00.000000 globalkit-1.7/PKG-INFO
```

### Comparing `GlobalKit-1.6/GlobalKit/alphabets.py` & `globalkit-1.7/GlobalKit/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from .extra import Alphabet
+from typing import Final
 
-# Create instances of the Alphabet class for various languages
-english = Alphabet('abcdefghijklmnopqrstuvwxyz', 'aeiouy', 'bcdfghjklmnpqrstvwxz')
-spanish = Alphabet('abcdefghijklmnñopqrstuvwxyz', 'aeiouáéíóúü', 'bcdfghjklmnñpqrstvwxyz')
-french = Alphabet('abcdefghijklmnopqrstuvwxyzàâçéèêëîïôùûüœ', 'aeiouàâéèêëîïôùûüœ', 'bcçdfghjklmnpqrstvwxyz')
-german = Alphabet('abcdefghijklmnopqrstuvwxyzäöüß', 'aeiouäöü', 'bcdfghjklmnpqrstvwxyzß')
-italian = Alphabet('abcdefghijklmnopqrstuvwxyzàèéìòù', 'aeiouàèéìòù', 'bcdfghjklmnpqrstvwxyz')
-portuguese = Alphabet('abcdefghijklmnopqrstuvwxyzáâãàçéêíóôõú', 'aeiouáâãàéêíóôõú', 'bcdfghjklmnpqrstvwxyzç')
-dutch = Alphabet('abcdefghijklmnopqrstuvwxyz', 'aeiou', 'bcdfghjklmnpqrstvwxyz')
-finnish = Alphabet('abcdefghijklmnopqrstuvwxyzåäö', 'aeiouyåäö', 'bcdfghjklmnpqrstvwxz')
-swedish = Alphabet('abcdefghijklmnopqrstuvwxyzåäö', 'aeiouyåäö', 'bcdfghjklmnpqrstvwxz')
-norwegian = Alphabet('abcdefghijklmnopqrstuvwxyzåæø', 'aeiouyåæø', 'bcdfghjklmnpqrstvwxz')
-russian = Alphabet('абвгдеёжзийклмнопрстуфхцчшщъыьэюя', 'аеёиоуэыюя', 'бвгджзйклмнпрстфхцчшщ', 'ъь')
-ukrainian = Alphabet('абвгґдеєжзиіїйклмнопрстуфхцчшщьюя', 'аеєиіїоуюя', 'бвгґджзйклмнпрстфхцчшщ', 'ь')
-polish = Alphabet('aąbcćdeęfghijklłmnńoópqrsśtuvwxyzźż', 'aeiouyąę', 'bcćdfghjklłmnńpqrsśtvwxzźż')
-bulgarian = Alphabet('абвгдежзийклмнопрстуфхцчшщъьюя', 'аеиоуъя', 'бвгджзйклнпрстфхцчшщ', 'ь')
+from .alphabet import Alphabet
 
-# Define other character sets
-digits: str = '0123456789'
-brackets: str = '()[]{}<>'
-space: str = ' '
-newline: str = '\n'
-tab: str = '\t'
+# Instances of the Alphabet dataclass
+english: Final[Alphabet] = Alphabet('abcdefghijklmnopqrstuvwxyz', 'aeiouy', 'bcdfghjklmnpqrstvwxz')
+spanish: Final[Alphabet] = Alphabet('abcdefghijklmnñopqrstuvwxyz', 'aeiouáéíóúü', 'bcdfghjklmnñpqrstvwxyz')
+french: Final[Alphabet] = Alphabet('abcdefghijklmnopqrstuvwxyzàâçéèêëîïôùûüœ', 'aeiouàâéèêëîïôùûüœ', 'bcçdfghjklmnpqrstvwxyz')
+german: Final[Alphabet] = Alphabet('abcdefghijklmnopqrstuvwxyzäöüß', 'aeiouäöü', 'bcdfghjklmnpqrstvwxyzß')
+italian: Final[Alphabet] = Alphabet('abcdefghijklmnopqrstuvwxyzàèéìòù', 'aeiouàèéìòù', 'bcdfghjklmnpqrstvwxyz')
+portuguese: Final[Alphabet] = Alphabet('abcdefghijklmnopqrstuvwxyzáâãàçéêíóôõú', 'aeiouáâãàéêíóôõú', 'bcdfghjklmnpqrstvwxyzç')
+dutch: Final[Alphabet] = Alphabet('abcdefghijklmnopqrstuvwxyz', 'aeiou', 'bcdfghjklmnpqrstvwxyz')
+finnish: Final[Alphabet] = Alphabet('abcdefghijklmnopqrstuvwxyzåäö', 'aeiouyåäö', 'bcdfghjklmnpqrstvwxz')
+swedish: Final[Alphabet] = Alphabet('abcdefghijklmnopqrstuvwxyzåäö', 'aeiouyåäö', 'bcdfghjklmnpqrstvwxz')
+norwegian: Final[Alphabet] = Alphabet('abcdefghijklmnopqrstuvwxyzåæø', 'aeiouyåæø', 'bcdfghjklmnpqrstvwxz')
+russian: Final[Alphabet] = Alphabet('абвгдеёжзийклмнопрстуфхцчшщъыьэюя', 'аеёиоуэыюя', 'бвгджзйклмнпрстфхцчшщ', 'ъь')
+ukrainian: Final[Alphabet] = Alphabet('абвгґдеєжзиіїйклмнопрстуфхцчшщьюя', 'аеєиіїоуюя', 'бвгґджзйклмнпрстфхцчшщ', 'ь')
+bulgarian: Final[Alphabet] = Alphabet('абвгдежзийклмнопрстуфхцчшщъьюя', 'аеиоуъя', 'бвгджзйклнпрстфхцчшщ', 'ь')
+polish: Final[Alphabet] = Alphabet('aąbcćdeęfghijklłmnńoópqrsśtuvwxyzźż', 'aeiouyąę', 'bcćdfghjklłmnńpqrsśtvwxzźż')
+
+# Other character sets
+digits: Final[str] = '0123456789'
+brackets: Final[str] = '()[]{}<>'
+space: Final[str] = ' '
+newline: Final[str] = '\n'
+tab: Final[str] = '\t'
```

### Comparing `GlobalKit-1.6/GlobalKit/extra.py` & `globalkit-1.7/GlobalKit/alphabet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-# Define a class to represent an alphabet
+from dataclasses import dataclass, field
+from typing import Optional
+
+
+@dataclass
 class Alphabet:
-    def __init__(self, full: str, vowels: str, consonants: str, special: str = None):
-        # Initialize the lowercase, uppercase, and full alphabet strings
-        self.full_lowercase: str = full.lower()
-        self.full_uppercase: str = full.upper()
-        self.full: str = self.full_lowercase + self.full_uppercase
-
-        # Initialize the lowercase, uppercase, and vowels strings
-        self.vowels_lowercase: str = vowels.lower()
-        self.vowels_uppercase: str = vowels.upper()
-        self.vowels: str = self.vowels_lowercase + self.vowels_uppercase
-
-        # Initialize the lowercase, uppercase, and consonants strings
-        self.consonants_lowercase: str = consonants.lower()
-        self.consonants_uppercase: str = consonants.upper()
-        self.consonants: str = self.consonants_lowercase + self.consonants_uppercase
-
-        # Check if special characters are provided
-        if special is None:
-            self.special_lowercase = None
-            self.special_uppercase = None
-            self.special = None
-        else:
-            # Initialize the lowercase, uppercase, and special characters strings
-            self.special_lowercase: str = special.lower()
-            self.special_uppercase: str = special.upper()
-            self.special: str = self.special_lowercase + self.special_uppercase
-
-    # Define a method to print the alphabet details
-    def __call__(self, *args, **kwargs):
-        # Print the full alphabet
-        print('Full:\t\t', ' '.join(self.full_lowercase))
-        print('-' * 100)
-
-        # Print the vowels
-        print('Vowels:\t\t', ' '.join(self.vowels_lowercase))
-
-        # Print the consonants
-        print('Consonants:\t', ' '.join(self.consonants_lowercase))
-
-        # Check if special characters are provided
-        if self.special is not None:
-            print('Special:\t', ' '.join(self.special_lowercase))
+	full_lowercase: str
+	full_uppercase: str = field(init=False)
+	full: str = field(init=False)
+
+	vowels_lowercase: str
+	vowels_uppercase: str = field(init=False)
+	vowels: str = field(init=False)
+
+	consonants_lowercase: str
+	consonants_uppercase: str = field(init=False)
+	consonants: str = field(init=False)
+
+	special_lowercase: Optional[str] = None
+	special_uppercase: Optional[str] = field(init=False)
+	special: Optional[str] = field(init=False)
+	has_special: bool = field(init=False)
+
+	def __post_init__(self) -> None:
+		self.full_lowercase = self.full_lowercase.lower().strip()
+		self.full_uppercase = self.full_lowercase.upper()
+		self.full = self.full_lowercase + self.full_uppercase
+
+		self.vowels_lowercase = self.vowels_lowercase.lower().strip()
+		self.vowels_uppercase = self.vowels_lowercase.upper()
+		self.vowels = self.vowels_lowercase + self.vowels_uppercase
+
+		self.consonants_lowercase = self.consonants_lowercase.lower().strip()
+		self.consonants_uppercase = self.consonants_lowercase.upper()
+		self.consonants = self.consonants_lowercase + self.consonants_uppercase
+
+		if self.special_lowercase is not None:
+			self.special_uppercase = self.special_lowercase.upper()
+			self.special = self.special_lowercase + self.special_uppercase
+			self.has_special = True
+		else:
+			self.special_uppercase = None
+			self.special = None
+			self.has_special = False
```

