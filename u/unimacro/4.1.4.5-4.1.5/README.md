# Comparing `tmp/unimacro-4.1.4.5.tar.gz` & `tmp/unimacro-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unimacro-4.1.4.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "unimacro-4.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `unimacro-4.1.4.5.tar` & `unimacro-4.1.5.tar`

### file list

```diff
@@ -1,205 +1,205 @@
--rw-r--r--   0        0        0     1512 2024-03-15 14:44:12.009781 unimacro-4.1.4.5/README.md
--rw-r--r--   0        0        0     2042 2024-03-15 14:44:12.045782 unimacro-4.1.4.5/pyproject.toml
--rw-r--r--   0        0        0    17719 2024-03-15 14:44:12.045782 unimacro-4.1.4.5/src/unimacro/BrowseGrammar.py
--rw-r--r--   0        0        0    22395 2024-03-15 14:44:12.045782 unimacro-4.1.4.5/src/unimacro/BrowseGrammarApp.py
--rw-r--r--   0        0        0     2345 2024-03-15 14:44:12.045782 unimacro-4.1.4.5/src/unimacro/D_.py
--rw-r--r--   0        0        0     2615 2024-03-15 14:44:12.045782 unimacro-4.1.4.5/src/unimacro/D_train.py
--rw-r--r--   0        0        0     8783 2024-03-15 14:44:12.045782 unimacro-4.1.4.5/src/unimacro/DialogServer.py
--rw-r--r--   0        0        0    13226 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_calculator.py
--rw-r--r--   0        0        0    24467 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_keystrokes.py
--rw-r--r--   0        0        0     9731 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_latex.py
--rw-r--r--   0        0        0    24857 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_number extended.py
--rw-r--r--   0        0        0    21073 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_oops.py
--rw-r--r--   0        0        0    34546 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_repeat.py
--rw-r--r--   0        0        0     2626 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_testtrayicon.py
--rw-r--r--   0        0        0     7251 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_unimacrotest.py
--rw-r--r--   0        0        0     9163 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/excel.py
--rw-r--r--   0        0        0    28498 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/frescobaldi.py
--rw-r--r--   0        0        0    12529 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/solitaire.py
--rw-r--r--   0        0        0     1669 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/winword_variable.py
--rw-r--r--   0        0        0     3557 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/xxxxnatspeak_dialog.py
--rw-r--r--   0        0        0    15156 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/TrainDialog.py
--rw-r--r--   0        0        0      713 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/README.txt
--rw-r--r--   0        0        0       38 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/__init__.py
--rw-r--r--   0        0        0     7976 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_brackets.py
--rw-r--r--   0        0        0    12892 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_clickbyvoice.py
--rw-r--r--   0        0        0     2780 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_debug_natlink.py.txt
--rw-r--r--   0        0        0     1716 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_debug_unimacro.py.txt
--rw-r--r--   0        0        0     8325 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_folders fillinstancevariables.txt
--rw-r--r--   0        0        0   101791 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_folders.py
--rw-r--r--   0        0        0    41422 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_general.py
--rw-r--r--   0        0        0    34074 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_lines.py
--rw-r--r--   0        0        0     4506 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_number simple.py
--rw-r--r--   0        0        0     5503 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_tags.py
--rw-r--r--   0        0        0    46227 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_tasks.py
--rw-r--r--   0        0        0      865 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/settings folders grammar.txt
--rw-r--r--   0        0        0      851 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/__init__.py
--rw-r--r--   0        0        0    30609 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/_control.py
--rw-r--r--   0        0        0     6540 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/check_unimacro_grammars.py
--rw-r--r--   0        0        0      766 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/defaulticons/idi_down.ico
--rw-r--r--   0        0        0      766 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/defaulticons/idi_down2.ico
--rw-r--r--   0        0        0      766 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/defaulticons/idi_left.ico
--rw-r--r--   0        0        0      766 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/defaulticons/idi_left2.ico
--rw-r--r--   0        0        0      766 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/defaulticons/idi_nodir.ico
--rw-r--r--   0        0        0      766 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/defaulticons/idi_right.ico
--rw-r--r--   0        0        0      766 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/defaulticons/idi_right2.ico
--rw-r--r--   0        0        0      766 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/defaulticons/idi_up.ico
--rw-r--r--   0        0        0      766 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/defaulticons/idi_up2.ico
--rw-r--r--   0        0        0     2602 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/dos83.py
--rw-r--r--   0        0        0    15036 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/enabledictation/_enabledictation.py
--rw-r--r--   0        0        0       90 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/foldersrememberdialog.py
--rw-r--r--   0        0        0    50189 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/iban.py
--rw-r--r--   0        0        0      894 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/icons/repeat.ico
--rw-r--r--   0        0        0      894 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/icons/repeat2.ico
--rw-r--r--   0        0        0      894 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/icons/waiting.ico
--rw-r--r--   0        0        0      894 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/icons/waiting2.ico
--rw-r--r--   0        0        0    13406 2024-03-15 14:44:12.049782 unimacro-4.1.4.5/src/unimacro/listdialogs.py
--rw-r--r--   0        0        0    11172 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/lynote.py
--rw-r--r--   0        0        0     9892 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/namelist.py
--rw-r--r--   0        0        0   132567 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/natlinkutilsbj.py
--rw-r--r--   0        0        0     2567 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/nld_spokenforms.ini
--rw-r--r--   0        0        0      196 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ahk/getintoforeground.ahk
--rw-r--r--   0        0        0       47 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ahk/showmessageswindow.ahk
--rw-r--r--   0        0        0    17742 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/_control.py
--rw-r--r--   0        0        0    48047 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/_dictationproject.py
--rw-r--r--   0        0        0    49150 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/_global_dictation.py
--rw-r--r--   0        0        0     9009 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/actions.ini
--rw-r--r--   0        0        0      245 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/config_scripts/disable_natlink.bat
--rw-r--r--   0        0        0      518 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_kaiser.bat
--rw-r--r--   0        0        0      606 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_kaiser_qh.bat
--rw-r--r--   0        0        0      517 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_qh.bat
--rw-r--r--   0        0        0     1384 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/enx_inifiles/Template List.txt
--rw-r--r--   0        0        0      599 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/enx_inifiles/_control.ini
--rw-r--r--   0        0        0     2536 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/enx_inifiles/_global_dictation.ini
--rw-r--r--   0        0        0     9009 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/enx_inifiles/actions.ini
--rw-r--r--   0        0        0      599 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/nld_inifiles/_control.ini
--rw-r--r--   0        0        0     2575 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/nld_inifiles/_global_dictation.ini
--rw-r--r--   0        0        0     1900 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_global_dictation/starting messages.txt
--rw-r--r--   0        0        0    12521 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/actions.ini
--rw-r--r--   0        0        0      440 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/deu_inifiles/_control.ini
--rw-r--r--   0        0        0     2379 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/deu_spokenforms.ini
--rw-r--r--   0        0        0      212 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_browser.ini
--rw-r--r--   0        0        0     2165 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_commands.ini
--rw-r--r--   0        0        0      380 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_control.ini
--rw-r--r--   0        0        0      208 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_documentation.ini
--rw-r--r--   0        0        0      426 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_editcomments.ini
--rw-r--r--   0        0        0      142 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_first_sample_docstring.ini
--rw-r--r--   0        0        0       86 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_gramoff.ini
--rw-r--r--   0        0        0       58 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_gramon.ini
--rw-r--r--   0        0        0     2461 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_keystrokes.ini
--rw-r--r--   0        0        0     2128 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_latex.ini
--rw-r--r--   0        0        0      586 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_modes.ini
--rw-r--r--   0        0        0      260 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_number.ini
--rw-r--r--   0        0        0      234 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_oops.ini
--rw-r--r--   0        0        0      885 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_repeat.ini
--rw-r--r--   0        0        0      174 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_second_sample_docstring.ini
--rw-r--r--   0        0        0      412 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_shownumbersplus.ini
--rw-r--r--   0        0        0      403 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_tags.ini
--rw-r--r--   0        0        0      179 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_unimacrosample_docstring.ini
--rw-r--r--   0        0        0      122 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_unimacrotest.ini
--rw-r--r--   0        0        0      726 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/chrome_browsing.ini
--rw-r--r--   0        0        0      538 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/firefox_browsing.ini
--rw-r--r--   0        0        0      130 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/natspeak_dialog.ini
--rw-r--r--   0        0        0      284 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/sol.ini
--rw-r--r--   0        0        0      284 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/solitaire.ini
--rw-r--r--   0        0        0      147 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/winword_styles_unimacro.ini
--rw-r--r--   0        0        0     2454 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/enx_spokenforms.ini
--rw-r--r--   0        0        0      430 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_control.ini
--rw-r--r--   0        0        0     2224 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_folders.ini
--rw-r--r--   0        0        0     1323 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_general.ini
--rw-r--r--   0        0        0     2096 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_keystrokes.ini
--rw-r--r--   0        0        0     1309 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_lines.ini
--rw-r--r--   0        0        0     1415 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_repeat.ini
--rw-r--r--   0        0        0     1779 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_tasks.ini
--rw-r--r--   0        0        0     1110 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/firefox_browsing.ini
--rw-r--r--   0        0        0     2527 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/esp_spokenforms.ini
--rw-r--r--   0        0        0     2592 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/ita_spokenforms.ini
--rw-r--r--   0        0        0      350 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_brackets.ini
--rw-r--r--   0        0        0      240 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_browser.ini
--rw-r--r--   0        0        0      671 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_clickbyvoice.ini
--rw-r--r--   0        0        0     3918 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_commands.ini
--rw-r--r--   0        0        0      449 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_control.ini
--rw-r--r--   0        0        0      215 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_documentation.ini
--rw-r--r--   0        0        0      487 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_editcomments.ini
--rw-r--r--   0        0        0      151 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_first_sample_docstring.ini
--rw-r--r--   0        0        0     2018 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_folders.ini
--rw-r--r--   0        0        0     1218 2024-03-15 14:44:12.053782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_general.ini
--rw-r--r--   0        0        0     2052 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_keystrokes.ini
--rw-r--r--   0        0        0      846 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_latex.ini
--rw-r--r--   0        0        0     1132 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_lines.ini
--rw-r--r--   0        0        0      633 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_modes.ini
--rw-r--r--   0        0        0      359 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_number extended.ini
--rw-r--r--   0        0        0      336 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_number simple.ini
--rw-r--r--   0        0        0      229 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_number.ini
--rw-r--r--   0        0        0      246 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_oops.ini
--rw-r--r--   0        0        0      955 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_repeat.ini
--rw-r--r--   0        0        0      181 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_second_sample_docstring.ini
--rw-r--r--   0        0        0      445 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_shownumbersplus.ini
--rw-r--r--   0        0        0      422 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_tags.ini
--rw-r--r--   0        0        0     2563 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_tasks.ini
--rw-r--r--   0        0        0      207 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_unimacrotest.ini
--rw-r--r--   0        0        0      208 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_unittest.ini
--rw-r--r--   0        0        0      851 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/chrome_browsing.ini
--rw-r--r--   0        0        0     1085 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/excel.ini
--rw-r--r--   0        0        0      684 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/firefox_browsing.ini
--rw-r--r--   0        0        0      148 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/natspeak_dialog.ini
--rw-r--r--   0        0        0      165 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/natspeak_sample_docstring.ini
--rw-r--r--   0        0        0      314 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/sol.ini
--rw-r--r--   0        0        0      314 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/solitaire.ini
--rw-r--r--   0        0        0      178 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/winword_styles_unimacro.ini
--rw-r--r--   0        0        0     2567 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/nld_spokenforms.ini
--rw-r--r--   0        0        0      333 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/othertest_spokenforms.ini
--rw-r--r--   0        0        0     3818 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/spokenforms - kopie.ini
--rw-r--r--   0        0        0     3818 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/spokenforms.ini
--rw-r--r--   0        0        0     2089 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/sample_ini/test_spokenforms.ini
--rw-r--r--   0        0        0    45180 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/scintillacon.py
--rw-r--r--   0        0        0    28013 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/spokenforms.py
--rw-r--r--   0        0        0     2441 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/testDialogForDictationGrammar.py
--rw-r--r--   0        0        0    10796 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/ActionsTest.py
--rw-r--r--   0        0        0     1223 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/BasicTest.py
--rw-r--r--   0        0        0     9081 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/BringupTest.py
--rw-r--r--   0        0        0     5414 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/ClipboardTest.py
--rw-r--r--   0        0        0     4520 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/MessageTest.py
--rw-r--r--   0        0        0      185 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/README.txt
--rw-r--r--   0        0        0     4119 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/SearchTest.py
--rw-r--r--   0        0        0    23554 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/TestCaseWithHelpers.py
--rw-r--r--   0        0        0     7513 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/UnimacroTestHelpers.py
--rw-r--r--   0        0        0     2659 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/UtilsTest.py
--rw-r--r--   0        0        0     5512 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/_Unimacro_regression.vcl
--rw-r--r--   0        0        0      356 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/print_hotspot.py
--rw-r--r--   0        0        0    42237 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_clipboardfiles/natlink.docx
--rw-r--r--   0        0        0    11804 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_clipboardfiles/testempty.docx
--rw-r--r--   0        0        0        0 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_clipboardfiles/testempty.txt
--rw-r--r--   0        0        0    17000 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_clipboardfiles/testlarge.txt
--rw-r--r--   0        0        0    11987 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_clipboardfiles/testsmall.docx
--rw-r--r--   0        0        0       34 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_clipboardfiles/testsmall.txt
--rw-r--r--   0        0        0     2105 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_inifiles/othertest_spokenforms.ini
--rw-r--r--   0        0        0     2095 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_inifiles/test_spokenforms.ini
--rw-r--r--   0        0        0      277 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_inifiles/testinifilehandling.ini
--rw-r--r--   0        0        0      362 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_inifiles/testreloadtranslated.ini
--rw-r--r--   0        0        0      358 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_inifiles/testruledoubleword.ini
--rw-r--r--   0        0        0       84 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_inifiles/testrulefour.ini
--rw-r--r--   0        0        0      414 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/test_inifiles/testruleonetwo.ini
--rw-r--r--   0        0        0      982 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/udostringconvention.py
--rw-r--r--   0        0        0     7865 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestActions.py
--rw-r--r--   0        0        0    25615 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestClipboard.py
--rw-r--r--   0        0        0    17467 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestDocstringGrammar.py
--rw-r--r--   0        0        0     4357 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestFolders.py
--rw-r--r--   0        0        0    45563 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestIniGrammar.py
--rw-r--r--   0        0        0    20694 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestLilypond.py
--rw-r--r--   0        0        0    32270 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestMessagefunctions.py
--rw-r--r--   0        0        0    26241 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestMonitorfunctions.py
--rw-r--r--   0        0        0    10216 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestMouse.py
--rw-r--r--   0        0        0     6562 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestNatlinkutilsqh.py
--rw-r--r--   0        0        0     8985 2024-03-15 14:44:12.057782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestNumbersConversion.py
--rw-r--r--   0        0        0     8015 2024-03-15 14:44:12.061782 unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestProfileKaiserDictation.py
--rw-r--r--   0        0        0    10575 2024-03-15 14:44:12.061782 unimacro-4.1.4.5/src/unimacro/unimacro_test/util.py
--rw-r--r--   0        0        0     1756 2024-03-15 14:44:12.061782 unimacro-4.1.4.5/src/unimacro/unimacro_tracing.py
--rw-r--r--   0        0        0     1536 2024-03-15 14:44:12.061782 unimacro-4.1.4.5/src/unimacro/unimacrofoldersremembertemplate.py
--rw-r--r--   0        0        0    15903 2024-03-15 14:44:12.061782 unimacro-4.1.4.5/src/unimacro/vocola_compatibility/Unimacro.vch
--rw-r--r--   0        0        0     6829 2024-03-15 14:44:12.061782 unimacro-4.1.4.5/src/unimacro/vocola_compatibility/_Unimacro_regression.vcl
--rw-r--r--   0        0        0     3276 2024-03-15 14:44:12.061782 unimacro-4.1.4.5/src/unimacro/windowinfo.py
--rw-r--r--   0        0        0     4482 2024-03-15 14:44:12.061782 unimacro-4.1.4.5/src/unimacro/windowparameters.py
--rw-r--r--   0        0        0    10950 2024-03-15 14:44:12.061782 unimacro-4.1.4.5/src/unimacro/xxxxxxxpythonwin_dict.py
--rw-r--r--   0        0        0      545 2024-03-15 14:44:12.061782 unimacro-4.1.4.5/src/unimacro/xxxxxxxunimacro_wxpythondialogs.py
--rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 unimacro-4.1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1512 2024-05-01 16:10:09.065824 unimacro-4.1.5/README.md
+-rw-r--r--   0        0        0     2042 2024-05-01 16:10:09.101824 unimacro-4.1.5/pyproject.toml
+-rw-r--r--   0        0        0    17719 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/BrowseGrammar.py
+-rw-r--r--   0        0        0    22395 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/BrowseGrammarApp.py
+-rw-r--r--   0        0        0     2345 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/D_.py
+-rw-r--r--   0        0        0     2615 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/D_train.py
+-rw-r--r--   0        0        0     8783 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/DialogServer.py
+-rw-r--r--   0        0        0    13226 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_calculator.py
+-rw-r--r--   0        0        0    24467 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_keystrokes.py
+-rw-r--r--   0        0        0     9731 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_latex.py
+-rw-r--r--   0        0        0    24857 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_number extended.py
+-rw-r--r--   0        0        0    21073 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_oops.py
+-rw-r--r--   0        0        0    34546 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_repeat.py
+-rw-r--r--   0        0        0     2626 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_testtrayicon.py
+-rw-r--r--   0        0        0     7251 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_unimacrotest.py
+-rw-r--r--   0        0        0     9163 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/excel.py
+-rw-r--r--   0        0        0    28498 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/frescobaldi.py
+-rw-r--r--   0        0        0    12529 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/solitaire.py
+-rw-r--r--   0        0        0     1669 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/winword_variable.py
+-rw-r--r--   0        0        0     3557 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/xxxxnatspeak_dialog.py
+-rw-r--r--   0        0        0    15156 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/TrainDialog.py
+-rw-r--r--   0        0        0      713 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/README.txt
+-rw-r--r--   0        0        0       38 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/__init__.py
+-rw-r--r--   0        0        0     7976 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/_brackets.py
+-rw-r--r--   0        0        0    12892 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/_clickbyvoice.py
+-rw-r--r--   0        0        0     2780 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/_debug_natlink.py.txt
+-rw-r--r--   0        0        0     1716 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/_debug_unimacro.py.txt
+-rw-r--r--   0        0        0     8325 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/_folders fillinstancevariables.txt
+-rw-r--r--   0        0        0   101894 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/_folders.py
+-rw-r--r--   0        0        0    41422 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/_general.py
+-rw-r--r--   0        0        0    34074 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/_lines.py
+-rw-r--r--   0        0        0     4506 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/_number simple.py
+-rw-r--r--   0        0        0     5503 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/_tags.py
+-rw-r--r--   0        0        0    46227 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/_tasks.py
+-rw-r--r--   0        0        0      865 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/UnimacroGrammars/settings folders grammar.txt
+-rw-r--r--   0        0        0      849 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/__init__.py
+-rw-r--r--   0        0        0    30609 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/_control.py
+-rw-r--r--   0        0        0     6540 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/check_unimacro_grammars.py
+-rw-r--r--   0        0        0      766 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/defaulticons/idi_down.ico
+-rw-r--r--   0        0        0      766 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/defaulticons/idi_down2.ico
+-rw-r--r--   0        0        0      766 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/defaulticons/idi_left.ico
+-rw-r--r--   0        0        0      766 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/defaulticons/idi_left2.ico
+-rw-r--r--   0        0        0      766 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/defaulticons/idi_nodir.ico
+-rw-r--r--   0        0        0      766 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/defaulticons/idi_right.ico
+-rw-r--r--   0        0        0      766 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/defaulticons/idi_right2.ico
+-rw-r--r--   0        0        0      766 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/defaulticons/idi_up.ico
+-rw-r--r--   0        0        0      766 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/defaulticons/idi_up2.ico
+-rw-r--r--   0        0        0     2602 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/dos83.py
+-rw-r--r--   0        0        0    15036 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/enabledictation/_enabledictation.py
+-rw-r--r--   0        0        0       90 2024-05-01 16:10:09.105825 unimacro-4.1.5/src/unimacro/foldersrememberdialog.py
+-rw-r--r--   0        0        0    50189 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/iban.py
+-rw-r--r--   0        0        0      894 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/icons/repeat.ico
+-rw-r--r--   0        0        0      894 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/icons/repeat2.ico
+-rw-r--r--   0        0        0      894 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/icons/waiting.ico
+-rw-r--r--   0        0        0      894 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/icons/waiting2.ico
+-rw-r--r--   0        0        0    13406 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/listdialogs.py
+-rw-r--r--   0        0        0    11172 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/lynote.py
+-rw-r--r--   0        0        0     9892 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/namelist.py
+-rw-r--r--   0        0        0   132567 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/natlinkutilsbj.py
+-rw-r--r--   0        0        0     2567 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/nld_spokenforms.ini
+-rw-r--r--   0        0        0      196 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ahk/getintoforeground.ahk
+-rw-r--r--   0        0        0       47 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ahk/showmessageswindow.ahk
+-rw-r--r--   0        0        0    17742 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/_control.py
+-rw-r--r--   0        0        0    48047 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/_dictationproject.py
+-rw-r--r--   0        0        0    49150 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/_global_dictation.py
+-rw-r--r--   0        0        0     9009 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/actions.ini
+-rw-r--r--   0        0        0      245 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/config_scripts/disable_natlink.bat
+-rw-r--r--   0        0        0      518 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_kaiser.bat
+-rw-r--r--   0        0        0      606 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_kaiser_qh.bat
+-rw-r--r--   0        0        0      517 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_qh.bat
+-rw-r--r--   0        0        0     1384 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/enx_inifiles/Template List.txt
+-rw-r--r--   0        0        0      599 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/enx_inifiles/_control.ini
+-rw-r--r--   0        0        0     2536 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/enx_inifiles/_global_dictation.ini
+-rw-r--r--   0        0        0     9009 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/enx_inifiles/actions.ini
+-rw-r--r--   0        0        0      599 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/nld_inifiles/_control.ini
+-rw-r--r--   0        0        0     2575 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/nld_inifiles/_global_dictation.ini
+-rw-r--r--   0        0        0     1900 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_global_dictation/starting messages.txt
+-rw-r--r--   0        0        0    12521 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/actions.ini
+-rw-r--r--   0        0        0      440 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/deu_inifiles/_control.ini
+-rw-r--r--   0        0        0     2379 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/deu_spokenforms.ini
+-rw-r--r--   0        0        0      212 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_browser.ini
+-rw-r--r--   0        0        0     2165 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_commands.ini
+-rw-r--r--   0        0        0      380 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_control.ini
+-rw-r--r--   0        0        0      208 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_documentation.ini
+-rw-r--r--   0        0        0      426 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_editcomments.ini
+-rw-r--r--   0        0        0      142 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_first_sample_docstring.ini
+-rw-r--r--   0        0        0       86 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_gramoff.ini
+-rw-r--r--   0        0        0       58 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_gramon.ini
+-rw-r--r--   0        0        0     2461 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_keystrokes.ini
+-rw-r--r--   0        0        0     2128 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_latex.ini
+-rw-r--r--   0        0        0      586 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_modes.ini
+-rw-r--r--   0        0        0      260 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_number.ini
+-rw-r--r--   0        0        0      234 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_oops.ini
+-rw-r--r--   0        0        0      885 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_repeat.ini
+-rw-r--r--   0        0        0      174 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_second_sample_docstring.ini
+-rw-r--r--   0        0        0      412 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_shownumbersplus.ini
+-rw-r--r--   0        0        0      403 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_tags.ini
+-rw-r--r--   0        0        0      179 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_unimacrosample_docstring.ini
+-rw-r--r--   0        0        0      122 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_unimacrotest.ini
+-rw-r--r--   0        0        0      726 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/chrome_browsing.ini
+-rw-r--r--   0        0        0      538 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/firefox_browsing.ini
+-rw-r--r--   0        0        0      130 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/natspeak_dialog.ini
+-rw-r--r--   0        0        0      284 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/sol.ini
+-rw-r--r--   0        0        0      284 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/solitaire.ini
+-rw-r--r--   0        0        0      147 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/winword_styles_unimacro.ini
+-rw-r--r--   0        0        0     2454 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/enx_spokenforms.ini
+-rw-r--r--   0        0        0      430 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_control.ini
+-rw-r--r--   0        0        0     2224 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_folders.ini
+-rw-r--r--   0        0        0     1323 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_general.ini
+-rw-r--r--   0        0        0     2096 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_keystrokes.ini
+-rw-r--r--   0        0        0     1309 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_lines.ini
+-rw-r--r--   0        0        0     1415 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_repeat.ini
+-rw-r--r--   0        0        0     1779 2024-05-01 16:10:09.109825 unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_tasks.ini
+-rw-r--r--   0        0        0     1110 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/firefox_browsing.ini
+-rw-r--r--   0        0        0     2527 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/esp_spokenforms.ini
+-rw-r--r--   0        0        0     2592 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/ita_spokenforms.ini
+-rw-r--r--   0        0        0      350 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_brackets.ini
+-rw-r--r--   0        0        0      240 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_browser.ini
+-rw-r--r--   0        0        0      671 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_clickbyvoice.ini
+-rw-r--r--   0        0        0     3918 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_commands.ini
+-rw-r--r--   0        0        0      449 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_control.ini
+-rw-r--r--   0        0        0      215 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_documentation.ini
+-rw-r--r--   0        0        0      487 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_editcomments.ini
+-rw-r--r--   0        0        0      151 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_first_sample_docstring.ini
+-rw-r--r--   0        0        0     2018 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_folders.ini
+-rw-r--r--   0        0        0     1218 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_general.ini
+-rw-r--r--   0        0        0     2052 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_keystrokes.ini
+-rw-r--r--   0        0        0      846 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_latex.ini
+-rw-r--r--   0        0        0     1132 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_lines.ini
+-rw-r--r--   0        0        0      633 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_modes.ini
+-rw-r--r--   0        0        0      359 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_number extended.ini
+-rw-r--r--   0        0        0      336 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_number simple.ini
+-rw-r--r--   0        0        0      229 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_number.ini
+-rw-r--r--   0        0        0      246 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_oops.ini
+-rw-r--r--   0        0        0      955 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_repeat.ini
+-rw-r--r--   0        0        0      181 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_second_sample_docstring.ini
+-rw-r--r--   0        0        0      445 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_shownumbersplus.ini
+-rw-r--r--   0        0        0      422 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_tags.ini
+-rw-r--r--   0        0        0     2563 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_tasks.ini
+-rw-r--r--   0        0        0      207 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_unimacrotest.ini
+-rw-r--r--   0        0        0      208 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_unittest.ini
+-rw-r--r--   0        0        0      851 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/chrome_browsing.ini
+-rw-r--r--   0        0        0     1085 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/excel.ini
+-rw-r--r--   0        0        0      684 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/firefox_browsing.ini
+-rw-r--r--   0        0        0      148 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/natspeak_dialog.ini
+-rw-r--r--   0        0        0      165 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/natspeak_sample_docstring.ini
+-rw-r--r--   0        0        0      314 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/sol.ini
+-rw-r--r--   0        0        0      314 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/solitaire.ini
+-rw-r--r--   0        0        0      178 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/winword_styles_unimacro.ini
+-rw-r--r--   0        0        0     2567 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/nld_spokenforms.ini
+-rw-r--r--   0        0        0      333 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/othertest_spokenforms.ini
+-rw-r--r--   0        0        0     3818 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/spokenforms - kopie.ini
+-rw-r--r--   0        0        0     3818 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/spokenforms.ini
+-rw-r--r--   0        0        0     2089 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/sample_ini/test_spokenforms.ini
+-rw-r--r--   0        0        0    45180 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/scintillacon.py
+-rw-r--r--   0        0        0    28013 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/spokenforms.py
+-rw-r--r--   0        0        0     2441 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/testDialogForDictationGrammar.py
+-rw-r--r--   0        0        0    10796 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/ActionsTest.py
+-rw-r--r--   0        0        0     1223 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/BasicTest.py
+-rw-r--r--   0        0        0     9081 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/BringupTest.py
+-rw-r--r--   0        0        0     5414 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/ClipboardTest.py
+-rw-r--r--   0        0        0     4520 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/MessageTest.py
+-rw-r--r--   0        0        0      185 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/README.txt
+-rw-r--r--   0        0        0     4119 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/SearchTest.py
+-rw-r--r--   0        0        0    23554 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/TestCaseWithHelpers.py
+-rw-r--r--   0        0        0     7513 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/UnimacroTestHelpers.py
+-rw-r--r--   0        0        0     2659 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/UtilsTest.py
+-rw-r--r--   0        0        0     5512 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/_Unimacro_regression.vcl
+-rw-r--r--   0        0        0      356 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/print_hotspot.py
+-rw-r--r--   0        0        0    42237 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_clipboardfiles/natlink.docx
+-rw-r--r--   0        0        0    11804 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_clipboardfiles/testempty.docx
+-rw-r--r--   0        0        0        0 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_clipboardfiles/testempty.txt
+-rw-r--r--   0        0        0    17000 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_clipboardfiles/testlarge.txt
+-rw-r--r--   0        0        0    11987 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_clipboardfiles/testsmall.docx
+-rw-r--r--   0        0        0       34 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_clipboardfiles/testsmall.txt
+-rw-r--r--   0        0        0     2105 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_inifiles/othertest_spokenforms.ini
+-rw-r--r--   0        0        0     2095 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_inifiles/test_spokenforms.ini
+-rw-r--r--   0        0        0      277 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_inifiles/testinifilehandling.ini
+-rw-r--r--   0        0        0      362 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_inifiles/testreloadtranslated.ini
+-rw-r--r--   0        0        0      358 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_inifiles/testruledoubleword.ini
+-rw-r--r--   0        0        0       84 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_inifiles/testrulefour.ini
+-rw-r--r--   0        0        0      414 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/test_inifiles/testruleonetwo.ini
+-rw-r--r--   0        0        0      982 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/udostringconvention.py
+-rw-r--r--   0        0        0     7865 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestActions.py
+-rw-r--r--   0        0        0    25615 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestClipboard.py
+-rw-r--r--   0        0        0    17467 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestDocstringGrammar.py
+-rw-r--r--   0        0        0     4357 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestFolders.py
+-rw-r--r--   0        0        0    45563 2024-05-01 16:10:09.113825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestIniGrammar.py
+-rw-r--r--   0        0        0    20694 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestLilypond.py
+-rw-r--r--   0        0        0    32270 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestMessagefunctions.py
+-rw-r--r--   0        0        0    26241 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestMonitorfunctions.py
+-rw-r--r--   0        0        0    10216 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestMouse.py
+-rw-r--r--   0        0        0     6562 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestNatlinkutilsqh.py
+-rw-r--r--   0        0        0     8985 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestNumbersConversion.py
+-rw-r--r--   0        0        0     8015 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/unimacro_test/unittestProfileKaiserDictation.py
+-rw-r--r--   0        0        0    10575 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/unimacro_test/util.py
+-rw-r--r--   0        0        0     1756 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/unimacro_tracing.py
+-rw-r--r--   0        0        0     1536 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/unimacrofoldersremembertemplate.py
+-rw-r--r--   0        0        0    15903 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/vocola_compatibility/Unimacro.vch
+-rw-r--r--   0        0        0     6829 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/vocola_compatibility/_Unimacro_regression.vcl
+-rw-r--r--   0        0        0     3276 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/windowinfo.py
+-rw-r--r--   0        0        0     4482 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/windowparameters.py
+-rw-r--r--   0        0        0    10950 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/xxxxxxxpythonwin_dict.py
+-rw-r--r--   0        0        0      545 2024-05-01 16:10:09.117825 unimacro-4.1.5/src/unimacro/xxxxxxxunimacro_wxpythondialogs.py
+-rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 unimacro-4.1.5/PKG-INFO
```

