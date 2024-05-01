# Comparing `tmp/rofimoji-6.2.0.tar.gz` & `tmp/rofimoji-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rofimoji-6.2.0.tar", max compression
+gzip compressed data, was "rofimoji-6.3.0.tar", max compression
```

## Comparing `rofimoji-6.2.0.tar` & `rofimoji-6.3.0.tar`

### file list

```diff
@@ -1,357 +1,373 @@
--rw-r--r--   0        0        0     1075 2023-09-16 08:10:06.869313 rofimoji-6.2.0/LICENSE
--rw-r--r--   0        0        0    18918 2023-06-10 08:38:34.113092 rofimoji-6.2.0/README.md
--rw-r--r--   0        0        0      893 2023-09-16 08:07:22.759622 rofimoji-6.2.0/pyproject.toml
--rw-r--r--   0        0        0       89 2022-12-29 11:56:19.212555 rofimoji-6.2.0/src/picker/__init__.py
--rw-r--r--   0        0        0      259 2022-11-13 10:52:07.457219 rofimoji-6.2.0/src/picker/__main__.py
--rw-r--r--   0        0        0      188 2022-11-13 10:52:07.457219 rofimoji-6.2.0/src/picker/abstractionhelper.py
--rw-r--r--   0        0        0     1221 2022-11-13 10:52:07.457219 rofimoji-6.2.0/src/picker/action.py
--rw-r--r--   0        0        0     5641 2023-05-16 15:30:20.608188 rofimoji-6.2.0/src/picker/argument_parsing.py
--rw-r--r--   0        0        0        0 2022-11-13 10:52:07.457219 rofimoji-6.2.0/src/picker/clipboarder/__init__.py
--rw-r--r--   0        0        0     4764 2022-11-13 10:52:07.457219 rofimoji-6.2.0/src/picker/clipboarder/clipboarder.py
--rw-r--r--   0        0        0      457 2022-11-13 10:52:07.460553 rofimoji-6.2.0/src/picker/contrib/grid.rasi
--rw-r--r--   0        0        0       23 2023-08-17 09:39:13.406636 rofimoji-6.2.0/src/picker/data/additional/emojis_smileys_emotion.csv
--rw-r--r--   0        0        0     2712 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/adlam.csv
--rw-r--r--   0        0        0     1737 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/aegean_numbers.csv
--rw-r--r--   0        0        0     1470 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/ahom.csv
--rw-r--r--   0        0        0     4551 2023-09-16 08:02:53.469953 rofimoji-6.2.0/src/picker/data/alchemical_symbols.csv
--rw-r--r--   0        0        0     2098 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/alphabetic_presentation_forms.csv
--rw-r--r--   0        0        0    18183 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/anatolian_hieroglyphs.csv
--rw-r--r--   0        0        0     2761 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/ancient_greek_musical_notation.csv
--rw-r--r--   0        0        0     2895 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/ancient_greek_numbers.csv
--rw-r--r--   0        0        0      344 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/ancient_symbols.csv
--rw-r--r--   0        0        0     8311 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/arabic.csv
--rw-r--r--   0        0        0     3561 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/arabic_extended-a.csv
--rw-r--r--   0        0        0     1906 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/arabic_extended-b.csv
--rw-r--r--   0        0        0       98 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/arabic_extended-c.csv
--rw-r--r--   0        0        0     5786 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/arabic_mathematical_alphabetic_symbols.csv
--rw-r--r--   0        0        0    32176 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/arabic_presentation_forms-a.csv
--rw-r--r--   0        0        0     5722 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/arabic_presentation_forms-b.csv
--rw-r--r--   0        0        0     2719 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/arabic_supplement.csv
--rw-r--r--   0        0        0     2715 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/armenian.csv
--rw-r--r--   0        0        0     3689 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/arrows.csv
--rw-r--r--   0        0        0     1729 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/avestan.csv
--rw-r--r--   0        0        0     3904 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/balinese.csv
--rw-r--r--   0        0        0     1870 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/bamum.csv
--rw-r--r--   0        0        0    18380 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/bamum_supplement.csv
--rw-r--r--   0        0        0     1876 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/basic_latin.csv
--rw-r--r--   0        0        0      968 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/bassa_vah.csv
--rw-r--r--   0        0        0     1419 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/batak.csv
--rw-r--r--   0        0        0     2451 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/bengali.csv
--rw-r--r--   0        0        0     2625 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/bhaiksuki.csv
--rw-r--r--   0        0        0      944 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/block_elements.csv
--rw-r--r--   0        0        0      981 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/bopomofo.csv
--rw-r--r--   0        0        0      774 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/bopomofo_extended.csv
--rw-r--r--   0        0        0     5625 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/box_drawing.csv
--rw-r--r--   0        0        0     2950 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/brahmi.csv
--rw-r--r--   0        0        0     7680 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/braille_patterns.csv
--rw-r--r--   0        0        0      716 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/buginese.csv
--rw-r--r--   0        0        0      404 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/buhid.csv
--rw-r--r--   0        0        0    11298 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/byzantine_musical_symbols.csv
--rw-r--r--   0        0        0     1078 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/carian.csv
--rw-r--r--   0        0        0     1885 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/caucasian_albanian.csv
--rw-r--r--   0        0        0     1675 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/chakma.csv
--rw-r--r--   0        0        0     1820 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/cham.csv
--rw-r--r--   0        0        0     2166 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/cherokee.csv
--rw-r--r--   0        0        0     2334 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/cherokee_supplement.csv
--rw-r--r--   0        0        0     4120 2023-09-16 08:02:53.469953 rofimoji-6.2.0/src/picker/data/chess_symbols.csv
--rw-r--r--   0        0        0      889 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/chorasmian.csv
--rw-r--r--   0        0        0   282678 2023-09-16 08:03:06.006610 rofimoji-6.2.0/src/picker/data/cjk_cantonese.csv
--rw-r--r--   0        0        0     6158 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/cjk_compatibility.csv
--rw-r--r--   0        0        0     1463 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/cjk_compatibility_forms.csv
--rw-r--r--   0        0        0    17464 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/cjk_compatibility_ideographs.csv
--rw-r--r--   0        0        0    21138 2023-09-16 08:02:53.469953 rofimoji-6.2.0/src/picker/data/cjk_compatibility_ideographs_supplement.csv
--rw-r--r--   0        0        0   164294 2023-09-16 08:03:06.049944 rofimoji-6.2.0/src/picker/data/cjk_japanese_kun.csv
--rw-r--r--   0        0        0   152011 2023-09-16 08:03:06.059944 rofimoji-6.2.0/src/picker/data/cjk_japanese_on.csv
--rw-r--r--   0        0        0    76750 2023-09-16 08:03:06.066610 rofimoji-6.2.0/src/picker/data/cjk_korean.csv
--rw-r--r--   0        0        0   390276 2023-09-16 08:03:06.033277 rofimoji-6.2.0/src/picker/data/cjk_mandarin.csv
--rw-r--r--   0        0        0     3072 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/cjk_radicals_supplement.csv
--rw-r--r--   0        0        0      714 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/cjk_strokes.csv
--rw-r--r--   0        0        0     1919 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/cjk_symbols_and_punctuation.csv
--rw-r--r--   0        0        0    43076 2023-09-16 08:03:06.043277 rofimoji-6.2.0/src/picker/data/cjk_tang.csv
--rw-r--r--   0        0        0    87736 2023-09-16 08:03:06.039944 rofimoji-6.2.0/src/picker/data/cjk_vietnamese.csv
--rw-r--r--   0        0        0     3356 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/combining_diacritical_marks.csv
--rw-r--r--   0        0        0     1141 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/combining_diacritical_marks_extended.csv
--rw-r--r--   0        0        0     1189 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/combining_diacritical_marks_for_symbols.csv
--rw-r--r--   0        0        0     2374 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/combining_diacritical_marks_supplement.csv
--rw-r--r--   0        0        0      581 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/combining_half_marks.csv
--rw-r--r--   0        0        0      347 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/common_indic_number_forms.csv
--rw-r--r--   0        0        0     1104 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/control_pictures.csv
--rw-r--r--   0        0        0     4234 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/coptic.csv
--rw-r--r--   0        0        0      919 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/coptic_epact_numbers.csv
--rw-r--r--   0        0        0      817 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/counting_rod_numerals.csv
--rw-r--r--   0        0        0    30373 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/cuneiform.csv
--rw-r--r--   0        0        0     5019 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/cuneiform_numbers_and_punctuation.csv
--rw-r--r--   0        0        0      556 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/currency_symbols.csv
--rw-r--r--   0        0        0     1535 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/cypriot_syllabary.csv
--rw-r--r--   0        0        0     2873 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/cypro-minoan.csv
--rw-r--r--   0        0        0     9424 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/cyrillic.csv
--rw-r--r--   0        0        0     1116 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/cyrillic_extended-a.csv
--rw-r--r--   0        0        0     3480 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/cyrillic_extended-b.csv
--rw-r--r--   0        0        0      338 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/cyrillic_extended-c.csv
--rw-r--r--   0        0        0     2654 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/cyrillic_extended-d.csv
--rw-r--r--   0        0        0     1746 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/cyrillic_supplement.csv
--rw-r--r--   0        0        0     2552 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/deseret.csv
--rw-r--r--   0        0        0     3580 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/devanagari.csv
--rw-r--r--   0        0        0      377 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/devanagari_extended-a.csv
--rw-r--r--   0        0        0     1089 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/devanagari_extended.csv
--rw-r--r--   0        0        0     6632 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/dingbats.csv
--rw-r--r--   0        0        0     2029 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/dives_akuru.csv
--rw-r--r--   0        0        0     1348 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/dogra.csv
--rw-r--r--   0        0        0     3298 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/domino_tiles.csv
--rw-r--r--   0        0        0     4069 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/duployan.csv
--rw-r--r--   0        0        0     7082 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/early_dynastic_cuneiform.csv
--rw-r--r--   0        0        0     1794 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/egyptian_hieroglyph_format_controls.csv
--rw-r--r--   0        0        0    32482 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/egyptian_hieroglyphs.csv
--rw-r--r--   0        0        0      930 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/elbasan.csv
--rw-r--r--   0        0        0      654 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/elymaic.csv
--rw-r--r--   0        0        0     5642 2023-09-16 07:58:11.613668 rofimoji-6.2.0/src/picker/data/emojis_activities.csv
--rw-r--r--   0        0        0     7330 2023-09-16 07:58:11.613668 rofimoji-6.2.0/src/picker/data/emojis_animals_nature.csv
--rw-r--r--   0        0        0      253 2023-09-16 07:58:11.613668 rofimoji-6.2.0/src/picker/data/emojis_component.csv
--rw-r--r--   0        0        0     7284 2023-09-16 07:58:11.613668 rofimoji-6.2.0/src/picker/data/emojis_flags.csv
--rw-r--r--   0        0        0     7931 2023-09-16 07:58:11.613668 rofimoji-6.2.0/src/picker/data/emojis_food_drink.csv
--rw-r--r--   0        0        0    16393 2023-09-16 07:58:11.613668 rofimoji-6.2.0/src/picker/data/emojis_objects.csv
--rw-r--r--   0        0        0    21230 2023-09-16 07:58:11.613668 rofimoji-6.2.0/src/picker/data/emojis_people_body.csv
--rw-r--r--   0        0        0    11962 2023-09-16 07:58:11.613668 rofimoji-6.2.0/src/picker/data/emojis_smileys_emotion.csv
--rw-r--r--   0        0        0    16126 2023-09-16 07:58:11.613668 rofimoji-6.2.0/src/picker/data/emojis_symbols.csv
--rw-r--r--   0        0        0    13690 2023-09-16 07:58:11.613668 rofimoji-6.2.0/src/picker/data/emojis_travel_places.csv
--rw-r--r--   0        0        0     2229 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/emoticons.csv
--rw-r--r--   0        0        0     7107 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/enclosed_alphanumeric_supplement.csv
--rw-r--r--   0        0        0     5169 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/enclosed_alphanumerics.csv
--rw-r--r--   0        0        0     7668 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/enclosed_cjk_letters_and_months.csv
--rw-r--r--   0        0        0     2570 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/enclosed_ideographic_supplement.csv
--rw-r--r--   0        0        0     9421 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/ethiopic.csv
--rw-r--r--   0        0        0      868 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/ethiopic_extended-a.csv
--rw-r--r--   0        0        0      903 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/ethiopic_extended-b.csv
--rw-r--r--   0        0        0     2095 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/ethiopic_extended.csv
--rw-r--r--   0        0        0      774 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/ethiopic_supplement.csv
--rw-r--r--   0        0        0    52276 2023-09-16 08:03:07.073276 rofimoji-6.2.0/src/picker/data/fontawesome6.csv
--rw-r--r--   0        0        0     2575 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/general_punctuation.csv
--rw-r--r--   0        0        0     3087 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/geometric_shapes.csv
--rw-r--r--   0        0        0     3236 2023-09-16 08:02:53.469953 rofimoji-6.2.0/src/picker/data/geometric_shapes_extended.csv
--rw-r--r--   0        0        0     2472 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/georgian.csv
--rw-r--r--   0        0        0     1908 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/georgian_extended.csv
--rw-r--r--   0        0        0     1200 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/georgian_supplement.csv
--rw-r--r--   0        0        0     2422 2023-09-16 08:03:06.853276 rofimoji-6.2.0/src/picker/data/gitmoji.csv
--rw-r--r--   0        0        0     3486 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/glagolitic.csv
--rw-r--r--   0        0        0     1500 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/glagolitic_supplement.csv
--rw-r--r--   0        0        0      684 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/gothic.csv
--rw-r--r--   0        0        0     2304 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/grantha.csv
--rw-r--r--   0        0        0     4218 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/greek_and_coptic.csv
--rw-r--r--   0        0        0    11730 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/greek_extended.csv
--rw-r--r--   0        0        0     2334 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/gujarati.csv
--rw-r--r--   0        0        0     1881 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/gunjala_gondi.csv
--rw-r--r--   0        0        0     1908 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/gurmukhi.csv
--rw-r--r--   0        0        0     7414 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/halfwidth_and_fullwidth_forms.csv
--rw-r--r--   0        0        0     2543 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/hangul_compatibility_jamo.csv
--rw-r--r--   0        0        0     7910 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/hangul_jamo.csv
--rw-r--r--   0        0        0      985 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/hangul_jamo_extended-a.csv
--rw-r--r--   0        0        0     2383 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/hangul_jamo_extended-b.csv
--rw-r--r--   0        0        0     1719 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/hanifi_rohingya.csv
--rw-r--r--   0        0        0      538 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/hanunoo.csv
--rw-r--r--   0        0        0      714 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/hatran.csv
--rw-r--r--   0        0        0     2344 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/hebrew.csv
--rw-r--r--   0        0        0     2318 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/hiragana.csv
--rw-r--r--   0        0        0      923 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/ideographic_description_characters.csv
--rw-r--r--   0        0        0      230 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/ideographic_symbols_and_punctuation.csv
--rw-r--r--   0        0        0     1173 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/imperial_aramaic.csv
--rw-r--r--   0        0        0     2591 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/indic_siyaq_numbers.csv
--rw-r--r--   0        0        0     1166 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/inscriptional_pahlavi.csv
--rw-r--r--   0        0        0     1307 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/inscriptional_parthian.csv
--rw-r--r--   0        0        0     3418 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/ipa_extensions.csv
--rw-r--r--   0        0        0     2438 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/javanese.csv
--rw-r--r--   0        0        0     1611 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/kaithi.csv
--rw-r--r--   0        0        0      570 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/kaktovik_numerals.csv
--rw-r--r--   0        0        0     1006 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/kana_extended-a.csv
--rw-r--r--   0        0        0      525 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/kana_extended-b.csv
--rw-r--r--   0        0        0     7167 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/kana_supplement.csv
--rw-r--r--   0        0        0      608 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/kanbun.csv
--rw-r--r--   0        0        0     5434 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/kangxi_radicals.csv
--rw-r--r--   0        0        0     2241 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/kannada.csv
--rw-r--r--   0        0        0     2323 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/katakana.csv
--rw-r--r--   0        0        0      464 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/katakana_phonetic_extensions.csv
--rw-r--r--   0        0        0     1997 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/kawi.csv
--rw-r--r--   0        0        0     1121 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/kayah_li.csv
--rw-r--r--   0        0        0     2145 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/kharoshthi.csv
--rw-r--r--   0        0        0    19270 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/khitan_small_script.csv
--rw-r--r--   0        0        0     2849 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/khmer.csv
--rw-r--r--   0        0        0      916 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/khmer_symbols.csv
--rw-r--r--   0        0        0     1526 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/khojki.csv
--rw-r--r--   0        0        0     1793 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/khudawadi.csv
--rw-r--r--   0        0        0     1779 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/lao.csv
--rw-r--r--   0        0        0     2978 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/latin-1_supplement.csv
--rw-r--r--   0        0        0     4762 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/latin_extended-a.csv
--rw-r--r--   0        0        0     7913 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/latin_extended-b.csv
--rw-r--r--   0        0        0     1235 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/latin_extended-c.csv
--rw-r--r--   0        0        0     7236 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/latin_extended-d.csv
--rw-r--r--   0        0        0     2474 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/latin_extended-e.csv
--rw-r--r--   0        0        0     2450 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/latin_extended-f.csv
--rw-r--r--   0        0        0     1799 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/latin_extended-g.csv
--rw-r--r--   0        0        0    11426 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/latin_extended_additional.csv
--rw-r--r--   0        0        0     1765 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/lepcha.csv
--rw-r--r--   0        0        0     1840 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/letterlike_symbols.csv
--rw-r--r--   0        0        0     1538 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/limbu.csv
--rw-r--r--   0        0        0     8429 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/linear_a.csv
--rw-r--r--   0        0        0     3958 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/linear_b_ideograms.csv
--rw-r--r--   0        0        0     2664 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/linear_b_syllabary.csv
--rw-r--r--   0        0        0      995 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/lisu.csv
--rw-r--r--   0        0        0       21 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/lisu_supplement.csv
--rw-r--r--   0        0        0      617 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/lycian.csv
--rw-r--r--   0        0        0      661 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/lydian.csv
--rw-r--r--   0        0        0      964 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/mahajani.csv
--rw-r--r--   0        0        0     1402 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/mahjong_tiles.csv
--rw-r--r--   0        0        0      590 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/makasar.csv
--rw-r--r--   0        0        0     3331 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/malayalam.csv
--rw-r--r--   0        0        0      760 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/mandaic.csv
--rw-r--r--   0        0        0     1695 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/manichaean.csv
--rw-r--r--   0        0        0     1903 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/marchen.csv
--rw-r--r--   0        0        0     2252 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/masaram_gondi.csv
--rw-r--r--   0        0        0    93185 2023-09-16 08:03:06.669943 rofimoji-6.2.0/src/picker/data/math.csv
--rw-r--r--   0        0        0    40125 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/mathematical_alphanumeric_symbols.csv
--rw-r--r--   0        0        0     6216 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/mathematical_operators.csv
--rw-r--r--   0        0        0      510 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/mayan_numerals.csv
--rw-r--r--   0        0        0     2969 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/medefaidrin.csv
--rw-r--r--   0        0        0     1668 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/meetei_mayek.csv
--rw-r--r--   0        0        0      681 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/meetei_mayek_extensions.csv
--rw-r--r--   0        0        0     8499 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/mende_kikakui.csv
--rw-r--r--   0        0        0     3826 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/meroitic_cursive.csv
--rw-r--r--   0        0        0     1298 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/meroitic_hieroglyphs.csv
--rw-r--r--   0        0        0     3532 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/miao.csv
--rw-r--r--   0        0        0     1541 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/miscellaneous_mathematical_symbols-a.csv
--rw-r--r--   0        0        0     4228 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/miscellaneous_mathematical_symbols-b.csv
--rw-r--r--   0        0        0     5475 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/miscellaneous_symbols.csv
--rw-r--r--   0        0        0     9010 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/miscellaneous_symbols_and_arrows.csv
--rw-r--r--   0        0        0    16261 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/miscellaneous_symbols_and_pictographs.csv
--rw-r--r--   0        0        0     7975 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/miscellaneous_technical.csv
--rw-r--r--   0        0        0     1736 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/modi.csv
--rw-r--r--   0        0        0     1413 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/modifier_tone_letters.csv
--rw-r--r--   0        0        0     4806 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/mongolian.csv
--rw-r--r--   0        0        0      535 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/mongolian_supplement.csv
--rw-r--r--   0        0        0      843 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/mro.csv
--rw-r--r--   0        0        0      893 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/multani.csv
--rw-r--r--   0        0        0     8605 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/musical_symbols.csv
--rw-r--r--   0        0        0     4595 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/myanmar.csv
--rw-r--r--   0        0        0     1000 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/myanmar_extended-a.csv
--rw-r--r--   0        0        0     1001 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/myanmar_extended-b.csv
--rw-r--r--   0        0        0     1272 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/nabataean.csv
--rw-r--r--   0        0        0     1148 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/nag_mundari.csv
--rw-r--r--   0        0        0     1875 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/nandinagari.csv
--rw-r--r--   0        0        0   290162 2023-05-20 08:41:43.841476 rofimoji-6.2.0/src/picker/data/nerd_font.csv
--rw-r--r--   0        0        0     2505 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/new_tai_lue.csv
--rw-r--r--   0        0        0     2148 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/newa.csv
--rw-r--r--   0        0        0     1440 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/nko.csv
--rw-r--r--   0        0        0     1772 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/number_forms.csv
--rw-r--r--   0        0        0    10692 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/nushu.csv
--rw-r--r--   0        0        0     2755 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/nyiakeng_puachue_hmong.csv
--rw-r--r--   0        0        0      673 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/ogham.csv
--rw-r--r--   0        0        0     1158 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/ol_chiki.csv
--rw-r--r--   0        0        0     4348 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/old_hungarian.csv
--rw-r--r--   0        0        0     1049 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/old_italic.csv
--rw-r--r--   0        0        0     1200 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/old_north_arabian.csv
--rw-r--r--   0        0        0     1221 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/old_permic.csv
--rw-r--r--   0        0        0     1338 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/old_persian.csv
--rw-r--r--   0        0        0     1434 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/old_sogdian.csv
--rw-r--r--   0        0        0     1228 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/old_south_arabian.csv
--rw-r--r--   0        0        0     2688 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/old_turkic.csv
--rw-r--r--   0        0        0      881 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/old_uyghur.csv
--rw-r--r--   0        0        0      227 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/optical_character_recognition.csv
--rw-r--r--   0        0        0     2060 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/oriya.csv
--rw-r--r--   0        0        0     1683 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/ornamental_dingbats.csv
--rw-r--r--   0        0        0     2060 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/osage.csv
--rw-r--r--   0        0        0      947 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/osmanya.csv
--rw-r--r--   0        0        0     2505 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/ottoman_siyaq_numbers.csv
--rw-r--r--   0        0        0     4001 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/pahawh_hmong.csv
--rw-r--r--   0        0        0      988 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/palmyrene.csv
--rw-r--r--   0        0        0     1776 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/pau_cin_hau.csv
--rw-r--r--   0        0        0     1415 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/phags-pa.csv
--rw-r--r--   0        0        0     1455 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/phaistos_disc.csv
--rw-r--r--   0        0        0      889 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/phoenician.csv
--rw-r--r--   0        0        0     4468 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/phonetic_extensions.csv
--rw-r--r--   0        0        0     2620 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/phonetic_extensions_supplement.csv
--rw-r--r--   0        0        0     2562 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/playing_cards.csv
--rw-r--r--   0        0        0     1093 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/psalter_pahlavi.csv
--rw-r--r--   0        0        0      841 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/rejang.csv
--rw-r--r--   0        0        0      881 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/rumi_numeral_symbols.csv
--rw-r--r--   0        0        0     2424 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/runic.csv
--rw-r--r--   0        0        0     1929 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/samaritan.csv
--rw-r--r--   0        0        0     2217 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/saurashtra.csv
--rw-r--r--   0        0        0     2452 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/sharada.csv
--rw-r--r--   0        0        0     1172 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/shavian.csv
--rw-r--r--   0        0        0      140 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/shorthand_format_controls.csv
--rw-r--r--   0        0        0     2805 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/siddham.csv
--rw-r--r--   0        0        0     3060 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/sinhala.csv
--rw-r--r--   0        0        0      679 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/sinhala_archaic_numbers.csv
--rw-r--r--   0        0        0      634 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/small_form_variants.csv
--rw-r--r--   0        0        0      269 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/small_kana_extension.csv
--rw-r--r--   0        0        0     1379 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/sogdian.csv
--rw-r--r--   0        0        0     1012 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/sora_sompeng.csv
--rw-r--r--   0        0        0     2345 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/soyombo.csv
--rw-r--r--   0        0        0     2565 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/spacing_modifier_letters.csv
--rw-r--r--   0        0        0      168 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/specials.csv
--rw-r--r--   0        0        0     1714 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/sundanese.csv
--rw-r--r--   0        0        0      330 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/sundanese_supplement.csv
--rw-r--r--   0        0        0     1147 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/superscripts_and_subscripts.csv
--rw-r--r--   0        0        0      526 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/supplemental_arrows-a.csv
--rw-r--r--   0        0        0     5599 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/supplemental_arrows-b.csv
--rw-r--r--   0        0        0     6639 2023-09-16 08:02:53.469953 rofimoji-6.2.0/src/picker/data/supplemental_arrows-c.csv
--rw-r--r--   0        0        0     8936 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/supplemental_mathematical_operators.csv
--rw-r--r--   0        0        0     2556 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/supplemental_punctuation.csv
--rw-r--r--   0        0        0     4767 2023-09-16 08:02:53.469953 rofimoji-6.2.0/src/picker/data/supplemental_symbols_and_pictographs.csv
--rw-r--r--   0        0        0    31771 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/sutton_signwriting.csv
--rw-r--r--   0        0        0     1281 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/syloti_nagri.csv
--rw-r--r--   0        0        0     1743 2023-09-16 08:02:53.469953 rofimoji-6.2.0/src/picker/data/symbols_and_pictographs_extended-a.csv
--rw-r--r--   0        0        0     8729 2023-09-16 08:02:53.469953 rofimoji-6.2.0/src/picker/data/symbols_for_legacy_computing.csv
--rw-r--r--   0        0        0     2135 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/syriac.csv
--rw-r--r--   0        0        0      385 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/syriac_supplement.csv
--rw-r--r--   0        0        0      524 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/tagalog.csv
--rw-r--r--   0        0        0      418 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/tagbanwa.csv
--rw-r--r--   0        0        0     2575 2023-09-16 08:02:53.469953 rofimoji-6.2.0/src/picker/data/tags.csv
--rw-r--r--   0        0        0      758 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/tai_le.csv
--rw-r--r--   0        0        0     3550 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/tai_tham.csv
--rw-r--r--   0        0        0     1897 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/tai_viet.csv
--rw-r--r--   0        0        0     2517 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/tai_xuan_jing_symbols.csv
--rw-r--r--   0        0        0     1511 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/takri.csv
--rw-r--r--   0        0        0     1534 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/tamil.csv
--rw-r--r--   0        0        0     1535 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/tamil_supplement.csv
--rw-r--r--   0        0        0     2028 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/tangsa.csv
--rw-r--r--   0        0        0    19968 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/tangut_components.csv
--rw-r--r--   0        0        0     2566 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/telugu.csv
--rw-r--r--   0        0        0     1234 2023-09-16 08:02:53.439953 rofimoji-6.2.0/src/picker/data/thaana.csv
--rw-r--r--   0        0        0     2340 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/thai.csv
--rw-r--r--   0        0        0     6455 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/tibetan.csv
--rw-r--r--   0        0        0     1582 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/tifinagh.csv
--rw-r--r--   0        0        0     2049 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/tirhuta.csv
--rw-r--r--   0        0        0      662 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/toto.csv
--rw-r--r--   0        0        0     2229 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/transport_and_map_symbols.csv
--rw-r--r--   0        0        0      791 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/ugaritic.csv
--rw-r--r--   0        0        0    20601 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/unified_canadian_aboriginal_syllabics.csv
--rw-r--r--   0        0        0      562 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended-a.csv
--rw-r--r--   0        0        0     2167 2023-09-16 08:02:53.443286 rofimoji-6.2.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended.csv
--rw-r--r--   0        0        0     6238 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/vai.csv
--rw-r--r--   0        0        0      407 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/variation_selectors.csv
--rw-r--r--   0        0        0     6637 2023-09-16 08:02:53.469953 rofimoji-6.2.0/src/picker/data/variation_selectors_supplement.csv
--rw-r--r--   0        0        0     1512 2023-09-16 08:02:53.446619 rofimoji-6.2.0/src/picker/data/vedic_extensions.csv
--rw-r--r--   0        0        0      524 2023-09-16 08:02:53.453286 rofimoji-6.2.0/src/picker/data/vertical_forms.csv
--rw-r--r--   0        0        0     2176 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/vithkuqi.csv
--rw-r--r--   0        0        0     1321 2023-09-16 08:02:53.466619 rofimoji-6.2.0/src/picker/data/wancho.csv
--rw-r--r--   0        0        0     2788 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/warang_citi.csv
--rw-r--r--   0        0        0     1286 2023-09-16 08:02:53.456619 rofimoji-6.2.0/src/picker/data/yezidi.csv
--rw-r--r--   0        0        0     1052 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/yi_radicals.csv
--rw-r--r--   0        0        0    23855 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/yi_syllables.csv
--rw-r--r--   0        0        0     1955 2023-09-16 08:02:53.449953 rofimoji-6.2.0/src/picker/data/yijing_hexagram_symbols.csv
--rw-r--r--   0        0        0     2586 2023-09-16 08:02:53.459953 rofimoji-6.2.0/src/picker/data/zanabazar_square.csv
--rw-r--r--   0        0        0     7873 2023-09-16 08:02:53.463286 rofimoji-6.2.0/src/picker/data/znamenny_musical_notation.csv
--rw-r--r--   0        0        0     4983 2023-09-16 08:07:33.169604 rofimoji-6.2.0/src/picker/docs/rofimoji.1
--rw-r--r--   0        0        0     4327 2023-09-16 08:07:22.739622 rofimoji-6.2.0/src/picker/docs/rofimoji.1.md
--rw-r--r--   0        0        0     1982 2023-09-16 08:10:09.785973 rofimoji-6.2.0/src/picker/emoji_data.py
--rw-r--r--   0        0        0     2882 2023-02-25 09:16:47.325872 rofimoji-6.2.0/src/picker/file_loader.py
--rw-r--r--   0        0        0     1108 2022-12-29 11:56:19.215888 rofimoji-6.2.0/src/picker/frecent.py
--rw-r--r--   0        0        0     7406 2022-12-29 11:56:19.215888 rofimoji-6.2.0/src/picker/mode.py
--rw-r--r--   0        0        0      558 2022-11-13 10:52:07.473886 rofimoji-6.2.0/src/picker/models.py
--rw-r--r--   0        0        0      708 2022-11-13 10:52:07.473886 rofimoji-6.2.0/src/picker/paths.py
--rw-r--r--   0        0        0     1172 2022-11-13 10:52:07.473886 rofimoji-6.2.0/src/picker/recent.py
--rw-r--r--   0        0        0        0 2022-11-13 10:52:07.473886 rofimoji-6.2.0/src/picker/selector/__init__.py
--rw-r--r--   0        0        0     9692 2023-09-09 09:52:46.914394 rofimoji-6.2.0/src/picker/selector/selector.py
--rw-r--r--   0        0        0     4074 2022-12-29 11:56:19.215888 rofimoji-6.2.0/src/picker/standalone.py
--rw-r--r--   0        0        0        0 2022-11-13 10:52:07.473886 rofimoji-6.2.0/src/picker/typer/__init__.py
--rw-r--r--   0        0        0     2496 2023-09-16 08:10:09.789306 rofimoji-6.2.0/src/picker/typer/typer.py
--rw-r--r--   0        0        0    19614 1970-01-01 00:00:00.000000 rofimoji-6.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-24 10:41:32.767624 rofimoji-6.3.0/LICENSE
+-rw-r--r--   0        0        0    19841 2024-04-27 13:42:04.149186 rofimoji-6.3.0/README.md
+-rw-r--r--   0        0        0      892 2024-05-01 08:34:01.938166 rofimoji-6.3.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2022-12-29 11:56:19.212555 rofimoji-6.3.0/src/picker/__init__.py
+-rw-r--r--   0        0        0      259 2024-03-29 09:38:49.773804 rofimoji-6.3.0/src/picker/__main__.py
+-rw-r--r--   0        0        0      188 2022-11-13 10:52:07.457219 rofimoji-6.3.0/src/picker/abstractionhelper.py
+-rw-r--r--   0        0        0     1204 2024-03-24 10:41:32.767624 rofimoji-6.3.0/src/picker/action.py
+-rw-r--r--   0        0        0     5849 2024-03-24 10:41:32.767624 rofimoji-6.3.0/src/picker/argument_parsing.py
+-rw-r--r--   0        0        0        0 2022-11-13 10:52:07.457219 rofimoji-6.3.0/src/picker/clipboarder/__init__.py
+-rw-r--r--   0        0        0     1127 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/clipboarder/clipboarder.py
+-rw-r--r--   0        0        0      677 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/clipboarder/noop.py
+-rw-r--r--   0        0        0     1093 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/clipboarder/wl.py
+-rw-r--r--   0        0        0     1885 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/clipboarder/xclip.py
+-rw-r--r--   0        0        0     1115 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/clipboarder/xsel.py
+-rw-r--r--   0        0        0      452 2024-03-24 10:45:56.170300 rofimoji-6.3.0/src/picker/contrib/grid-icons-only.rasi
+-rw-r--r--   0        0        0      457 2024-03-24 10:44:13.180796 rofimoji-6.3.0/src/picker/contrib/grid.rasi
+-rw-r--r--   0        0        0       23 2023-08-17 09:39:13.406636 rofimoji-6.3.0/src/picker/data/additional/emojis_smileys_emotion.csv
+-rw-r--r--   0        0        0     2712 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/adlam.csv
+-rw-r--r--   0        0        0     1737 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/aegean_numbers.csv
+-rw-r--r--   0        0        0     1470 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/ahom.csv
+-rw-r--r--   0        0        0     4551 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/alchemical_symbols.csv
+-rw-r--r--   0        0        0     2098 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/alphabetic_presentation_forms.csv
+-rw-r--r--   0        0        0    18183 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/anatolian_hieroglyphs.csv
+-rw-r--r--   0        0        0     2761 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/ancient_greek_musical_notation.csv
+-rw-r--r--   0        0        0     2895 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/ancient_greek_numbers.csv
+-rw-r--r--   0        0        0      344 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/ancient_symbols.csv
+-rw-r--r--   0        0        0     8311 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/arabic.csv
+-rw-r--r--   0        0        0     3561 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/arabic_extended-a.csv
+-rw-r--r--   0        0        0     1906 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/arabic_extended-b.csv
+-rw-r--r--   0        0        0       98 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/arabic_extended-c.csv
+-rw-r--r--   0        0        0     5786 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/arabic_mathematical_alphabetic_symbols.csv
+-rw-r--r--   0        0        0    32176 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/arabic_presentation_forms-a.csv
+-rw-r--r--   0        0        0     5722 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/arabic_presentation_forms-b.csv
+-rw-r--r--   0        0        0     2719 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/arabic_supplement.csv
+-rw-r--r--   0        0        0     2715 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/armenian.csv
+-rw-r--r--   0        0        0     3689 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/arrows.csv
+-rw-r--r--   0        0        0     1729 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/avestan.csv
+-rw-r--r--   0        0        0     3904 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/balinese.csv
+-rw-r--r--   0        0        0     1870 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/bamum.csv
+-rw-r--r--   0        0        0    18380 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/bamum_supplement.csv
+-rw-r--r--   0        0        0     1876 2024-04-27 08:12:37.573949 rofimoji-6.3.0/src/picker/data/basic_latin.csv
+-rw-r--r--   0        0        0      968 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/bassa_vah.csv
+-rw-r--r--   0        0        0     1419 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/batak.csv
+-rw-r--r--   0        0        0     2451 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/bengali.csv
+-rw-r--r--   0        0        0     2625 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/bhaiksuki.csv
+-rw-r--r--   0        0        0      944 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/block_elements.csv
+-rw-r--r--   0        0        0      981 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/bopomofo.csv
+-rw-r--r--   0        0        0      774 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/bopomofo_extended.csv
+-rw-r--r--   0        0        0     5625 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/box_drawing.csv
+-rw-r--r--   0        0        0     2950 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/brahmi.csv
+-rw-r--r--   0        0        0     7680 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/braille_patterns.csv
+-rw-r--r--   0        0        0      716 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/buginese.csv
+-rw-r--r--   0        0        0      404 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/buhid.csv
+-rw-r--r--   0        0        0    11298 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/byzantine_musical_symbols.csv
+-rw-r--r--   0        0        0     1078 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/carian.csv
+-rw-r--r--   0        0        0     1885 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/caucasian_albanian.csv
+-rw-r--r--   0        0        0     1675 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/chakma.csv
+-rw-r--r--   0        0        0     1820 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/cham.csv
+-rw-r--r--   0        0        0     2166 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/cherokee.csv
+-rw-r--r--   0        0        0     2334 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/cherokee_supplement.csv
+-rw-r--r--   0        0        0     4120 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/chess_symbols.csv
+-rw-r--r--   0        0        0      889 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/chorasmian.csv
+-rw-r--r--   0        0        0   282678 2024-04-27 08:12:40.473965 rofimoji-6.3.0/src/picker/data/cjk_cantonese.csv
+-rw-r--r--   0        0        0     6158 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/cjk_compatibility.csv
+-rw-r--r--   0        0        0     1463 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/cjk_compatibility_forms.csv
+-rw-r--r--   0        0        0    17464 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/cjk_compatibility_ideographs.csv
+-rw-r--r--   0        0        0    21138 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/cjk_compatibility_ideographs_supplement.csv
+-rw-r--r--   0        0        0   164294 2024-04-27 08:12:40.523965 rofimoji-6.3.0/src/picker/data/cjk_japanese_kun.csv
+-rw-r--r--   0        0        0   152011 2024-04-27 08:12:40.537299 rofimoji-6.3.0/src/picker/data/cjk_japanese_on.csv
+-rw-r--r--   0        0        0    76750 2024-04-27 08:12:40.543966 rofimoji-6.3.0/src/picker/data/cjk_korean.csv
+-rw-r--r--   0        0        0   390276 2024-04-27 08:12:40.503965 rofimoji-6.3.0/src/picker/data/cjk_mandarin.csv
+-rw-r--r--   0        0        0     3072 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/cjk_radicals_supplement.csv
+-rw-r--r--   0        0        0      714 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/cjk_strokes.csv
+-rw-r--r--   0        0        0     1919 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/cjk_symbols_and_punctuation.csv
+-rw-r--r--   0        0        0    43076 2024-04-27 08:12:40.513965 rofimoji-6.3.0/src/picker/data/cjk_tang.csv
+-rw-r--r--   0        0        0    87736 2024-04-27 08:12:40.510632 rofimoji-6.3.0/src/picker/data/cjk_vietnamese.csv
+-rw-r--r--   0        0        0     3356 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/combining_diacritical_marks.csv
+-rw-r--r--   0        0        0     1141 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_extended.csv
+-rw-r--r--   0        0        0     1189 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_for_symbols.csv
+-rw-r--r--   0        0        0     2374 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_supplement.csv
+-rw-r--r--   0        0        0      581 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/combining_half_marks.csv
+-rw-r--r--   0        0        0      347 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/common_indic_number_forms.csv
+-rw-r--r--   0        0        0     1104 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/control_pictures.csv
+-rw-r--r--   0        0        0     4234 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/coptic.csv
+-rw-r--r--   0        0        0      919 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/coptic_epact_numbers.csv
+-rw-r--r--   0        0        0      817 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/counting_rod_numerals.csv
+-rw-r--r--   0        0        0    30373 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/cuneiform.csv
+-rw-r--r--   0        0        0     5019 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/cuneiform_numbers_and_punctuation.csv
+-rw-r--r--   0        0        0      556 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/currency_symbols.csv
+-rw-r--r--   0        0        0     1535 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/cypriot_syllabary.csv
+-rw-r--r--   0        0        0     2873 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/cypro-minoan.csv
+-rw-r--r--   0        0        0     9424 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/cyrillic.csv
+-rw-r--r--   0        0        0     1116 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/cyrillic_extended-a.csv
+-rw-r--r--   0        0        0     3480 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/cyrillic_extended-b.csv
+-rw-r--r--   0        0        0      338 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/cyrillic_extended-c.csv
+-rw-r--r--   0        0        0     2654 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/cyrillic_extended-d.csv
+-rw-r--r--   0        0        0     1746 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/cyrillic_supplement.csv
+-rw-r--r--   0        0        0     2552 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/deseret.csv
+-rw-r--r--   0        0        0     3580 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/devanagari.csv
+-rw-r--r--   0        0        0      377 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/devanagari_extended-a.csv
+-rw-r--r--   0        0        0     1089 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/devanagari_extended.csv
+-rw-r--r--   0        0        0     6632 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/dingbats.csv
+-rw-r--r--   0        0        0     2029 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/dives_akuru.csv
+-rw-r--r--   0        0        0     1348 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/dogra.csv
+-rw-r--r--   0        0        0     3298 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/domino_tiles.csv
+-rw-r--r--   0        0        0     4069 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/duployan.csv
+-rw-r--r--   0        0        0     7082 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/early_dynastic_cuneiform.csv
+-rw-r--r--   0        0        0     1794 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/egyptian_hieroglyph_format_controls.csv
+-rw-r--r--   0        0        0    32482 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/egyptian_hieroglyphs.csv
+-rw-r--r--   0        0        0      930 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/elbasan.csv
+-rw-r--r--   0        0        0      654 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/elymaic.csv
+-rw-r--r--   0        0        0     5642 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_activities.csv
+-rw-r--r--   0        0        0     7330 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_animals_nature.csv
+-rw-r--r--   0        0        0      253 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_component.csv
+-rw-r--r--   0        0        0     7284 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_flags.csv
+-rw-r--r--   0        0        0     7931 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_food_drink.csv
+-rw-r--r--   0        0        0    16393 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_objects.csv
+-rw-r--r--   0        0        0    21230 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_people_body.csv
+-rw-r--r--   0        0        0    11962 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_smileys_emotion.csv
+-rw-r--r--   0        0        0    16126 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_symbols.csv
+-rw-r--r--   0        0        0    13690 2024-04-14 14:48:24.660490 rofimoji-6.3.0/src/picker/data/emojis_travel_places.csv
+-rw-r--r--   0        0        0     2229 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/emoticons.csv
+-rw-r--r--   0        0        0     7107 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/enclosed_alphanumeric_supplement.csv
+-rw-r--r--   0        0        0     5169 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/enclosed_alphanumerics.csv
+-rw-r--r--   0        0        0     7668 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/enclosed_cjk_letters_and_months.csv
+-rw-r--r--   0        0        0     2570 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/enclosed_ideographic_supplement.csv
+-rw-r--r--   0        0        0     9421 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/ethiopic.csv
+-rw-r--r--   0        0        0      868 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/ethiopic_extended-a.csv
+-rw-r--r--   0        0        0      903 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/ethiopic_extended-b.csv
+-rw-r--r--   0        0        0     2095 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/ethiopic_extended.csv
+-rw-r--r--   0        0        0      774 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/ethiopic_supplement.csv
+-rw-r--r--   0        0        0    52690 2024-04-27 08:12:41.863973 rofimoji-6.3.0/src/picker/data/fontawesome6.csv
+-rw-r--r--   0        0        0     2575 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/general_punctuation.csv
+-rw-r--r--   0        0        0     3087 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/geometric_shapes.csv
+-rw-r--r--   0        0        0     3236 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/geometric_shapes_extended.csv
+-rw-r--r--   0        0        0     2472 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/georgian.csv
+-rw-r--r--   0        0        0     1908 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/georgian_extended.csv
+-rw-r--r--   0        0        0     1200 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/georgian_supplement.csv
+-rw-r--r--   0        0        0     2433 2024-04-27 08:12:41.490638 rofimoji-6.3.0/src/picker/data/gitmoji.csv
+-rw-r--r--   0        0        0     3486 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/glagolitic.csv
+-rw-r--r--   0        0        0     1500 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/glagolitic_supplement.csv
+-rw-r--r--   0        0        0      684 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/gothic.csv
+-rw-r--r--   0        0        0     2304 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/grantha.csv
+-rw-r--r--   0        0        0     4218 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/greek_and_coptic.csv
+-rw-r--r--   0        0        0    11730 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/greek_extended.csv
+-rw-r--r--   0        0        0     2334 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/gujarati.csv
+-rw-r--r--   0        0        0     1881 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/gunjala_gondi.csv
+-rw-r--r--   0        0        0     1908 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/gurmukhi.csv
+-rw-r--r--   0        0        0     7414 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/halfwidth_and_fullwidth_forms.csv
+-rw-r--r--   0        0        0     2543 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/hangul_compatibility_jamo.csv
+-rw-r--r--   0        0        0     7910 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/hangul_jamo.csv
+-rw-r--r--   0        0        0      985 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/hangul_jamo_extended-a.csv
+-rw-r--r--   0        0        0     2383 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/hangul_jamo_extended-b.csv
+-rw-r--r--   0        0        0     1719 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/hanifi_rohingya.csv
+-rw-r--r--   0        0        0      538 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/hanunoo.csv
+-rw-r--r--   0        0        0      714 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/hatran.csv
+-rw-r--r--   0        0        0     2344 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/hebrew.csv
+-rw-r--r--   0        0        0     2318 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/hiragana.csv
+-rw-r--r--   0        0        0      923 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/ideographic_description_characters.csv
+-rw-r--r--   0        0        0      230 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/ideographic_symbols_and_punctuation.csv
+-rw-r--r--   0        0        0     1173 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/imperial_aramaic.csv
+-rw-r--r--   0        0        0     2591 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/indic_siyaq_numbers.csv
+-rw-r--r--   0        0        0     1166 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/inscriptional_pahlavi.csv
+-rw-r--r--   0        0        0     1307 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/inscriptional_parthian.csv
+-rw-r--r--   0        0        0     3418 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/ipa_extensions.csv
+-rw-r--r--   0        0        0     2438 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/javanese.csv
+-rw-r--r--   0        0        0     1611 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/kaithi.csv
+-rw-r--r--   0        0        0      570 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/kaktovik_numerals.csv
+-rw-r--r--   0        0        0     1006 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/kana_extended-a.csv
+-rw-r--r--   0        0        0      525 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/kana_extended-b.csv
+-rw-r--r--   0        0        0     7167 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/kana_supplement.csv
+-rw-r--r--   0        0        0      608 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/kanbun.csv
+-rw-r--r--   0        0        0     5434 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/kangxi_radicals.csv
+-rw-r--r--   0        0        0     2241 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/kannada.csv
+-rw-r--r--   0        0        0    43839 2024-04-27 13:35:29.036304 rofimoji-6.3.0/src/picker/data/kaomoji.csv
+-rw-r--r--   0        0        0     2323 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/katakana.csv
+-rw-r--r--   0        0        0      464 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/katakana_phonetic_extensions.csv
+-rw-r--r--   0        0        0     1997 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/kawi.csv
+-rw-r--r--   0        0        0     1121 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/kayah_li.csv
+-rw-r--r--   0        0        0     2145 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/kharoshthi.csv
+-rw-r--r--   0        0        0    19270 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/khitan_small_script.csv
+-rw-r--r--   0        0        0     2849 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/khmer.csv
+-rw-r--r--   0        0        0      916 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/khmer_symbols.csv
+-rw-r--r--   0        0        0     1526 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/khojki.csv
+-rw-r--r--   0        0        0     1793 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/khudawadi.csv
+-rw-r--r--   0        0        0     1779 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/lao.csv
+-rw-r--r--   0        0        0     2978 2024-04-27 08:12:37.573949 rofimoji-6.3.0/src/picker/data/latin-1_supplement.csv
+-rw-r--r--   0        0        0     4762 2024-04-27 08:12:37.573949 rofimoji-6.3.0/src/picker/data/latin_extended-a.csv
+-rw-r--r--   0        0        0     7913 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/latin_extended-b.csv
+-rw-r--r--   0        0        0     1235 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/latin_extended-c.csv
+-rw-r--r--   0        0        0     7236 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/latin_extended-d.csv
+-rw-r--r--   0        0        0     2474 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/latin_extended-e.csv
+-rw-r--r--   0        0        0     2450 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/latin_extended-f.csv
+-rw-r--r--   0        0        0     1799 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/latin_extended-g.csv
+-rw-r--r--   0        0        0    11426 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/latin_extended_additional.csv
+-rw-r--r--   0        0        0     1765 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/lepcha.csv
+-rw-r--r--   0        0        0     1840 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/letterlike_symbols.csv
+-rw-r--r--   0        0        0     1538 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/limbu.csv
+-rw-r--r--   0        0        0     8429 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/linear_a.csv
+-rw-r--r--   0        0        0     3958 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/linear_b_ideograms.csv
+-rw-r--r--   0        0        0     2664 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/linear_b_syllabary.csv
+-rw-r--r--   0        0        0      995 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/lisu.csv
+-rw-r--r--   0        0        0       21 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/lisu_supplement.csv
+-rw-r--r--   0        0        0      617 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/lycian.csv
+-rw-r--r--   0        0        0      661 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/lydian.csv
+-rw-r--r--   0        0        0      964 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/mahajani.csv
+-rw-r--r--   0        0        0     1402 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/mahjong_tiles.csv
+-rw-r--r--   0        0        0      590 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/makasar.csv
+-rw-r--r--   0        0        0     3331 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/malayalam.csv
+-rw-r--r--   0        0        0      760 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/mandaic.csv
+-rw-r--r--   0        0        0     1695 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/manichaean.csv
+-rw-r--r--   0        0        0     1903 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/marchen.csv
+-rw-r--r--   0        0        0     2252 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/masaram_gondi.csv
+-rw-r--r--   0        0        0    93185 2024-04-27 08:12:41.153969 rofimoji-6.3.0/src/picker/data/math.csv
+-rw-r--r--   0        0        0    40125 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/mathematical_alphanumeric_symbols.csv
+-rw-r--r--   0        0        0     6216 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/mathematical_operators.csv
+-rw-r--r--   0        0        0      510 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/mayan_numerals.csv
+-rw-r--r--   0        0        0     2969 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/medefaidrin.csv
+-rw-r--r--   0        0        0     1668 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/meetei_mayek.csv
+-rw-r--r--   0        0        0      681 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/meetei_mayek_extensions.csv
+-rw-r--r--   0        0        0     8499 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/mende_kikakui.csv
+-rw-r--r--   0        0        0     3826 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/meroitic_cursive.csv
+-rw-r--r--   0        0        0     1298 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/meroitic_hieroglyphs.csv
+-rw-r--r--   0        0        0     3532 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/miao.csv
+-rw-r--r--   0        0        0     1541 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/miscellaneous_mathematical_symbols-a.csv
+-rw-r--r--   0        0        0     4228 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/miscellaneous_mathematical_symbols-b.csv
+-rw-r--r--   0        0        0     5475 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/miscellaneous_symbols.csv
+-rw-r--r--   0        0        0     9010 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/miscellaneous_symbols_and_arrows.csv
+-rw-r--r--   0        0        0    16261 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/miscellaneous_symbols_and_pictographs.csv
+-rw-r--r--   0        0        0     7975 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/miscellaneous_technical.csv
+-rw-r--r--   0        0        0     1736 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/modi.csv
+-rw-r--r--   0        0        0     1413 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/modifier_tone_letters.csv
+-rw-r--r--   0        0        0     4806 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/mongolian.csv
+-rw-r--r--   0        0        0      535 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/mongolian_supplement.csv
+-rw-r--r--   0        0        0      843 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/mro.csv
+-rw-r--r--   0        0        0      893 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/multani.csv
+-rw-r--r--   0        0        0     8605 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/musical_symbols.csv
+-rw-r--r--   0        0        0     4595 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/myanmar.csv
+-rw-r--r--   0        0        0     1000 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/myanmar_extended-a.csv
+-rw-r--r--   0        0        0     1001 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/myanmar_extended-b.csv
+-rw-r--r--   0        0        0     1272 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/nabataean.csv
+-rw-r--r--   0        0        0     1148 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/nag_mundari.csv
+-rw-r--r--   0        0        0     1875 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/nandinagari.csv
+-rw-r--r--   0        0        0   290162 2023-05-20 08:41:43.841476 rofimoji-6.3.0/src/picker/data/nerd_font.csv
+-rw-r--r--   0        0        0     2505 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/new_tai_lue.csv
+-rw-r--r--   0        0        0     2148 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/newa.csv
+-rw-r--r--   0        0        0     1440 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/nko.csv
+-rw-r--r--   0        0        0     1772 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/number_forms.csv
+-rw-r--r--   0        0        0    10692 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/nushu.csv
+-rw-r--r--   0        0        0     2755 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/nyiakeng_puachue_hmong.csv
+-rw-r--r--   0        0        0      673 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/ogham.csv
+-rw-r--r--   0        0        0     1158 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/ol_chiki.csv
+-rw-r--r--   0        0        0     4348 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_hungarian.csv
+-rw-r--r--   0        0        0     1049 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_italic.csv
+-rw-r--r--   0        0        0     1200 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_north_arabian.csv
+-rw-r--r--   0        0        0     1221 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_permic.csv
+-rw-r--r--   0        0        0     1338 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_persian.csv
+-rw-r--r--   0        0        0     1434 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/old_sogdian.csv
+-rw-r--r--   0        0        0     1228 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_south_arabian.csv
+-rw-r--r--   0        0        0     2688 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/old_turkic.csv
+-rw-r--r--   0        0        0      881 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/old_uyghur.csv
+-rw-r--r--   0        0        0      227 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/optical_character_recognition.csv
+-rw-r--r--   0        0        0     2060 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/oriya.csv
+-rw-r--r--   0        0        0     1683 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/ornamental_dingbats.csv
+-rw-r--r--   0        0        0     2060 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/osage.csv
+-rw-r--r--   0        0        0      947 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/osmanya.csv
+-rw-r--r--   0        0        0     2505 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/ottoman_siyaq_numbers.csv
+-rw-r--r--   0        0        0     4001 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/pahawh_hmong.csv
+-rw-r--r--   0        0        0      988 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/palmyrene.csv
+-rw-r--r--   0        0        0     1776 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/pau_cin_hau.csv
+-rw-r--r--   0        0        0     1415 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/phags-pa.csv
+-rw-r--r--   0        0        0     1455 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/phaistos_disc.csv
+-rw-r--r--   0        0        0      889 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/phoenician.csv
+-rw-r--r--   0        0        0     4468 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/phonetic_extensions.csv
+-rw-r--r--   0        0        0     2620 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/phonetic_extensions_supplement.csv
+-rw-r--r--   0        0        0     2562 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/playing_cards.csv
+-rw-r--r--   0        0        0     1093 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/psalter_pahlavi.csv
+-rw-r--r--   0        0        0      841 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/rejang.csv
+-rw-r--r--   0        0        0      881 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/rumi_numeral_symbols.csv
+-rw-r--r--   0        0        0     2424 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/runic.csv
+-rw-r--r--   0        0        0     1929 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/samaritan.csv
+-rw-r--r--   0        0        0     2217 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/saurashtra.csv
+-rw-r--r--   0        0        0     2452 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/sharada.csv
+-rw-r--r--   0        0        0     1172 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/shavian.csv
+-rw-r--r--   0        0        0      140 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/shorthand_format_controls.csv
+-rw-r--r--   0        0        0     2805 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/siddham.csv
+-rw-r--r--   0        0        0     3060 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/sinhala.csv
+-rw-r--r--   0        0        0      679 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/sinhala_archaic_numbers.csv
+-rw-r--r--   0        0        0      634 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/small_form_variants.csv
+-rw-r--r--   0        0        0      269 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/small_kana_extension.csv
+-rw-r--r--   0        0        0     1379 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/sogdian.csv
+-rw-r--r--   0        0        0     1012 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/sora_sompeng.csv
+-rw-r--r--   0        0        0     2345 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/soyombo.csv
+-rw-r--r--   0        0        0     2565 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/spacing_modifier_letters.csv
+-rw-r--r--   0        0        0      168 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/specials.csv
+-rw-r--r--   0        0        0     1714 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/sundanese.csv
+-rw-r--r--   0        0        0      330 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/sundanese_supplement.csv
+-rw-r--r--   0        0        0     1147 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/superscripts_and_subscripts.csv
+-rw-r--r--   0        0        0      526 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/supplemental_arrows-a.csv
+-rw-r--r--   0        0        0     5599 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/supplemental_arrows-b.csv
+-rw-r--r--   0        0        0     6639 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/supplemental_arrows-c.csv
+-rw-r--r--   0        0        0     8936 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/supplemental_mathematical_operators.csv
+-rw-r--r--   0        0        0     2556 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/supplemental_punctuation.csv
+-rw-r--r--   0        0        0     4767 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/supplemental_symbols_and_pictographs.csv
+-rw-r--r--   0        0        0    31771 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/sutton_signwriting.csv
+-rw-r--r--   0        0        0     1281 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/syloti_nagri.csv
+-rw-r--r--   0        0        0     1743 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/symbols_and_pictographs_extended-a.csv
+-rw-r--r--   0        0        0     8729 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/symbols_for_legacy_computing.csv
+-rw-r--r--   0        0        0     2135 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/syriac.csv
+-rw-r--r--   0        0        0      385 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/syriac_supplement.csv
+-rw-r--r--   0        0        0      524 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/tagalog.csv
+-rw-r--r--   0        0        0      418 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/tagbanwa.csv
+-rw-r--r--   0        0        0     2575 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/tags.csv
+-rw-r--r--   0        0        0      758 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/tai_le.csv
+-rw-r--r--   0        0        0     3550 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/tai_tham.csv
+-rw-r--r--   0        0        0     1897 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/tai_viet.csv
+-rw-r--r--   0        0        0     2517 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/tai_xuan_jing_symbols.csv
+-rw-r--r--   0        0        0     1511 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/takri.csv
+-rw-r--r--   0        0        0     1534 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/tamil.csv
+-rw-r--r--   0        0        0     1535 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/tamil_supplement.csv
+-rw-r--r--   0        0        0     2028 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/tangsa.csv
+-rw-r--r--   0        0        0    19968 2024-04-27 08:12:37.597283 rofimoji-6.3.0/src/picker/data/tangut_components.csv
+-rw-r--r--   0        0        0     2566 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/telugu.csv
+-rw-r--r--   0        0        0     1234 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/thaana.csv
+-rw-r--r--   0        0        0     2340 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/thai.csv
+-rw-r--r--   0        0        0     6455 2024-04-27 08:12:37.577282 rofimoji-6.3.0/src/picker/data/tibetan.csv
+-rw-r--r--   0        0        0     1582 2024-04-27 08:12:37.583949 rofimoji-6.3.0/src/picker/data/tifinagh.csv
+-rw-r--r--   0        0        0     2049 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/tirhuta.csv
+-rw-r--r--   0        0        0      662 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/toto.csv
+-rw-r--r--   0        0        0     2229 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/transport_and_map_symbols.csv
+-rw-r--r--   0        0        0      791 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/ugaritic.csv
+-rw-r--r--   0        0        0    20601 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics.csv
+-rw-r--r--   0        0        0      562 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended-a.csv
+-rw-r--r--   0        0        0     2167 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended.csv
+-rw-r--r--   0        0        0     6238 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/vai.csv
+-rw-r--r--   0        0        0      407 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/variation_selectors.csv
+-rw-r--r--   0        0        0     6637 2024-04-27 08:12:37.603949 rofimoji-6.3.0/src/picker/data/variation_selectors_supplement.csv
+-rw-r--r--   0        0        0     1512 2024-04-27 08:12:37.580616 rofimoji-6.3.0/src/picker/data/vedic_extensions.csv
+-rw-r--r--   0        0        0      524 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/vertical_forms.csv
+-rw-r--r--   0        0        0     2176 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/vithkuqi.csv
+-rw-r--r--   0        0        0     1321 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/wancho.csv
+-rw-r--r--   0        0        0     2788 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/warang_citi.csv
+-rw-r--r--   0        0        0     1286 2024-04-27 08:12:37.590616 rofimoji-6.3.0/src/picker/data/yezidi.csv
+-rw-r--r--   0        0        0     1052 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/yi_radicals.csv
+-rw-r--r--   0        0        0    23855 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/yi_syllables.csv
+-rw-r--r--   0        0        0     1955 2024-04-27 08:12:37.587283 rofimoji-6.3.0/src/picker/data/yijing_hexagram_symbols.csv
+-rw-r--r--   0        0        0     2586 2024-04-27 08:12:37.593949 rofimoji-6.3.0/src/picker/data/zanabazar_square.csv
+-rw-r--r--   0        0        0     7873 2024-04-27 08:12:37.600616 rofimoji-6.3.0/src/picker/data/znamenny_musical_notation.csv
+-rw-r--r--   0        0        0     5389 2024-05-01 08:34:38.924572 rofimoji-6.3.0/src/picker/docs/rofimoji.1
+-rw-r--r--   0        0        0     4620 2024-05-01 08:34:31.074626 rofimoji-6.3.0/src/picker/docs/rofimoji.1.md
+-rw-r--r--   0        0        0     1982 2023-09-16 08:10:09.785973 rofimoji-6.3.0/src/picker/emoji_data.py
+-rw-r--r--   0        0        0     3130 2024-03-29 09:38:49.797137 rofimoji-6.3.0/src/picker/file_loader.py
+-rw-r--r--   0        0        0     1106 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/frecent.py
+-rw-r--r--   0        0        0     7720 2024-03-29 09:41:20.083560 rofimoji-6.3.0/src/picker/mode.py
+-rw-r--r--   0        0        0     1241 2024-03-29 09:38:49.797137 rofimoji-6.3.0/src/picker/models.py
+-rw-r--r--   0        0        0      708 2022-11-13 10:52:07.473886 rofimoji-6.3.0/src/picker/paths.py
+-rw-r--r--   0        0        0     1584 2024-03-24 15:38:05.955336 rofimoji-6.3.0/src/picker/recent.py
+-rw-r--r--   0        0        0        0 2022-11-13 10:52:07.473886 rofimoji-6.3.0/src/picker/selector/__init__.py
+-rw-r--r--   0        0        0     1869 2024-03-24 10:52:21.399476 rofimoji-6.3.0/src/picker/selector/bemenu.py
+-rw-r--r--   0        0        0     1846 2024-03-24 10:52:21.402810 rofimoji-6.3.0/src/picker/selector/dmenu.py
+-rw-r--r--   0        0        0     1964 2024-03-24 10:52:21.399476 rofimoji-6.3.0/src/picker/selector/fuzzel.py
+-rw-r--r--   0        0        0     4378 2024-03-29 09:38:49.797137 rofimoji-6.3.0/src/picker/selector/rofi.py
+-rw-r--r--   0        0        0     2540 2024-03-29 09:38:49.797137 rofimoji-6.3.0/src/picker/selector/selector.py
+-rw-r--r--   0        0        0     2081 2024-03-24 10:52:21.399476 rofimoji-6.3.0/src/picker/selector/tofi.py
+-rw-r--r--   0        0        0     1846 2024-03-24 10:52:21.399476 rofimoji-6.3.0/src/picker/selector/wmenu.py
+-rw-r--r--   0        0        0     1956 2024-03-24 10:52:21.399476 rofimoji-6.3.0/src/picker/selector/wofi.py
+-rw-r--r--   0        0        0     3809 2024-04-26 19:41:42.529177 rofimoji-6.3.0/src/picker/standalone.py
+-rw-r--r--   0        0        0        0 2022-11-13 10:52:07.473886 rofimoji-6.3.0/src/picker/typer/__init__.py
+-rw-r--r--   0        0        0      636 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/typer/noop.py
+-rw-r--r--   0        0        0      998 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/typer/typer.py
+-rw-r--r--   0        0        0      648 2024-03-24 10:41:32.770958 rofimoji-6.3.0/src/picker/typer/wtype.py
+-rw-r--r--   0        0        0     1224 2024-04-14 14:51:30.446733 rofimoji-6.3.0/src/picker/typer/xdotool.py
+-rw-r--r--   0        0        0    20588 1970-01-01 00:00:00.000000 rofimoji-6.3.0/PKG-INFO
```

### Comparing `rofimoji-6.2.0/LICENSE` & `rofimoji-6.3.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017-2023 Fabian Winter
+Copyright (c) 2017-2024 Fabian Winter
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `rofimoji-6.2.0/README.md` & `rofimoji-6.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Rofimoji: A character picker for rofi
 Do you want to use one of those fancy emojis? Or one of those other interesting characters Unicode offers? But you haven't found a good picker yet?
 
-Fear no more, `rofimoji` invokes the power of [rofi](https://github.com/DaveDavenport/rofi/) (and other dmenu-derivatives like [wofi](https://hg.sr.ht/~scoopta/wofi) or [fuzzel](https://codeberg.org/dnkl/fuzzel)) to give you exactly the picker you always wanted.
+Fear no more, `rofimoji` invokes the power of [rofi](https://github.com/DaveDavenport/rofi/) (and [other dmenu-derivatives](#supported-selectors)) to give you exactly the picker you always wanted.
 
 ## Main features
 - Insert the select character directly, or copy it to the clipboard.
 - Characters (and especially emojis) are fuzzy-searchable with keywords.
 - [It remembers the ones you use most and presents them first.](#most-recently-used-characters)
 - Emojis by default, but you can have any Unicode block you want - you can even [use your own](#custom-character-files-and-descriptions)!
 
@@ -58,27 +58,28 @@
 | long option                                                                                                             | short option | possible values                                                                                                | default value                               | description                                                                                                                                                                                                                                                                                                         |
 |-------------------------------------------------------------------------------------------------------------------------|--------------|----------------------------------------------------------------------------------------------------------------|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `--action`                                                                                                              | `-a`         | `type`, `copy`, `clipboard`, `unicode`, `copy-unicode`, `print`, `menu`                                        | `type`                                      | Choose what `rofimoji` should do with the selected characters. See [Actions](#actions) below for details.                                                                                                                                                                                                           |
 | `--files`                                                                                                               | `-f`         | `all`, `<yourfile>` or [any of the files in `data`](https://github.com/fdw/rofimoji/tree/main/src/picker/data) | `emojis`                                    | Define which file(s) to load characters from. A file name without extension (f.e. `emojis_smileys_emotion`) is enough for the distributed ones or any in `${XDG_DATA_HOME}/rofimoji/data`. Globbing with `*` is possible.<br/>`all` is a shortcut for all default files at once. Use with caution, that is a *lot*. |
 | `--skin-tone`                                                                                                           | `-s`         | `light`, `medium-light`, `moderate`, `dark brown`, `black`, as well as `neutral` and `ask`                     | `ask`                                       | Define the skin tone of supporting emojis. `ask` will always ask the user.                                                                                                                                                                                                                                          |
 | `--max-recent`                                                                                                          |              | 0-10                                                                                                           | 10                                          | Show at most this many recently picked characters. The number will be capped at 10. Set to `0` to disable the whole feature.                                                                                                                                                                                        |
 | `--no-frecency`<br/>(`no-frecency=True` in the config file)                                                             |              | -                                                                                                              | `<false>`                                   | By default, `rofimoji` shows frequently used items first. With this option, they're shown in the order of the file.                                                                                                                                                                                                 |
-| `--hidden-descriptions`<br/>(`hidden-descriptions=True` in the config file)                                             |              | -                                                                                                              | `<false>`                                   | Only list the characters, but not their description. This is useful for [grid themes](#rofi-theming). Note that they're still searchable, even though the description is not shown.                                                                                                                                 | 
+| `--hidden-descriptions`<br/>(`hidden-descriptions=True` in the config file)                                             |              | -                                                                                                              | `<false>`                                   | Only list the characters, but not their description. This is useful for [grid themes](#rofi-theming) in `rofi`. Note that they're still searchable, even though the description is not shown. Not used with other selectors.                                                                                        |
+| `--use-icons`                                                                                                           |              |                                                                                                                | `false`                                     | Show characters as icons in `rofi`. Not used for other selectors.                                                                                                                                                                                                                                                   |
 | `--prompt`                                                                                                              | `-r`         | any string                                                                                                     | `😀 `                                       | Define the prompt text for `rofimoji`.                                                                                                                                                                                                                                                                              |
-| `--selector-args`                                                                                                       |              |                                                                                                                |                                             | Define arguments that `rofimoji` will pass through to the selector (`rofi`, `wofi` or `fuzzel`).<br/>Please note that you need to specify it as `--selector-args="<selector-args>"` or `--selector-args " <selector-args>"` because of a [bug in argparse](https://bugs.python.org/issue9334)                       |
-| `--selector`                                                                                                            |              | `rofi`, `wofi`, `fuzzel`                                                                                       | (automatically chosen)                      | Show the selection dialog with this application.                                                                                                                                                                                                                                                                    |
+| `--selector-args`                                                                                                       |              |                                                                                                                |                                             | Define arguments that `rofimoji` will pass through to the selector.<br/>Please note that you need to specify it as `--selector-args="<selector-args>"` or `--selector-args " <selector-args>"` because of a [bug in argparse](https://bugs.python.org/issue9334)                                                    |
+| `--selector`                                                                                                            |              | `rofi`, `wofi`, `fuzzel`, `dmenu`, `tofi`, `bemenu`, `wmenu`                                                   | (automatically chosen)                      | Show the selection dialog with this application.                                                                                                                                                                                                                                                                    |
 | `--clipboarder`                                                                                                         |              | `xsel`, `xclip`, `wl-copy`                                                                                     | (automatically chosen)                      | Access the clipboard with this application.                                                                                                                                                                                                                                                                         |
 | `--typer`                                                                                                               |              | `xdotool`, `wtype`                                                                                             | (automatically chosen)                      | Type the characters using this application.                                                                                                                                                                                                                                                                         |
 | `--keybinding-copy`, `--keybinding-type`, `--keybinding-clipboard`, `--keybinding-unicode`, `--keybinding-copy-unicode` |              |                                                                                                                | `Alt+c`, `Alt+t`, `Alt+p`, `Alt+u`, `Alt+i` | Choose different keybindings than the default values.                                                                                                                                                                                                                                                               |
 
 ## Example config file
 `~/.config/rofimoji.rc`:
 ```
 action = copy
