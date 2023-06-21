# Comparing `tmp/glyphsets-0.6.1.tar.gz` & `tmp/glyphsets-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glyphsets-0.6.1.tar", last modified: Wed May  3 15:30:47 2023, max compression
+gzip compressed data, was "glyphsets-0.6.2.tar", last modified: Wed Jun 21 17:24:49 2023, max compression
```

## Comparing `glyphsets-0.6.1.tar` & `glyphsets-0.6.2.tar`

### file list

```diff
@@ -1,505 +1,505 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.920824 glyphsets-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.860823 glyphsets-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-03 15:30:34.000000 glyphsets-0.6.1/.github/workflows/publish-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-03 15:30:34.000000 glyphsets-0.6.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 15:30:34.000000 glyphsets-0.6.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/Archive/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.860823 glyphsets-0.6.1/Archive/GF Glyph Sets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.860823 glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.860823 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.860823 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/historical_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_italic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs_smallcaps.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/historical_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_italic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    16079 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-core.nam
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/RECOMMENDED.md
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/TROUBLESHOOTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.864823 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    75853 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   104148 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/locl.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/plus_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/pro_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/plus_optional-glyphs_case-accents.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/pro_optional-glyphs_case-punctuation.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/plus_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/pro_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_either_4.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_either_19.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PRO_either_4.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    43666 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.868823 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/Info/
--rw-r--r--   0 runner    (1001) docker     (123)    89964 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/
--rw-r--r--   0 runner    (1001) docker     (123)    35092 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/Directory.png
--rw-r--r--   0 runner    (1001) docker     (123)    98535 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/ListFilters.png
--rw-r--r--   0 runner    (1001) docker     (123)    84092 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png
--rw-r--r--   0 runner    (1001) docker     (123)    24052 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    71431 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-1.png
--rw-r--r--   0 runner    (1001) docker     (123)    33541 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-2.png
--rw-r--r--   0 runner    (1001) docker     (123)    45217 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-3.png
--rw-r--r--   0 runner    (1001) docker     (123)    53065 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/list-filter.png
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-03 15:30:34.000000 glyphsets-0.6.1/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Arabic/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist
--rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Arabic/nam/
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Plus.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.872823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclItalic.nam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclRoman.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Historical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclItalic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Historical.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclItalic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Greek/
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    56469 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist
--rw-r--r--   0 runner    (1001) docker     (123)    30534 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    26352 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    28310 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Greek/nam/
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Core.nam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Expert.nam
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/Greek/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.876823 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Latin/
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    38180 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist
--rw-r--r--   0 runner    (1001) docker     (123)    62282 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    46764 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Latin/nam/
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_African.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Core.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/Latin/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.880823 glyphsets-0.6.1/GF_glyphsets/Phonetics/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    17764 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAHistorical.nam
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_SinoExt.nam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_UPA.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_APA.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAHistorical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_SinoExt.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_UPA.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_APA.txt
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAHistorical.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_SinoExt.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_UPA.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/TransLatin/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/
--rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs
--rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/TransLatin/nam/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.884823 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Arabic.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.888824 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Arabic.txt
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-03 15:30:34.000000 glyphsets-0.6.1/GF_glyphsets/update-gs.sh
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 15:30:34.000000 glyphsets-0.6.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.856823 glyphsets-0.6.1/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.888824 glyphsets-0.6.1/Lib/glyphsets/
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/codepoints.py
--rw-r--r--   0 runner    (1001) docker     (123)   588180 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/data.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.916824 glyphsets-0.6.1/Lib/glyphsets/encodings/
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/adlam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ahom_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    57487 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/arabic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/armenian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/avestan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/balinese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/bamum_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/batak_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/bengali_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/braille_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/buginese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/buhid_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/carian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/chakma_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   284694 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   298348 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   241902 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/chorasmian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/coptic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    46227 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cypro-minoan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/deseret_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/dives-akuru_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/dogra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/duployan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    41018 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/georgian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/gothic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/grantha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/greek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/hatran_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/hebrew_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    91251 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/japanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/javanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/kannada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/kawi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    21734 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/khitan-small-script_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/khmer_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/khojki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    80178 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/korean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/lao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    37112 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/latin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/limbu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/lisu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/lycian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/lydian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/makasar_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/marchen_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   190939 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/math.nam
--rw-r--r--   0 runner    (1001) docker     (123)    95179 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/math_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/meroitic-cursive_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/meroitic-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/miao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/modi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/mro_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/multani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    24495 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/music_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nag-mundari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nandinagari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/newa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nko_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nushu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ogham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/old-uyghur_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/oriya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/osage_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ottoman-siyaq-numbers_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/rejang_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/runic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/sharada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/shavian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/siddham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    35208 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/sinhala_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   117935 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/symbols_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/syriac_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/takri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tamil_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)   212192 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tangut_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/telugu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/thaana_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/thai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/toto_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/vai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/vithkuqi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/wancho_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/wgl-latin.enc
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)    30939 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/yi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-03 15:30:34.000000 glyphsets-0.6.1/Lib/glyphsets/test_strings.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.888824 glyphsets-0.6.1/Lib/glyphsets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 15:30:47.000000 glyphsets-0.6.1/Lib/glyphsets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-03 15:30:47.920824 glyphsets-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-03 15:30:34.000000 glyphsets-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 15:30:34.000000 glyphsets-0.6.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.920824 glyphsets-0.6.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-03 15:30:34.000000 glyphsets-0.6.1/scripts/create-glyphset.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:30:47.920824 glyphsets-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-03 15:30:34.000000 glyphsets-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.920824 glyphsets-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:30:47.920824 glyphsets-0.6.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    90712 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/data/MavenPro[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/test_glyphdata.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/test_teststrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/test_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-03 15:30:34.000000 glyphsets-0.6.1/tests/testcoverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.097371 glyphsets-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.025371 glyphsets-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.033371 glyphsets-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-21 17:24:35.000000 glyphsets-0.6.2/.github/workflows/publish-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-21 17:24:35.000000 glyphsets-0.6.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 17:24:35.000000 glyphsets-0.6.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.029371 glyphsets-0.6.2/Archive/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.033371 glyphsets-0.6.2/Archive/GF Glyph Sets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.033371 glyphsets-0.6.2/Archive/GF Glyph Sets/Arabic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Arabic/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.033371 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    10080 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.029371 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.037371 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/historical_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_italic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs_smallcaps.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.037371 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/historical_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_italic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    16079 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.037371 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/
+-rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.029371 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.037371 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.041371 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/RECOMMENDED.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/TROUBLESHOOTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.041371 glyphsets-0.6.2/Archive/GF Glyph Sets/Vietnamese/
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Vietnamese/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.041371 glyphsets-0.6.2/Archive/GF Glyph Sets/Vietnamese/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    75853 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   104148 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/Vietnamese/img/locl.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.041371 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.041371 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/nice names/plus_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/nice names/pro_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/plus_optional-glyphs_case-accents.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/pro_optional-glyphs_case-punctuation.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.041371 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/uni names/plus_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/uni names/pro_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.045371 glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_either_4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_either_19.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PRO_either_4.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.045371 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.045371 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/Glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    43666 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.045371 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/Glyphs/Info/
+-rw-r--r--   0 runner    (1001) docker     (123)    89964 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.045371 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    35092 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/Directory.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98535 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/ListFilters.png
+-rw-r--r--   0 runner    (1001) docker     (123)    84092 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24052 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    71431 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/fix-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33541 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/fix-2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45217 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/fix-3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53065 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/list-filter.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-21 17:24:35.000000 glyphsets-0.6.2/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.045371 glyphsets-0.6.2/GF_glyphsets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.045371 glyphsets-0.6.2/GF_glyphsets/Arabic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Arabic/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.045371 glyphsets-0.6.2/GF_glyphsets/Arabic/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist
+-rw-r--r--   0 runner    (1001) docker     (123)    15494 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.045371 glyphsets-0.6.2/GF_glyphsets/Arabic/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.029371 glyphsets-0.6.2/GF_glyphsets/Arabic/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.045371 glyphsets-0.6.2/GF_glyphsets/Arabic/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.049371 glyphsets-0.6.2/GF_glyphsets/Arabic/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Plus.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.049371 glyphsets-0.6.2/GF_glyphsets/Cyrillic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.049371 glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    21500 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.049371 glyphsets-0.6.2/GF_glyphsets/Cyrillic/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclItalic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclRoman.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.029371 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.049371 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Historical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclItalic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.049371 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Historical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclItalic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.049371 glyphsets-0.6.2/GF_glyphsets/Greek/
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.053371 glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    56469 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist
+-rw-r--r--   0 runner    (1001) docker     (123)    30534 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    26352 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    28310 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.053371 glyphsets-0.6.2/GF_glyphsets/Greek/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_Expert.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.029371 glyphsets-0.6.2/GF_glyphsets/Greek/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.053371 glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.053371 glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.053371 glyphsets-0.6.2/GF_glyphsets/Latin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.057371 glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    38180 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist
+-rw-r--r--   0 runner    (1001) docker     (123)    62282 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    46764 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    16570 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.057371 glyphsets-0.6.2/GF_glyphsets/Latin/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_African.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.029371 glyphsets-0.6.2/GF_glyphsets/Latin/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.057371 glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.057371 glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.057371 glyphsets-0.6.2/GF_glyphsets/Phonetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.061371 glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    17764 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.061371 glyphsets-0.6.2/GF_glyphsets/Phonetics/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAHistorical.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/nam/GF_Phonetics_SinoExt.nam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/nam/GF_Phonetics_UPA.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.029371 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.061371 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_APA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAHistorical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_SinoExt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_UPA.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.061371 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_APA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAHistorical.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_SinoExt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_UPA.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.061371 glyphsets-0.6.2/GF_glyphsets/TransLatin/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/TransLatin/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.061371 glyphsets-0.6.2/GF_glyphsets/TransLatin/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7427 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.061371 glyphsets-0.6.2/GF_glyphsets/TransLatin/nam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.029371 glyphsets-0.6.2/GF_glyphsets/TransLatin/txt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.061371 glyphsets-0.6.2/GF_glyphsets/TransLatin/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Arabic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.061371 glyphsets-0.6.2/GF_glyphsets/TransLatin/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Arabic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-21 17:24:35.000000 glyphsets-0.6.2/GF_glyphsets/update-gs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 17:24:35.000000 glyphsets-0.6.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.029371 glyphsets-0.6.2/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.065371 glyphsets-0.6.2/Lib/glyphsets/
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-21 17:24:48.000000 glyphsets-0.6.2/Lib/glyphsets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/codepoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)   588180 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.093371 glyphsets-0.6.2/Lib/glyphsets/encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/adlam_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/ahom_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    20007 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    57487 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/arabic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/armenian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/avestan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/balinese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/bamum_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/batak_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/bengali_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/braille_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/buginese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/buhid_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/carian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/chakma_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/cham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   284694 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   298348 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   241902 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/chorasmian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/coptic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    46227 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/cypro-minoan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/deseret_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/dives-akuru_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/dogra_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/duployan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    41018 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/georgian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/gothic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/grantha_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/greek_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/hatran_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/hebrew_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    91251 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/japanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/javanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/kannada_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/kawi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    21734 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/khitan-small-script_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/khmer_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/khojki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    80178 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/korean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/lao_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    37362 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/latin_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/limbu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/lisu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/lycian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/lydian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/makasar_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/marchen_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   190939 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/math.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    95179 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/math_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     8592 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/meroitic-cursive_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/meroitic-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/miao_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/modi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/mro_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/multani_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    24495 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/music_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/nag-mundari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/nandinagari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/newa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/nko_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/nushu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/ogham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/old-uyghur_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/oriya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/osage_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/ottoman-siyaq-numbers_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/rejang_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/runic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/sharada_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/shavian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/siddham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    35208 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/sinhala_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   117935 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/symbols_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/syriac_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/takri_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tamil_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)   212192 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tangut_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/telugu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/thaana_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/thai_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/toto_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/vai_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/vithkuqi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/wancho_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/wgl-latin.enc
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)    30939 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/yi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-21 17:24:35.000000 glyphsets-0.6.2/Lib/glyphsets/test_strings.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.065371 glyphsets-0.6.2/Lib/glyphsets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-21 17:24:48.000000 glyphsets-0.6.2/Lib/glyphsets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23057 2023-06-21 17:24:49.000000 glyphsets-0.6.2/Lib/glyphsets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:24:48.000000 glyphsets-0.6.2/Lib/glyphsets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-21 17:24:48.000000 glyphsets-0.6.2/Lib/glyphsets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:24:48.000000 glyphsets-0.6.2/Lib/glyphsets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-21 17:24:48.000000 glyphsets-0.6.2/Lib/glyphsets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 17:24:48.000000 glyphsets-0.6.2/Lib/glyphsets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-21 17:24:49.097371 glyphsets-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-21 17:24:35.000000 glyphsets-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 17:24:35.000000 glyphsets-0.6.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.093371 glyphsets-0.6.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-21 17:24:35.000000 glyphsets-0.6.2/scripts/create-glyphset.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:24:49.097371 glyphsets-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-21 17:24:35.000000 glyphsets-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.093371 glyphsets-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-21 17:24:35.000000 glyphsets-0.6.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:24:49.093371 glyphsets-0.6.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    90712 2023-06-21 17:24:35.000000 glyphsets-0.6.2/tests/data/MavenPro[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-21 17:24:35.000000 glyphsets-0.6.2/tests/test_glyphdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-21 17:24:35.000000 glyphsets-0.6.2/tests/test_teststrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-21 17:24:35.000000 glyphsets-0.6.2/tests/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-21 17:24:35.000000 glyphsets-0.6.2/tests/testcoverage.py
```

### Comparing `glyphsets-0.6.1/.github/workflows/publish-release.yml` & `glyphsets-0.6.2/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/.github/workflows/test.yml` & `glyphsets-0.6.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Arabic/README.md` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Arabic/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-core.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/README.md` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/README.md` & `glyphsets-0.6.2/Archive/GF Glyph Sets/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/RECOMMENDED.md` & `glyphsets-0.6.2/Archive/GF Glyph Sets/RECOMMENDED.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/TROUBLESHOOTING.md` & `glyphsets-0.6.2/Archive/GF Glyph Sets/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/README.md` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Vietnamese/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/Vietnamese/img/locl.png` & `glyphsets-0.6.2/Archive/GF Glyph Sets/Vietnamese/img/locl.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt` & `glyphsets-0.6.2/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/README.md` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/Directory.png` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/Directory.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/ListFilters.png` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/ListFilters.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-1.png` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/fix-1.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-2.png` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/fix-2.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/fix-3.png` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/fix-3.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Archive/GF Glyph Sets/tutorials/img/list-filter.png` & `glyphsets-0.6.2/Archive/GF Glyph Sets/tutorials/img/list-filter.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/CHANGELOG.md` & `glyphsets-0.6.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Arabic/README.md` & `glyphsets-0.6.2/GF_glyphsets/Arabic/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist` & `glyphsets-0.6.2/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam` & `glyphsets-0.6.2/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam` & `glyphsets-0.6.2/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt` & `glyphsets-0.6.2/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt` & `glyphsets-0.6.2/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt` & `glyphsets-0.6.2/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/README.md` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt` & `glyphsets-0.6.2/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/README.md` & `glyphsets-0.6.2/GF_glyphsets/Greek/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist` & `glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam` & `glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam` & `glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam` & `glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Core.nam` & `glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam` & `glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam` & `glyphsets-0.6.2/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt` & `glyphsets-0.6.2/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/README.md` & `glyphsets-0.6.2/GF_glyphsets/Latin/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist` & `glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_African.nam` & `glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_African.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam` & `glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Core.nam` & `glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam` & `glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam` & `glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam` & `glyphsets-0.6.2/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt` & `glyphsets-0.6.2/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt` & `glyphsets-0.6.2/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/README.md` & `glyphsets-0.6.2/GF_glyphsets/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist` & `glyphsets-0.6.2/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs` & `glyphsets-0.6.2/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs` & `glyphsets-0.6.2/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam` & `glyphsets-0.6.2/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam` & `glyphsets-0.6.2/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt` & `glyphsets-0.6.2/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt` & `glyphsets-0.6.2/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/GF_glyphsets/update-gs.sh` & `glyphsets-0.6.2/GF_glyphsets/update-gs.sh`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/LICENSE` & `glyphsets-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/__init__.py` & `glyphsets-0.6.2/Lib/glyphsets/__init__.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/__main__.py` & `glyphsets-0.6.2/Lib/glyphsets/__main__.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/codepoints.py` & `glyphsets-0.6.2/Lib/glyphsets/codepoints.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/data.json` & `glyphsets-0.6.2/Lib/glyphsets/data.json`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/README.md` & `glyphsets-0.6.2/Lib/glyphsets/encodings/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/adlam_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/adlam_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/ahom_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/ahom_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/arabic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/arabic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/armenian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/armenian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/avestan_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/avestan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/balinese_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/balinese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/bamum_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/bamum_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/batak_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/batak_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/bengali_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/bengali_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/braille_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/braille_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/buginese_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/buginese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/buhid_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/buhid_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/carian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/carian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/chakma_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/chakma_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/cham_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/cham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/chorasmian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/chorasmian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/coptic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/coptic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/cypro-minoan_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/cypro-minoan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/deseret_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/deseret_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/dives-akuru_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/dives-akuru_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/dogra_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/dogra_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/duployan_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/duployan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/georgian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/georgian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/gothic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/gothic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/grantha_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/grantha_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/greek_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/greek_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/hatran_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/hatran_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/hebrew_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/hebrew_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/japanese_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/japanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/javanese_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/javanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/kannada_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/kannada_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/kawi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/kawi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/khitan-small-script_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/khitan-small-script_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/khmer_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/khmer_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/khojki_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/khojki_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/korean_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/korean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/lao_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/lao_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam`

 * *Files 1% similar despite different names*

```diff
@@ -423,14 +423,22 @@
 0x02A9  ʩ LATIN SMALL LETTER FENG DIGRAPH
 0x02AA  ʪ LATIN SMALL LETTER LS DIGRAPH
 0x02AB  ʫ LATIN SMALL LETTER LZ DIGRAPH
 0x02AC  ʬ LATIN LETTER BILABIAL PERCUSSIVE
 0x02AD  ʭ LATIN LETTER BIDENTAL PERCUSSIVE
 0x02AE  ʮ LATIN SMALL LETTER TURNED H WITH FISHHOOK
 0x02AF  ʯ LATIN SMALL LETTER TURNED H WITH FISHHOOK AND TAIL
+0x0300    COMBINING GRAVE ACCENT
+0x0301    COMBINING ACUTE ACCENT
+0x0303    COMBINING TILDE
+0x0304    COMBINING MACRON
+0x0308    COMBINING DIAERESIS
+0x0309    COMBINING HOOK ABOVE
+0x0323    COMBINING DOT BELOW
+0x0329    COMBINING VERTICAL LINE BELOW
 0x1E00  Ḁ LATIN CAPITAL LETTER A WITH RING BELOW
 0x1E01  ḁ LATIN SMALL LETTER A WITH RING BELOW
 0x1E02  Ḃ LATIN CAPITAL LETTER B WITH DOT ABOVE
 0x1E03  ḃ LATIN SMALL LETTER B WITH DOT ABOVE
 0x1E04  Ḅ LATIN CAPITAL LETTER B WITH DOT BELOW
 0x1E05  ḅ LATIN SMALL LETTER B WITH DOT BELOW
 0x1E06  Ḇ LATIN CAPITAL LETTER B WITH LINE BELOW
```

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/latin_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/latin_unique-glyphs.nam`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,22 @@
 0x0152  Œ LATIN CAPITAL LIGATURE OE
 0x0153  œ LATIN SMALL LIGATURE OE
 0x02BB  ʻ MODIFIER LETTER TURNED COMMA
 0x02BC  ʼ MODIFIER LETTER APOSTROPHE
 0x02C6  ˆ MODIFIER LETTER CIRCUMFLEX ACCENT
 0x02DA  ˚ RING ABOVE
 0x02DC  ˜ SMALL TILDE
+0x0300    COMBINING GRAVE ACCENT
+0x0301    COMBINING ACUTE ACCENT
+0x0303    COMBINING TILDE
+0x0304    COMBINING MACRON
+0x0308    COMBINING DIAERESIS
+0x0309    COMBINING HOOK ABOVE
+0x0323    COMBINING DOT BELOW
+0x0329    COMBINING VERTICAL LINE BELOW
 0x2002    EN SPACE
 0x200B    ZERO WIDTH SPACE
 0x2009    THIN SPACE
 0x2013  – EN DASH
 0x2014  — EM DASH
 0x2018  ‘ LEFT SINGLE QUOTATION MARK
 0x2019  ’ RIGHT SINGLE QUOTATION MARK
```

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/limbu_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/limbu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/lisu_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/lisu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/lycian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/lycian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/lydian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/lydian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/makasar_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/makasar_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/marchen_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/marchen_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/math.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/math.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/math_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/math_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/meroitic-cursive_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/meroitic-cursive_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/meroitic-hieroglyphs_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/meroitic-hieroglyphs_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/miao_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/miao_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/modi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/modi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/mro_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/mro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/multani_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/multani_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/music_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/music_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/nag-mundari_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/nag-mundari_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/nandinagari_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/nandinagari_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/newa_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/newa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/nko_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/nko_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/nushu_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/nushu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/ogham_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/ogham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/old-uyghur_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/old-uyghur_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/oriya_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/oriya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/osage_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/osage_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/ottoman-siyaq-numbers_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/ottoman-siyaq-numbers_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/rejang_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/rejang_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/runic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/runic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/sharada_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/sharada_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/shavian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/shavian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/siddham_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/siddham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/sinhala_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/sinhala_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/symbols_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/symbols_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/syriac_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/syriac_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/takri_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/takri_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tamil_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tamil_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tangut_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tangut_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/telugu_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/telugu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/thaana_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/thaana_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/thai_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/thai_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/toto_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/toto_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/vai_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/vai_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 0x01A1  ơ LATIN SMALL LETTER O WITH HORN
 0x01AF  Ư LATIN CAPITAL LETTER U WITH HORN
 0x0128  Ĩ LATIN CAPITAL LETTER I WITH TILDE
 0x0129  ĩ LATIN SMALL LETTER I WITH TILDE
 0x0168  Ũ LATIN CAPITAL LETTER U WITH TILDE
 0x0169  ũ LATIN SMALL LETTER U WITH TILDE
 0x01B0  ư LATIN SMALL LETTER U WITH HORN
+0x0300    COMBINING GRAVE ACCENT
+0x0301    COMBINING ACUTE ACCENT
+0x0303    COMBINING TILDE
+0x0304    COMBINING MACRON
+0x0308    COMBINING DIAERESIS
+0x0309    COMBINING HOOK ABOVE
+0x0323    COMBINING DOT BELOW
+0x0329    COMBINING VERTICAL LINE BELOW
 0x1EA0  Ạ LATIN CAPITAL LETTER A WITH DOT BELOW
 0x1EA1  ạ LATIN SMALL LETTER A WITH DOT BELOW
 0x1EA2  Ả LATIN CAPITAL LETTER A WITH HOOK ABOVE
 0x1EA3  ả LATIN SMALL LETTER A WITH HOOK ABOVE
 0x1EA4  Ấ LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND ACUTE
 0x1EA5  ấ LATIN SMALL LETTER A WITH CIRCUMFLEX AND ACUTE
 0x1EA6  Ầ LATIN CAPITAL LETTER A WITH CIRCUMFLEX AND GRAVE
```

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/vithkuqi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/vithkuqi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/wancho_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/wancho_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/wgl-latin.enc` & `glyphsets-0.6.2/Lib/glyphsets/encodings/wgl-latin.enc`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/yi_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/yi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam` & `glyphsets-0.6.2/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/subsets.py` & `glyphsets-0.6.2/Lib/glyphsets/subsets.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets/test_strings.json` & `glyphsets-0.6.2/Lib/glyphsets/test_strings.json`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/Lib/glyphsets.egg-info/PKG-INFO` & `glyphsets-0.6.2/Lib/glyphsets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glyphsets
-Version: 0.6.1
+Version: 0.6.2
 Summary: A python API for evaluating coverage of glyph sets in font projects.
 Home-page: https://github.com/googlefonts/glyphsets/
 Author: Dave Crossland, Eli Heuer, Felipe Sanches, Lasse Fister, Marc Foley, Roderick Sheeter
 Author-email: dave@lab6.com
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `glyphsets-0.6.1/Lib/glyphsets.egg-info/SOURCES.txt` & `glyphsets-0.6.2/Lib/glyphsets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/PKG-INFO` & `glyphsets-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glyphsets
-Version: 0.6.1
+Version: 0.6.2
 Summary: A python API for evaluating coverage of glyph sets in font projects.
 Home-page: https://github.com/googlefonts/glyphsets/
 Author: Dave Crossland, Eli Heuer, Felipe Sanches, Lasse Fister, Marc Foley, Roderick Sheeter
 Author-email: dave@lab6.com
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `glyphsets-0.6.1/README.md` & `glyphsets-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/scripts/create-glyphset.py` & `glyphsets-0.6.2/scripts/create-glyphset.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/setup.py` & `glyphsets-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/tests/__init__.py` & `glyphsets-0.6.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/tests/data/MavenPro[wght].ttf` & `glyphsets-0.6.2/tests/data/MavenPro[wght].ttf`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/tests/test_glyphdata.py` & `glyphsets-0.6.2/tests/test_glyphdata.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.1/tests/testcoverage.py` & `glyphsets-0.6.2/tests/testcoverage.py`

 * *Files identical despite different names*