### Comparing `unimacro-4.1.4.5/README.md` & `unimacro-4.1.5/README.md`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/pyproject.toml` & `unimacro-4.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/BrowseGrammar.py` & `unimacro-4.1.5/src/unimacro/BrowseGrammar.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/BrowseGrammarApp.py` & `unimacro-4.1.5/src/unimacro/BrowseGrammarApp.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/D_.py` & `unimacro-4.1.5/src/unimacro/D_.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/D_train.py` & `unimacro-4.1.5/src/unimacro/D_train.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/DialogServer.py` & `unimacro-4.1.5/src/unimacro/DialogServer.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_calculator.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_calculator.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_keystrokes.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_keystrokes.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_latex.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_latex.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_number extended.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_number extended.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_oops.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_oops.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_repeat.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_repeat.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_testtrayicon.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_testtrayicon.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/_unimacrotest.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/_unimacrotest.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/excel.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/excel.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/frescobaldi.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/frescobaldi.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/solitaire.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/solitaire.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/winword_variable.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/winword_variable.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/OtherUnimacroGrammars/xxxxnatspeak_dialog.py` & `unimacro-4.1.5/src/unimacro/OtherUnimacroGrammars/xxxxnatspeak_dialog.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/TrainDialog.py` & `unimacro-4.1.5/src/unimacro/TrainDialog.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/README.txt` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/README.txt`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_brackets.py` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/_brackets.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_clickbyvoice.py` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/_clickbyvoice.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_debug_natlink.py.txt` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/_debug_natlink.py.txt`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_debug_unimacro.py.txt` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/_debug_unimacro.py.txt`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_folders fillinstancevariables.txt` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/_folders fillinstancevariables.txt`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_folders.py` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/_folders.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 from dtactions.unimacro import unimacroutils
 # from dtactions.unimacro.unimacroactions import Message
 # from dtactions.unimacro import unimacroactions as actions
 import unimacro.natlinkutilsbj as natbj
 # from unimacro.unimacro_wxpythondialogs import InputBox
 # import natlinkcore.natlinkutils as natut
 
