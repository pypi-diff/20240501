# Comparing `tmp/laoshi-0.0.3.tar.gz` & `tmp/laoshi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laoshi-0.0.3.tar", max compression
+gzip compressed data, was "laoshi-0.1.1.tar", max compression
```

## Comparing `laoshi-0.0.3.tar` & `laoshi-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    16726 2024-04-05 10:19:14.171508 laoshi-0.0.3/LICENSE
--rw-r--r--   0        0        0       48 2024-04-05 10:19:14.171508 laoshi-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-05 10:19:14.171508 laoshi-0.0.3/laoshi/__init__.py
--rw-r--r--   0        0        0     1173 2024-04-05 10:19:14.175508 laoshi-0.0.3/laoshi/converter.py
--rw-r--r--   0        0        0     4903 2024-04-05 10:19:14.175508 laoshi-0.0.3/laoshi/deckmanager.py
--rw-r--r--   0        0        0     3967 2024-04-05 10:19:14.175508 laoshi-0.0.3/laoshi/flashcardgenerator.py
--rw-r--r--   0        0        0     2176 2024-04-05 10:19:14.175508 laoshi-0.0.3/laoshi/main.py
--rw-r--r--   0        0        0      888 2024-04-05 10:19:14.175508 laoshi-0.0.3/laoshi/speaker.py
--rw-r--r--   0        0        0      467 2024-04-05 10:19:14.175508 laoshi-0.0.3/laoshi/translator.py
--rw-r--r--   0        0        0      540 2024-04-05 10:19:14.175508 laoshi-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      722 1970-01-01 00:00:00.000000 laoshi-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    16726 2024-05-01 07:05:22.091877 laoshi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1813 2024-05-01 07:05:22.091877 laoshi-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-01 07:05:22.091877 laoshi-0.1.1/laoshi/__init__.py
+-rw-r--r--   0        0        0     1173 2024-05-01 07:05:22.091877 laoshi-0.1.1/laoshi/converter.py
+-rw-r--r--   0        0        0     4903 2024-05-01 07:05:22.091877 laoshi-0.1.1/laoshi/deckmanager.py
+-rw-r--r--   0        0        0     3967 2024-05-01 07:05:22.091877 laoshi-0.1.1/laoshi/flashcardgenerator.py
+-rw-r--r--   0        0        0     2392 2024-05-01 07:05:22.091877 laoshi-0.1.1/laoshi/main.py
+-rw-r--r--   0        0        0      888 2024-05-01 07:05:22.091877 laoshi-0.1.1/laoshi/speaker.py
+-rw-r--r--   0        0        0      467 2024-05-01 07:05:22.091877 laoshi-0.1.1/laoshi/translator.py
+-rw-r--r--   0        0        0      540 2024-05-01 07:05:22.091877 laoshi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2487 1970-01-01 00:00:00.000000 laoshi-0.1.1/PKG-INFO
```

### Comparing `laoshi-0.0.3/LICENSE` & `laoshi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `laoshi-0.0.3/laoshi/converter.py` & `laoshi-0.1.1/laoshi/converter.py`

 * *Files identical despite different names*

### Comparing `laoshi-0.0.3/laoshi/deckmanager.py` & `laoshi-0.1.1/laoshi/deckmanager.py`

 * *Files identical despite different names*

### Comparing `laoshi-0.0.3/laoshi/flashcardgenerator.py` & `laoshi-0.1.1/laoshi/flashcardgenerator.py`

 * *Files identical despite different names*

### Comparing `laoshi-0.0.3/laoshi/main.py` & `laoshi-0.1.1/laoshi/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 SIMPLIFIED = "simplified"
 TRADITIONAL = "traditional"
 CHINESE_OPTIONS = [TRADITIONAL, SIMPLIFIED, "pinyin"]
 
 
 @click.group()
 def cli_group():
-    """cli group function for click"""
+    """cli application to learn chinese."""
 
 
 @cli_group.command(help="Convert characters")
 @click.option(
     "-t",
     "--to",
     default="pinyin",
@@ -36,36 +36,40 @@
 
 @cli_group.command(help="Translate a phrase")
 @click.option(
     "-t",
     "--to",
     default="en",
 )
+@click.option('--pinyin', '-p', is_flag=True)
 @click.argument("phrase")
-def translate(to: str, phrase: str):
+def translate(to: str, pinyin: bool, phrase: str):
     """Translate a phrase"""
-    click.echo(Translator().translate(phrase, dest=to))
+    translation = Translator().translate(phrase, dest=to)
+    if pinyin:
+        translation = translation + f' ({Converter.to_pinyin(phrase)})'
+    click.echo(translation)
 
 
 @cli_group.group()
 def manage_deck():
-    """Manage deck group"""
+    """Manage deck subcommand"""
 
 
 @manage_deck.command()
 @click.option(
     "-c",
     "--character",
     default="simplified",
     type=click.Choice([SIMPLIFIED, TRADITIONAL]),
 )
 @click.argument("deck_name")
 @click.argument("seed")
 def create_deck(character: str, deck_name: str, seed: str):
-    """Create a deck function for click"""
+    """Create a deck command from one seed word or phrase"""
     with FlashCardGenerator() as generator:
         flashcard = generator.create_flashcard(character, seed)
         DeckManager(deck_name).create_deck(flashcard)
 
 
 @manage_deck.command()
 @click.option(
@@ -73,15 +77,15 @@
     "--character",
     default="simplified",
     type=click.Choice([SIMPLIFIED, TRADITIONAL]),
 )
 @click.argument("deck_name")
 @click.argument("word")
 def add_note(character: str, deck_name: str, word: str):
-    """add note function for click"""
+    """add a note to an Anki deck with a word"""
     with FlashCardGenerator() as generator:
         flashcard = generator.create_flashcard(character, word)
         DeckManager(deck_name).add_note(flashcard)
 
 
 if __name__ == "__main__":
     cli_group()
```

### Comparing `laoshi-0.0.3/laoshi/speaker.py` & `laoshi-0.1.1/laoshi/speaker.py`

 * *Files identical despite different names*

### Comparing `laoshi-0.0.3/pyproject.toml` & `laoshi-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "laoshi"
-version = "0.0.3"
+version = "0.1.1"
 description = ""
 authors = ["Ruben Serradas <rubenserradas@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pypinyin = "^0.50.0"
```