-files = [emojis, hebrew]
+files = [emojis, math]
 skin-tone = moderate
 ```
 
 ## Actions
 
 The `--action` (`-a`) option defines what action will be taken when a character is selected. Multiple actions can be specified with a space character in between (for example: `-a type copy`).
 The options are:
@@ -100,58 +101,78 @@
 Therefore, `rofimoji` uses both and also restores both.
 To use this workaround, you can either use the keybinding `alt+p` or start it as `rofimoji --action clipboard` (`-a clipboard`).
 If you want to have it directly typed instead, you can hit `alt+t`, even though it was started with `--action clipboard`. Note that you can [change the keybindings](#options).
 
 Finally, with `--action copy` (or `-a copy`) you can also tell `rofimoji` to only copy the selected characters to your clipboard.
 
 ## Display server support
-`rofimoji` supports both X11 and Wayland by using either `rofi`, `xsel`/`xclip` and `xdotool` on X11 or `wofi`/`fuzzel`/some other adapter `rofi`, `wl-copy` and `wtype` on Wayland. It tries to automatically choose the right one for the currently running session.
+`rofimoji` supports both X11 and Wayland by using the correct tools for each environment (see [Supported Selectors](#supported-selectors)). It tries to automatically choose the right one for the currently running session.
 If you want to manually overwrite this, have a look at the `--selector`, `--clipboarder` and `--typer` options [above](#options).
 
-Please note that neither `wofi` nor `fuzzel` support custom keyboard shortcuts, recent files or a grid theme at the moment.
-
 ## Most recently used characters
 By default, `rofimoji` will show the last ten recently used characters separately; you can insert them with `alt+1`, `alt+2` and so on. It will use the default [insertion method](#insertion-method).
 If you don't want this, you can set `--max-recent` to `0`.
 
 Additionally, `rofimoji` also remembers in general which characters are used more frequently and sorts the list accordingly. You can disable this behavior with `--no-frecency`.
 
-## Supported characters
-Obviously, `rofimoji` is mostly used for emojis. However, it also supports all other Unicode blocks, for example [mathematical symbols](https://github.com/fdw/rofimoji/blob/main/src/picker/data/math.csv), [Greek and Coptic](https://github.com/fdw/rofimoji/blob/main/src/picker/data/greek_and_coptic.csv) or [Linear B (Ideograms)](https://github.com/fdw/rofimoji/blob/main/src/picker/data/linear_b_ideograms.csv). Simply load them with `-f` (see [options](#options)).
-If you miss something that should be there, please open an issue.
+## Rofi theming
+By default, `rofimoji` re-uses the existing rofi configuration, but you can pass your own using `--selector-args` (for example `--selector-args="-theme ~/your-rofi-theme.rasi"`).
+
+If you would like a more character-focused theme, you can use packaged [`grid.rasi`](https://github.com/fdw/rofimoji/blob/main/src/picker/contrib/grid.rasi) together with the `--hidden-descriptions` parameter. This theme still imports the existing `rofi` configuration but moves the entries into a grid. Of course, you can base your own theme on this. (If you have improvements, please open a PR!)
+To use the arrow keys in `rofi` only for the grid and not the query, pass these `-selector-args`: `-kb-row-left Left -kb-row-right Right -kb-move-char-back Control+b -kb-move-char-forward Control+f`.
+
+![Screenshot of rofimoji with a grid theme](screenshot-grid.png?raw=true)
+
+# Supported characters
+- [Unicode emojis](https://home.unicode.org/emoji/about-emoji/) with the official descriptions and tags. Also supports skin tones and gender variants.
+- All other [Unicode](https://home.unicode.org/) characters, split into the official blocks
+- CJK character sets from Unicode
+- [Font Awesome 6](https://fontawesome.com/)
+- [Nerd Fonts](https://www.nerdfonts.com/)
+- [Gitmoji](https://gitmoji.dev/)
+- Kaomoji, from [w33ble](https://github.com/w33ble/emoticon-data)
+
+If you miss something, please open an issue!
 
 ## Custom character files and descriptions
 If the predefined ones are not enough, you can define additional character files and load them with `-f` (see [options](#options)). In each line, one 'character' can be defined, followed by a single space character (` `). After that, you can write whatever description you want.
 
 If the character is also in another selected file, all descriptions will be combined. If you give it the same name as one of those included with `rofimoji`, yours will be preferred.
 
 For added comfort, `rofimoji` will automatically load an "additional" file for predefined ones. This file needs to called `<filename>.additional.csv` and lie in `${XDG_DATA_DIR}/rofimoji/data/`. For example, if you want to extend `emojis_smileys_emotion`, call the file `emojis_smileys_emotions.additional.csv`. This is helpful if you want additional descriptions: You can define such an additional character file, add the character and your description and your descriptions will now also be shown.
 
 If you think your file is useful to others, please open a PR to include it in a future version of `rofimoji`.
 
-## Rofi theming
-By default, `rofimoji` re-uses the existing rofi configuration, but you can pass your own using `--selector-args` (for example `--selector-args="-theme ~/your-rofi-theme.rasi"`).
-
-If you would like a more character-focused theme, you can use packaged [`grid.rasi`](https://github.com/fdw/rofimoji/blob/main/src/picker/contrib/grid.rasi) together with the `--hidden-descriptions` parameter. This theme still imports the existing `rofi` configuration but moves the entries into a grid. Of course, you can base your own theme on this. (If you have improvements, please open a PR!)
-To use the arrow keys in `rofi` only for the grid and not the query, pass these `-selector-args`: `-kb-row-left Left -kb-row-right Right -kb-move-char-back Control+b -kb-move-char-forward Control+f`.
-
-![Screenshot of rofimoji with a grid theme](screenshot-grid.png?raw=true)
-
 # Installation
 ## From distribution repositories
 [![Packaging status](https://repology.org/badge/vertical-allrepos/rofimoji.svg)](https://repology.org/project/rofimoji/versions)
 
 ## From PyPI
-`rofimoji` is on [PyPI](https://pypi.org/project/rofimoji/). You can install it with `pipx install --user rofimoji` (or `sudo pipx install rofimoji`).
+`rofimoji` is on [PyPI](https://pypi.org/project/rofimoji/). You can install it with `pipx install rofimoji` (or `sudo pipx install rofimoji`).
 
 ## From Github
 Download the wheel file of the [latest release](https://github.com/fdw/rofimoji/releases/) and install it with  `sudo pip install $filename` (or you can use `pip install --user $filename` to only install it for the local user).
 Afterwards, there should be a `rofimoji` on your `$PATH`.
 This also installs the python dependency `configargparse`.
 
 ## Dependencies
 What else do you need:
 - Python 3.8 or higher
 - A font that can display your scripts, (for emojis, [EmojiOne](https://github.com/emojione/emojione) or [Noto Emoji](https://www.google.com/get/noto/) work)
-- `rofi` (in version 1.6.0 or higher if you want to use the mode), `wofi` or `fuzzel`
-- A tool to programmatically type characters into applications. Either `xdotool` for X11 or `wtype` for Wayland
-- A tool to copy the characters to the clipboard. `xsel` and `xclip` work on X11; `wl-copy` on Wayland
+- Optionally, a tool to programmatically type characters into applications. Either `xdotool` for X11 or `wtype` for Wayland
+- Optionally, a tool to copy the characters to the clipboard. `xsel` and `xclip` work on X11; `wl-copy` on Wayland
+
+### Supported Selectors
+Please note that only `rofi` (both on X and Wayland) supports custom keyboard shortcuts, recent files or a grid theme at the moment. For all others, only basic functionality works.
+
+#### X.org
+- [rofi](https://github.com/davatorium/rofi)
+- [bemenu](https://github.com/Cloudef/bemenu)
+- [dmenu](https://tools.suckless.org/dmenu/)
+
+#### Wayland
+- [rofi fork for Wayland](https://github.com/lbonn/rofi)
+- [wofi](https://hg.sr.ht/~scoopta/wofi)
+- [fuzzel](https://codeberg.org/dnkl/fuzzel)
+- [tofi](https://github.com/philj56/tofi)
+- [bemenu](https://github.com/Cloudef/bemenu)
+- [wmenu](https://git.sr.ht/~adnano/wmenu)
```