+# manipulating file names with env variables etc...
+envvars = extenvvars.ExtEnvVars()
+
 thisDir = str(Path(__file__).parent)
 status = natlinkstatus.NatlinkStatus()
 # for getting unicode explorer window titles:
 GetWindowText = ctypes.windll.user32.GetWindowTextW
 GetWindowTextLength = ctypes.windll.user32.GetWindowTextLengthW
 
 # for substituting environment variable like %HOME% in a file path:
@@ -156,28 +159,28 @@
 <thiswebsite> exported = (this website) (<websitecommands>|<remember>);
 <websitecommands> = ('open with') {websiteopenprograms}|
                     <namepathcopy>;
 <remember> = remember;  
 <namepathcopy> = (copy (name|path)) | ((name|path) copy);
 
 """
-
     def initialize(self):
         # self.envDict = natlinkcorefunctions.getAllFolderEnvironmentVariables()   # for (generalised) environment variables
         self.subfiles = self.subfiles = self.activeFolder = self.activeTimerFolder = None  # for catching on the fly in explorer windows (CabinetClassW)
         self.className = None
         self.dialogWindowTitle = "" # for recent folders dialog, grammar in natspeak.py
         self.dialogNumberRange = [] # ditto
         self.catchRemember = ""
         self.inTimerRecentFolders = False
-        self.prevDisplayRecentFolders = None   # displaying recent folders list
         self.prevActiveFolder = None
         self.subfoldersDict = {}
         self.subfilesDict = {}
         self.foldersSet = set()
+
+
         if not self.language:
             self.error("no valid language in grammar "+__name__+" grammar not initialized")
             return
         self.load(self.gramSpec)
         self.switchOnOrOff() # initialises lists from inifile, and switches on
         
     def loggerName(self) ->str:
@@ -543,15 +546,15 @@
 
 
     def getFolderFromVirtualDrive(self, vd):
         """check validity of virtual drive contents
         also make alternative paths possible  like (C|D):/Documents
         """
         # natlinkcorefunctions.printAllEnvVariables()
-        vd = extenvvars.expandEnvVariables(vd)
+        vd = envvars.expandEnvVariables(vd)
         for possiblePath in loop_through_alternative_paths(vd):
             folder = self.substituteFolder(possiblePath)
             if os.path.isdir(folder):
                 return os.path.normpath(folder)
         return None 
 
     def acceptVirtualDrivesFolder(self, vd, realfolder, foldername=None):
@@ -620,16 +623,16 @@
             return None
         if os.path.isdir(f):
             nf = os.path.normpath(f)
             if nf != self.prevActiveFolder:
                 self.debug("getActiveFolder, got: %s",nf)
                 self.prevActiveFolder = nf
             return nf
-        result = extenvvars.getFolderFromLibraryName(f)
-        if result and os.path.isdir(f):
+        result = envvars.getFolderFromLibraryName(f)
+        if result and os.path.isdir(result):
             self.debug("getActiveFolder, via getFolderFromLibraryName %s: %s", f, result)
             return os.path.normpath(result)
         self.warning('getActiveFolder, strange invalid path for folder: %s', f)
         return None
     
     def fillListsForActiveFolder(self, activeFolder):
         """fill list of files and subfolders