### Comparing `rofimoji-6.2.0/pyproject.toml` & `rofimoji-6.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rofimoji"
-version = "6.2.0"
+version = "6.3.0"
 description = "Simple character picker using rofi"
 authors = ["Fabian Winter <5821180+fdw@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fdw/rofimoji"
 repository = "https://github.com/fdw/rofimoji"
 packages =[
@@ -20,20 +20,20 @@
 rofimoji = 'picker.__main__:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 ConfigArgParse = "^1.3"
 
 [tool.poetry.group.dev.dependencies]
-beautifulsoup4 = "^4.12.2"
-lxml = "^4.9.2"
+beautifulsoup4 = "^4.12.3"
+lxml = "^4.9.4"
 requests = "^2.31.0"
-tqdm = "^4.65.0"
-black = "^22.12.0"
-isort = "^5.12.0"
+tqdm = "^4.66.2"
+black = "^24.3.0"
+isort = "^5.13.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `rofimoji-6.2.0/src/picker/action.py` & `rofimoji-6.3.0/src/picker/action.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .models import Action
 from .typer.typer import Typer
 
 
 def execute_action(
     characters: str,
     actions: List[Action],
-    active_window: Optional[str] = None,
+    active_window: str,
     typer_preference: Optional[str] = None,
     clipboarder_preference: Optional[str] = None,
 ) -> None:
     typer = Typer.best_option(typer_preference)
     clipboarder = Clipboarder.best_option(clipboarder_preference)
 
     for action in actions:
```

### Comparing `rofimoji-6.2.0/src/picker/argument_parsing.py` & `rofimoji-6.3.0/src/picker/argument_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     )
     parser.add_argument("--prompt", "-r", dest="prompt", action="store", default="😀 ", help="Set rofimoj's  prompt")
     parser.add_argument(
         "--selector-args",
         dest="selector_args",
         action="store",
         default=False,
-        help="A string of arguments to give to the selector (rofi, wofi or fuzzel)",
+        help="A string of arguments to give to the selector",
     )
     parser.add_argument(
         "--max-recent",
         dest="max_recent",
         action="store",
         type=int,
         default=10,
@@ -87,19 +87,26 @@
         "--hidden-descriptions",
         dest="show_description",
         action="store_false",
         help="Show only the character without its description",
     )
     parser.set_defaults(show_description=True)
     parser.add_argument(
+        "--use-icons",
+        dest="use_icons",
+        action="store_true",
+        help="Use rofi's icon to show the character",
+    )
+    parser.set_defaults(use_icons=False)
+    parser.add_argument(
         "--selector",
         dest="selector",
         action="store",
         type=str,
-        choices=["rofi", "wofi", "fuzzel", "dmenu"],
+        choices=["rofi", "wofi", "fuzzel", "dmenu", "tofi", "bemenu", "wmenu"],
         default=None,
         help="Choose the application to select the characters with",
     )
     parser.add_argument(
         "--clipboarder",
         dest="clipboarder",
         action="store",
```

### Comparing `rofimoji-6.2.0/src/picker/data/adlam.csv` & `rofimoji-6.3.0/src/picker/data/adlam.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/aegean_numbers.csv` & `rofimoji-6.3.0/src/picker/data/aegean_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ahom.csv` & `rofimoji-6.3.0/src/picker/data/ahom.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/alchemical_symbols.csv` & `rofimoji-6.3.0/src/picker/data/alchemical_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/alphabetic_presentation_forms.csv` & `rofimoji-6.3.0/src/picker/data/alphabetic_presentation_forms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/anatolian_hieroglyphs.csv` & `rofimoji-6.3.0/src/picker/data/anatolian_hieroglyphs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ancient_greek_musical_notation.csv` & `rofimoji-6.3.0/src/picker/data/ancient_greek_musical_notation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ancient_greek_numbers.csv` & `rofimoji-6.3.0/src/picker/data/ancient_greek_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/arabic.csv` & `rofimoji-6.3.0/src/picker/data/arabic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/arabic_extended-a.csv` & `rofimoji-6.3.0/src/picker/data/arabic_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/arabic_extended-b.csv` & `rofimoji-6.3.0/src/picker/data/arabic_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/arabic_mathematical_alphabetic_symbols.csv` & `rofimoji-6.3.0/src/picker/data/arabic_mathematical_alphabetic_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/arabic_presentation_forms-a.csv` & `rofimoji-6.3.0/src/picker/data/arabic_presentation_forms-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/arabic_presentation_forms-b.csv` & `rofimoji-6.3.0/src/picker/data/arabic_presentation_forms-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/arabic_supplement.csv` & `rofimoji-6.3.0/src/picker/data/arabic_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/armenian.csv` & `rofimoji-6.3.0/src/picker/data/armenian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/arrows.csv` & `rofimoji-6.3.0/src/picker/data/arrows.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/avestan.csv` & `rofimoji-6.3.0/src/picker/data/avestan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/balinese.csv` & `rofimoji-6.3.0/src/picker/data/balinese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/bamum.csv` & `rofimoji-6.3.0/src/picker/data/bamum.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/bamum_supplement.csv` & `rofimoji-6.3.0/src/picker/data/bamum_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/basic_latin.csv` & `rofimoji-6.3.0/src/picker/data/basic_latin.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/bassa_vah.csv` & `rofimoji-6.3.0/src/picker/data/bassa_vah.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/batak.csv` & `rofimoji-6.3.0/src/picker/data/batak.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/bengali.csv` & `rofimoji-6.3.0/src/picker/data/bengali.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/bhaiksuki.csv` & `rofimoji-6.3.0/src/picker/data/bhaiksuki.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/block_elements.csv` & `rofimoji-6.3.0/src/picker/data/block_elements.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/bopomofo.csv` & `rofimoji-6.3.0/src/picker/data/bopomofo.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/bopomofo_extended.csv` & `rofimoji-6.3.0/src/picker/data/bopomofo_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/box_drawing.csv` & `rofimoji-6.3.0/src/picker/data/box_drawing.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/brahmi.csv` & `rofimoji-6.3.0/src/picker/data/brahmi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/braille_patterns.csv` & `rofimoji-6.3.0/src/picker/data/braille_patterns.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/buginese.csv` & `rofimoji-6.3.0/src/picker/data/buginese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/byzantine_musical_symbols.csv` & `rofimoji-6.3.0/src/picker/data/byzantine_musical_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/carian.csv` & `rofimoji-6.3.0/src/picker/data/carian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/caucasian_albanian.csv` & `rofimoji-6.3.0/src/picker/data/caucasian_albanian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/chakma.csv` & `rofimoji-6.3.0/src/picker/data/chakma.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cham.csv` & `rofimoji-6.3.0/src/picker/data/cham.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cherokee.csv` & `rofimoji-6.3.0/src/picker/data/cherokee.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cherokee_supplement.csv` & `rofimoji-6.3.0/src/picker/data/cherokee_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/chess_symbols.csv` & `rofimoji-6.3.0/src/picker/data/chess_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/chorasmian.csv` & `rofimoji-6.3.0/src/picker/data/chorasmian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_cantonese.csv` & `rofimoji-6.3.0/src/picker/data/cjk_cantonese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_compatibility.csv` & `rofimoji-6.3.0/src/picker/data/cjk_compatibility.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_compatibility_forms.csv` & `rofimoji-6.3.0/src/picker/data/cjk_compatibility_forms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_compatibility_ideographs.csv` & `rofimoji-6.3.0/src/picker/data/cjk_compatibility_ideographs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_compatibility_ideographs_supplement.csv` & `rofimoji-6.3.0/src/picker/data/cjk_compatibility_ideographs_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_japanese_kun.csv` & `rofimoji-6.3.0/src/picker/data/cjk_japanese_kun.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_japanese_on.csv` & `rofimoji-6.3.0/src/picker/data/cjk_japanese_on.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_korean.csv` & `rofimoji-6.3.0/src/picker/data/cjk_korean.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_mandarin.csv` & `rofimoji-6.3.0/src/picker/data/cjk_mandarin.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_radicals_supplement.csv` & `rofimoji-6.3.0/src/picker/data/cjk_radicals_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_strokes.csv` & `rofimoji-6.3.0/src/picker/data/cjk_strokes.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_symbols_and_punctuation.csv` & `rofimoji-6.3.0/src/picker/data/cjk_symbols_and_punctuation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_tang.csv` & `rofimoji-6.3.0/src/picker/data/cjk_tang.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cjk_vietnamese.csv` & `rofimoji-6.3.0/src/picker/data/cjk_vietnamese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/combining_diacritical_marks.csv` & `rofimoji-6.3.0/src/picker/data/combining_diacritical_marks.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/combining_diacritical_marks_extended.csv` & `rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/combining_diacritical_marks_for_symbols.csv` & `rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_for_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/combining_diacritical_marks_supplement.csv` & `rofimoji-6.3.0/src/picker/data/combining_diacritical_marks_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/combining_half_marks.csv` & `rofimoji-6.3.0/src/picker/data/combining_half_marks.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/control_pictures.csv` & `rofimoji-6.3.0/src/picker/data/control_pictures.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/coptic.csv` & `rofimoji-6.3.0/src/picker/data/coptic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/coptic_epact_numbers.csv` & `rofimoji-6.3.0/src/picker/data/coptic_epact_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/counting_rod_numerals.csv` & `rofimoji-6.3.0/src/picker/data/counting_rod_numerals.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cuneiform.csv` & `rofimoji-6.3.0/src/picker/data/cuneiform.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cuneiform_numbers_and_punctuation.csv` & `rofimoji-6.3.0/src/picker/data/cuneiform_numbers_and_punctuation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/currency_symbols.csv` & `rofimoji-6.3.0/src/picker/data/currency_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cypriot_syllabary.csv` & `rofimoji-6.3.0/src/picker/data/cypriot_syllabary.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cypro-minoan.csv` & `rofimoji-6.3.0/src/picker/data/cypro-minoan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cyrillic.csv` & `rofimoji-6.3.0/src/picker/data/cyrillic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cyrillic_extended-a.csv` & `rofimoji-6.3.0/src/picker/data/cyrillic_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cyrillic_extended-b.csv` & `rofimoji-6.3.0/src/picker/data/cyrillic_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cyrillic_extended-d.csv` & `rofimoji-6.3.0/src/picker/data/cyrillic_extended-d.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/cyrillic_supplement.csv` & `rofimoji-6.3.0/src/picker/data/cyrillic_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/deseret.csv` & `rofimoji-6.3.0/src/picker/data/deseret.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/devanagari.csv` & `rofimoji-6.3.0/src/picker/data/devanagari.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/devanagari_extended.csv` & `rofimoji-6.3.0/src/picker/data/devanagari_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/dingbats.csv` & `rofimoji-6.3.0/src/picker/data/dingbats.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/dives_akuru.csv` & `rofimoji-6.3.0/src/picker/data/dives_akuru.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/dogra.csv` & `rofimoji-6.3.0/src/picker/data/dogra.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/domino_tiles.csv` & `rofimoji-6.3.0/src/picker/data/domino_tiles.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/duployan.csv` & `rofimoji-6.3.0/src/picker/data/duployan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/early_dynastic_cuneiform.csv` & `rofimoji-6.3.0/src/picker/data/early_dynastic_cuneiform.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/egyptian_hieroglyph_format_controls.csv` & `rofimoji-6.3.0/src/picker/data/egyptian_hieroglyph_format_controls.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/egyptian_hieroglyphs.csv` & `rofimoji-6.3.0/src/picker/data/egyptian_hieroglyphs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/elbasan.csv` & `rofimoji-6.3.0/src/picker/data/elbasan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/elymaic.csv` & `rofimoji-6.3.0/src/picker/data/elymaic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/emojis_activities.csv` & `rofimoji-6.3.0/src/picker/data/emojis_activities.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/emojis_animals_nature.csv` & `rofimoji-6.3.0/src/picker/data/emojis_animals_nature.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/emojis_flags.csv` & `rofimoji-6.3.0/src/picker/data/emojis_flags.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/emojis_food_drink.csv` & `rofimoji-6.3.0/src/picker/data/emojis_food_drink.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/emojis_objects.csv` & `rofimoji-6.3.0/src/picker/data/emojis_objects.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/emojis_people_body.csv` & `rofimoji-6.3.0/src/picker/data/emojis_people_body.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/emojis_smileys_emotion.csv` & `rofimoji-6.3.0/src/picker/data/emojis_smileys_emotion.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/emojis_symbols.csv` & `rofimoji-6.3.0/src/picker/data/emojis_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/emojis_travel_places.csv` & `rofimoji-6.3.0/src/picker/data/emojis_travel_places.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/emoticons.csv` & `rofimoji-6.3.0/src/picker/data/emoticons.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/enclosed_alphanumeric_supplement.csv` & `rofimoji-6.3.0/src/picker/data/enclosed_alphanumeric_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/enclosed_alphanumerics.csv` & `rofimoji-6.3.0/src/picker/data/enclosed_alphanumerics.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/enclosed_cjk_letters_and_months.csv` & `rofimoji-6.3.0/src/picker/data/enclosed_cjk_letters_and_months.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/enclosed_ideographic_supplement.csv` & `rofimoji-6.3.0/src/picker/data/enclosed_ideographic_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ethiopic.csv` & `rofimoji-6.3.0/src/picker/data/ethiopic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ethiopic_extended-a.csv` & `rofimoji-6.3.0/src/picker/data/ethiopic_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ethiopic_extended-b.csv` & `rofimoji-6.3.0/src/picker/data/ethiopic_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ethiopic_extended.csv` & `rofimoji-6.3.0/src/picker/data/ethiopic_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ethiopic_supplement.csv` & `rofimoji-6.3.0/src/picker/data/ethiopic_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/fontawesome6.csv` & `rofimoji-6.3.0/src/picker/data/fontawesome6.csv`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,15 @@
  fa-black-tie
  fa-blackberry
  fa-blender
  fa-blender-phone
  fa-blog
  fa-blogger
  fa-blogger-b
+ fa-bluesky
  fa-bluetooth
  fa-bluetooth-b
  fa-bold
  fa-bolt <small>(fa-zap)</small>
  fa-bolt-lightning
  fa-bomb
  fa-bone
@@ -211,14 +212,16 @@
  fa-box-archive <small>(fa-archive)</small>
  fa-box-open
  fa-box-tissue
  fa-boxes-packing
  fa-boxes-stacked <small>(fa-boxes, fa-boxes-alt)</small>
  fa-braille
  fa-brain
+ fa-brave
+ fa-brave-reverse
  fa-brazilian-real-sign
  fa-bread-slice
  fa-bridge
  fa-bridge-circle-check
  fa-bridge-circle-exclamation
  fa-bridge-circle-xmark
  fa-bridge-lock
@@ -762,14 +765,15 @@
  fa-goodreads-g
  fa-google
  fa-google-drive
  fa-google-pay
  fa-google-play
  fa-google-plus
  fa-google-plus-g
+ fa-google-scholar
  fa-google-wallet
  fa-gopuram
  fa-graduation-cap <small>(fa-mortar-board)</small>
  fa-gratipay
  fa-grav
 > fa-greater-than
  fa-greater-than-equal
@@ -948,23 +952,24 @@
  fa-jira
  fa-joget
  fa-joint
  fa-joomla
  fa-js
  fa-jsfiddle
  fa-jug-detergent
+ fa-jxl
 K fa-k
  fa-kaaba
  fa-kaggle
  fa-key
  fa-keybase
  fa-keyboard
  fa-keycdn
  fa-khanda
- fa-kickstarter
+ fa-kickstarter <small>(fa-square-kickstarter)</small>
  fa-kickstarter-k
  fa-kip-sign
  fa-kit-medical <small>(fa-first-aid)</small>
  fa-kitchen-set
  fa-kiwi-bird
  fa-korvue
 L fa-l
@@ -985,14 +990,15 @@
  fa-leanpub
  fa-left-long <small>(fa-long-arrow-alt-left)</small>
  fa-left-right <small>(fa-arrows-alt-h)</small>
  fa-lemon
  fa-less
 < fa-less-than
  fa-less-than-equal
+ fa-letterboxd
  fa-life-ring
  fa-lightbulb
  fa-line
  fa-lines-leaning
  fa-link <small>(fa-chain)</small>
  fa-link-slash <small>(fa-chain-broken, fa-chain-slash, fa-unlink)</small>
  fa-linkedin
@@ -1073,14 +1079,15 @@
  fa-microphone-lines <small>(fa-microphone-alt)</small>
  fa-microphone-lines-slash <small>(fa-microphone-alt-slash)</small>
  fa-microphone-slash
  fa-microscope
  fa-microsoft
  fa-mill-sign
  fa-minimize <small>(fa-compress-arrows-alt)</small>
+ fa-mintbit
  fa-minus <small>(fa-subtract)</small>
  fa-mitten
  fa-mix
  fa-mixcloud
  fa-mixer
  fa-mizuni
  fa-mobile <small>(fa-mobile-android, fa-mobile-phone)</small>
@@ -1141,14 +1148,15 @@
  fa-odysee
  fa-oil-can
  fa-oil-well
  fa-old-republic
  fa-om
  fa-opencart
  fa-openid
+ fa-opensuse
  fa-opera
  fa-optin-monster
  fa-orcid
  fa-osi
  fa-otter
  fa-outdent <small>(fa-dedent)</small>
 P fa-p
@@ -1253,14 +1261,15 @@
  fa-pied-piper-hat
  fa-pied-piper-pp
  fa-piggy-bank
  fa-pills
  fa-pinterest
  fa-pinterest-p
  fa-pix
+ fa-pixiv
  fa-pizza-slice
  fa-place-of-worship
  fa-plane
  fa-plane-arrival
  fa-plane-circle-check
  fa-plane-circle-exclamation
  fa-plane-circle-xmark
@@ -1401,40 +1410,42 @@
  fa-section
  fa-seedling <small>(fa-sprout)</small>
  fa-sellcast
  fa-sellsy
  fa-server
  fa-servicestack
  fa-shapes <small>(fa-triangle-circle-square)</small>
- fa-share <small>(fa-arrow-turn-right, fa-mail-forward)</small>
+ fa-share <small>(fa-mail-forward)</small>
  fa-share-from-square <small>(fa-share-square)</small>
  fa-share-nodes <small>(fa-share-alt)</small>
  fa-sheet-plastic
  fa-shekel-sign <small>(fa-ils, fa-shekel, fa-sheqel, fa-sheqel-sign)</small>
  fa-shield <small>(fa-shield-blank)</small>
  fa-shield-cat
  fa-shield-dog
  fa-shield-halved <small>(fa-shield-alt)</small>
  fa-shield-heart
  fa-shield-virus
  fa-ship
  fa-shirt <small>(fa-t-shirt, fa-tshirt)</small>
  fa-shirtsinbulk
  fa-shoe-prints
+ fa-shoelace
  fa-shop <small>(fa-store-alt)</small>
  fa-shop-lock
  fa-shop-slash <small>(fa-store-alt-slash)</small>
  fa-shopify
  fa-shopware
  fa-shower
  fa-shrimp
  fa-shuffle <small>(fa-random)</small>
  fa-shuttle-space <small>(fa-space-shuttle)</small>
  fa-sign-hanging <small>(fa-sign)</small>
  fa-signal <small>(fa-signal-5, fa-signal-perfect)</small>
+ fa-signal-messenger
  fa-signature
  fa-signs-post <small>(fa-map-signs)</small>
  fa-sim-card
  fa-simplybuilt
  fa-sink
  fa-sistrix
  fa-sitemap
@@ -1496,14 +1507,15 @@
  fa-square-gitlab <small>(fa-gitlab-square)</small>
  fa-square-google-plus <small>(fa-google-plus-square)</small>
  fa-square-h <small>(fa-h-square)</small>
  fa-square-hacker-news <small>(fa-hacker-news-square)</small>
  fa-square-instagram <small>(fa-instagram-square)</small>
  fa-square-js <small>(fa-js-square)</small>
  fa-square-lastfm <small>(fa-lastfm-square)</small>
+ fa-square-letterboxd
  fa-square-minus <small>(fa-minus-square)</small>
  fa-square-nfi
  fa-square-odnoklassniki <small>(fa-odnoklassniki-square)</small>
  fa-square-parking <small>(fa-parking)</small>
  fa-square-pen <small>(fa-pen-square, fa-pencil-square)</small>
  fa-square-person-confined
  fa-square-phone <small>(fa-phone-square)</small>
@@ -1519,17 +1531,20 @@
  fa-square-share-nodes <small>(fa-share-alt-square)</small>
  fa-square-snapchat <small>(fa-snapchat-square)</small>
  fa-square-steam <small>(fa-steam-square)</small>
  fa-square-threads
  fa-square-tumblr <small>(fa-tumblr-square)</small>
  fa-square-twitter <small>(fa-twitter-square)</small>
  fa-square-up-right <small>(fa-external-link-square-alt)</small>
+ fa-square-upwork
  fa-square-viadeo <small>(fa-viadeo-square)</small>
  fa-square-vimeo <small>(fa-vimeo-square)</small>
  fa-square-virus
+ fa-square-web-awesome
+ fa-square-web-awesome-stroke
  fa-square-whatsapp <small>(fa-whatsapp-square)</small>
  fa-square-x-twitter
  fa-square-xing <small>(fa-xing-square)</small>
  fa-square-xmark <small>(fa-times-square, fa-xmark-square)</small>
  fa-square-youtube <small>(fa-youtube-square)</small>
  fa-squarespace
  fa-stack-exchange
@@ -1580,15 +1595,17 @@
  fa-swift
  fa-symfony
  fa-synagogue
  fa-syringe
 T fa-t
  fa-table
  fa-table-cells <small>(fa-th)</small>
+ fa-table-cells-column-lock
  fa-table-cells-large <small>(fa-th-large)</small>
+ fa-table-cells-row-lock
  fa-table-columns <small>(fa-columns)</small>
  fa-table-list <small>(fa-th-list)</small>
  fa-table-tennis-paddle-ball <small>(fa-ping-pong-paddle-ball, fa-table-tennis)</small>
  fa-tablet <small>(fa-tablet-android)</small>
  fa-tablet-button
  fa-tablet-screen-button <small>(fa-tablet-alt)</small>
  fa-tablets
@@ -1712,14 +1729,15 @@
  fa-up-down <small>(fa-arrows-alt-v)</small>
  fa-up-down-left-right <small>(fa-arrows-alt)</small>
  fa-up-long <small>(fa-long-arrow-alt-up)</small>
  fa-up-right-and-down-left-from-center <small>(fa-expand-alt)</small>
  fa-up-right-from-square <small>(fa-external-link-alt)</small>
  fa-upload
  fa-ups
+ fa-upwork
  fa-usb
  fa-user
  fa-user-astronaut
  fa-user-check
  fa-user-clock
  fa-user-doctor <small>(fa-user-md)</small>
  fa-user-gear <small>(fa-user-cog)</small>
@@ -1798,14 +1816,16 @@
  fa-wand-sparkles
  fa-warehouse
  fa-watchman-monitoring
  fa-water
  fa-water-ladder <small>(fa-ladder-water, fa-swimming-pool)</small>
  fa-wave-square
  fa-waze
+ fa-web-awesome
+ fa-webflow
  fa-weebly
  fa-weibo
  fa-weight-hanging
  fa-weight-scale <small>(fa-weight)</small>
  fa-weixin
  fa-whatsapp
  fa-wheat-awn <small>(fa-wheat-alt)</small>
```

### Comparing `rofimoji-6.2.0/src/picker/data/general_punctuation.csv` & `rofimoji-6.3.0/src/picker/data/general_punctuation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/geometric_shapes.csv` & `rofimoji-6.3.0/src/picker/data/geometric_shapes.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/geometric_shapes_extended.csv` & `rofimoji-6.3.0/src/picker/data/geometric_shapes_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/georgian.csv` & `rofimoji-6.3.0/src/picker/data/georgian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/georgian_extended.csv` & `rofimoji-6.3.0/src/picker/data/georgian_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/georgian_supplement.csv` & `rofimoji-6.3.0/src/picker/data/georgian_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/gitmoji.csv` & `rofimoji-6.3.0/src/picker/data/gitmoji.csv`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 🚑 critical hotfix.
 ✨ introduce new features.
 📝 add or update documentation.
 🚀 deploy stuff.
 💄 add or update the ui and style files.
 🎉 begin a project.
 ✅ add, update, or pass tests.
-🔒 fix security issues.
+🔒 fix security or privacy issues.
 🔐 add or update secrets.
 🔖 release / version tags.
 🚨 fix compiler / linter warnings.
 🚧 work in progress.
 💚 fix ci build.
 ⬇ downgrade dependencies.
 ⬆ upgrade dependencies.
```

### Comparing `rofimoji-6.2.0/src/picker/data/glagolitic.csv` & `rofimoji-6.3.0/src/picker/data/glagolitic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/glagolitic_supplement.csv` & `rofimoji-6.3.0/src/picker/data/glagolitic_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/gothic.csv` & `rofimoji-6.3.0/src/picker/data/gothic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/grantha.csv` & `rofimoji-6.3.0/src/picker/data/grantha.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/greek_and_coptic.csv` & `rofimoji-6.3.0/src/picker/data/greek_and_coptic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/greek_extended.csv` & `rofimoji-6.3.0/src/picker/data/greek_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/gujarati.csv` & `rofimoji-6.3.0/src/picker/data/gujarati.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/gunjala_gondi.csv` & `rofimoji-6.3.0/src/picker/data/gunjala_gondi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/gurmukhi.csv` & `rofimoji-6.3.0/src/picker/data/gurmukhi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/halfwidth_and_fullwidth_forms.csv` & `rofimoji-6.3.0/src/picker/data/halfwidth_and_fullwidth_forms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/hangul_compatibility_jamo.csv` & `rofimoji-6.3.0/src/picker/data/hangul_compatibility_jamo.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/hangul_jamo.csv` & `rofimoji-6.3.0/src/picker/data/hangul_jamo.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/hangul_jamo_extended-a.csv` & `rofimoji-6.3.0/src/picker/data/hangul_jamo_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/hangul_jamo_extended-b.csv` & `rofimoji-6.3.0/src/picker/data/hangul_jamo_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/hanifi_rohingya.csv` & `rofimoji-6.3.0/src/picker/data/hanifi_rohingya.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/hanunoo.csv` & `rofimoji-6.3.0/src/picker/data/hanunoo.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/hatran.csv` & `rofimoji-6.3.0/src/picker/data/hatran.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/hebrew.csv` & `rofimoji-6.3.0/src/picker/data/hebrew.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/hiragana.csv` & `rofimoji-6.3.0/src/picker/data/hiragana.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ideographic_description_characters.csv` & `rofimoji-6.3.0/src/picker/data/ideographic_description_characters.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/imperial_aramaic.csv` & `rofimoji-6.3.0/src/picker/data/imperial_aramaic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/indic_siyaq_numbers.csv` & `rofimoji-6.3.0/src/picker/data/indic_siyaq_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/inscriptional_pahlavi.csv` & `rofimoji-6.3.0/src/picker/data/inscriptional_pahlavi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/inscriptional_parthian.csv` & `rofimoji-6.3.0/src/picker/data/inscriptional_parthian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ipa_extensions.csv` & `rofimoji-6.3.0/src/picker/data/ipa_extensions.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/javanese.csv` & `rofimoji-6.3.0/src/picker/data/javanese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/kaithi.csv` & `rofimoji-6.3.0/src/picker/data/kaithi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/kaktovik_numerals.csv` & `rofimoji-6.3.0/src/picker/data/kaktovik_numerals.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/kana_extended-a.csv` & `rofimoji-6.3.0/src/picker/data/kana_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/kana_extended-b.csv` & `rofimoji-6.3.0/src/picker/data/kana_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/kana_supplement.csv` & `rofimoji-6.3.0/src/picker/data/kana_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/kanbun.csv` & `rofimoji-6.3.0/src/picker/data/kanbun.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/kangxi_radicals.csv` & `rofimoji-6.3.0/src/picker/data/kangxi_radicals.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/kannada.csv` & `rofimoji-6.3.0/src/picker/data/kannada.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/katakana.csv` & `rofimoji-6.3.0/src/picker/data/katakana.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/kawi.csv` & `rofimoji-6.3.0/src/picker/data/kawi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/kayah_li.csv` & `rofimoji-6.3.0/src/picker/data/kayah_li.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/kharoshthi.csv` & `rofimoji-6.3.0/src/picker/data/kharoshthi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/khitan_small_script.csv` & `rofimoji-6.3.0/src/picker/data/khitan_small_script.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/khmer.csv` & `rofimoji-6.3.0/src/picker/data/khmer.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/khmer_symbols.csv` & `rofimoji-6.3.0/src/picker/data/khmer_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/khojki.csv` & `rofimoji-6.3.0/src/picker/data/khojki.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/khudawadi.csv` & `rofimoji-6.3.0/src/picker/data/khudawadi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/lao.csv` & `rofimoji-6.3.0/src/picker/data/lao.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/latin-1_supplement.csv` & `rofimoji-6.3.0/src/picker/data/latin-1_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/latin_extended-a.csv` & `rofimoji-6.3.0/src/picker/data/latin_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/latin_extended-b.csv` & `rofimoji-6.3.0/src/picker/data/latin_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/latin_extended-c.csv` & `rofimoji-6.3.0/src/picker/data/latin_extended-c.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/latin_extended-d.csv` & `rofimoji-6.3.0/src/picker/data/latin_extended-d.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/latin_extended-e.csv` & `rofimoji-6.3.0/src/picker/data/latin_extended-e.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/latin_extended-f.csv` & `rofimoji-6.3.0/src/picker/data/latin_extended-f.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/latin_extended-g.csv` & `rofimoji-6.3.0/src/picker/data/latin_extended-g.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/latin_extended_additional.csv` & `rofimoji-6.3.0/src/picker/data/latin_extended_additional.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/lepcha.csv` & `rofimoji-6.3.0/src/picker/data/lepcha.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/letterlike_symbols.csv` & `rofimoji-6.3.0/src/picker/data/letterlike_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/limbu.csv` & `rofimoji-6.3.0/src/picker/data/limbu.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/linear_a.csv` & `rofimoji-6.3.0/src/picker/data/linear_a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/linear_b_ideograms.csv` & `rofimoji-6.3.0/src/picker/data/linear_b_ideograms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/linear_b_syllabary.csv` & `rofimoji-6.3.0/src/picker/data/linear_b_syllabary.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/lisu.csv` & `rofimoji-6.3.0/src/picker/data/lisu.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/lycian.csv` & `rofimoji-6.3.0/src/picker/data/lycian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/lydian.csv` & `rofimoji-6.3.0/src/picker/data/lydian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/mahajani.csv` & `rofimoji-6.3.0/src/picker/data/mahajani.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/mahjong_tiles.csv` & `rofimoji-6.3.0/src/picker/data/mahjong_tiles.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/makasar.csv` & `rofimoji-6.3.0/src/picker/data/makasar.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/malayalam.csv` & `rofimoji-6.3.0/src/picker/data/malayalam.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/mandaic.csv` & `rofimoji-6.3.0/src/picker/data/mandaic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/manichaean.csv` & `rofimoji-6.3.0/src/picker/data/manichaean.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/marchen.csv` & `rofimoji-6.3.0/src/picker/data/marchen.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/masaram_gondi.csv` & `rofimoji-6.3.0/src/picker/data/masaram_gondi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/math.csv` & `rofimoji-6.3.0/src/picker/data/math.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/mathematical_alphanumeric_symbols.csv` & `rofimoji-6.3.0/src/picker/data/mathematical_alphanumeric_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/mathematical_operators.csv` & `rofimoji-6.3.0/src/picker/data/mathematical_operators.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/medefaidrin.csv` & `rofimoji-6.3.0/src/picker/data/medefaidrin.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/meetei_mayek.csv` & `rofimoji-6.3.0/src/picker/data/meetei_mayek.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/meetei_mayek_extensions.csv` & `rofimoji-6.3.0/src/picker/data/meetei_mayek_extensions.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/mende_kikakui.csv` & `rofimoji-6.3.0/src/picker/data/mende_kikakui.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/meroitic_cursive.csv` & `rofimoji-6.3.0/src/picker/data/meroitic_cursive.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/meroitic_hieroglyphs.csv` & `rofimoji-6.3.0/src/picker/data/meroitic_hieroglyphs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/miao.csv` & `rofimoji-6.3.0/src/picker/data/miao.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/miscellaneous_mathematical_symbols-a.csv` & `rofimoji-6.3.0/src/picker/data/miscellaneous_mathematical_symbols-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/miscellaneous_mathematical_symbols-b.csv` & `rofimoji-6.3.0/src/picker/data/miscellaneous_mathematical_symbols-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/miscellaneous_symbols.csv` & `rofimoji-6.3.0/src/picker/data/miscellaneous_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/miscellaneous_symbols_and_arrows.csv` & `rofimoji-6.3.0/src/picker/data/miscellaneous_symbols_and_arrows.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/miscellaneous_symbols_and_pictographs.csv` & `rofimoji-6.3.0/src/picker/data/miscellaneous_symbols_and_pictographs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/miscellaneous_technical.csv` & `rofimoji-6.3.0/src/picker/data/miscellaneous_technical.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/modi.csv` & `rofimoji-6.3.0/src/picker/data/modi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/modifier_tone_letters.csv` & `rofimoji-6.3.0/src/picker/data/modifier_tone_letters.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/mongolian.csv` & `rofimoji-6.3.0/src/picker/data/mongolian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/mongolian_supplement.csv` & `rofimoji-6.3.0/src/picker/data/mongolian_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/mro.csv` & `rofimoji-6.3.0/src/picker/data/mro.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/multani.csv` & `rofimoji-6.3.0/src/picker/data/multani.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/musical_symbols.csv` & `rofimoji-6.3.0/src/picker/data/musical_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/myanmar.csv` & `rofimoji-6.3.0/src/picker/data/myanmar.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/myanmar_extended-a.csv` & `rofimoji-6.3.0/src/picker/data/myanmar_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/myanmar_extended-b.csv` & `rofimoji-6.3.0/src/picker/data/myanmar_extended-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/nabataean.csv` & `rofimoji-6.3.0/src/picker/data/nabataean.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/nag_mundari.csv` & `rofimoji-6.3.0/src/picker/data/nag_mundari.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/nandinagari.csv` & `rofimoji-6.3.0/src/picker/data/nandinagari.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/nerd_font.csv` & `rofimoji-6.3.0/src/picker/data/nerd_font.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/new_tai_lue.csv` & `rofimoji-6.3.0/src/picker/data/new_tai_lue.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/newa.csv` & `rofimoji-6.3.0/src/picker/data/newa.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/nko.csv` & `rofimoji-6.3.0/src/picker/data/nko.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/number_forms.csv` & `rofimoji-6.3.0/src/picker/data/number_forms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/nushu.csv` & `rofimoji-6.3.0/src/picker/data/nushu.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/nyiakeng_puachue_hmong.csv` & `rofimoji-6.3.0/src/picker/data/nyiakeng_puachue_hmong.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ogham.csv` & `rofimoji-6.3.0/src/picker/data/ogham.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ol_chiki.csv` & `rofimoji-6.3.0/src/picker/data/ol_chiki.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/old_hungarian.csv` & `rofimoji-6.3.0/src/picker/data/old_hungarian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/old_italic.csv` & `rofimoji-6.3.0/src/picker/data/old_italic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/old_north_arabian.csv` & `rofimoji-6.3.0/src/picker/data/old_north_arabian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/old_permic.csv` & `rofimoji-6.3.0/src/picker/data/old_permic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/old_persian.csv` & `rofimoji-6.3.0/src/picker/data/old_persian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/old_sogdian.csv` & `rofimoji-6.3.0/src/picker/data/old_sogdian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/old_south_arabian.csv` & `rofimoji-6.3.0/src/picker/data/old_south_arabian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/old_turkic.csv` & `rofimoji-6.3.0/src/picker/data/old_turkic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/old_uyghur.csv` & `rofimoji-6.3.0/src/picker/data/old_uyghur.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/oriya.csv` & `rofimoji-6.3.0/src/picker/data/oriya.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ornamental_dingbats.csv` & `rofimoji-6.3.0/src/picker/data/ornamental_dingbats.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/osage.csv` & `rofimoji-6.3.0/src/picker/data/osage.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/osmanya.csv` & `rofimoji-6.3.0/src/picker/data/osmanya.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ottoman_siyaq_numbers.csv` & `rofimoji-6.3.0/src/picker/data/ottoman_siyaq_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/pahawh_hmong.csv` & `rofimoji-6.3.0/src/picker/data/pahawh_hmong.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/palmyrene.csv` & `rofimoji-6.3.0/src/picker/data/palmyrene.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/pau_cin_hau.csv` & `rofimoji-6.3.0/src/picker/data/pau_cin_hau.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/phags-pa.csv` & `rofimoji-6.3.0/src/picker/data/phags-pa.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/phaistos_disc.csv` & `rofimoji-6.3.0/src/picker/data/phaistos_disc.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/phoenician.csv` & `rofimoji-6.3.0/src/picker/data/phoenician.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/phonetic_extensions.csv` & `rofimoji-6.3.0/src/picker/data/phonetic_extensions.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/phonetic_extensions_supplement.csv` & `rofimoji-6.3.0/src/picker/data/phonetic_extensions_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/playing_cards.csv` & `rofimoji-6.3.0/src/picker/data/playing_cards.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/psalter_pahlavi.csv` & `rofimoji-6.3.0/src/picker/data/psalter_pahlavi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/rejang.csv` & `rofimoji-6.3.0/src/picker/data/rejang.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/rumi_numeral_symbols.csv` & `rofimoji-6.3.0/src/picker/data/rumi_numeral_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/runic.csv` & `rofimoji-6.3.0/src/picker/data/runic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/samaritan.csv` & `rofimoji-6.3.0/src/picker/data/samaritan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/saurashtra.csv` & `rofimoji-6.3.0/src/picker/data/saurashtra.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/sharada.csv` & `rofimoji-6.3.0/src/picker/data/sharada.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/shavian.csv` & `rofimoji-6.3.0/src/picker/data/shavian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/siddham.csv` & `rofimoji-6.3.0/src/picker/data/siddham.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/sinhala.csv` & `rofimoji-6.3.0/src/picker/data/sinhala.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/sinhala_archaic_numbers.csv` & `rofimoji-6.3.0/src/picker/data/sinhala_archaic_numbers.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/small_form_variants.csv` & `rofimoji-6.3.0/src/picker/data/small_form_variants.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/sogdian.csv` & `rofimoji-6.3.0/src/picker/data/sogdian.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/sora_sompeng.csv` & `rofimoji-6.3.0/src/picker/data/sora_sompeng.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/soyombo.csv` & `rofimoji-6.3.0/src/picker/data/soyombo.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/spacing_modifier_letters.csv` & `rofimoji-6.3.0/src/picker/data/spacing_modifier_letters.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/sundanese.csv` & `rofimoji-6.3.0/src/picker/data/sundanese.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/superscripts_and_subscripts.csv` & `rofimoji-6.3.0/src/picker/data/superscripts_and_subscripts.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/supplemental_arrows-a.csv` & `rofimoji-6.3.0/src/picker/data/supplemental_arrows-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/supplemental_arrows-b.csv` & `rofimoji-6.3.0/src/picker/data/supplemental_arrows-b.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/supplemental_arrows-c.csv` & `rofimoji-6.3.0/src/picker/data/supplemental_arrows-c.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/supplemental_mathematical_operators.csv` & `rofimoji-6.3.0/src/picker/data/supplemental_mathematical_operators.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/supplemental_punctuation.csv` & `rofimoji-6.3.0/src/picker/data/supplemental_punctuation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/supplemental_symbols_and_pictographs.csv` & `rofimoji-6.3.0/src/picker/data/supplemental_symbols_and_pictographs.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/sutton_signwriting.csv` & `rofimoji-6.3.0/src/picker/data/sutton_signwriting.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/syloti_nagri.csv` & `rofimoji-6.3.0/src/picker/data/syloti_nagri.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/symbols_and_pictographs_extended-a.csv` & `rofimoji-6.3.0/src/picker/data/symbols_and_pictographs_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/symbols_for_legacy_computing.csv` & `rofimoji-6.3.0/src/picker/data/symbols_for_legacy_computing.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/syriac.csv` & `rofimoji-6.3.0/src/picker/data/syriac.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tagalog.csv` & `rofimoji-6.3.0/src/picker/data/tagalog.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tags.csv` & `rofimoji-6.3.0/src/picker/data/tags.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tai_le.csv` & `rofimoji-6.3.0/src/picker/data/tai_le.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tai_tham.csv` & `rofimoji-6.3.0/src/picker/data/tai_tham.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tai_viet.csv` & `rofimoji-6.3.0/src/picker/data/tai_viet.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tai_xuan_jing_symbols.csv` & `rofimoji-6.3.0/src/picker/data/tai_xuan_jing_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/takri.csv` & `rofimoji-6.3.0/src/picker/data/takri.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tamil.csv` & `rofimoji-6.3.0/src/picker/data/tamil.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tamil_supplement.csv` & `rofimoji-6.3.0/src/picker/data/tamil_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tangsa.csv` & `rofimoji-6.3.0/src/picker/data/tangsa.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tangut_components.csv` & `rofimoji-6.3.0/src/picker/data/tangut_components.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/telugu.csv` & `rofimoji-6.3.0/src/picker/data/telugu.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/thaana.csv` & `rofimoji-6.3.0/src/picker/data/thaana.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/thai.csv` & `rofimoji-6.3.0/src/picker/data/thai.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tibetan.csv` & `rofimoji-6.3.0/src/picker/data/tibetan.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tifinagh.csv` & `rofimoji-6.3.0/src/picker/data/tifinagh.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/tirhuta.csv` & `rofimoji-6.3.0/src/picker/data/tirhuta.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/toto.csv` & `rofimoji-6.3.0/src/picker/data/toto.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/transport_and_map_symbols.csv` & `rofimoji-6.3.0/src/picker/data/transport_and_map_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/ugaritic.csv` & `rofimoji-6.3.0/src/picker/data/ugaritic.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/unified_canadian_aboriginal_syllabics.csv` & `rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended-a.csv` & `rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended-a.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended.csv` & `rofimoji-6.3.0/src/picker/data/unified_canadian_aboriginal_syllabics_extended.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/vai.csv` & `rofimoji-6.3.0/src/picker/data/vai.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/variation_selectors_supplement.csv` & `rofimoji-6.3.0/src/picker/data/variation_selectors_supplement.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/vedic_extensions.csv` & `rofimoji-6.3.0/src/picker/data/vedic_extensions.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/vertical_forms.csv` & `rofimoji-6.3.0/src/picker/data/vertical_forms.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/vithkuqi.csv` & `rofimoji-6.3.0/src/picker/data/vithkuqi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/wancho.csv` & `rofimoji-6.3.0/src/picker/data/wancho.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/warang_citi.csv` & `rofimoji-6.3.0/src/picker/data/warang_citi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/yezidi.csv` & `rofimoji-6.3.0/src/picker/data/yezidi.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/yi_radicals.csv` & `rofimoji-6.3.0/src/picker/data/yi_radicals.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/yi_syllables.csv` & `rofimoji-6.3.0/src/picker/data/yi_syllables.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/yijing_hexagram_symbols.csv` & `rofimoji-6.3.0/src/picker/data/yijing_hexagram_symbols.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/zanabazar_square.csv` & `rofimoji-6.3.0/src/picker/data/zanabazar_square.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/data/znamenny_musical_notation.csv` & `rofimoji-6.3.0/src/picker/data/znamenny_musical_notation.csv`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/docs/rofimoji.1` & `rofimoji-6.3.0/src/picker/docs/rofimoji.1`

 * *Files 16% similar despite different names*

```diff
@@ -1,109 +1,118 @@
-.\" Automatically generated by Pandoc 3.1.8
+.\" Automatically generated by Pandoc 3.1.12.2
 .\"
-.TH "ROFIMOJI" "1" "September 16, 2023" "Version 6.2.0" "Rofi Third-party Add-on Documentation"
+.TH "ROFIMOJI" "1" "May 01, 2024" "Version 6.3.0" "Rofi Third\-party Add\-on Documentation"
 .SH NAME
-\f[B]rofimoji\f[R] - A character (emoji) picker for rofi
+\f[B]rofimoji\f[R] \- An emoji and general character picker for rofi and
+rofi\-likes
 .SH SYNOPSIS
 .PP
-\f[B]rofimoji\f[R] [\f[B]-h\f[R]] [\f[B]--version\f[R]]
-[\f[B]--action\f[R]
-{\f[I]type\f[R],\f[I]copy\f[R],\f[I]clipboard\f[R],\f[I]unicode\f[R],\f[I]copy-unicode\f[R],\f[I]print\f[R],\f[I]menu\f[R]}]
-[\f[B]--skin-tone\f[R]
-{\f[I]neutral\f[R],\f[I]light\f[R],\f[I]medium-light\f[R],\f[I]moderate\f[R],\f[I]dark
-brown\f[R],\f[I]black\f[R],\f[I]ask\f[R]}] [\f[B]--files\f[R]
+\f[B]rofimoji\f[R] [\f[B]\-h\f[R]] [\f[B]\-\-version\f[R]]
+[\f[B]\-\-action\f[R]
+{\f[I]type\f[R],\f[I]copy\f[R],\f[I]clipboard\f[R],\f[I]unicode\f[R],\f[I]copy\-unicode\f[R],\f[I]print\f[R],\f[I]menu\f[R]}]
+[\f[B]\-\-skin\-tone\f[R]
+{\f[I]neutral\f[R],\f[I]light\f[R],\f[I]medium\-light\f[R],\f[I]moderate\f[R],\f[I]dark
+brown\f[R],\f[I]black\f[R],\f[I]ask\f[R]}] [\f[B]\-\-files\f[R]
 {\f[I]all\f[R],\f[I]FILE\f[R] [\f[I]FILE\f[R] \&...]]}
-[\f[B]--prompt\f[R] \f[I]PROMPT\f[R]] [\f[B]--selector-args\f[R]
-\f[I]SELECTOR_ARGS\f[R]] [\f[B]--max-recent\f[R] \f[I]MAX_RECENT\f[R]]
-[\f[B]--no-frecency\f[R]] [\f[B]--hidden-descriptions\f[R]]
-[\f[B]--clipboarder\f[R] \f[I]CLIPBOARDER\f[R]] [\f[B]--typer\f[R]
-\f[I]TYPER\f[R]] [\f[B]--selector\f[R] \f[I]SELECTOR\f[R]]
+[\f[B]\-\-prompt\f[R] \f[I]PROMPT\f[R]] [\f[B]\-\-selector\-args\f[R]
+\f[I]SELECTOR_ARGS\f[R]] [\f[B]\-\-max\-recent\f[R]
+\f[I]MAX_RECENT\f[R]] [\f[B]\-\-no\-frecency\f[R]]
+[\f[B]\-\-hidden\-descriptions\f[R]] [\f[B]\-\-clipboarder\f[R]
+\f[I]CLIPBOARDER\f[R]] [\f[B]\-\-typer\f[R] \f[I]TYPER\f[R]]
+[\f[B]\-\-selector\f[R] \f[I]SELECTOR\f[R]]
 .SH DESCRIPTION
 Select, insert, or copy Unicode characters like emoji using rofi.
 .SH OPTIONS
 .TP
--h, --help
+\-h, \-\-help
 Prints brief usage information.
 .TP
---version
+\-\-version
 show program\[cq]s version number and exit
 .TP
---action, -a
-Possible values: type, copy, clipboard, unicode, copy-unicode, print,
+\-\-action, \-a
+Possible values: type, copy, clipboard, unicode, copy\-unicode, print,
 menu
 .RS
 .PP
 Choose what to do with the selected characters: Directly type them with
 the \[lq]Typer\[rq], copy them to the clipboard using the
 \[lq]Clipboarder\[rq], or insert them indirectly using the clipboard.
 \[lq]unicode\[rq] will type the unicode codepoints of the chosen
-characters, \[lq]copy-unicode\[rq] will copy it.
+characters, \[lq]copy\-unicode\[rq] will copy it.
 \[lq]print\[rq] just outputs them on stdout.
 If you want to decide on the fly, use \[lq]menu\[rq].
 .RE
 .TP
---skin-tone=\f[I]skin-tone\f[R], -s \f[I]skin-tone\f[R]
-Possible values: neutral, light, medium-light, moderate, dark brown,
-black, ask
-.RS
-.PP
-Decide on a skin-tone for all supported emojis.
-If not set (or set to \[lq]ask\[rq]), you will be asked for each one
-.RE
-.TP
---files \f[I]FILE\f[R] [\f[I]FILE\f[R] \&...], -f \f[I]FILE\f[R] [\f[I]FILE\f[R] \&...]
+\-\-files \f[I]FILE\f[R] [\f[I]FILE\f[R] \&...], \-f \f[I]FILE\f[R] [\f[I]FILE\f[R] \&...]
 Read characters from this file (or these files), one entry per line.
 Absolute and relative paths are supported, as is globbing
-(\f[CR]--files /home/you/characters.csv ../other*.csv\f[R]).
+(\f[CR]\-\-files /home/you/characters.csv ../other*.csv\f[R]).
 A filename without extension is enough
-(\f[CR]--files musical_symbols supplemental_arrows\f[R]) for included
+(\f[CR]\-\-files musical_symbols supplemental_arrows\f[R]) for included
 character files and all in \f[CR]${XDG_DATA_HOME}/rofimoji/data\f[R].
 Here, too, globbing is supported and done by default.
 In the config file, several files need to be listed as
 \f[CR]files=[_FILE_, _FILE_]\f[R].
 .TP
---prompt \f[I]PROMPT\f[R], -r \f[I]PROMPT\f[R]
-Set rofimoji\[cq]s prompt
-.TP
---selector-args \f[I]SELECTOR-ARGS\f[R]
-A string of arguments to give to the selector.
+\-\-skin\-tone=\f[I]skin\-tone\f[R], \-s \f[I]skin\-tone\f[R]
+Possible values: neutral, light, medium\-light, moderate, dark brown,
+black, ask
+.RS
+.PP
+Decide on a skin\-tone for all supported emojis.
+If not set (or set to \[lq]ask\[rq]), you will be asked for each one
+.RE
 .TP
---max-recent \f[I]MAX-RECENT\f[R]
+\-\-max\-recent \f[I]MAX\-RECENT\f[R]
 Show at most this number of recently used characters (cannot be larger
 than 10)
 .TP
---no-frecency
+\-\-no\-frecency
 Don\[cq]t show frequently used characters at the start.
 .TP
---hidden-descriptions
+\-\-hidden\-descriptions
 Only list the characters, but not their description.
 Note that you can still search through the descriptions.
+Only used for \f[CR]rofi\f[R].
 .TP
---clipboarder \f[I]CLIPBOARDER\f[R]
-Possible values: xsel, xclip, wl-copy
+\-\-use\-icons
+Show characters as icons on \f[CR]rofi\f[R].
+Not used with other selectors.
+.TP
+\-\-prompt \f[I]PROMPT\f[R], \-r \f[I]PROMPT\f[R]
+Set rofimoji\[cq]s prompt
+.TP
+\-\-selector\-args \f[I]SELECTOR\-ARGS\f[R]
+A string of arguments to give to the selector.
+.TP
+\-\-selector \f[I]SELECTOR\f[R]
+Possible values: rofi, wofi, fuzzel, dmenu, tofi, bemenu, wmenu
 .RS
 .PP
-Choose the application to access the clipboard with manually.
+Choose the selector application manually.
+Usually \f[CR]rofi\f[R], but you may want something else.
 .RE
 .TP
---typer \f[I]TYPER\f[R]
-Possible values: xdotool, wtype
+\-\-clipboarder \f[I]CLIPBOARDER\f[R]
+Possible values: xsel, xclip, wl\-copy
 .RS
 .PP
-Choose the application to type with manually.
+Choose the application to access the clipboard with manually.
 .RE
 .TP
---selector \f[I]SELECTOR\f[R]
-Possible values: rofi, wofi, fuzzel, dmenu
+\-\-typer \f[I]TYPER\f[R]
+Possible values: xdotool, wtype
 .RS
 .PP
-Choose the selector application manually.
-Usually \f[CR]rofi\f[R], but for Wayland, you may want \f[CR]wofi\f[R]
-or \f[CR]fuzzel\f[R].
+Choose the application to type with manually.
 .RE
+.TP
+\-\-keybinding\-copy, \-\-keybinding\-type, \-\-keybinding\-clipboard, \-\-keybinding\-unicode, \-\-keybinding\-copy\-unicode
+Define different keybindings for these actions.
 .SH KEYBINDINGS
 (optional) Select multiple emoji with shift+enter
 .PP
 \f[I]enter\f[R] to insert the emoji directly
 .PP
 \f[I]alt+c\f[R] to copy it to the clipboard
 .PP
@@ -119,31 +128,31 @@
 \f[I]alt+i\f[R] to copy the Unicode codepoint to the clipboard
 .PP
 Please note that wofi does not support keybindings other than
 \f[I]enter\f[R].
 .SH FILES
 .TP
 \f[I]\[ti]/.config/rofimoji.rc\f[R]
-Per-user configuration file.
+Per\-user configuration file.
 .TP
-\f[I]/etc/xdg/xdg-i3/rofimoji.rc\f[R]
+\f[I]/etc/xdg/xdg\-i3/rofimoji.rc\f[R]
 Global configuration file.
 .TP
 \f[I]\[ti]/.local/share/rofimoji/recent\f[R]
 Stores the recently used characters
 .TP
 \f[I]\[ti]/.local/share/rofimoji/data/\f[BI]filename\f[I].additional.csv\f[R]
 Contains additional characters or additional descriptions for the
 character set in \f[B]filename\f[R]
 .SH CONFIGURATION
-Args that start with \[lq]--\[rq] (eg.
---version) can also be set in a config file.
+Args that start with \[lq]\-\-\[rq] (eg.
+\-\-version) can also be set in a config file.
 .PP
 Config file syntax allows: key=value, flag=true, stuff=[a,b,c] (for
 details, see syntax at
-https://github.com/fdw/rofimoji#example-config-file).
+https://github.com/fdw/rofimoji#example\-config\-file).
 If an arg is specified in more than one place, then commandline values
 override values from the config file.
 .SH WEBSITE
 https://github.com/fdw/rofimoji
 .SH AUTHORS
 Fabian Winter.
```

### Comparing `rofimoji-6.2.0/src/picker/docs/rofimoji.1.md` & `rofimoji-6.3.0/src/picker/docs/rofimoji.1.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-% ROFIMOJI(1) Version 6.2.0 | Rofi Third-party Add-on Documentation
+% ROFIMOJI(1) Version 6.3.0 | Rofi Third-party Add-on Documentation
 % Fabian Winter
-% September 16, 2023
+% May 01, 2024
 
 # NAME
 
 
-**rofimoji** \- A character (emoji) picker for rofi
+**rofimoji** \- An emoji and general character picker for rofi and rofi-likes
 
 # SYNOPSIS
 
 | **rofimoji** \[**-h**] \[**\--version**] \[**\--action** {*type*,*copy*,*clipboard*,*unicode*,*copy-unicode*,*print*,*menu*}]
          \[**\--skin-tone** {*neutral*,*light*,*medium-light*,*moderate*,*dark brown*,*black*,*ask*}]
          \[**\--files** {*all*,*FILE* \[*FILE* ...]]} \[**\--prompt** *PROMPT*]
          \[**\--selector-args** *SELECTOR_ARGS*] \[**\--max-recent** *MAX_RECENT*] \[**\--no-frecency**] \[**\--hidden-descriptions**]
@@ -32,65 +32,74 @@
 \--action, -a
 
 : Possible values: type, copy, clipboard, unicode, copy-unicode, print, menu
 
       Choose what to do with the selected characters: Directly type them with the "Typer", copy them to the clipboard using the "Clipboarder", or insert them indirectly using the clipboard. "unicode" will type the unicode codepoints of the chosen characters, "copy-unicode" will copy it. "print" just outputs them on stdout.
       If you want to decide on the fly, use "menu".
 
-\--skin-tone=_skin-tone_, -s _skin-tone_
-
-: Possible values: neutral, light, medium-light, moderate, dark brown, black, ask
-
-      Decide on a skin-tone for all supported emojis. If not
-      set (or set to "ask"), you will be asked for each one
-
 \--files _FILE_ [_FILE_ ...], -f _FILE_ [_FILE_ ...]
 
 :  Read characters from this file (or these files), one entry per line. Absolute and relative paths are supported, as is globbing (`--files /home/you/characters.csv ../other*.csv`).
 :  A filename without extension is enough (`--files musical_symbols supplemental_arrows`) for included character files and all in `${XDG_DATA_HOME}/rofimoji/data`. Here, too, globbing is supported and done by default.
 :  In the config file, several files need to be listed as `files=[_FILE_, _FILE_]`.
 
-\--prompt _PROMPT_, -r _PROMPT_
-
-:  Set rofimoji's prompt
+\--skin-tone=_skin-tone_, -s _skin-tone_
 
-\--selector-args _SELECTOR-ARGS_
+: Possible values: neutral, light, medium-light, moderate, dark brown, black, ask
 
-:  A string of arguments to give to the selector.
+      Decide on a skin-tone for all supported emojis. If not
+      set (or set to "ask"), you will be asked for each one
 
 \--max-recent _MAX-RECENT_
 
-:  Show at most this number of recently used characters
+: Show at most this number of recently used characters
    (cannot be larger than 10)
 
 \--no-frecency
 
-:  Don't show frequently used characters at the start.
+: Don't show frequently used characters at the start.
 
 \--hidden-descriptions
 
-:  Only list the characters, but not their description. Note that you can still search through the descriptions.
+: Only list the characters, but not their description. Note that you can still search through the descriptions. Only used for `rofi`.
+
+\--use-icons
+
+: Show characters as icons on `rofi`. Not used with other selectors.
+
+\--prompt _PROMPT_, -r _PROMPT_
+
+: Set rofimoji's prompt
+
+\--selector-args _SELECTOR-ARGS_
+
+: A string of arguments to give to the selector.
+
+\--selector _SELECTOR_
+
+: Possible values: rofi, wofi, fuzzel, dmenu, tofi, bemenu, wmenu
+
+      Choose the selector application manually. Usually `rofi`, but you may want something else.
 
 \--clipboarder _CLIPBOARDER_
 
 : Possible values: xsel, xclip, wl-copy
 
       Choose the application to access the clipboard with manually.
 
 \--typer _TYPER_
 
 : Possible values: xdotool, wtype
 
       Choose the application to type with manually.
 
-\--selector _SELECTOR_
+\--keybinding-copy, \--keybinding-type, \--keybinding-clipboard, \--keybinding-unicode, \--keybinding-copy-unicode
 
-: Possible values: rofi, wofi, fuzzel, dmenu
+: Define different keybindings for these actions.
 
-      Choose the selector application manually. Usually `rofi`, but for Wayland, you may want `wofi` or `fuzzel`.
 
 # KEYBINDINGS
 
 (optional) Select multiple emoji with shift+enter
 
 *enter* to insert the emoji directly
```

### Comparing `rofimoji-6.2.0/src/picker/emoji_data.py` & `rofimoji-6.3.0/src/picker/emoji_data.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/file_loader.py` & `rofimoji-6.3.0/src/picker/file_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 from glob import glob
 from typing import Dict, List
 
+from .models import CharacterEntry
 from .paths import *
 
 
-def read_characters_from_files(files: List[str], frecent: List[str], use_additional: bool) -> Dict[str, str]:
-    all_characters: Dict[str, List[str]] = {}
+def read_characters_from_files(files: List[str], frecent: List[str], use_additional: bool) -> List[CharacterEntry]:
+    all_characters: Dict[str, CharacterEntry] = {}
 
     for character in frecent:
-        all_characters[character] = []
+        all_characters[character] = CharacterEntry(character)
 
     for file in __resolve_all_filenames(files, use_additional):
         characters_from_file = __load_from_file(file)
-        for line in characters_from_file:
-            parsed_line = line.split(" ", 1)
-            all_characters.setdefault(parsed_line[0], []).append(parsed_line[1]) if 1 < len(parsed_line) else ""
+        for character_entry in characters_from_file:
+            all_characters.setdefault(character_entry.character, character_entry)
 
-    return {character: ", ".join(descriptions) for character, descriptions in all_characters.items()}
+    return list(all_characters.values())
 
 
 def __resolve_all_filenames(file_names: List[str], use_additional: bool) -> List[Path]:
     resolved_file_names = []
     for file_name in file_names:
         resolved_file_names += __resolve_filename(file_name, use_additional)
 
     return resolved_file_names
 
 
 def __resolve_filename(file_name: str, use_additional: bool) -> List[Path]:
     resolved_file_names = []
 
-    for file in glob(os.path.expanduser(file_name)):
-        resolved_file_names.append(Path(file))
+    for absolute_file in glob(os.path.expanduser(file_name)):
+        resolved_file_names.append(Path(absolute_file))
 
     if resolved_file_names:
         return resolved_file_names
 
-    for file in custom_additional_files_location.glob(file_name if "*" in file_name else f"{file_name}*"):
-        if not file.name.endswith(".additional.csv"):
-            resolved_file_names.append(file)
+    for custom_files in custom_additional_files_location.glob(file_name if "*" in file_name else f"{file_name}*"):
+        if not custom_files.name.endswith(".additional.csv"):
+            resolved_file_names.append(custom_files)
 
     if resolved_file_names:
         return resolved_file_names
 
-    for file in (Path(__file__).parent / "data").glob(file_name if "*" in file_name else f"{file_name}*"):
-        resolved_file_names.append(file)
-        resolved_file_names += __load_additional_files(file, use_additional)
+    for distributed_file in (Path(__file__).parent / "data").glob(file_name if "*" in file_name else f"{file_name}*"):
+        resolved_file_names.append(distributed_file)
+        resolved_file_names += __load_additional_files(distributed_file, use_additional)
 
     if resolved_file_names:
         return resolved_file_names
 
     if file_name == "all":
         nested_file_names = [
             __resolve_filename(file.stem, use_additional) for file in (Path(__file__).parent / "data").glob("*.csv")
@@ -68,9 +68,16 @@
     provided_additional_file = Path(__file__).parent / "data" / "additional" / f"{original_file.stem}.csv"
     if use_additional and provided_additional_file.is_file():
         additional_files.append(provided_additional_file)
 
     return additional_files
 
 
-def __load_from_file(file: Path) -> List[str]:
-    return file.read_text().strip("\n").split("\n")
+def __load_from_file(file: Path) -> List[CharacterEntry]:
+    lines = file.read_text().strip("\n").split("\n")
+
+    all_character_entries = []
+    for line in lines:
+        parsed_line = line.split(" ", 1)
+        all_character_entries.append(CharacterEntry(parsed_line[0], parsed_line[1]))
+
+    return all_character_entries
```

### Comparing `rofimoji-6.2.0/src/picker/frecent.py` & `rofimoji-6.3.0/src/picker/frecent.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,11 +27,11 @@
     new_file_name.parent.mkdir(parents=True, exist_ok=True)
 
     frecencies = __load_frecent_characters()
 
     frecencies[chosen_character] = frecencies.get(chosen_character, 0) + 1.1
 
     with new_file_name.open("w+") as new_file:
-        for (character, frecency) in sorted(frecencies.items(), key=lambda item: item[1], reverse=True):
+        for character, frecency in sorted(frecencies.items(), key=lambda item: item[1], reverse=True):
             new_file.write(f"{math.floor(frecency)} {character}\n")
 
     new_file_name.rename(frecency_file_location)
```

### Comparing `rofimoji-6.2.0/src/picker/mode.py` & `rofimoji-6.3.0/src/picker/mode.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from . import emoji_data
 from .action import execute_action
 from .argument_parsing import parse_arguments_flexible
 from .clipboarder.clipboarder import Clipboarder
 from .file_loader import read_characters_from_files
 from .frecent import load_frecent_characters, save_frecent_characters
-from .models import Action
+from .models import Action, CharacterEntry
 from .paths import *
 from .recent import load_recent_characters, save_recent_characters
 from .typer.typer import Typer
 
 
 class Step(IntEnum):
     SHOW_ALL = auto()
@@ -87,15 +87,15 @@
     clipboarder: Clipboarder
 
     def mode(self) -> None:
         if os.environ.get("ROFI_RETV") == "0":
             State.remove_cache()
 
         chosen = sys.argv[-1]
-        state = State.load_from_cache(chosen, int(os.environ.get("ROFI_RETV")))
+        state = State.load_from_cache(chosen, int(os.environ.get("ROFI_RETV", "")))
         self.__parse_args()
         state.actions = self.args.actions
 
         if state.step == Step.SHOW_ALL:
             self.show_characters(state)
         if state.step == Step.SHORTCUTS:
             self.handle_shortcuts(state)
@@ -115,15 +115,17 @@
 
     def __parse_args(self) -> None:
         self.args = parse_arguments_flexible()
         self.typer = Typer.best_option(self.args.typer)
         self.clipboarder = Clipboarder.best_option(self.args.clipboarder)
 
     def show_characters(self, state: State) -> None:
-        recent_characters = self.__format_recent_characters(load_recent_characters(self.args.max_recent))
+        recent_characters = self.__format_recent_characters(
+            load_recent_characters(self.args.max_recent, self.args.files)
+        )
 
         state.output = "\x00markup-rows\x1ftrue\n"
         state.output += "\x00use-hot-keys\x1ftrue\n"
         if len(recent_characters) > 0:
             state.output += f"\x00message\x1f{recent_characters}"
         state.output += "\n".join(
             self.__format_characters(
@@ -137,23 +139,33 @@
         state.step += 1
 
     def __format_recent_characters(self, recent_characters: List[str]) -> str:
         pairings = [f"\u200e{(index + 1) % 10}: {character}" for index, character in enumerate(recent_characters)]
 
         return " | ".join(pairings)
 
-    def __format_characters(self, characters: Dict[str, str]) -> List[str]:
+    def __format_characters(self, characters: List[CharacterEntry]) -> List[str]:
         if self.args.show_description:
-            return [f"{key} {value}" for key, value in characters.items() if value != ""]
+            return [
+                f"{character.character} {character.description}"
+                for character in characters
+                if character.description != ""
+            ]
         else:
-            return [f"{key}\0meta\x1f{value}" for key, value in characters.items() if value != ""]
+            return [
+                f"{character.character}\0meta\x1f{character.description}"
+                for character in characters
+                if character.description != ""
+            ]
 
     def handle_shortcuts(self, state: State) -> None:
         if 10 <= state.return_code <= 19:
-            state.processed_characters = load_recent_characters(self.args.max_recent)[state.return_code - 10]
+            state.processed_characters = load_recent_characters(self.args.max_recent, self.args.files)[
+                state.return_code - 10
+            ]
             state.reset_current_input()
             state.step += 2
             return
         elif state.return_code:
             new_actions = self.__choose_action_from_return_code(state.return_code)
             if new_actions:
                 state.actions = new_actions
```

### Comparing `rofimoji-6.2.0/src/picker/paths.py` & `rofimoji-6.3.0/src/picker/paths.py`

 * *Files identical despite different names*

### Comparing `rofimoji-6.2.0/src/picker/recent.py` & `rofimoji-6.3.0/src/picker/recent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from typing import List
 
 from .paths import *
 
 
-def load_recent_characters(max_recent: int) -> List[str]:
+def load_recent_characters(max_recent: int, files: List[str]) -> List[str]:
     try:
-        return [char.strip("\n") for char in recents_file_location.read_text().strip("\n").split("\n")][:max_recent]
+        return [char.strip("\n") for char in __filename_for(files).read_text().strip("\n").split("\n")][:max_recent]
     except FileNotFoundError:
         return []
+    except NotADirectoryError:
+        recents = [char.strip("\n") for char in recents_file_location.read_text().strip("\n").split("\n")][:max_recent]
+        recents_file_location.unlink()
+        save_recent_characters("".join(recents), max_recent, files)
+        return recents
 
 
-def save_recent_characters(new_characters: str, max_recent: int) -> None:
+def save_recent_characters(new_characters: str, max_recent: int, files: List[str]) -> None:
     if max_recent == 0:
         return
     max_recent = min(max_recent, 10)
 
-    old_file_name = recents_file_location
-    new_file_name = old_file_name.with_name("recent.tmp")
+    old_file_name = __filename_for(files)
+    new_file_name = old_file_name.with_suffix(".tmp")
 
     new_file_name.parent.mkdir(parents=True, exist_ok=True)
     with new_file_name.open("w+") as new_file:
         new_file.write(new_characters + "\n")
 
         try:
             with old_file_name.open("r") as old_file:
@@ -33,7 +38,11 @@
                         index += 1
 
             old_file_name.unlink()
         except FileNotFoundError:
             pass
 
     new_file_name.rename(old_file_name)
+
+
+def __filename_for(files: List[str]) -> Path:
+    return recents_file_location / "-".join(files)
```

### Comparing `rofimoji-6.2.0/src/picker/standalone.py` & `rofimoji-6.3.0/src/picker/standalone.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import Dict, List, Tuple, Union
+from typing import List, Tuple, Union
 
 from . import emoji_data
 from .action import execute_action
 from .argument_parsing import parse_arguments_strict
 from .clipboarder.clipboarder import Clipboarder
 from .file_loader import read_characters_from_files
 from .frecent import load_frecent_characters, save_frecent_characters
@@ -26,43 +26,37 @@
 
         if action == CANCEL():
             sys.exit()
         elif action != DEFAULT():
             self.args.actions = [action]
 
         if isinstance(value, Shortcut):
-            characters = load_recent_characters(self.args.max_recent)[value.index]
+            characters = load_recent_characters(self.args.max_recent, self.args.files)[value.index]
         else:
             characters = self.__process_chosen_characters(value)
 
         if Action.MENU in self.args.actions:
             self.args.actions = self.selector.show_action_menu(self.args.selector_args)
 
-        save_recent_characters(characters, self.args.max_recent)
+        save_recent_characters(characters, self.args.max_recent, self.args.files)
         execute_action(characters, self.args.actions, self.active_window, self.args.typer, self.args.clipboarder)
 
     def __open_main_selector_window(self) -> Tuple[Union[Action, DEFAULT, CANCEL], Union[List[str], Shortcut]]:
         return self.selector.show_character_selection(
-            self.__format_characters(
-                read_characters_from_files(
-                    self.args.files, load_frecent_characters() if self.args.frecency else [], self.args.use_additional
-                )
+            read_characters_from_files(
+                self.args.files, load_frecent_characters() if self.args.frecency else [], self.args.use_additional
             ),
-            load_recent_characters(self.args.max_recent),
+            load_recent_characters(self.args.max_recent, self.args.files),
             self.args.prompt,
+            self.args.show_description,
+            self.args.use_icons,
             self.args.keybindings,
             self.args.selector_args,
         )
 
-    def __format_characters(self, characters: Dict[str, str]) -> List[str]:
-        if self.args.show_description:
-            return [f"{key} {value}" for key, value in characters.items() if value != ""]
-        else:
-            return [f"{key}\0meta\x1f{value}" for key, value in characters.items() if value != ""]
-
     def __process_chosen_characters(self, characters: List[str]) -> str:
         characters_with_skin_tones = []
         for character in characters:
             save_frecent_characters(character)
             characters_with_skin_tones.append(self.__add_skin_tone_to_character(character))
 
         return "".join(characters_with_skin_tones)
```

### Comparing `rofimoji-6.2.0/PKG-INFO` & `rofimoji-6.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: rofimoji
-Version: 6.2.0
+Version: 6.3.0
 Summary: Simple character picker using rofi
 Home-page: https://github.com/fdw/rofimoji
 License: MIT
 Author: Fabian Winter
 Author-email: 5821180+fdw@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ConfigArgParse (>=1.3,<2.0)
 Project-URL: Repository, https://github.com/fdw/rofimoji
 Description-Content-Type: text/markdown
 
 # Rofimoji: A character picker for rofi
 Do you want to use one of those fancy emojis? Or one of those other interesting characters Unicode offers? But you haven't found a good picker yet?
 
-Fear no more, `rofimoji` invokes the power of [rofi](https://github.com/DaveDavenport/rofi/) (and other dmenu-derivatives like [wofi](https://hg.sr.ht/~scoopta/wofi) or [fuzzel](https://codeberg.org/dnkl/fuzzel)) to give you exactly the picker you always wanted.
+Fear no more, `rofimoji` invokes the power of [rofi](https://github.com/DaveDavenport/rofi/) (and [other dmenu-derivatives](#supported-selectors)) to give you exactly the picker you always wanted.
 
 ## Main features
 - Insert the select character directly, or copy it to the clipboard.
 - Characters (and especially emojis) are fuzzy-searchable with keywords.
 - [It remembers the ones you use most and presents them first.](#most-recently-used-characters)
 - Emojis by default, but you can have any Unicode block you want - you can even [use your own](#custom-character-files-and-descriptions)!
 
@@ -77,27 +78,28 @@
 | long option                                                                                                             | short option | possible values                                                                                                | default value                               | description                                                                                                                                                                                                                                                                                                         |
 |-------------------------------------------------------------------------------------------------------------------------|--------------|----------------------------------------------------------------------------------------------------------------|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `--action`                                                                                                              | `-a`         | `type`, `copy`, `clipboard`, `unicode`, `copy-unicode`, `print`, `menu`                                        | `type`                                      | Choose what `rofimoji` should do with the selected characters. See [Actions](#actions) below for details.                                                                                                                                                                                                           |
 | `--files`                                                                                                               | `-f`         | `all`, `<yourfile>` or [any of the files in `data`](https://github.com/fdw/rofimoji/tree/main/src/picker/data) | `emojis`                                    | Define which file(s) to load characters from. A file name without extension (f.e. `emojis_smileys_emotion`) is enough for the distributed ones or any in `${XDG_DATA_HOME}/rofimoji/data`. Globbing with `*` is possible.<br/>`all` is a shortcut for all default files at once. Use with caution, that is a *lot*. |
 | `--skin-tone`                                                                                                           | `-s`         | `light`, `medium-light`, `moderate`, `dark brown`, `black`, as well as `neutral` and `ask`                     | `ask`                                       | Define the skin tone of supporting emojis. `ask` will always ask the user.                                                                                                                                                                                                                                          |
 | `--max-recent`                                                                                                          |              | 0-10                                                                                                           | 10                                          | Show at most this many recently picked characters. The number will be capped at 10. Set to `0` to disable the whole feature.                                                                                                                                                                                        |
 | `--no-frecency`<br/>(`no-frecency=True` in the config file)                                                             |              | -                                                                                                              | `<false>`                                   | By default, `rofimoji` shows frequently used items first. With this option, they're shown in the order of the file.                                                                                                                                                                                                 |
-| `--hidden-descriptions`<br/>(`hidden-descriptions=True` in the config file)                                             |              | -                                                                                                              | `<false>`                                   | Only list the characters, but not their description. This is useful for [grid themes](#rofi-theming). Note that they're still searchable, even though the description is not shown.                                                                                                                                 | 
+| `--hidden-descriptions`<br/>(`hidden-descriptions=True` in the config file)                                             |              | -                                                                                                              | `<false>`                                   | Only list the characters, but not their description. This is useful for [grid themes](#rofi-theming) in `rofi`. Note that they're still searchable, even though the description is not shown. Not used with other selectors.                                                                                        |
+| `--use-icons`                                                                                                           |              |                                                                                                                | `false`                                     | Show characters as icons in `rofi`. Not used for other selectors.                                                                                                                                                                                                                                                   |
 | `--prompt`                                                                                                              | `-r`         | any string                                                                                                     | `😀 `                                       | Define the prompt text for `rofimoji`.                                                                                                                                                                                                                                                                              |
-| `--selector-args`                                                                                                       |              |                                                                                                                |                                             | Define arguments that `rofimoji` will pass through to the selector (`rofi`, `wofi` or `fuzzel`).<br/>Please note that you need to specify it as `--selector-args="<selector-args>"` or `--selector-args " <selector-args>"` because of a [bug in argparse](https://bugs.python.org/issue9334)                       |
-| `--selector`                                                                                                            |              | `rofi`, `wofi`, `fuzzel`                                                                                       | (automatically chosen)                      | Show the selection dialog with this application.                                                                                                                                                                                                                                                                    |
+| `--selector-args`                                                                                                       |              |                                                                                                                |                                             | Define arguments that `rofimoji` will pass through to the selector.<br/>Please note that you need to specify it as `--selector-args="<selector-args>"` or `--selector-args " <selector-args>"` because of a [bug in argparse](https://bugs.python.org/issue9334)                                                    |
+| `--selector`                                                                                                            |              | `rofi`, `wofi`, `fuzzel`, `dmenu`, `tofi`, `bemenu`, `wmenu`                                                   | (automatically chosen)                      | Show the selection dialog with this application.                                                                                                                                                                                                                                                                    |
 | `--clipboarder`                                                                                                         |              | `xsel`, `xclip`, `wl-copy`                                                                                     | (automatically chosen)                      | Access the clipboard with this application.                                                                                                                                                                                                                                                                         |
 | `--typer`                                                                                                               |              | `xdotool`, `wtype`                                                                                             | (automatically chosen)                      | Type the characters using this application.                                                                                                                                                                                                                                                                         |
 | `--keybinding-copy`, `--keybinding-type`, `--keybinding-clipboard`, `--keybinding-unicode`, `--keybinding-copy-unicode` |              |                                                                                                                | `Alt+c`, `Alt+t`, `Alt+p`, `Alt+u`, `Alt+i` | Choose different keybindings than the default values.                                                                                                                                                                                                                                                               |
 
 ## Example config file
 `~/.config/rofimoji.rc`:
 ```
 action = copy
-files = [emojis, hebrew]
+files = [emojis, math]
 skin-tone = moderate
 ```
 
 ## Actions
 
 The `--action` (`-a`) option defines what action will be taken when a character is selected. Multiple actions can be specified with a space character in between (for example: `-a type copy`).
 The options are:
@@ -119,59 +121,79 @@
 Therefore, `rofimoji` uses both and also restores both.
 To use this workaround, you can either use the keybinding `alt+p` or start it as `rofimoji --action clipboard` (`-a clipboard`).
 If you want to have it directly typed instead, you can hit `alt+t`, even though it was started with `--action clipboard`. Note that you can [change the keybindings](#options).
 
 Finally, with `--action copy` (or `-a copy`) you can also tell `rofimoji` to only copy the selected characters to your clipboard.
 
 ## Display server support
-`rofimoji` supports both X11 and Wayland by using either `rofi`, `xsel`/`xclip` and `xdotool` on X11 or `wofi`/`fuzzel`/some other adapter `rofi`, `wl-copy` and `wtype` on Wayland. It tries to automatically choose the right one for the currently running session.
+`rofimoji` supports both X11 and Wayland by using the correct tools for each environment (see [Supported Selectors](#supported-selectors)). It tries to automatically choose the right one for the currently running session.
 If you want to manually overwrite this, have a look at the `--selector`, `--clipboarder` and `--typer` options [above](#options).
 
-Please note that neither `wofi` nor `fuzzel` support custom keyboard shortcuts, recent files or a grid theme at the moment.
-
 ## Most recently used characters
 By default, `rofimoji` will show the last ten recently used characters separately; you can insert them with `alt+1`, `alt+2` and so on. It will use the default [insertion method](#insertion-method).
 If you don't want this, you can set `--max-recent` to `0`.
 
 Additionally, `rofimoji` also remembers in general which characters are used more frequently and sorts the list accordingly. You can disable this behavior with `--no-frecency`.
 
-## Supported characters
-Obviously, `rofimoji` is mostly used for emojis. However, it also supports all other Unicode blocks, for example [mathematical symbols](https://github.com/fdw/rofimoji/blob/main/src/picker/data/math.csv), [Greek and Coptic](https://github.com/fdw/rofimoji/blob/main/src/picker/data/greek_and_coptic.csv) or [Linear B (Ideograms)](https://github.com/fdw/rofimoji/blob/main/src/picker/data/linear_b_ideograms.csv). Simply load them with `-f` (see [options](#options)).
-If you miss something that should be there, please open an issue.
+## Rofi theming
+By default, `rofimoji` re-uses the existing rofi configuration, but you can pass your own using `--selector-args` (for example `--selector-args="-theme ~/your-rofi-theme.rasi"`).
+
+If you would like a more character-focused theme, you can use packaged [`grid.rasi`](https://github.com/fdw/rofimoji/blob/main/src/picker/contrib/grid.rasi) together with the `--hidden-descriptions` parameter. This theme still imports the existing `rofi` configuration but moves the entries into a grid. Of course, you can base your own theme on this. (If you have improvements, please open a PR!)
+To use the arrow keys in `rofi` only for the grid and not the query, pass these `-selector-args`: `-kb-row-left Left -kb-row-right Right -kb-move-char-back Control+b -kb-move-char-forward Control+f`.
+
+![Screenshot of rofimoji with a grid theme](screenshot-grid.png?raw=true)
+
+# Supported characters
+- [Unicode emojis](https://home.unicode.org/emoji/about-emoji/) with the official descriptions and tags. Also supports skin tones and gender variants.
+- All other [Unicode](https://home.unicode.org/) characters, split into the official blocks
+- CJK character sets from Unicode
+- [Font Awesome 6](https://fontawesome.com/)
+- [Nerd Fonts](https://www.nerdfonts.com/)
+- [Gitmoji](https://gitmoji.dev/)
+- Kaomoji, from [w33ble](https://github.com/w33ble/emoticon-data)
+
+If you miss something, please open an issue!
 
 ## Custom character files and descriptions
 If the predefined ones are not enough, you can define additional character files and load them with `-f` (see [options](#options)). In each line, one 'character' can be defined, followed by a single space character (` `). After that, you can write whatever description you want.
 
 If the character is also in another selected file, all descriptions will be combined. If you give it the same name as one of those included with `rofimoji`, yours will be preferred.
 
 For added comfort, `rofimoji` will automatically load an "additional" file for predefined ones. This file needs to called `<filename>.additional.csv` and lie in `${XDG_DATA_DIR}/rofimoji/data/`. For example, if you want to extend `emojis_smileys_emotion`, call the file `emojis_smileys_emotions.additional.csv`. This is helpful if you want additional descriptions: You can define such an additional character file, add the character and your description and your descriptions will now also be shown.
 
 If you think your file is useful to others, please open a PR to include it in a future version of `rofimoji`.
 
-## Rofi theming
-By default, `rofimoji` re-uses the existing rofi configuration, but you can pass your own using `--selector-args` (for example `--selector-args="-theme ~/your-rofi-theme.rasi"`).
-
-If you would like a more character-focused theme, you can use packaged [`grid.rasi`](https://github.com/fdw/rofimoji/blob/main/src/picker/contrib/grid.rasi) together with the `--hidden-descriptions` parameter. This theme still imports the existing `rofi` configuration but moves the entries into a grid. Of course, you can base your own theme on this. (If you have improvements, please open a PR!)
-To use the arrow keys in `rofi` only for the grid and not the query, pass these `-selector-args`: `-kb-row-left Left -kb-row-right Right -kb-move-char-back Control+b -kb-move-char-forward Control+f`.
-
-![Screenshot of rofimoji with a grid theme](screenshot-grid.png?raw=true)
-
 # Installation
 ## From distribution repositories
 [![Packaging status](https://repology.org/badge/vertical-allrepos/rofimoji.svg)](https://repology.org/project/rofimoji/versions)
 
 ## From PyPI
-`rofimoji` is on [PyPI](https://pypi.org/project/rofimoji/). You can install it with `pipx install --user rofimoji` (or `sudo pipx install rofimoji`).
+`rofimoji` is on [PyPI](https://pypi.org/project/rofimoji/). You can install it with `pipx install rofimoji` (or `sudo pipx install rofimoji`).
 
 ## From Github
 Download the wheel file of the [latest release](https://github.com/fdw/rofimoji/releases/) and install it with  `sudo pip install $filename` (or you can use `pip install --user $filename` to only install it for the local user).
 Afterwards, there should be a `rofimoji` on your `$PATH`.
 This also installs the python dependency `configargparse`.
 
 ## Dependencies
 What else do you need:
 - Python 3.8 or higher
 - A font that can display your scripts, (for emojis, [EmojiOne](https://github.com/emojione/emojione) or [Noto Emoji](https://www.google.com/get/noto/) work)
-- `rofi` (in version 1.6.0 or higher if you want to use the mode), `wofi` or `fuzzel`
-- A tool to programmatically type characters into applications. Either `xdotool` for X11 or `wtype` for Wayland
-- A tool to copy the characters to the clipboard. `xsel` and `xclip` work on X11; `wl-copy` on Wayland
+- Optionally, a tool to programmatically type characters into applications. Either `xdotool` for X11 or `wtype` for Wayland
+- Optionally, a tool to copy the characters to the clipboard. `xsel` and `xclip` work on X11; `wl-copy` on Wayland
+
+### Supported Selectors
+Please note that only `rofi` (both on X and Wayland) supports custom keyboard shortcuts, recent files or a grid theme at the moment. For all others, only basic functionality works.
+
+#### X.org
+- [rofi](https://github.com/davatorium/rofi)
+- [bemenu](https://github.com/Cloudef/bemenu)
+- [dmenu](https://tools.suckless.org/dmenu/)
+
+#### Wayland
+- [rofi fork for Wayland](https://github.com/lbonn/rofi)
+- [wofi](https://hg.sr.ht/~scoopta/wofi)
+- [fuzzel](https://codeberg.org/dnkl/fuzzel)
+- [tofi](https://github.com/philj56/tofi)
+- [bemenu](https://github.com/Cloudef/bemenu)
+- [wmenu](https://git.sr.ht/~adnano/wmenu)
```