@@ -870,26 +873,21 @@
   
     def displayRecentFolders(self):
         """display the list of recent folders
         """
         mess_list = ["--- recent folders:"]
         if not self.recentfoldersDict:
             message = 'recent folders list is empty at the moment'
-            self.prevDisplayRecentFolders = message
             self.info(message)
             return
         for name, value in reversed(self.recentfoldersDict.items()):
             mess_list.append('- %s: %s'% (name, value))
         mess_list.append('-'*20)
         message = '\n'.join(mess_list)  
-        if message == self.prevDisplayRecentFolders:
-            self.info("recent folders, no change")
-        else:
-            self.prevDisplayRecentFolders = message
-            Message(message)
+        Message(message)
         
         
     # def gotoRecentFolder(self, chooseNum):
     #     """service function which can be called fr_RECNTom natspeak_dialog
     #     pass the number of the choicelist (0 based)
     #     """
     #     wantedFolder = self.recentfoldersList[chooseNum]
@@ -1256,17 +1254,17 @@
         text = '\n\n'.join(texts)
         if not self.checkForChanges:
             self.checkForChanges = 10  # switch this on 10 utterances
         pausetime = 3
         # reset variables, no action in gotResults:
         self.wantedFile = self.wantedFolder = self.wantedWebsite = ""
         self.info(f'thisDir: {thisDir}')
-        UnimacroDirectory = extenvvars.expandEnvVariableAtStart('%Unimacro%')
+        UnimacroDirectory = envvars.expandEnvVariableAtStart('%Unimacro%')
         self.info(f'UnimacroDirectory: {UnimacroDirectory}')
-        UnimacroGrammarsDirectory = extenvvars.expandEnvVariableAtStart('%UnimacroGrammars%')
+        UnimacroGrammarsDirectory = envvars.expandEnvVariableAtStart('%UnimacroGrammars%')
         self.info(f'UnimacroGrammarsDirectory: {UnimacroGrammarsDirectory}')
         makeFromTemplateAndExecute(UnimacroDirectory, "unimacrofoldersremembertemplate.py", UnimacroGrammarsDirectory, "rememberdialog.py",
                                       prompt, text, default, inifile, section, value, pausetime=pausetime)
 
 
     def get_active_explorer(self, hndle=None):
         """give only handle when debugging with unittestFolder
@@ -1625,15 +1623,15 @@
         """honor environment variables like %HOME%, %PROGRAMFILES%
 
         %HOME% is also recognised by ~ (at front of name)
         
         With expandEnvVars, also NATLINK and related variables can be handled.
         NATLINKDIRECTORY, COREDIRECTORY etc.
         """
-        substitute = extenvvars.expandEnvVariables(folder)
+        substitute = envvars.expandEnvVariables(folder)
         return substitute
 
     def substituteFilename(self, filename):
         """substitute virtual drive into for  into filename,and possibly the spoken form
 
         If a virtual drive is not in folder name, simply
         the name is returned, otherwise the contents of
@@ -2443,18 +2441,23 @@
 if __name__ == "__main__":
     ## interactive use, for debugging:
     with natlink.natConnect():
         try:
             thisGrammar = ThisGrammar(inifile_stem="_folders")
             # thisGrammar.startInifile()
             thisGrammar.initialize()
+            # print(thisGrammar.envvars)
+            # get hndle of a explore window (via _general "give window info") and try interactive
+            # thisGrammar.catchTimerRecentFolders(132524, "CabinetWClass")
+            active_folder = thisGrammar.getActiveFolder(198434)
+            print(f'active_folder: {active_folder}')
 
             # get hndle of a explore window (via _general "give window info") and try interactive
             # thisGrammar.catchTimerRecentFolders(132524, "CabinetWClass")
-            thisGrammar.getActiveFolder(67062)
+            thisGrammar.getActiveFol>>> master
             thisGrammar.displayRecentFolders()
 
             # # Words = ['folder', 'dtactions']
             # Fr = {}
             # Words = ['subfolder', 'hello']
             # thisGrammar.gotResultsInit(Words, Fr)
             # thisGrammar.gotResults_subfolder(Words, Fr)
```

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_general.py` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/_general.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_lines.py` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/_lines.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_number simple.py` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/_number simple.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_tags.py` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/_tags.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/_tasks.py` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/_tasks.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/UnimacroGrammars/settings folders grammar.txt` & `unimacro-4.1.5/src/unimacro/UnimacroGrammars/settings folders grammar.txt`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/__init__.py` & `unimacro-4.1.5/src/unimacro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 
 def control_logger_name() -> str : 
         return "natlink.unimacro.control"
 
 def logname() -> str:
     """ Returns the name of the unimacro logger."""
     return "natlink.unimacro"
-__version__ = '4.1.4.5'   
+__version__ = '4.1.5'
```

### Comparing `unimacro-4.1.4.5/src/unimacro/_control.py` & `unimacro-4.1.5/src/unimacro/_control.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/check_unimacro_grammars.py` & `unimacro-4.1.5/src/unimacro/check_unimacro_grammars.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/defaulticons/idi_down.ico` & `unimacro-4.1.5/src/unimacro/defaulticons/idi_down.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/defaulticons/idi_down2.ico` & `unimacro-4.1.5/src/unimacro/defaulticons/idi_down2.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/defaulticons/idi_left.ico` & `unimacro-4.1.5/src/unimacro/defaulticons/idi_left.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/defaulticons/idi_left2.ico` & `unimacro-4.1.5/src/unimacro/defaulticons/idi_left2.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/defaulticons/idi_nodir.ico` & `unimacro-4.1.5/src/unimacro/defaulticons/idi_nodir.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/defaulticons/idi_right.ico` & `unimacro-4.1.5/src/unimacro/defaulticons/idi_right.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/defaulticons/idi_right2.ico` & `unimacro-4.1.5/src/unimacro/defaulticons/idi_right2.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/defaulticons/idi_up.ico` & `unimacro-4.1.5/src/unimacro/defaulticons/idi_up.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/defaulticons/idi_up2.ico` & `unimacro-4.1.5/src/unimacro/defaulticons/idi_up2.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/dos83.py` & `unimacro-4.1.5/src/unimacro/dos83.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/enabledictation/_enabledictation.py` & `unimacro-4.1.5/src/unimacro/enabledictation/_enabledictation.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/iban.py` & `unimacro-4.1.5/src/unimacro/iban.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/icons/repeat.ico` & `unimacro-4.1.5/src/unimacro/icons/repeat.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/icons/repeat2.ico` & `unimacro-4.1.5/src/unimacro/icons/repeat2.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/icons/waiting.ico` & `unimacro-4.1.5/src/unimacro/icons/waiting.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/icons/waiting2.ico` & `unimacro-4.1.5/src/unimacro/icons/waiting2.ico`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/listdialogs.py` & `unimacro-4.1.5/src/unimacro/listdialogs.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/lynote.py` & `unimacro-4.1.5/src/unimacro/lynote.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/namelist.py` & `unimacro-4.1.5/src/unimacro/namelist.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/natlinkutilsbj.py` & `unimacro-4.1.5/src/unimacro/natlinkutilsbj.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/nld_spokenforms.ini` & `unimacro-4.1.5/src/unimacro/nld_spokenforms.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/_control.py` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/_control.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/_dictationproject.py` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/_dictationproject.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/_global_dictation.py` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/_global_dictation.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/actions.ini` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/actions.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_kaiser.bat` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_kaiser.bat`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_kaiser_qh.bat` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_kaiser_qh.bat`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_qh.bat` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/config_scripts/enable_natlink_qh.bat`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/enx_inifiles/Template List.txt` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/enx_inifiles/Template List.txt`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/enx_inifiles/_control.ini` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/enx_inifiles/_control.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/enx_inifiles/_global_dictation.ini` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/enx_inifiles/_global_dictation.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/enx_inifiles/actions.ini` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/enx_inifiles/actions.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/nld_inifiles/_control.ini` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/nld_inifiles/_control.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/nld_inifiles/_global_dictation.ini` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/nld_inifiles/_global_dictation.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_global_dictation/starting messages.txt` & `unimacro-4.1.5/src/unimacro/sample_global_dictation/starting messages.txt`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/actions.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/actions.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/deu_spokenforms.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/deu_spokenforms.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_commands.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_commands.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_keystrokes.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_keystrokes.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_latex.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_latex.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_modes.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_modes.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/_repeat.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/_repeat.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/chrome_browsing.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/chrome_browsing.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/enx_inifiles/firefox_browsing.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/enx_inifiles/firefox_browsing.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/enx_spokenforms.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/enx_spokenforms.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_folders.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_folders.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_general.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_general.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_keystrokes.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_keystrokes.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_lines.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_lines.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_repeat.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_repeat.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/_tasks.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/_tasks.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/esp_inifiles/firefox_browsing.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/esp_inifiles/firefox_browsing.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/esp_spokenforms.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/esp_spokenforms.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/ita_spokenforms.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/ita_spokenforms.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_clickbyvoice.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_clickbyvoice.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_commands.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_commands.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_folders.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_folders.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_general.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_general.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_keystrokes.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_keystrokes.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_latex.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_latex.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_lines.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_lines.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_modes.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_modes.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_repeat.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_repeat.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/_tasks.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/_tasks.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/chrome_browsing.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/chrome_browsing.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/excel.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/excel.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_inifiles/firefox_browsing.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_inifiles/firefox_browsing.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/nld_spokenforms.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/nld_spokenforms.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/spokenforms - kopie.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/spokenforms - kopie.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/spokenforms.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/spokenforms.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/sample_ini/test_spokenforms.ini` & `unimacro-4.1.5/src/unimacro/sample_ini/test_spokenforms.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/scintillacon.py` & `unimacro-4.1.5/src/unimacro/scintillacon.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/spokenforms.py` & `unimacro-4.1.5/src/unimacro/spokenforms.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/testDialogForDictationGrammar.py` & `unimacro-4.1.5/src/unimacro/testDialogForDictationGrammar.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/ActionsTest.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/ActionsTest.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/BasicTest.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/BasicTest.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/BringupTest.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/BringupTest.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/ClipboardTest.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/ClipboardTest.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/MessageTest.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/MessageTest.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/SearchTest.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/SearchTest.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/TestCaseWithHelpers.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/TestCaseWithHelpers.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/UnimacroTestHelpers.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/UnimacroTestHelpers.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/UtilsTest.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/UtilsTest.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/_Unimacro_regression.vcl` & `unimacro-4.1.5/src/unimacro/unimacro_test/_Unimacro_regression.vcl`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/test_clipboardfiles/natlink.docx` & `unimacro-4.1.5/src/unimacro/unimacro_test/test_clipboardfiles/natlink.docx`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/test_clipboardfiles/testempty.docx` & `unimacro-4.1.5/src/unimacro/unimacro_test/test_clipboardfiles/testempty.docx`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/test_clipboardfiles/testsmall.docx` & `unimacro-4.1.5/src/unimacro/unimacro_test/test_clipboardfiles/testsmall.docx`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/test_inifiles/othertest_spokenforms.ini` & `unimacro-4.1.5/src/unimacro/unimacro_test/test_inifiles/othertest_spokenforms.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/test_inifiles/test_spokenforms.ini` & `unimacro-4.1.5/src/unimacro/unimacro_test/test_inifiles/test_spokenforms.ini`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/udostringconvention.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/udostringconvention.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestActions.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestActions.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestClipboard.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestClipboard.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestDocstringGrammar.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestDocstringGrammar.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestFolders.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestFolders.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestIniGrammar.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestIniGrammar.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestLilypond.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestLilypond.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestMessagefunctions.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestMessagefunctions.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestMonitorfunctions.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestMonitorfunctions.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestMouse.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestMouse.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestNatlinkutilsqh.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestNatlinkutilsqh.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestNumbersConversion.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestNumbersConversion.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/unittestProfileKaiserDictation.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/unittestProfileKaiserDictation.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_test/util.py` & `unimacro-4.1.5/src/unimacro/unimacro_test/util.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacro_tracing.py` & `unimacro-4.1.5/src/unimacro/unimacro_tracing.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/unimacrofoldersremembertemplate.py` & `unimacro-4.1.5/src/unimacro/unimacrofoldersremembertemplate.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/vocola_compatibility/Unimacro.vch` & `unimacro-4.1.5/src/unimacro/vocola_compatibility/Unimacro.vch`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/vocola_compatibility/_Unimacro_regression.vcl` & `unimacro-4.1.5/src/unimacro/vocola_compatibility/_Unimacro_regression.vcl`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/windowinfo.py` & `unimacro-4.1.5/src/unimacro/windowinfo.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/windowparameters.py` & `unimacro-4.1.5/src/unimacro/windowparameters.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/xxxxxxxpythonwin_dict.py` & `unimacro-4.1.5/src/unimacro/xxxxxxxpythonwin_dict.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/src/unimacro/xxxxxxxunimacro_wxpythondialogs.py` & `unimacro-4.1.5/src/unimacro/xxxxxxxunimacro_wxpythondialogs.py`

 * *Files identical despite different names*

### Comparing `unimacro-4.1.4.5/PKG-INFO` & `unimacro-4.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimacro
-Version: 4.1.4.5
+Version: 4.1.5
 Summary: Unimacro __init__
 Author-email: "Quintijn Hoogenboom (maintainer)" <q.hoogenboom@antenna.nl>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
```

