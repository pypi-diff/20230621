# Comparing `tmp/pyradium-0.0.8.tar.gz` & `tmp/pyradium-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyradium-0.0.8.tar", last modified: Thu Jan  6 11:04:35 2022, max compression
+gzip compressed data, was "pyradium-0.0.9.tar", last modified: Sun Jan 30 22:24:17 2022, max compression
```

## Comparing `pyradium-0.0.8.tar` & `pyradium-0.0.9.tar`

### file list

```diff
@@ -1,232 +1,235 @@
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.820834 pyradium-0.0.8/
--rw-------   0 joe       (1000) joe       (1000)       52 2022-01-01 15:12:48.000000 pyradium-0.0.8/.gitignore
--rw-------   0 joe       (1000) joe       (1000)       77 2021-10-28 21:08:12.000000 pyradium-0.0.8/.travis.yml
--rw-------   0 joe       (1000) joe       (1000)    35142 2020-03-30 11:18:51.000000 pyradium-0.0.8/LICENSE
--rw-------   0 joe       (1000) joe       (1000)      107 2021-10-28 21:08:12.000000 pyradium-0.0.8/MANIFEST.in
--rw-------   0 joe       (1000) joe       (1000)    17813 2022-01-06 11:04:35.820834 pyradium-0.0.8/PKG-INFO
--rw-------   0 joe       (1000) joe       (1000)    14401 2022-01-04 10:52:31.000000 pyradium-0.0.8/README.md
--rwx------   0 joe       (1000) joe       (1000)      251 2021-11-05 22:49:09.000000 pyradium-0.0.8/autorender
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.800834 pyradium-0.0.8/docs/
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.800834 pyradium-0.0.8/docs/imgs/
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.804834 pyradium-0.0.8/docs/imgs/anim/
--rw-------   0 joe       (1000) joe       (1000)    31808 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/imgs/anim/21da33acb6f14b9f6bf7eae05bf191b0.png
--rw-------   0 joe       (1000) joe       (1000)    77589 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/imgs/anim/5e5767ae71a36650597d24fa84dd0b70.png
--rw-------   0 joe       (1000) joe       (1000)    24965 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/imgs/anim/908fe8fbd07106b45d209de37d64f385.png
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.804834 pyradium-0.0.8/docs/imgs/img/
--rw-------   0 joe       (1000) joe       (1000)    58960 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/imgs/img/2a58e4b31d16431abd7c4746e55fb701.png
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.804834 pyradium-0.0.8/docs/imgs/latex/
--rw-------   0 joe       (1000) joe       (1000)     3589 2021-11-02 07:47:47.000000 pyradium-0.0.8/docs/imgs/latex/6f86f5675c6bdba9e0f5d8e317fda102.png
--rw-------   0 joe       (1000) joe       (1000)     4637 2021-11-02 07:47:47.000000 pyradium-0.0.8/docs/imgs/latex/7c191ca8017c318fa68b68357c1ac979.png
--rw-------   0 joe       (1000) joe       (1000)     4157 2021-11-02 07:47:47.000000 pyradium-0.0.8/docs/imgs/latex/a28a8ba6d3dd046c7e3dfc4e80c1e76e.png
--rw-------   0 joe       (1000) joe       (1000)    40175 2021-11-02 07:47:47.000000 pyradium-0.0.8/docs/index.html
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.800834 pyradium-0.0.8/docs/template/
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.804834 pyradium-0.0.8/docs/template/antonio/
--rw-------   0 joe       (1000) joe       (1000)     3336 2021-11-02 07:47:47.000000 pyradium-0.0.8/docs/template/antonio/antonio.css
--rw-------   0 joe       (1000) joe       (1000)     2776 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/antonio/bar.svg
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.804834 pyradium-0.0.8/docs/template/antonio/font_fira/
--rw-------   0 joe       (1000) joe       (1000)    22336 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/antonio/font_fira/FiraSans-Bold-latin.woff2
--rw-------   0 joe       (1000) joe       (1000)    20952 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/antonio/font_fira/FiraSans-Light-latin.woff2
--rw-------   0 joe       (1000) joe       (1000)    21244 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/antonio/font_fira/FiraSans-Regular-latin.woff2
--rw-------   0 joe       (1000) joe       (1000)     7003 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/antonio/font_fira.css
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.804834 pyradium-0.0.8/docs/template/antonio/font_latinmodernmono/
--rw-------   0 joe       (1000) joe       (1000)    63584 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/antonio/font_latinmodernmono/lmmono10-italic.otf
--rw-------   0 joe       (1000) joe       (1000)    64684 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/antonio/font_latinmodernmono/lmmono10-regular.otf
--rw-------   0 joe       (1000) joe       (1000)      437 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/antonio/font_latinmodernmono.css
--rw-------   0 joe       (1000) joe       (1000)     3970 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/antonio/quote.svg
--rw-------   0 joe       (1000) joe       (1000)     2547 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/antonio/triangle1.svg
--rw-------   0 joe       (1000) joe       (1000)     2539 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/antonio/triangle2.svg
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.804834 pyradium-0.0.8/docs/template/base/
--rw-------   0 joe       (1000) joe       (1000)     1993 2021-11-02 07:47:47.000000 pyradium-0.0.8/docs/template/base/cursor.svg
--rw-------   0 joe       (1000) joe       (1000)     4207 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/base/pygments.css
--rw-------   0 joe       (1000) joe       (1000)     1809 2021-11-02 07:47:47.000000 pyradium-0.0.8/docs/template/base/pyradium.css
--rw-------   0 joe       (1000) joe       (1000)     9408 2021-11-02 07:47:47.000000 pyradium-0.0.8/docs/template/base/pyradium.js
--rw-------   0 joe       (1000) joe       (1000)     3208 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/base/pyradium_feedback.js
--rw-------   0 joe       (1000) joe       (1000)     1024 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/base/pyradium_forms.css
--rw-------   0 joe       (1000) joe       (1000)     2396 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/base/pyradium_forms.js
--rw-------   0 joe       (1000) joe       (1000)      775 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/base/pyradium_menu.css
--rw-------   0 joe       (1000) joe       (1000)      742 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/base/pyradium_modal.css
--rw-------   0 joe       (1000) joe       (1000)     1461 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/base/pyradium_modal.js
--rw-------   0 joe       (1000) joe       (1000)      341 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/base/pyradium_print.css
--rw-------   0 joe       (1000) joe       (1000)      852 2021-10-30 08:29:55.000000 pyradium-0.0.8/docs/template/base/pyradium_tooltip.css
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.804834 pyradium-0.0.8/examples/
--rw-------   0 joe       (1000) joe       (1000)     4968 2021-10-29 11:32:06.000000 pyradium-0.0.8/examples/3dbox.svg
--rw-------   0 joe       (1000) joe       (1000)      704 2021-11-03 07:03:57.000000 pyradium-0.0.8/examples/acronyms.json
--rw-------   0 joe       (1000) joe       (1000)     9401 2021-07-21 20:22:13.000000 pyradium-0.0.8/examples/animation.svg
--rw-------   0 joe       (1000) joe       (1000)     8159 2022-01-06 10:49:21.000000 pyradium-0.0.8/examples/example.xml
--rw-------   0 joe       (1000) joe       (1000)      826 2022-01-01 15:12:48.000000 pyradium-0.0.8/examples/histo.gnuplot
--rw-------   0 joe       (1000) joe       (1000)      137 2021-07-13 13:01:05.000000 pyradium-0.0.8/examples/my_data.py
--rwx------   0 joe       (1000) joe       (1000)      117 2021-10-28 21:08:12.000000 pyradium-0.0.8/examples/my_script
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.804834 pyradium-0.0.8/examples/sub/
--rw-------   0 joe       (1000) joe       (1000)      397 2021-10-28 21:08:12.000000 pyradium-0.0.8/examples/sub/example_sub.xml
--rw-------   0 joe       (1000) joe       (1000)       57 2021-07-13 13:01:05.000000 pyradium-0.0.8/examples/terminal_output.txt
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.804834 pyradium-0.0.8/licenses/
--rw-------   0 joe       (1000) joe       (1000)    18657 2021-07-21 20:22:13.000000 pyradium-0.0.8/licenses/CC-BY-4.0.txt
--rw-------   0 joe       (1000) joe       (1000)     1517 2021-07-21 20:22:13.000000 pyradium-0.0.8/licenses/GUST.txt
--rw-------   0 joe       (1000) joe       (1000)     4371 2021-07-08 19:38:29.000000 pyradium-0.0.8/licenses/OFL.txt
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.808834 pyradium-0.0.8/pyradium/
--rw-------   0 joe       (1000) joe       (1000)     2419 2021-10-29 20:01:44.000000 pyradium-0.0.8/pyradium/Acronyms.py
--rw-------   0 joe       (1000) joe       (1000)     2453 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/ActionAcroSort.py
--rw-------   0 joe       (1000) joe       (1000)     3647 2022-01-04 10:46:27.000000 pyradium-0.0.8/pyradium/ActionDictAdd.py
--rw-------   0 joe       (1000) joe       (1000)     1817 2021-10-30 07:40:42.000000 pyradium-0.0.8/pyradium/ActionDumpMetadata.py
--rw-------   0 joe       (1000) joe       (1000)     2688 2021-10-30 07:40:42.000000 pyradium-0.0.8/pyradium/ActionHashPresentation.py
--rw-------   0 joe       (1000) joe       (1000)     1129 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/ActionPurge.py
--rw-------   0 joe       (1000) joe       (1000)     5606 2021-11-17 16:14:17.000000 pyradium-0.0.8/pyradium/ActionRender.py
--rw-------   0 joe       (1000) joe       (1000)     1272 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/ActionServe.py
--rw-------   0 joe       (1000) joe       (1000)     1696 2021-11-17 16:14:17.000000 pyradium-0.0.8/pyradium/ActionShowStyleOpts.py
--rw-------   0 joe       (1000) joe       (1000)     5559 2022-01-04 10:36:46.000000 pyradium-0.0.8/pyradium/ActionSpellcheck.py
--rw-------   0 joe       (1000) joe       (1000)     4070 2021-12-04 20:05:31.000000 pyradium-0.0.8/pyradium/Agenda.py
--rw-------   0 joe       (1000) joe       (1000)     1486 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/BaseAction.py
--rw-------   0 joe       (1000) joe       (1000)      920 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/BaseDirective.py
--rw-------   0 joe       (1000) joe       (1000)     2515 2021-10-29 20:01:44.000000 pyradium-0.0.8/pyradium/CmdlineEscape.py
--rw-------   0 joe       (1000) joe       (1000)     2196 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/CmdlineParser.py
--rw-------   0 joe       (1000) joe       (1000)     2690 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/Controller.py
--rw-------   0 joe       (1000) joe       (1000)     1049 2021-11-05 22:49:09.000000 pyradium-0.0.8/pyradium/Enums.py
--rw-------   0 joe       (1000) joe       (1000)     2029 2022-01-06 10:47:35.000000 pyradium-0.0.8/pyradium/Exceptions.py
--rw-------   0 joe       (1000) joe       (1000)     2975 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/ExtendedJSONEncoder.py
--rw-------   0 joe       (1000) joe       (1000)     1573 2021-11-02 07:47:47.000000 pyradium-0.0.8/pyradium/FileLookup.py
--rw-------   0 joe       (1000) joe       (1000)     3162 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/FriendlyArgumentParser.py
--rw-------   0 joe       (1000) joe       (1000)     9802 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/GenericTOC.py
--rw-------   0 joe       (1000) joe       (1000)     1575 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/Logging.py
--rw-------   0 joe       (1000) joe       (1000)     6745 2021-11-02 07:47:47.000000 pyradium-0.0.8/pyradium/MultiCommand.py
--rw-------   0 joe       (1000) joe       (1000)     1272 2021-11-09 08:52:25.000000 pyradium-0.0.8/pyradium/OrderedSet.py
--rw-------   0 joe       (1000) joe       (1000)     3524 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/PauseRenderer.py
--rw-------   0 joe       (1000) joe       (1000)     1597 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/PrefixMatcher.py
--rw-------   0 joe       (1000) joe       (1000)     4611 2021-11-08 09:20:20.000000 pyradium-0.0.8/pyradium/Presentation.py
--rw-------   0 joe       (1000) joe       (1000)     1471 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/RenderableSlide.py
--rw-------   0 joe       (1000) joe       (1000)     5885 2021-11-05 22:49:09.000000 pyradium-0.0.8/pyradium/RenderedPresentation.py
--rw-------   0 joe       (1000) joe       (1000)     9069 2022-01-06 10:49:04.000000 pyradium-0.0.8/pyradium/Renderer.py
--rw-------   0 joe       (1000) joe       (1000)     3828 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/RendererCache.py
--rw-------   0 joe       (1000) joe       (1000)     3162 2021-11-17 16:14:17.000000 pyradium-0.0.8/pyradium/RenderingParameters.py
--rw-------   0 joe       (1000) joe       (1000)     4388 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/SVGTransformation.py
--rw-------   0 joe       (1000) joe       (1000)     9001 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/Schedule.py
--rw-------   0 joe       (1000) joe       (1000)     4874 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/Slide.py
--rw-------   0 joe       (1000) joe       (1000)    12542 2021-11-10 11:11:44.000000 pyradium-0.0.8/pyradium/Spellcheck.py
--rw-------   0 joe       (1000) joe       (1000)     4043 2021-11-10 11:11:44.000000 pyradium-0.0.8/pyradium/SpellcheckDictionary.py
--rw-------   0 joe       (1000) joe       (1000)     4416 2021-11-17 16:14:17.000000 pyradium-0.0.8/pyradium/StyleParameters.py
--rw-------   0 joe       (1000) joe       (1000)     1679 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/TOC.py
--rw-------   0 joe       (1000) joe       (1000)     7086 2021-11-05 22:49:09.000000 pyradium-0.0.8/pyradium/Tools.py
--rw-------   0 joe       (1000) joe       (1000)      934 2022-01-06 11:04:06.000000 pyradium-0.0.8/pyradium/__init__.py
--rw-------   0 joe       (1000) joe       (1000)    11569 2021-11-19 14:52:36.000000 pyradium-0.0.8/pyradium/__main__.py
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.812834 pyradium-0.0.8/pyradium/renderer/
--rw-------   0 joe       (1000) joe       (1000)     2104 2021-10-29 20:01:44.000000 pyradium-0.0.8/pyradium/renderer/ExecRenderer.py
--rw-------   0 joe       (1000) joe       (1000)     4160 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/renderer/ImageRenderer.py
--rw-------   0 joe       (1000) joe       (1000)     7901 2022-01-03 14:01:37.000000 pyradium-0.0.8/pyradium/renderer/LatexFormulaRenderer.py
--rw-------   0 joe       (1000) joe       (1000)     2489 2022-01-01 15:12:48.000000 pyradium-0.0.8/pyradium/renderer/PlotRenderer.py
--rw-------   0 joe       (1000) joe       (1000)      890 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/renderer/__init__.py
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.800834 pyradium-0.0.8/pyradium/templates/
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.812834 pyradium-0.0.8/pyradium/templates/antonio/
--rw-------   0 joe       (1000) joe       (1000)     4216 2022-01-06 10:41:34.000000 pyradium-0.0.8/pyradium/templates/antonio/antonio.css
--rw-------   0 joe       (1000) joe       (1000)     2776 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/bar.svg
--rw-------   0 joe       (1000) joe       (1000)     3798 2022-01-06 10:28:54.000000 pyradium-0.0.8/pyradium/templates/antonio/configuration.json
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.812834 pyradium-0.0.8/pyradium/templates/antonio/emojis/
--rw-------   0 joe       (1000) joe       (1000)     4977 2021-11-19 14:52:36.000000 pyradium-0.0.8/pyradium/templates/antonio/emojis/0-puke.svg
--rw-------   0 joe       (1000) joe       (1000)     2346 2021-11-19 14:52:36.000000 pyradium-0.0.8/pyradium/templates/antonio/emojis/1-bad.svg
--rw-------   0 joe       (1000) joe       (1000)     2335 2021-11-19 14:52:36.000000 pyradium-0.0.8/pyradium/templates/antonio/emojis/2-good.svg
--rw-------   0 joe       (1000) joe       (1000)     5370 2021-11-19 14:52:36.000000 pyradium-0.0.8/pyradium/templates/antonio/emojis/3-great.svg
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.816834 pyradium-0.0.8/pyradium/templates/antonio/font_fira/
--rw-------   0 joe       (1000) joe       (1000)    19440 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-cyrillic-ext.woff2
--rw-------   0 joe       (1000) joe       (1000)    11100 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-cyrillic.woff2
--rw-------   0 joe       (1000) joe       (1000)     8336 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-greek-ext.woff2
--rw-------   0 joe       (1000) joe       (1000)    13728 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-greek.woff2
--rw-------   0 joe       (1000) joe       (1000)    32540 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-latin-ext.woff2
--rw-------   0 joe       (1000) joe       (1000)    22336 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-latin.woff2
--rw-------   0 joe       (1000) joe       (1000)     7428 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-vietnamese.woff2
--rw-------   0 joe       (1000) joe       (1000)    17432 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-cyrillic-ext.woff2
--rw-------   0 joe       (1000) joe       (1000)    10124 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-cyrillic.woff2
--rw-------   0 joe       (1000) joe       (1000)     8228 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-greek-ext.woff2
--rw-------   0 joe       (1000) joe       (1000)    12752 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-greek.woff2
--rw-------   0 joe       (1000) joe       (1000)    29276 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-latin-ext.woff2
--rw-------   0 joe       (1000) joe       (1000)    20952 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-latin.woff2
--rw-------   0 joe       (1000) joe       (1000)     6836 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-vietnamese.woff2
--rw-------   0 joe       (1000) joe       (1000)    17572 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-cyrillic-ext.woff2
--rw-------   0 joe       (1000) joe       (1000)    10176 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-cyrillic.woff2
--rw-------   0 joe       (1000) joe       (1000)     7964 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-greek-ext.woff2
--rw-------   0 joe       (1000) joe       (1000)    12816 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-greek.woff2
--rw-------   0 joe       (1000) joe       (1000)    29764 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-latin-ext.woff2
--rw-------   0 joe       (1000) joe       (1000)    21244 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-latin.woff2
--rw-------   0 joe       (1000) joe       (1000)     7140 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-vietnamese.woff2
--rw-------   0 joe       (1000) joe       (1000)     7003 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_fira.css
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.816834 pyradium-0.0.8/pyradium/templates/antonio/font_latinmodernmono/
--rw-------   0 joe       (1000) joe       (1000)    63584 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_latinmodernmono/lmmono10-italic.otf
--rw-------   0 joe       (1000) joe       (1000)    64684 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/font_latinmodernmono/lmmono10-regular.otf
--rw-------   0 joe       (1000) joe       (1000)      441 2021-11-05 17:24:35.000000 pyradium-0.0.8/pyradium/templates/antonio/font_latinmodernmono.css
--rw-------   0 joe       (1000) joe       (1000)     3970 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/quote.svg
--rw-------   0 joe       (1000) joe       (1000)      424 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/slide_acronyms.html
--rw-------   0 joe       (1000) joe       (1000)      126 2021-11-04 11:41:39.000000 pyradium-0.0.8/pyradium/templates/antonio/slide_animation.html
--rw-------   0 joe       (1000) joe       (1000)       63 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/slide_default.html
--rw-------   0 joe       (1000) joe       (1000)     3057 2021-12-04 20:02:17.000000 pyradium-0.0.8/pyradium/templates/antonio/slide_feedback.html
--rw-------   0 joe       (1000) joe       (1000)      416 2021-11-04 11:41:39.000000 pyradium-0.0.8/pyradium/templates/antonio/slide_final.html
--rw-------   0 joe       (1000) joe       (1000)      191 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/slide_leftright.html
--rw-------   0 joe       (1000) joe       (1000)      378 2021-11-04 11:41:39.000000 pyradium-0.0.8/pyradium/templates/antonio/slide_quote.html
--rw-------   0 joe       (1000) joe       (1000)      622 2022-01-06 10:40:24.000000 pyradium-0.0.8/pyradium/templates/antonio/slide_sectiontitle.html
--rw-------   0 joe       (1000) joe       (1000)      463 2021-11-04 11:41:39.000000 pyradium-0.0.8/pyradium/templates/antonio/slide_title.html
--rw-------   0 joe       (1000) joe       (1000)      546 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/slide_toc.html
--rw-------   0 joe       (1000) joe       (1000)      995 2021-11-04 11:41:39.000000 pyradium-0.0.8/pyradium/templates/antonio/template_slide.html
--rw-------   0 joe       (1000) joe       (1000)     2547 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/triangle1.svg
--rw-------   0 joe       (1000) joe       (1000)     2539 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/antonio/triangle2.svg
--rw-------   0 joe       (1000) joe       (1000)     2601 2022-01-06 10:28:02.000000 pyradium-0.0.8/pyradium/templates/antonio/tribar.svg
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.816834 pyradium-0.0.8/pyradium/templates/base/
--rw-------   0 joe       (1000) joe       (1000)     2147 2021-11-06 15:09:13.000000 pyradium-0.0.8/pyradium/templates/base/controller_acronym.py
--rw-------   0 joe       (1000) joe       (1000)     2952 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/templates/base/controller_animation.py
--rw-------   0 joe       (1000) joe       (1000)     1955 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/templates/base/controller_toc.py
--rw-------   0 joe       (1000) joe       (1000)     1993 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/base/cursor.svg
--rw-------   0 joe       (1000) joe       (1000)     3735 2021-11-08 09:20:20.000000 pyradium-0.0.8/pyradium/templates/base/index.html
--rw-------   0 joe       (1000) joe       (1000)     3703 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/templates/base/media_error.svg
--rw-------   0 joe       (1000) joe       (1000)     2302 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/base/media_pause.svg
--rw-------   0 joe       (1000) joe       (1000)     2430 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/base/media_play.svg
--rw-------   0 joe       (1000) joe       (1000)     1974 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/base/media_stop.svg
--rw-------   0 joe       (1000) joe       (1000)     4207 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/base/pygments.css
--rw-------   0 joe       (1000) joe       (1000)     1961 2021-11-04 11:41:39.000000 pyradium-0.0.8/pyradium/templates/base/pyradium.css
--rw-------   0 joe       (1000) joe       (1000)     9791 2021-11-08 09:20:20.000000 pyradium-0.0.8/pyradium/templates/base/pyradium.js
--rw-------   0 joe       (1000) joe       (1000)     3208 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_feedback.js
--rw-------   0 joe       (1000) joe       (1000)      996 2021-12-04 20:02:17.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_forms.css
--rw-------   0 joe       (1000) joe       (1000)     2396 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_forms.js
--rw-------   0 joe       (1000) joe       (1000)       34 2021-11-08 09:20:20.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_info.css
--rw-------   0 joe       (1000) joe       (1000)      865 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_menu.css
--rw-------   0 joe       (1000) joe       (1000)      808 2021-11-08 09:20:20.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_modal.css
--rw-------   0 joe       (1000) joe       (1000)     1693 2021-11-08 09:20:20.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_modal.js
--rw-------   0 joe       (1000) joe       (1000)      341 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_print.css
--rw-------   0 joe       (1000) joe       (1000)     1218 2021-11-04 11:41:39.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_timer.css
--rw-------   0 joe       (1000) joe       (1000)    18714 2021-11-08 09:20:20.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_timer.js
--rw-------   0 joe       (1000) joe       (1000)     5837 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_tools.js
--rw-------   0 joe       (1000) joe       (1000)      905 2021-11-08 09:20:20.000000 pyradium-0.0.8/pyradium/templates/base/pyradium_tooltip.css
--rw-------   0 joe       (1000) joe       (1000)      385 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/templates/base/slide.html
--rw-------   0 joe       (1000) joe       (1000)     3234 2021-11-08 09:20:20.000000 pyradium-0.0.8/pyradium/templates/base/timer.html
--rw-------   0 joe       (1000) joe       (1000)      103 2021-12-04 20:05:31.000000 pyradium-0.0.8/pyradium/templates/base/x
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.816834 pyradium-0.0.8/pyradium/tests/
--rw-------   0 joe       (1000) joe       (1000)     2826 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/tests/CmdlineParserTests.py
--rw-------   0 joe       (1000) joe       (1000)     5230 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/tests/TimeSpecificationTests.py
--rw-------   0 joe       (1000) joe       (1000)     1001 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/tests/__init__.py
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.820834 pyradium-0.0.8/pyradium/xmlhooks/
--rw-------   0 joe       (1000) joe       (1000)     2253 2021-11-08 09:20:20.000000 pyradium-0.0.8/pyradium/xmlhooks/AcronymHook.py
--rw-------   0 joe       (1000) joe       (1000)     1299 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/xmlhooks/ArrowHook.py
--rw-------   0 joe       (1000) joe       (1000)     1569 2021-11-05 22:49:09.000000 pyradium-0.0.8/pyradium/xmlhooks/CodeHook.py
--rw-------   0 joe       (1000) joe       (1000)     1203 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/xmlhooks/DebugHook.py
--rw-------   0 joe       (1000) joe       (1000)     1288 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/xmlhooks/EmoHook.py
--rw-------   0 joe       (1000) joe       (1000)     2631 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/xmlhooks/ExecHook.py
--rw-------   0 joe       (1000) joe       (1000)     2065 2021-11-04 11:41:39.000000 pyradium-0.0.8/pyradium/xmlhooks/ImgHook.py
--rw-------   0 joe       (1000) joe       (1000)     1341 2021-11-19 14:52:36.000000 pyradium-0.0.8/pyradium/xmlhooks/LinkHook.py
--rw-------   0 joe       (1000) joe       (1000)     1401 2021-10-29 20:01:44.000000 pyradium-0.0.8/pyradium/xmlhooks/MonospaceHook.py
--rw-------   0 joe       (1000) joe       (1000)     1387 2022-01-05 11:28:40.000000 pyradium-0.0.8/pyradium/xmlhooks/NoLinebreakHook.py
--rw-------   0 joe       (1000) joe       (1000)     1141 2021-11-19 14:52:36.000000 pyradium-0.0.8/pyradium/xmlhooks/NoSpellcheckHook.py
--rw-------   0 joe       (1000) joe       (1000)     1579 2021-11-08 09:20:20.000000 pyradium-0.0.8/pyradium/xmlhooks/NthHook.py
--rw-------   0 joe       (1000) joe       (1000)     2066 2022-01-01 15:12:48.000000 pyradium-0.0.8/pyradium/xmlhooks/PlotHook.py
--rw-------   0 joe       (1000) joe       (1000)     1442 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/xmlhooks/QuoteHook.py
--rw-------   0 joe       (1000) joe       (1000)     1336 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/xmlhooks/SymbolHook.py
--rw-------   0 joe       (1000) joe       (1000)     1340 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium/xmlhooks/TerminalHook.py
--rw-------   0 joe       (1000) joe       (1000)     2466 2021-11-04 11:41:39.000000 pyradium-0.0.8/pyradium/xmlhooks/TexHook.py
--rw-------   0 joe       (1000) joe       (1000)     1560 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/xmlhooks/TimeHook.py
--rw-------   0 joe       (1000) joe       (1000)     4202 2021-11-03 07:03:57.000000 pyradium-0.0.8/pyradium/xmlhooks/XMLHookRegistry.py
--rw-------   0 joe       (1000) joe       (1000)     1505 2022-01-05 11:22:25.000000 pyradium-0.0.8/pyradium/xmlhooks/__init__.py
-drwx------   0 joe       (1000) joe       (1000)        0 2022-01-06 11:04:35.812834 pyradium-0.0.8/pyradium.egg-info/
--rw-------   0 joe       (1000) joe       (1000)    17813 2022-01-06 11:04:35.000000 pyradium-0.0.8/pyradium.egg-info/PKG-INFO
--rw-------   0 joe       (1000) joe       (1000)     7624 2022-01-06 11:04:35.000000 pyradium-0.0.8/pyradium.egg-info/SOURCES.txt
--rw-------   0 joe       (1000) joe       (1000)        1 2022-01-06 11:04:35.000000 pyradium-0.0.8/pyradium.egg-info/dependency_links.txt
--rw-------   0 joe       (1000) joe       (1000)       53 2022-01-06 11:04:35.000000 pyradium-0.0.8/pyradium.egg-info/entry_points.txt
--rw-------   0 joe       (1000) joe       (1000)       14 2022-01-06 11:04:35.000000 pyradium-0.0.8/pyradium.egg-info/requires.txt
--rw-------   0 joe       (1000) joe       (1000)        9 2022-01-06 11:04:35.000000 pyradium-0.0.8/pyradium.egg-info/top_level.txt
--rwx------   0 joe       (1000) joe       (1000)      977 2021-10-28 21:08:12.000000 pyradium-0.0.8/pyradium.py
--rwx------   0 joe       (1000) joe       (1000)      322 2021-10-28 21:08:12.000000 pyradium-0.0.8/rerender
--rwx------   0 joe       (1000) joe       (1000)     1902 2021-10-28 21:08:12.000000 pyradium-0.0.8/serve
--rw-------   0 joe       (1000) joe       (1000)       38 2022-01-06 11:04:35.820834 pyradium-0.0.8/setup.cfg
--rw-------   0 joe       (1000) joe       (1000)     1331 2021-11-02 07:47:47.000000 pyradium-0.0.8/setup.py
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.149730 pyradium-0.0.9/
+-rw-------   0 joe       (1000) joe       (1000)       52 2022-01-01 15:12:48.000000 pyradium-0.0.9/.gitignore
+-rw-------   0 joe       (1000) joe       (1000)       77 2021-10-28 21:08:12.000000 pyradium-0.0.9/.travis.yml
+-rw-------   0 joe       (1000) joe       (1000)    35142 2020-03-30 11:18:51.000000 pyradium-0.0.9/LICENSE
+-rw-------   0 joe       (1000) joe       (1000)      107 2021-10-28 21:08:12.000000 pyradium-0.0.9/MANIFEST.in
+-rw-------   0 joe       (1000) joe       (1000)    17813 2022-01-30 22:24:17.149730 pyradium-0.0.9/PKG-INFO
+-rw-------   0 joe       (1000) joe       (1000)    14401 2022-01-04 10:52:31.000000 pyradium-0.0.9/README.md
+-rwx------   0 joe       (1000) joe       (1000)      251 2021-11-05 22:49:09.000000 pyradium-0.0.9/autorender
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.117730 pyradium-0.0.9/docs/
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.113730 pyradium-0.0.9/docs/imgs/
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.117730 pyradium-0.0.9/docs/imgs/anim/
+-rw-------   0 joe       (1000) joe       (1000)    31808 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/imgs/anim/21da33acb6f14b9f6bf7eae05bf191b0.png
+-rw-------   0 joe       (1000) joe       (1000)    77589 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/imgs/anim/5e5767ae71a36650597d24fa84dd0b70.png
+-rw-------   0 joe       (1000) joe       (1000)    24965 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/imgs/anim/908fe8fbd07106b45d209de37d64f385.png
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.117730 pyradium-0.0.9/docs/imgs/img/
+-rw-------   0 joe       (1000) joe       (1000)    58960 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/imgs/img/2a58e4b31d16431abd7c4746e55fb701.png
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.117730 pyradium-0.0.9/docs/imgs/latex/
+-rw-------   0 joe       (1000) joe       (1000)     3589 2021-11-02 07:47:47.000000 pyradium-0.0.9/docs/imgs/latex/6f86f5675c6bdba9e0f5d8e317fda102.png
+-rw-------   0 joe       (1000) joe       (1000)     4637 2021-11-02 07:47:47.000000 pyradium-0.0.9/docs/imgs/latex/7c191ca8017c318fa68b68357c1ac979.png
+-rw-------   0 joe       (1000) joe       (1000)     4157 2021-11-02 07:47:47.000000 pyradium-0.0.9/docs/imgs/latex/a28a8ba6d3dd046c7e3dfc4e80c1e76e.png
+-rw-------   0 joe       (1000) joe       (1000)    40175 2021-11-02 07:47:47.000000 pyradium-0.0.9/docs/index.html
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.113730 pyradium-0.0.9/docs/template/
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.121730 pyradium-0.0.9/docs/template/antonio/
+-rw-------   0 joe       (1000) joe       (1000)     3336 2021-11-02 07:47:47.000000 pyradium-0.0.9/docs/template/antonio/antonio.css
+-rw-------   0 joe       (1000) joe       (1000)     2776 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/antonio/bar.svg
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.121730 pyradium-0.0.9/docs/template/antonio/font_fira/
+-rw-------   0 joe       (1000) joe       (1000)    22336 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/antonio/font_fira/FiraSans-Bold-latin.woff2
+-rw-------   0 joe       (1000) joe       (1000)    20952 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/antonio/font_fira/FiraSans-Light-latin.woff2
+-rw-------   0 joe       (1000) joe       (1000)    21244 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/antonio/font_fira/FiraSans-Regular-latin.woff2
+-rw-------   0 joe       (1000) joe       (1000)     7003 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/antonio/font_fira.css
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.121730 pyradium-0.0.9/docs/template/antonio/font_latinmodernmono/
+-rw-------   0 joe       (1000) joe       (1000)    63584 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/antonio/font_latinmodernmono/lmmono10-italic.otf
+-rw-------   0 joe       (1000) joe       (1000)    64684 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/antonio/font_latinmodernmono/lmmono10-regular.otf
+-rw-------   0 joe       (1000) joe       (1000)      437 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/antonio/font_latinmodernmono.css
+-rw-------   0 joe       (1000) joe       (1000)     3970 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/antonio/quote.svg
+-rw-------   0 joe       (1000) joe       (1000)     2547 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/antonio/triangle1.svg
+-rw-------   0 joe       (1000) joe       (1000)     2539 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/antonio/triangle2.svg
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.125730 pyradium-0.0.9/docs/template/base/
+-rw-------   0 joe       (1000) joe       (1000)     1993 2021-11-02 07:47:47.000000 pyradium-0.0.9/docs/template/base/cursor.svg
+-rw-------   0 joe       (1000) joe       (1000)     4207 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/base/pygments.css
+-rw-------   0 joe       (1000) joe       (1000)     1809 2021-11-02 07:47:47.000000 pyradium-0.0.9/docs/template/base/pyradium.css
+-rw-------   0 joe       (1000) joe       (1000)     9408 2021-11-02 07:47:47.000000 pyradium-0.0.9/docs/template/base/pyradium.js
+-rw-------   0 joe       (1000) joe       (1000)     3208 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/base/pyradium_feedback.js
+-rw-------   0 joe       (1000) joe       (1000)     1024 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/base/pyradium_forms.css
+-rw-------   0 joe       (1000) joe       (1000)     2396 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/base/pyradium_forms.js
+-rw-------   0 joe       (1000) joe       (1000)      775 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/base/pyradium_menu.css
+-rw-------   0 joe       (1000) joe       (1000)      742 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/base/pyradium_modal.css
+-rw-------   0 joe       (1000) joe       (1000)     1461 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/base/pyradium_modal.js
+-rw-------   0 joe       (1000) joe       (1000)      341 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/base/pyradium_print.css
+-rw-------   0 joe       (1000) joe       (1000)      852 2021-10-30 08:29:55.000000 pyradium-0.0.9/docs/template/base/pyradium_tooltip.css
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.125730 pyradium-0.0.9/examples/
+-rw-------   0 joe       (1000) joe       (1000)     6299 2022-01-12 20:12:24.000000 pyradium-0.0.9/examples/3dbox.svg
+-rw-------   0 joe       (1000) joe       (1000)      837 2022-01-30 22:19:17.000000 pyradium-0.0.9/examples/acronyms.json
+-rw-------   0 joe       (1000) joe       (1000)     9401 2021-07-21 20:22:13.000000 pyradium-0.0.9/examples/animation.svg
+-rw-------   0 joe       (1000) joe       (1000)     8625 2022-01-30 22:19:37.000000 pyradium-0.0.9/examples/example.xml
+-rw-------   0 joe       (1000) joe       (1000)      826 2022-01-01 15:12:48.000000 pyradium-0.0.9/examples/histo.gnuplot
+-rw-------   0 joe       (1000) joe       (1000)      137 2021-07-13 13:01:05.000000 pyradium-0.0.9/examples/my_data.py
+-rwx------   0 joe       (1000) joe       (1000)      117 2021-10-28 21:08:12.000000 pyradium-0.0.9/examples/my_script
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.125730 pyradium-0.0.9/examples/sub/
+-rw-------   0 joe       (1000) joe       (1000)      397 2021-10-28 21:08:12.000000 pyradium-0.0.9/examples/sub/example_sub.xml
+-rw-------   0 joe       (1000) joe       (1000)       57 2021-07-13 13:01:05.000000 pyradium-0.0.9/examples/terminal_output.txt
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.125730 pyradium-0.0.9/licenses/
+-rw-------   0 joe       (1000) joe       (1000)    18657 2021-07-21 20:22:13.000000 pyradium-0.0.9/licenses/CC-BY-4.0.txt
+-rw-------   0 joe       (1000) joe       (1000)     1517 2021-07-21 20:22:13.000000 pyradium-0.0.9/licenses/GUST.txt
+-rw-------   0 joe       (1000) joe       (1000)     4371 2021-07-08 19:38:29.000000 pyradium-0.0.9/licenses/OFL.txt
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.137730 pyradium-0.0.9/pyradium/
+-rw-------   0 joe       (1000) joe       (1000)     3514 2022-01-10 13:23:27.000000 pyradium-0.0.9/pyradium/Acrofile.py
+-rw-------   0 joe       (1000) joe       (1000)     2424 2022-01-30 22:21:07.000000 pyradium-0.0.9/pyradium/Acronyms.py
+-rw-------   0 joe       (1000) joe       (1000)     2011 2022-01-10 13:27:00.000000 pyradium-0.0.9/pyradium/ActionAcroAdd.py
+-rw-------   0 joe       (1000) joe       (1000)     1112 2022-01-10 13:17:51.000000 pyradium-0.0.9/pyradium/ActionAcroSort.py
+-rw-------   0 joe       (1000) joe       (1000)     3647 2022-01-04 10:46:27.000000 pyradium-0.0.9/pyradium/ActionDictAdd.py
+-rw-------   0 joe       (1000) joe       (1000)     1817 2021-10-30 07:40:42.000000 pyradium-0.0.9/pyradium/ActionDumpMetadata.py
+-rw-------   0 joe       (1000) joe       (1000)     2688 2021-10-30 07:40:42.000000 pyradium-0.0.9/pyradium/ActionHashPresentation.py
+-rw-------   0 joe       (1000) joe       (1000)     1129 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/ActionPurge.py
+-rw-------   0 joe       (1000) joe       (1000)     5606 2021-11-17 16:14:17.000000 pyradium-0.0.9/pyradium/ActionRender.py
+-rw-------   0 joe       (1000) joe       (1000)     1272 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/ActionServe.py
+-rw-------   0 joe       (1000) joe       (1000)     1696 2021-11-17 16:14:17.000000 pyradium-0.0.9/pyradium/ActionShowStyleOpts.py
+-rw-------   0 joe       (1000) joe       (1000)     5559 2022-01-04 10:36:46.000000 pyradium-0.0.9/pyradium/ActionSpellcheck.py
+-rw-------   0 joe       (1000) joe       (1000)     4070 2021-12-04 20:05:31.000000 pyradium-0.0.9/pyradium/Agenda.py
+-rw-------   0 joe       (1000) joe       (1000)     1486 2021-11-03 07:03:57.000000 pyradium-0.0.9/pyradium/BaseAction.py
+-rw-------   0 joe       (1000) joe       (1000)      920 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/BaseDirective.py
+-rw-------   0 joe       (1000) joe       (1000)     2515 2021-10-29 20:01:44.000000 pyradium-0.0.9/pyradium/CmdlineEscape.py
+-rw-------   0 joe       (1000) joe       (1000)     2196 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/CmdlineParser.py
+-rw-------   0 joe       (1000) joe       (1000)     2690 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/Controller.py
+-rw-------   0 joe       (1000) joe       (1000)     1049 2021-11-05 22:49:09.000000 pyradium-0.0.9/pyradium/Enums.py
+-rw-------   0 joe       (1000) joe       (1000)     2255 2022-01-12 20:17:56.000000 pyradium-0.0.9/pyradium/Exceptions.py
+-rw-------   0 joe       (1000) joe       (1000)     2975 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/ExtendedJSONEncoder.py
+-rw-------   0 joe       (1000) joe       (1000)     1573 2021-11-02 07:47:47.000000 pyradium-0.0.9/pyradium/FileLookup.py
+-rw-------   0 joe       (1000) joe       (1000)     3162 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/FriendlyArgumentParser.py
+-rw-------   0 joe       (1000) joe       (1000)     9802 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/GenericTOC.py
+-rw-------   0 joe       (1000) joe       (1000)     1575 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/Logging.py
+-rw-------   0 joe       (1000) joe       (1000)     6745 2021-11-02 07:47:47.000000 pyradium-0.0.9/pyradium/MultiCommand.py
+-rw-------   0 joe       (1000) joe       (1000)     1272 2021-11-09 08:52:25.000000 pyradium-0.0.9/pyradium/OrderedSet.py
+-rw-------   0 joe       (1000) joe       (1000)     3524 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/PauseRenderer.py
+-rw-------   0 joe       (1000) joe       (1000)     1597 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/PrefixMatcher.py
+-rw-------   0 joe       (1000) joe       (1000)     4611 2021-11-08 09:20:20.000000 pyradium-0.0.9/pyradium/Presentation.py
+-rw-------   0 joe       (1000) joe       (1000)     1471 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/RenderableSlide.py
+-rw-------   0 joe       (1000) joe       (1000)     5885 2021-11-05 22:49:09.000000 pyradium-0.0.9/pyradium/RenderedPresentation.py
+-rw-------   0 joe       (1000) joe       (1000)     9069 2022-01-06 10:49:04.000000 pyradium-0.0.9/pyradium/Renderer.py
+-rw-------   0 joe       (1000) joe       (1000)     3828 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/RendererCache.py
+-rw-------   0 joe       (1000) joe       (1000)     3162 2021-11-17 16:14:17.000000 pyradium-0.0.9/pyradium/RenderingParameters.py
+-rw-------   0 joe       (1000) joe       (1000)     5052 2022-01-12 16:12:03.000000 pyradium-0.0.9/pyradium/SVGTransformation.py
+-rw-------   0 joe       (1000) joe       (1000)     9001 2021-11-03 07:03:57.000000 pyradium-0.0.9/pyradium/Schedule.py
+-rw-------   0 joe       (1000) joe       (1000)     4874 2021-11-03 07:03:57.000000 pyradium-0.0.9/pyradium/Slide.py
+-rw-------   0 joe       (1000) joe       (1000)    12542 2021-11-10 11:11:44.000000 pyradium-0.0.9/pyradium/Spellcheck.py
+-rw-------   0 joe       (1000) joe       (1000)     4043 2021-11-10 11:11:44.000000 pyradium-0.0.9/pyradium/SpellcheckDictionary.py
+-rw-------   0 joe       (1000) joe       (1000)     4416 2021-11-17 16:14:17.000000 pyradium-0.0.9/pyradium/StyleParameters.py
+-rw-------   0 joe       (1000) joe       (1000)     1679 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/TOC.py
+-rw-------   0 joe       (1000) joe       (1000)     7349 2022-01-21 11:49:52.000000 pyradium-0.0.9/pyradium/Tools.py
+-rw-------   0 joe       (1000) joe       (1000)      934 2022-01-30 22:23:52.000000 pyradium-0.0.9/pyradium/__init__.py
+-rw-------   0 joe       (1000) joe       (1000)    12002 2022-01-10 13:22:43.000000 pyradium-0.0.9/pyradium/__main__.py
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.137730 pyradium-0.0.9/pyradium/renderer/
+-rw-------   0 joe       (1000) joe       (1000)     2104 2021-10-29 20:01:44.000000 pyradium-0.0.9/pyradium/renderer/ExecRenderer.py
+-rw-------   0 joe       (1000) joe       (1000)     4160 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/renderer/ImageRenderer.py
+-rw-------   0 joe       (1000) joe       (1000)     7901 2022-01-03 14:01:37.000000 pyradium-0.0.9/pyradium/renderer/LatexFormulaRenderer.py
+-rw-------   0 joe       (1000) joe       (1000)     2489 2022-01-01 15:12:48.000000 pyradium-0.0.9/pyradium/renderer/PlotRenderer.py
+-rw-------   0 joe       (1000) joe       (1000)      890 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/renderer/__init__.py
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.113730 pyradium-0.0.9/pyradium/templates/
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.137730 pyradium-0.0.9/pyradium/templates/antonio/
+-rw-------   0 joe       (1000) joe       (1000)     4274 2022-01-12 20:32:41.000000 pyradium-0.0.9/pyradium/templates/antonio/antonio.css
+-rw-------   0 joe       (1000) joe       (1000)     2776 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/bar.svg
+-rw-------   0 joe       (1000) joe       (1000)     3798 2022-01-06 10:28:54.000000 pyradium-0.0.9/pyradium/templates/antonio/configuration.json
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.137730 pyradium-0.0.9/pyradium/templates/antonio/emojis/
+-rw-------   0 joe       (1000) joe       (1000)     4977 2021-11-19 14:52:36.000000 pyradium-0.0.9/pyradium/templates/antonio/emojis/0-puke.svg
+-rw-------   0 joe       (1000) joe       (1000)     2346 2021-11-19 14:52:36.000000 pyradium-0.0.9/pyradium/templates/antonio/emojis/1-bad.svg
+-rw-------   0 joe       (1000) joe       (1000)     2335 2021-11-19 14:52:36.000000 pyradium-0.0.9/pyradium/templates/antonio/emojis/2-good.svg
+-rw-------   0 joe       (1000) joe       (1000)     5370 2021-11-19 14:52:36.000000 pyradium-0.0.9/pyradium/templates/antonio/emojis/3-great.svg
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.141730 pyradium-0.0.9/pyradium/templates/antonio/font_fira/
+-rw-------   0 joe       (1000) joe       (1000)    19440 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-cyrillic-ext.woff2
+-rw-------   0 joe       (1000) joe       (1000)    11100 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-cyrillic.woff2
+-rw-------   0 joe       (1000) joe       (1000)     8336 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-greek-ext.woff2
+-rw-------   0 joe       (1000) joe       (1000)    13728 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-greek.woff2
+-rw-------   0 joe       (1000) joe       (1000)    32540 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-latin-ext.woff2
+-rw-------   0 joe       (1000) joe       (1000)    22336 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-latin.woff2
+-rw-------   0 joe       (1000) joe       (1000)     7428 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-vietnamese.woff2
+-rw-------   0 joe       (1000) joe       (1000)    17432 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-cyrillic-ext.woff2
+-rw-------   0 joe       (1000) joe       (1000)    10124 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-cyrillic.woff2
+-rw-------   0 joe       (1000) joe       (1000)     8228 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-greek-ext.woff2
+-rw-------   0 joe       (1000) joe       (1000)    12752 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-greek.woff2
+-rw-------   0 joe       (1000) joe       (1000)    29276 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-latin-ext.woff2
+-rw-------   0 joe       (1000) joe       (1000)    20952 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-latin.woff2
+-rw-------   0 joe       (1000) joe       (1000)     6836 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-vietnamese.woff2
+-rw-------   0 joe       (1000) joe       (1000)    17572 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-cyrillic-ext.woff2
+-rw-------   0 joe       (1000) joe       (1000)    10176 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-cyrillic.woff2
+-rw-------   0 joe       (1000) joe       (1000)     7964 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-greek-ext.woff2
+-rw-------   0 joe       (1000) joe       (1000)    12816 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-greek.woff2
+-rw-------   0 joe       (1000) joe       (1000)    29764 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-latin-ext.woff2
+-rw-------   0 joe       (1000) joe       (1000)    21244 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-latin.woff2
+-rw-------   0 joe       (1000) joe       (1000)     7140 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-vietnamese.woff2
+-rw-------   0 joe       (1000) joe       (1000)     7003 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_fira.css
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.145730 pyradium-0.0.9/pyradium/templates/antonio/font_latinmodernmono/
+-rw-------   0 joe       (1000) joe       (1000)    63584 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_latinmodernmono/lmmono10-italic.otf
+-rw-------   0 joe       (1000) joe       (1000)    64684 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/font_latinmodernmono/lmmono10-regular.otf
+-rw-------   0 joe       (1000) joe       (1000)      441 2021-11-05 17:24:35.000000 pyradium-0.0.9/pyradium/templates/antonio/font_latinmodernmono.css
+-rw-------   0 joe       (1000) joe       (1000)     3970 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/quote.svg
+-rw-------   0 joe       (1000) joe       (1000)      424 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/slide_acronyms.html
+-rw-------   0 joe       (1000) joe       (1000)      126 2021-11-04 11:41:39.000000 pyradium-0.0.9/pyradium/templates/antonio/slide_animation.html
+-rw-------   0 joe       (1000) joe       (1000)       63 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/slide_default.html
+-rw-------   0 joe       (1000) joe       (1000)     3057 2021-12-04 20:02:17.000000 pyradium-0.0.9/pyradium/templates/antonio/slide_feedback.html
+-rw-------   0 joe       (1000) joe       (1000)      416 2021-11-04 11:41:39.000000 pyradium-0.0.9/pyradium/templates/antonio/slide_final.html
+-rw-------   0 joe       (1000) joe       (1000)      191 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/slide_leftright.html
+-rw-------   0 joe       (1000) joe       (1000)      378 2021-11-04 11:41:39.000000 pyradium-0.0.9/pyradium/templates/antonio/slide_quote.html
+-rw-------   0 joe       (1000) joe       (1000)      622 2022-01-06 10:40:24.000000 pyradium-0.0.9/pyradium/templates/antonio/slide_sectiontitle.html
+-rw-------   0 joe       (1000) joe       (1000)      463 2021-11-04 11:41:39.000000 pyradium-0.0.9/pyradium/templates/antonio/slide_title.html
+-rw-------   0 joe       (1000) joe       (1000)      546 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/slide_toc.html
+-rw-------   0 joe       (1000) joe       (1000)      995 2021-11-04 11:41:39.000000 pyradium-0.0.9/pyradium/templates/antonio/template_slide.html
+-rw-------   0 joe       (1000) joe       (1000)     2547 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/triangle1.svg
+-rw-------   0 joe       (1000) joe       (1000)     2539 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/antonio/triangle2.svg
+-rw-------   0 joe       (1000) joe       (1000)     2601 2022-01-06 10:28:02.000000 pyradium-0.0.9/pyradium/templates/antonio/tribar.svg
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.145730 pyradium-0.0.9/pyradium/templates/base/
+-rw-------   0 joe       (1000) joe       (1000)     2147 2021-11-06 15:09:13.000000 pyradium-0.0.9/pyradium/templates/base/controller_acronym.py
+-rw-------   0 joe       (1000) joe       (1000)     3740 2022-01-12 15:47:09.000000 pyradium-0.0.9/pyradium/templates/base/controller_animation.py
+-rw-------   0 joe       (1000) joe       (1000)     1955 2021-11-03 07:03:57.000000 pyradium-0.0.9/pyradium/templates/base/controller_toc.py
+-rw-------   0 joe       (1000) joe       (1000)     1993 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/base/cursor.svg
+-rw-------   0 joe       (1000) joe       (1000)     3735 2021-11-08 09:20:20.000000 pyradium-0.0.9/pyradium/templates/base/index.html
+-rw-------   0 joe       (1000) joe       (1000)     3703 2021-11-03 07:03:57.000000 pyradium-0.0.9/pyradium/templates/base/media_error.svg
+-rw-------   0 joe       (1000) joe       (1000)     2302 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/base/media_pause.svg
+-rw-------   0 joe       (1000) joe       (1000)     2430 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/base/media_play.svg
+-rw-------   0 joe       (1000) joe       (1000)     1974 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/base/media_stop.svg
+-rw-------   0 joe       (1000) joe       (1000)     4277 2022-01-18 15:55:54.000000 pyradium-0.0.9/pyradium/templates/base/pygments.css
+-rw-------   0 joe       (1000) joe       (1000)     2115 2022-01-29 14:25:39.000000 pyradium-0.0.9/pyradium/templates/base/pyradium.css
+-rw-------   0 joe       (1000) joe       (1000)     9791 2021-11-08 09:20:20.000000 pyradium-0.0.9/pyradium/templates/base/pyradium.js
+-rw-------   0 joe       (1000) joe       (1000)     3208 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_feedback.js
+-rw-------   0 joe       (1000) joe       (1000)      996 2021-12-04 20:02:17.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_forms.css
+-rw-------   0 joe       (1000) joe       (1000)     2396 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_forms.js
+-rw-------   0 joe       (1000) joe       (1000)       34 2021-11-08 09:20:20.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_info.css
+-rw-------   0 joe       (1000) joe       (1000)      865 2021-11-03 07:03:57.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_menu.css
+-rw-------   0 joe       (1000) joe       (1000)      808 2021-11-08 09:20:20.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_modal.css
+-rw-------   0 joe       (1000) joe       (1000)     1693 2021-11-08 09:20:20.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_modal.js
+-rw-------   0 joe       (1000) joe       (1000)      341 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_print.css
+-rw-------   0 joe       (1000) joe       (1000)     1218 2021-11-04 11:41:39.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_timer.css
+-rw-------   0 joe       (1000) joe       (1000)    18714 2021-11-08 09:20:20.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_timer.js
+-rw-------   0 joe       (1000) joe       (1000)     5837 2021-11-03 07:03:57.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_tools.js
+-rw-------   0 joe       (1000) joe       (1000)      905 2021-11-08 09:20:20.000000 pyradium-0.0.9/pyradium/templates/base/pyradium_tooltip.css
+-rw-------   0 joe       (1000) joe       (1000)      385 2021-11-03 07:03:57.000000 pyradium-0.0.9/pyradium/templates/base/slide.html
+-rw-------   0 joe       (1000) joe       (1000)     3234 2021-11-08 09:20:20.000000 pyradium-0.0.9/pyradium/templates/base/timer.html
+-rw-------   0 joe       (1000) joe       (1000)      103 2021-12-04 20:05:31.000000 pyradium-0.0.9/pyradium/templates/base/x
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.145730 pyradium-0.0.9/pyradium/tests/
+-rw-------   0 joe       (1000) joe       (1000)     2826 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/tests/CmdlineParserTests.py
+-rw-------   0 joe       (1000) joe       (1000)     5230 2021-11-03 07:03:57.000000 pyradium-0.0.9/pyradium/tests/TimeSpecificationTests.py
+-rw-------   0 joe       (1000) joe       (1000)     1001 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/tests/__init__.py
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.149730 pyradium-0.0.9/pyradium/xmlhooks/
+-rw-------   0 joe       (1000) joe       (1000)     2253 2022-01-30 22:21:48.000000 pyradium-0.0.9/pyradium/xmlhooks/AcronymHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1299 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/xmlhooks/ArrowHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1569 2021-11-05 22:49:09.000000 pyradium-0.0.9/pyradium/xmlhooks/CodeHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1203 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/xmlhooks/DebugHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1288 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/xmlhooks/EmoHook.py
+-rw-------   0 joe       (1000) joe       (1000)     2631 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/xmlhooks/ExecHook.py
+-rw-------   0 joe       (1000) joe       (1000)     3098 2022-01-12 20:23:13.000000 pyradium-0.0.9/pyradium/xmlhooks/ImgHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1341 2021-11-19 14:52:36.000000 pyradium-0.0.9/pyradium/xmlhooks/LinkHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1401 2021-10-29 20:01:44.000000 pyradium-0.0.9/pyradium/xmlhooks/MonospaceHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1387 2022-01-05 11:28:40.000000 pyradium-0.0.9/pyradium/xmlhooks/NoLinebreakHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1141 2021-11-19 14:52:36.000000 pyradium-0.0.9/pyradium/xmlhooks/NoSpellcheckHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1579 2021-11-08 09:20:20.000000 pyradium-0.0.9/pyradium/xmlhooks/NthHook.py
+-rw-------   0 joe       (1000) joe       (1000)     2066 2022-01-01 15:12:48.000000 pyradium-0.0.9/pyradium/xmlhooks/PlotHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1442 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/xmlhooks/QuoteHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1336 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/xmlhooks/SymbolHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1340 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium/xmlhooks/TerminalHook.py
+-rw-------   0 joe       (1000) joe       (1000)     2799 2022-01-12 20:30:11.000000 pyradium-0.0.9/pyradium/xmlhooks/TexHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1560 2021-11-03 07:03:57.000000 pyradium-0.0.9/pyradium/xmlhooks/TimeHook.py
+-rw-------   0 joe       (1000) joe       (1000)     1159 2022-01-21 11:41:07.000000 pyradium-0.0.9/pyradium/xmlhooks/VerbatimHook.py
+-rw-------   0 joe       (1000) joe       (1000)     4409 2022-01-21 11:59:21.000000 pyradium-0.0.9/pyradium/xmlhooks/XMLHookRegistry.py
+-rw-------   0 joe       (1000) joe       (1000)     1544 2022-01-21 11:41:27.000000 pyradium-0.0.9/pyradium/xmlhooks/__init__.py
+drwx------   0 joe       (1000) joe       (1000)        0 2022-01-30 22:24:17.137730 pyradium-0.0.9/pyradium.egg-info/
+-rw-------   0 joe       (1000) joe       (1000)    17813 2022-01-30 22:24:16.000000 pyradium-0.0.9/pyradium.egg-info/PKG-INFO
+-rw-------   0 joe       (1000) joe       (1000)     7705 2022-01-30 22:24:17.000000 pyradium-0.0.9/pyradium.egg-info/SOURCES.txt
+-rw-------   0 joe       (1000) joe       (1000)        1 2022-01-30 22:24:16.000000 pyradium-0.0.9/pyradium.egg-info/dependency_links.txt
+-rw-------   0 joe       (1000) joe       (1000)       53 2022-01-30 22:24:16.000000 pyradium-0.0.9/pyradium.egg-info/entry_points.txt
+-rw-------   0 joe       (1000) joe       (1000)       14 2022-01-30 22:24:16.000000 pyradium-0.0.9/pyradium.egg-info/requires.txt
+-rw-------   0 joe       (1000) joe       (1000)        9 2022-01-30 22:24:16.000000 pyradium-0.0.9/pyradium.egg-info/top_level.txt
+-rwx------   0 joe       (1000) joe       (1000)      977 2021-10-28 21:08:12.000000 pyradium-0.0.9/pyradium.py
+-rwx------   0 joe       (1000) joe       (1000)      322 2021-10-28 21:08:12.000000 pyradium-0.0.9/rerender
+-rwx------   0 joe       (1000) joe       (1000)     1902 2021-10-28 21:08:12.000000 pyradium-0.0.9/serve
+-rw-------   0 joe       (1000) joe       (1000)       38 2022-01-30 22:24:17.149730 pyradium-0.0.9/setup.cfg
+-rw-------   0 joe       (1000) joe       (1000)     1331 2021-11-02 07:47:47.000000 pyradium-0.0.9/setup.py
```

### Comparing `pyradium-0.0.8/LICENSE` & `pyradium-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/PKG-INFO` & `pyradium-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyradium
-Version: 0.0.8
+Version: 0.0.9
 Summary: Creating HTML presentations with LaTeX-ish features from XML source
 Home-page: https://github.com/johndoe31415/pyradium
 Author: Johannes Bauer
 Author-email: joe@johannes-bauer.com
 License: gpl-3.0
-Download-URL: https://github.com/johndoe31415/pyradium/archive/0.0.8.tar.gz
+Download-URL: https://github.com/johndoe31415/pyradium/archive/0.0.9.tar.gz
 Description: # pyradium
         [![Build Status](https://travis-ci.com/johndoe31415/pyradium.svg?branch=master)](https://travis-ci.com/johndoe31415/pyradium)
         
         This is a tool which takes XML input that describes a presentation and renders
         it into a presentation HTML. It borrows ideas from LaTeX-beamer but also
         combines the flexible way of creating visually appealing documents using
         HTML/CSS. it In particular, the features are:
```

### Comparing `pyradium-0.0.8/README.md` & `pyradium-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/imgs/anim/21da33acb6f14b9f6bf7eae05bf191b0.png` & `pyradium-0.0.9/docs/imgs/anim/21da33acb6f14b9f6bf7eae05bf191b0.png`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/imgs/anim/5e5767ae71a36650597d24fa84dd0b70.png` & `pyradium-0.0.9/docs/imgs/anim/5e5767ae71a36650597d24fa84dd0b70.png`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/imgs/anim/908fe8fbd07106b45d209de37d64f385.png` & `pyradium-0.0.9/docs/imgs/anim/908fe8fbd07106b45d209de37d64f385.png`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/imgs/img/2a58e4b31d16431abd7c4746e55fb701.png` & `pyradium-0.0.9/docs/imgs/img/2a58e4b31d16431abd7c4746e55fb701.png`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/imgs/latex/6f86f5675c6bdba9e0f5d8e317fda102.png` & `pyradium-0.0.9/docs/imgs/latex/6f86f5675c6bdba9e0f5d8e317fda102.png`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/imgs/latex/7c191ca8017c318fa68b68357c1ac979.png` & `pyradium-0.0.9/docs/imgs/latex/7c191ca8017c318fa68b68357c1ac979.png`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/imgs/latex/a28a8ba6d3dd046c7e3dfc4e80c1e76e.png` & `pyradium-0.0.9/docs/imgs/latex/a28a8ba6d3dd046c7e3dfc4e80c1e76e.png`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/index.html` & `pyradium-0.0.9/docs/index.html`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/antonio/antonio.css` & `pyradium-0.0.9/docs/template/antonio/antonio.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/antonio/bar.svg` & `pyradium-0.0.9/docs/template/antonio/bar.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/antonio/font_fira/FiraSans-Bold-latin.woff2` & `pyradium-0.0.9/docs/template/antonio/font_fira/FiraSans-Bold-latin.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/antonio/font_fira/FiraSans-Light-latin.woff2` & `pyradium-0.0.9/docs/template/antonio/font_fira/FiraSans-Light-latin.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/antonio/font_fira/FiraSans-Regular-latin.woff2` & `pyradium-0.0.9/docs/template/antonio/font_fira/FiraSans-Regular-latin.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/antonio/font_fira.css` & `pyradium-0.0.9/docs/template/antonio/font_fira.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/antonio/font_latinmodernmono/lmmono10-italic.otf` & `pyradium-0.0.9/docs/template/antonio/font_latinmodernmono/lmmono10-italic.otf`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/antonio/font_latinmodernmono/lmmono10-regular.otf` & `pyradium-0.0.9/docs/template/antonio/font_latinmodernmono/lmmono10-regular.otf`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/antonio/quote.svg` & `pyradium-0.0.9/docs/template/antonio/quote.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/antonio/triangle1.svg` & `pyradium-0.0.9/docs/template/antonio/triangle1.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/antonio/triangle2.svg` & `pyradium-0.0.9/docs/template/antonio/triangle2.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/base/cursor.svg` & `pyradium-0.0.9/docs/template/base/cursor.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/base/pygments.css` & `pyradium-0.0.9/docs/template/base/pygments.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/base/pyradium.css` & `pyradium-0.0.9/docs/template/base/pyradium.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/base/pyradium.js` & `pyradium-0.0.9/docs/template/base/pyradium.js`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/base/pyradium_feedback.js` & `pyradium-0.0.9/docs/template/base/pyradium_feedback.js`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/base/pyradium_forms.css` & `pyradium-0.0.9/docs/template/base/pyradium_forms.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/base/pyradium_forms.js` & `pyradium-0.0.9/docs/template/base/pyradium_forms.js`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/base/pyradium_menu.css` & `pyradium-0.0.9/docs/template/base/pyradium_menu.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/base/pyradium_modal.css` & `pyradium-0.0.9/docs/template/base/pyradium_modal.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/base/pyradium_modal.js` & `pyradium-0.0.9/docs/template/base/pyradium_modal.js`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/docs/template/base/pyradium_tooltip.css` & `pyradium-0.0.9/docs/template/base/pyradium_tooltip.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/examples/3dbox.svg` & `pyradium-0.0.9/examples/3dbox.svg`

 * *Files 19% similar despite different names*

```diff
@@ -66,18 +66,18 @@
 00000410: 3636 3636 3636 220a 2020 2020 2062 6f72  666666".     bor
 00000420: 6465 726f 7061 6369 7479 3d22 312e 3022  deropacity="1.0"
 00000430: 0a20 2020 2020 696e 6b73 6361 7065 3a70  .     inkscape:p
 00000440: 6167 656f 7061 6369 7479 3d22 302e 3022  ageopacity="0.0"
 00000450: 0a20 2020 2020 696e 6b73 6361 7065 3a70  .     inkscape:p
 00000460: 6167 6573 6861 646f 773d 2232 220a 2020  ageshadow="2".  
 00000470: 2020 2069 6e6b 7363 6170 653a 7a6f 6f6d     inkscape:zoom
-00000480: 3d22 312e 3422 0a20 2020 2020 696e 6b73  ="1.4".     inks
-00000490: 6361 7065 3a63 783d 2233 372e 3130 3137  cape:cx="37.1017
-000004a0: 3337 220a 2020 2020 2069 6e6b 7363 6170  37".     inkscap
-000004b0: 653a 6379 3d22 2d31 3139 2e34 3830 3339  e:cy="-119.48039
+00000480: 3d22 3131 2e32 220a 2020 2020 2069 6e6b  ="11.2".     ink
+00000490: 7363 6170 653a 6378 3d22 3239 2e36 3432  scape:cx="29.642
+000004a0: 3235 3922 0a20 2020 2020 696e 6b73 6361  259".     inksca
+000004b0: 7065 3a63 793d 2233 332e 3935 3130 3531  pe:cy="33.951051
 000004c0: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
 000004d0: 646f 6375 6d65 6e74 2d75 6e69 7473 3d22  document-units="
 000004e0: 6d6d 220a 2020 2020 2069 6e6b 7363 6170  mm".     inkscap
 000004f0: 653a 6375 7272 656e 742d 6c61 7965 723d  e:current-layer=
 00000500: 226c 6179 6572 3122 0a20 2020 2020 696e  "layer1".     in
 00000510: 6b73 6361 7065 3a64 6f63 756d 656e 742d  kscape:document-
 00000520: 726f 7461 7469 6f6e 3d22 3022 0a20 2020  rotation="0".   
@@ -86,226 +86,309 @@
 00000550: 696e 2d74 6f70 3d22 3022 0a20 2020 2020  in-top="0".     
 00000560: 6669 742d 6d61 7267 696e 2d6c 6566 743d  fit-margin-left=
 00000570: 2230 220a 2020 2020 2066 6974 2d6d 6172  "0".     fit-mar
 00000580: 6769 6e2d 7269 6768 743d 2230 220a 2020  gin-right="0".  
 00000590: 2020 2066 6974 2d6d 6172 6769 6e2d 626f     fit-margin-bo
 000005a0: 7474 6f6d 3d22 3022 0a20 2020 2020 696e  ttom="0".     in
 000005b0: 6b73 6361 7065 3a77 696e 646f 772d 7769  kscape:window-wi
-000005c0: 6474 683d 2231 3932 3022 0a20 2020 2020  dth="1920".     
+000005c0: 6474 683d 2233 3834 3022 0a20 2020 2020  dth="3840".     
 000005d0: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-000005e0: 6865 6967 6874 3d22 3939 3622 0a20 2020  height="996".   
-000005f0: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
-00000600: 772d 783d 2231 3932 3022 0a20 2020 2020  w-x="1920".     
-00000610: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-00000620: 793d 2232 3822 0a20 2020 2020 696e 6b73  y="28".     inks
-00000630: 6361 7065 3a77 696e 646f 772d 6d61 7869  cape:window-maxi
-00000640: 6d69 7a65 643d 2231 2220 2f3e 0a20 203c  mized="1" />.  <
-00000650: 6d65 7461 6461 7461 0a20 2020 2020 6964  metadata.     id
-00000660: 3d22 6d65 7461 6461 7461 3522 3e0a 2020  ="metadata5">.  
-00000670: 2020 3c72 6466 3a52 4446 3e0a 2020 2020    <rdf:RDF>.    
-00000680: 2020 3c63 633a 576f 726b 0a20 2020 2020    <cc:Work.     
-00000690: 2020 2020 7264 663a 6162 6f75 743d 2222      rdf:about=""
-000006a0: 3e0a 2020 2020 2020 2020 3c64 633a 666f  >.        <dc:fo
-000006b0: 726d 6174 3e69 6d61 6765 2f73 7667 2b78  rmat>image/svg+x
-000006c0: 6d6c 3c2f 6463 3a66 6f72 6d61 743e 0a20  ml</dc:format>. 
-000006d0: 2020 2020 2020 203c 6463 3a74 7970 650a         <dc:type.
-000006e0: 2020 2020 2020 2020 2020 2072 6466 3a72             rdf:r
-000006f0: 6573 6f75 7263 653d 2268 7474 703a 2f2f  esource="http://
-00000700: 7075 726c 2e6f 7267 2f64 632f 6463 6d69  purl.org/dc/dcmi
-00000710: 7479 7065 2f53 7469 6c6c 496d 6167 6522  type/StillImage"
-00000720: 202f 3e0a 2020 2020 2020 2020 3c64 633a   />.        <dc:
-00000730: 7469 746c 653e 3c2f 6463 3a74 6974 6c65  title></dc:title
-00000740: 3e0a 2020 2020 2020 3c2f 6363 3a57 6f72  >.      </cc:Wor
-00000750: 6b3e 0a20 2020 203c 2f72 6466 3a52 4446  k>.    </rdf:RDF
-00000760: 3e0a 2020 3c2f 6d65 7461 6461 7461 3e0a  >.  </metadata>.
-00000770: 2020 3c67 0a20 2020 2020 696e 6b73 6361    <g.     inksca
-00000780: 7065 3a6c 6162 656c 3d22 4c61 7965 7220  pe:label="Layer 
-00000790: 3122 0a20 2020 2020 696e 6b73 6361 7065  1".     inkscape
-000007a0: 3a67 726f 7570 6d6f 6465 3d22 6c61 7965  :groupmode="laye
-000007b0: 7222 0a20 2020 2020 6964 3d22 6c61 7965  r".     id="laye
-000007c0: 7231 220a 2020 2020 2074 7261 6e73 666f  r1".     transfo
-000007d0: 726d 3d22 7472 616e 736c 6174 6528 2d31  rm="translate(-1
-000007e0: 3630 2e32 3332 3838 2c2d 3137 332e 3932  60.23288,-173.92
-000007f0: 3835 3529 223e 0a20 2020 203c 670a 2020  855)">.    <g.  
-00000800: 2020 2020 2073 6f64 6970 6f64 693a 7479       sodipodi:ty
-00000810: 7065 3d22 696e 6b73 6361 7065 3a62 6f78  pe="inkscape:box
-00000820: 3364 220a 2020 2020 2020 2069 643d 2267  3d".       id="g
-00000830: 3833 3522 0a20 2020 2020 2020 7374 796c  835".       styl
-00000840: 653d 2266 696c 6c3a 6e6f 6e65 3b73 7472  e="fill:none;str
-00000850: 6f6b 653a 2330 3030 3030 303b 7374 726f  oke:#000000;stro
-00000860: 6b65 2d6c 696e 656a 6f69 6e3a 726f 756e  ke-linejoin:roun
-00000870: 6422 0a20 2020 2020 2020 696e 6b73 6361  d".       inksca
-00000880: 7065 3a70 6572 7370 6563 7469 7665 4944  pe:perspectiveID
-00000890: 3d22 2370 6572 7370 6563 7469 7665 3833  ="#perspective83
-000008a0: 3322 0a20 2020 2020 2020 696e 6b73 6361  3".       inksca
-000008b0: 7065 3a63 6f72 6e65 7230 3d22 302e 3331  pe:corner0="0.31
-000008c0: 3436 3633 3834 203a 2030 2e31 3138 3739  466384 : 0.11879
-000008d0: 3735 3620 3a20 3020 3a20 3122 0a20 2020  756 : 0 : 1".   
-000008e0: 2020 2020 696e 6b73 6361 7065 3a63 6f72      inkscape:cor
-000008f0: 6e65 7237 3d22 302e 3131 3939 3533 3820  ner7="0.1199538 
-00000900: 3a20 302e 3130 3137 3637 3732 203a 2030  : 0.10176772 : 0
-00000910: 2e32 3039 3232 3830 3920 3a20 3122 3e0a  .20922809 : 1">.
-00000920: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
-00000930: 2020 2020 2073 6f64 6970 6f64 693a 7479       sodipodi:ty
-00000940: 7065 3d22 696e 6b73 6361 7065 3a62 6f78  pe="inkscape:box
-00000950: 3364 7369 6465 220a 2020 2020 2020 2020  3dside".        
-00000960: 2069 643d 2270 6174 6838 3437 220a 2020   id="path847".  
-00000970: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00000980: 6c6c 3a23 6539 6539 6666 3b66 696c 6c2d  ll:#e9e9ff;fill-
-00000990: 7275 6c65 3a65 7665 6e6f 6464 3b73 7472  rule:evenodd;str
-000009a0: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
-000009b0: 7769 6474 683a 3170 783b 7374 726f 6b65  width:1px;stroke
-000009c0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-000009d0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 726f  roke-linejoin:ro
-000009e0: 756e 643b 7374 726f 6b65 2d6f 7061 6369  und;stroke-opaci
-000009f0: 7479 3a31 220a 2020 2020 2020 2020 2069  ty:1".         i
-00000a00: 6e6b 7363 6170 653a 626f 7833 6473 6964  nkscape:box3dsid
-00000a10: 6574 7970 653d 2231 3122 0a20 2020 2020  etype="11".     
-00000a20: 2020 2020 643d 226d 2031 3738 2e32 3635      d="m 178.265
-00000a30: 3138 2c31 3930 2e35 3536 3239 2031 342e  18,190.55629 14.
-00000a40: 3331 3731 2c2d 362e 3636 3134 3420 7620  3171,-6.66144 v 
-00000a50: 3132 2e38 3132 3237 206c 202d 3134 2e33  12.81227 l -14.3
-00000a60: 3137 312c 352e 3032 3433 3920 7a22 0a20  171,5.02439 z". 
-00000a70: 2020 2020 2020 2020 706f 696e 7473 3d22          points="
-00000a80: 3139 322e 3538 3232 382c 3138 332e 3839  192.58228,183.89
-00000a90: 3438 3520 3139 322e 3538 3232 382c 3139  485 192.58228,19
-00000aa0: 362e 3730 3731 3220 3137 382e 3236 3531  6.70712 178.2651
-00000ab0: 382c 3230 312e 3733 3135 3120 3137 382e  8,201.73151 178.
-00000ac0: 3236 3531 382c 3139 302e 3535 3632 3920  26518,190.55629 
-00000ad0: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
-00000ae0: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
-00000af0: 6469 3a74 7970 653d 2269 6e6b 7363 6170  di:type="inkscap
-00000b00: 653a 626f 7833 6473 6964 6522 0a20 2020  e:box3dside".   
-00000b10: 2020 2020 2020 6964 3d22 7061 7468 3833        id="path83
-00000b20: 3722 0a20 2020 2020 2020 2020 7374 796c  7".         styl
-00000b30: 653d 2266 696c 6c3a 2333 3533 3536 343b  e="fill:#353564;
-00000b40: 6669 6c6c 2d72 756c 653a 6576 656e 6f64  fill-rule:evenod
-00000b50: 643b 7374 726f 6b65 3a6e 6f6e 653b 7374  d;stroke:none;st
-00000b60: 726f 6b65 2d77 6964 7468 3a31 7078 3b73  roke-width:1px;s
-00000b70: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00000b80: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00000b90: 696e 3a72 6f75 6e64 3b73 7472 6f6b 652d  in:round;stroke-
-00000ba0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00000bb0: 2020 2020 696e 6b73 6361 7065 3a62 6f78      inkscape:box
-00000bc0: 3364 7369 6465 7479 7065 3d22 3622 0a20  3dsidetype="6". 
-00000bd0: 2020 2020 2020 2020 643d 226d 2031 3630          d="m 160
-00000be0: 2e33 3938 332c 3138 332e 3331 3931 3120  .3983,183.31911 
-00000bf0: 7620 3132 2e39 3533 3736 206c 2031 372e  v 12.95376 l 17.
-00000c00: 3836 3638 382c 352e 3435 3836 3420 7620  86688,5.45864 v 
-00000c10: 2d31 312e 3137 3532 3220 7a22 0a20 2020  -11.17522 z".   
-00000c20: 2020 2020 2020 706f 696e 7473 3d22 3136        points="16
-00000c30: 302e 3339 3833 2c31 3936 2e32 3732 3837  0.3983,196.27287
-00000c40: 2031 3738 2e32 3635 3138 2c32 3031 2e37   178.26518,201.7
-00000c50: 3331 3531 2031 3738 2e32 3635 3138 2c31  3151 178.26518,1
-00000c60: 3930 2e35 3536 3239 2031 3630 2e33 3938  90.55629 160.398
-00000c70: 332c 3138 332e 3331 3931 3120 2220 2f3e  3,183.31911 " />
-00000c80: 0a20 2020 2020 203c 7061 7468 0a20 2020  .      <path.   
-00000c90: 2020 2020 2020 736f 6469 706f 6469 3a74        sodipodi:t
-00000ca0: 7970 653d 2269 6e6b 7363 6170 653a 626f  ype="inkscape:bo
-00000cb0: 7833 6473 6964 6522 0a20 2020 2020 2020  x3dside".       
-00000cc0: 2020 6964 3d22 7061 7468 3833 3922 0a20    id="path839". 
-00000cd0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-00000ce0: 696c 6c3a 2334 6434 6439 663b 6669 6c6c  ill:#4d4d9f;fill
-00000cf0: 2d72 756c 653a 6576 656e 6f64 643b 7374  -rule:evenodd;st
-00000d00: 726f 6b65 3a6e 6f6e 653b 7374 726f 6b65  roke:none;stroke
-00000d10: 2d77 6964 7468 3a31 7078 3b73 7472 6f6b  -width:1px;strok
-00000d20: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00000d30: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a72  troke-linejoin:r
-00000d40: 6f75 6e64 3b73 7472 6f6b 652d 6f70 6163  ound;stroke-opac
-00000d50: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
-00000d60: 696e 6b73 6361 7065 3a62 6f78 3364 7369  inkscape:box3dsi
-00000d70: 6465 7479 7065 3d22 3522 0a20 2020 2020  detype="5".     
-00000d80: 2020 2020 643d 226d 2031 3630 2e33 3938      d="m 160.398
-00000d90: 332c 3138 332e 3331 3931 3120 3133 2e38  3,183.31911 13.8
-00000da0: 3835 3534 2c2d 392e 3136 3431 3320 3138  8554,-9.16413 18
-00000db0: 2e32 3938 3434 2c39 2e37 3339 3837 202d  .29844,9.73987 -
-00000dc0: 3134 2e33 3137 312c 362e 3636 3134 3420  14.3171,6.66144 
-00000dd0: 7a22 0a20 2020 2020 2020 2020 706f 696e  z".         poin
-00000de0: 7473 3d22 3137 342e 3238 3338 342c 3137  ts="174.28384,17
-00000df0: 342e 3135 3439 3820 3139 322e 3538 3232  4.15498 192.5822
-00000e00: 382c 3138 332e 3839 3438 3520 3137 382e  8,183.89485 178.
-00000e10: 3236 3531 382c 3139 302e 3535 3632 3920  26518,190.55629 
-00000e20: 3136 302e 3339 3833 2c31 3833 2e33 3139  160.3983,183.319
-00000e30: 3131 2022 202f 3e0a 2020 2020 2020 3c70  11 " />.      <p
-00000e40: 6174 680a 2020 2020 2020 2020 2073 6f64  ath.         sod
-00000e50: 6970 6f64 693a 7479 7065 3d22 696e 6b73  ipodi:type="inks
-00000e60: 6361 7065 3a62 6f78 3364 7369 6465 220a  cape:box3dside".
-00000e70: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00000e80: 6838 3435 220a 2020 2020 2020 2020 2073  h845".         s
-00000e90: 7479 6c65 3d22 6669 6c6c 3a23 6166 6166  tyle="fill:#afaf
-00000ea0: 6465 3b66 696c 6c2d 7275 6c65 3a65 7665  de;fill-rule:eve
-00000eb0: 6e6f 6464 3b73 7472 6f6b 653a 6e6f 6e65  nodd;stroke:none
-00000ec0: 3b73 7472 6f6b 652d 7769 6474 683a 3170  ;stroke-width:1p
-00000ed0: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
-00000ee0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00000ef0: 656a 6f69 6e3a 726f 756e 643b 7374 726f  ejoin:round;stro
-00000f00: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00000f10: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00000f20: 626f 7833 6473 6964 6574 7970 653d 2231  box3dsidetype="1
-00000f30: 3322 0a20 2020 2020 2020 2020 643d 226d  3".         d="m
-00000f40: 2031 3630 2e33 3938 332c 3139 362e 3237   160.3983,196.27
-00000f50: 3238 3720 3133 2e38 3835 3534 2c2d 362e  287 13.88554,-6.
-00000f60: 3931 3230 3520 3138 2e32 3938 3434 2c37  91205 18.29844,7
-00000f70: 2e33 3436 3320 2d31 342e 3331 3731 2c35  .3463 -14.3171,5
-00000f80: 2e30 3234 3339 207a 220a 2020 2020 2020  .02439 z".      
-00000f90: 2020 2070 6f69 6e74 733d 2231 3734 2e32     points="174.2
-00000fa0: 3833 3834 2c31 3839 2e33 3630 3832 2031  8384,189.36082 1
-00000fb0: 3932 2e35 3832 3238 2c31 3936 2e37 3037  92.58228,196.707
-00000fc0: 3132 2031 3738 2e32 3635 3138 2c32 3031  12 178.26518,201
-00000fd0: 2e37 3331 3531 2031 3630 2e33 3938 332c  .73151 160.3983,
-00000fe0: 3139 362e 3237 3238 3720 2220 2f3e 0a20  196.27287 " />. 
-00000ff0: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
-00001000: 2020 2020 736f 6469 706f 6469 3a74 7970      sodipodi:typ
-00001010: 653d 2269 6e6b 7363 6170 653a 626f 7833  e="inkscape:box3
-00001020: 6473 6964 6522 0a20 2020 2020 2020 2020  dside".         
-00001030: 6964 3d22 7061 7468 3834 3322 0a20 2020  id="path843".   
-00001040: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00001050: 6c3a 2364 3764 3766 663b 6669 6c6c 2d72  l:#d7d7ff;fill-r
-00001060: 756c 653a 6576 656e 6f64 643b 7374 726f  ule:evenodd;stro
-00001070: 6b65 3a6e 6f6e 653b 7374 726f 6b65 2d77  ke:none;stroke-w
-00001080: 6964 7468 3a31 7078 3b73 7472 6f6b 652d  idth:1px;stroke-
-00001090: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-000010a0: 6f6b 652d 6c69 6e65 6a6f 696e 3a72 6f75  oke-linejoin:rou
-000010b0: 6e64 3b73 7472 6f6b 652d 6f70 6163 6974  nd;stroke-opacit
-000010c0: 793a 3122 0a20 2020 2020 2020 2020 696e  y:1".         in
-000010d0: 6b73 6361 7065 3a62 6f78 3364 7369 6465  kscape:box3dside
-000010e0: 7479 7065 3d22 3134 220a 2020 2020 2020  type="14".      
-000010f0: 2020 2064 3d22 6d20 3137 342e 3238 3338     d="m 174.2838
-00001100: 342c 3137 342e 3135 3439 3820 7620 3135  4,174.15498 v 15
-00001110: 2e32 3035 3834 206c 2031 382e 3239 3834  .20584 l 18.2984
-00001120: 342c 372e 3334 3633 2076 202d 3132 2e38  4,7.3463 v -12.8
-00001130: 3132 3237 207a 220a 2020 2020 2020 2020  1227 z".        
-00001140: 2070 6f69 6e74 733d 2231 3734 2e32 3833   points="174.283
-00001150: 3834 2c31 3839 2e33 3630 3832 2031 3932  84,189.36082 192
-00001160: 2e35 3832 3238 2c31 3936 2e37 3037 3132  .58228,196.70712
-00001170: 2031 3932 2e35 3832 3238 2c31 3833 2e38   192.58228,183.8
-00001180: 3934 3835 2031 3734 2e32 3833 3834 2c31  9485 174.28384,1
-00001190: 3734 2e31 3534 3938 2022 202f 3e0a 2020  74.15498 " />.  
-000011a0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-000011b0: 2020 2073 6f64 6970 6f64 693a 7479 7065     sodipodi:type
-000011c0: 3d22 696e 6b73 6361 7065 3a62 6f78 3364  ="inkscape:box3d
-000011d0: 7369 6465 220a 2020 2020 2020 2020 2069  side".         i
-000011e0: 643d 2270 6174 6838 3431 220a 2020 2020  d="path841".    
-000011f0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00001200: 3a23 3836 3836 6266 3b66 696c 6c2d 7275  :#8686bf;fill-ru
-00001210: 6c65 3a65 7665 6e6f 6464 3b73 7472 6f6b  le:evenodd;strok
-00001220: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
-00001230: 6474 683a 3170 783b 7374 726f 6b65 2d6c  dth:1px;stroke-l
-00001240: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
-00001250: 6b65 2d6c 696e 656a 6f69 6e3a 726f 756e  ke-linejoin:roun
-00001260: 643b 7374 726f 6b65 2d6f 7061 6369 7479  d;stroke-opacity
-00001270: 3a31 220a 2020 2020 2020 2020 2069 6e6b  :1".         ink
-00001280: 7363 6170 653a 626f 7833 6473 6964 6574  scape:box3dsidet
-00001290: 7970 653d 2233 220a 2020 2020 2020 2020  ype="3".        
-000012a0: 2064 3d22 6d20 3136 302e 3339 3833 2c31   d="m 160.3983,1
-000012b0: 3833 2e33 3139 3131 2031 332e 3838 3535  83.31911 13.8855
-000012c0: 342c 2d39 2e31 3634 3133 2076 2031 352e  4,-9.16413 v 15.
-000012d0: 3230 3538 3420 6c20 2d31 332e 3838 3535  20584 l -13.8855
-000012e0: 342c 362e 3931 3230 3520 7a22 0a20 2020  4,6.91205 z".   
-000012f0: 2020 2020 2020 706f 696e 7473 3d22 3137        points="17
-00001300: 342e 3238 3338 342c 3137 342e 3135 3439  4.28384,174.1549
-00001310: 3820 3137 342e 3238 3338 342c 3138 392e  8 174.28384,189.
-00001320: 3336 3038 3220 3136 302e 3339 3833 2c31  36082 160.3983,1
-00001330: 3936 2e32 3732 3837 2031 3630 2e33 3938  96.27287 160.398
-00001340: 332c 3138 332e 3331 3931 3120 2220 2f3e  3,183.31911 " />
-00001350: 0a20 2020 203c 2f67 3e0a 2020 3c2f 673e  .    </g>.  </g>
-00001360: 0a3c 2f73 7667 3e0a                      .</svg>.
+000005e0: 6865 6967 6874 3d22 3230 3731 220a 2020  height="2071".  
+000005f0: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
+00000600: 6f77 2d78 3d22 3338 3430 220a 2020 2020  ow-x="3840".    
+00000610: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
+00000620: 2d79 3d22 3238 220a 2020 2020 2069 6e6b  -y="28".     ink
+00000630: 7363 6170 653a 7769 6e64 6f77 2d6d 6178  scape:window-max
+00000640: 696d 697a 6564 3d22 3122 202f 3e0a 2020  imized="1" />.  
+00000650: 3c6d 6574 6164 6174 610a 2020 2020 2069  <metadata.     i
+00000660: 643d 226d 6574 6164 6174 6135 223e 0a20  d="metadata5">. 
+00000670: 2020 203c 7264 663a 5244 463e 0a20 2020     <rdf:RDF>.   
+00000680: 2020 203c 6363 3a57 6f72 6b0a 2020 2020     <cc:Work.    
+00000690: 2020 2020 2072 6466 3a61 626f 7574 3d22       rdf:about="
+000006a0: 223e 0a20 2020 2020 2020 203c 6463 3a66  ">.        <dc:f
+000006b0: 6f72 6d61 743e 696d 6167 652f 7376 672b  ormat>image/svg+
+000006c0: 786d 6c3c 2f64 633a 666f 726d 6174 3e0a  xml</dc:format>.
+000006d0: 2020 2020 2020 2020 3c64 633a 7479 7065          <dc:type
+000006e0: 0a20 2020 2020 2020 2020 2020 7264 663a  .           rdf:
+000006f0: 7265 736f 7572 6365 3d22 6874 7470 3a2f  resource="http:/
+00000700: 2f70 7572 6c2e 6f72 672f 6463 2f64 636d  /purl.org/dc/dcm
+00000710: 6974 7970 652f 5374 696c 6c49 6d61 6765  itype/StillImage
+00000720: 2220 2f3e 0a20 2020 2020 2020 203c 6463  " />.        <dc
+00000730: 3a74 6974 6c65 202f 3e0a 2020 2020 2020  :title />.      
+00000740: 3c2f 6363 3a57 6f72 6b3e 0a20 2020 203c  </cc:Work>.    <
+00000750: 2f72 6466 3a52 4446 3e0a 2020 3c2f 6d65  /rdf:RDF>.  </me
+00000760: 7461 6461 7461 3e0a 2020 3c67 0a20 2020  tadata>.  <g.   
+00000770: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
+00000780: 3d22 4c61 7965 7220 3122 0a20 2020 2020  ="Layer 1".     
+00000790: 696e 6b73 6361 7065 3a67 726f 7570 6d6f  inkscape:groupmo
+000007a0: 6465 3d22 6c61 7965 7222 0a20 2020 2020  de="layer".     
+000007b0: 6964 3d22 6c61 7965 7231 220a 2020 2020  id="layer1".    
+000007c0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+000007d0: 736c 6174 6528 2d31 3630 2e32 3332 3838  slate(-160.23288
+000007e0: 2c2d 3137 332e 3932 3835 3529 223e 0a20  ,-173.92855)">. 
+000007f0: 2020 203c 670a 2020 2020 2020 2073 6f64     <g.       sod
+00000800: 6970 6f64 693a 7479 7065 3d22 696e 6b73  ipodi:type="inks
+00000810: 6361 7065 3a62 6f78 3364 220a 2020 2020  cape:box3d".    
+00000820: 2020 2069 643d 2267 3833 3522 0a20 2020     id="g835".   
+00000830: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00000840: 6e6f 6e65 3b73 7472 6f6b 653a 2330 3030  none;stroke:#000
+00000850: 3030 303b 7374 726f 6b65 2d6c 696e 656a  000;stroke-linej
+00000860: 6f69 6e3a 726f 756e 6422 0a20 2020 2020  oin:round".     
+00000870: 2020 696e 6b73 6361 7065 3a70 6572 7370    inkscape:persp
+00000880: 6563 7469 7665 4944 3d22 2370 6572 7370  ectiveID="#persp
+00000890: 6563 7469 7665 3833 3322 0a20 2020 2020  ective833".     
+000008a0: 2020 696e 6b73 6361 7065 3a63 6f72 6e65    inkscape:corne
+000008b0: 7230 3d22 302e 3331 3436 3633 3834 203a  r0="0.31466384 :
+000008c0: 2030 2e31 3138 3739 3735 3620 3a20 3020   0.11879756 : 0 
+000008d0: 3a20 3122 0a20 2020 2020 2020 696e 6b73  : 1".       inks
+000008e0: 6361 7065 3a63 6f72 6e65 7237 3d22 302e  cape:corner7="0.
+000008f0: 3131 3939 3533 3820 3a20 302e 3130 3137  1199538 : 0.1017
+00000900: 3637 3732 203a 2030 2e32 3039 3232 3830  6772 : 0.2092280
+00000910: 3920 3a20 3122 3e0a 2020 2020 2020 3c70  9 : 1">.      <p
+00000920: 6174 680a 2020 2020 2020 2020 2073 6f64  ath.         sod
+00000930: 6970 6f64 693a 7479 7065 3d22 696e 6b73  ipodi:type="inks
+00000940: 6361 7065 3a62 6f78 3364 7369 6465 220a  cape:box3dside".
+00000950: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00000960: 6838 3437 220a 2020 2020 2020 2020 2073  h847".         s
+00000970: 7479 6c65 3d22 6669 6c6c 3a23 6539 6539  tyle="fill:#e9e9
+00000980: 6666 3b66 696c 6c2d 7275 6c65 3a65 7665  ff;fill-rule:eve
+00000990: 6e6f 6464 3b73 7472 6f6b 653a 6e6f 6e65  nodd;stroke:none
+000009a0: 3b73 7472 6f6b 652d 7769 6474 683a 3170  ;stroke-width:1p
+000009b0: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
+000009c0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+000009d0: 656a 6f69 6e3a 726f 756e 643b 7374 726f  ejoin:round;stro
+000009e0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+000009f0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00000a00: 626f 7833 6473 6964 6574 7970 653d 2231  box3dsidetype="1
+00000a10: 3122 0a20 2020 2020 2020 2020 643d 226d  1".         d="m
+00000a20: 2031 3738 2e32 3635 3138 2c31 3930 2e35   178.26518,190.5
+00000a30: 3536 3239 2031 342e 3331 3731 2c2d 362e  5629 14.3171,-6.
+00000a40: 3636 3134 3420 7620 3132 2e38 3132 3237  66144 v 12.81227
+00000a50: 206c 202d 3134 2e33 3137 312c 352e 3032   l -14.3171,5.02
+00000a60: 3433 3920 7a22 0a20 2020 2020 2020 2020  439 z".         
+00000a70: 706f 696e 7473 3d22 3139 322e 3538 3232  points="192.5822
+00000a80: 382c 3138 332e 3839 3438 3520 3139 322e  8,183.89485 192.
+00000a90: 3538 3232 382c 3139 362e 3730 3731 3220  58228,196.70712 
+00000aa0: 3137 382e 3236 3531 382c 3230 312e 3733  178.26518,201.73
+00000ab0: 3135 3120 3137 382e 3236 3531 382c 3139  151 178.26518,19
+00000ac0: 302e 3535 3632 3920 2220 2f3e 0a20 2020  0.55629 " />.   
+00000ad0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00000ae0: 2020 736f 6469 706f 6469 3a74 7970 653d    sodipodi:type=
+00000af0: 2269 6e6b 7363 6170 653a 626f 7833 6473  "inkscape:box3ds
+00000b00: 6964 6522 0a20 2020 2020 2020 2020 6964  ide".         id
+00000b10: 3d22 7061 7468 3833 3722 0a20 2020 2020  ="path837".     
+00000b20: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00000b30: 2333 3533 3536 343b 6669 6c6c 2d72 756c  #353564;fill-rul
+00000b40: 653a 6576 656e 6f64 643b 7374 726f 6b65  e:evenodd;stroke
+00000b50: 3a6e 6f6e 653b 7374 726f 6b65 2d77 6964  :none;stroke-wid
+00000b60: 7468 3a31 7078 3b73 7472 6f6b 652d 6c69  th:1px;stroke-li
+00000b70: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00000b80: 652d 6c69 6e65 6a6f 696e 3a72 6f75 6e64  e-linejoin:round
+00000b90: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00000ba0: 3122 0a20 2020 2020 2020 2020 696e 6b73  1".         inks
+00000bb0: 6361 7065 3a62 6f78 3364 7369 6465 7479  cape:box3dsidety
+00000bc0: 7065 3d22 3622 0a20 2020 2020 2020 2020  pe="6".         
+00000bd0: 643d 226d 2031 3630 2e33 3938 332c 3138  d="m 160.3983,18
+00000be0: 332e 3331 3931 3120 7620 3132 2e39 3533  3.31911 v 12.953
+00000bf0: 3736 206c 2031 372e 3836 3638 382c 352e  76 l 17.86688,5.
+00000c00: 3435 3836 3420 7620 2d31 312e 3137 3532  45864 v -11.1752
+00000c10: 3220 7a22 0a20 2020 2020 2020 2020 706f  2 z".         po
+00000c20: 696e 7473 3d22 3136 302e 3339 3833 2c31  ints="160.3983,1
+00000c30: 3936 2e32 3732 3837 2031 3738 2e32 3635  96.27287 178.265
+00000c40: 3138 2c32 3031 2e37 3331 3531 2031 3738  18,201.73151 178
+00000c50: 2e32 3635 3138 2c31 3930 2e35 3536 3239  .26518,190.55629
+00000c60: 2031 3630 2e33 3938 332c 3138 332e 3331   160.3983,183.31
+00000c70: 3931 3120 2220 2f3e 0a20 2020 2020 203c  911 " />.      <
+00000c80: 7061 7468 0a20 2020 2020 2020 2020 736f  path.         so
+00000c90: 6469 706f 6469 3a74 7970 653d 2269 6e6b  dipodi:type="ink
+00000ca0: 7363 6170 653a 626f 7833 6473 6964 6522  scape:box3dside"
+00000cb0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+00000cc0: 7468 3833 3922 0a20 2020 2020 2020 2020  th839".         
+00000cd0: 7374 796c 653d 2266 696c 6c3a 2334 6434  style="fill:#4d4
+00000ce0: 6439 663b 6669 6c6c 2d72 756c 653a 6576  d9f;fill-rule:ev
+00000cf0: 656e 6f64 643b 7374 726f 6b65 3a6e 6f6e  enodd;stroke:non
+00000d00: 653b 7374 726f 6b65 2d77 6964 7468 3a31  e;stroke-width:1
+00000d10: 7078 3b73 7472 6f6b 652d 6c69 6e65 6361  px;stroke-lineca
+00000d20: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00000d30: 6e65 6a6f 696e 3a72 6f75 6e64 3b73 7472  nejoin:round;str
+00000d40: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00000d50: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00000d60: 3a62 6f78 3364 7369 6465 7479 7065 3d22  :box3dsidetype="
+00000d70: 3522 0a20 2020 2020 2020 2020 643d 226d  5".         d="m
+00000d80: 2031 3630 2e33 3938 332c 3138 332e 3331   160.3983,183.31
+00000d90: 3931 3120 3133 2e38 3835 3534 2c2d 392e  911 13.88554,-9.
+00000da0: 3136 3431 3320 3138 2e32 3938 3434 2c39  16413 18.29844,9
+00000db0: 2e37 3339 3837 202d 3134 2e33 3137 312c  .73987 -14.3171,
+00000dc0: 362e 3636 3134 3420 7a22 0a20 2020 2020  6.66144 z".     
+00000dd0: 2020 2020 706f 696e 7473 3d22 3137 342e      points="174.
+00000de0: 3238 3338 342c 3137 342e 3135 3439 3820  28384,174.15498 
+00000df0: 3139 322e 3538 3232 382c 3138 332e 3839  192.58228,183.89
+00000e00: 3438 3520 3137 382e 3236 3531 382c 3139  485 178.26518,19
+00000e10: 302e 3535 3632 3920 3136 302e 3339 3833  0.55629 160.3983
+00000e20: 2c31 3833 2e33 3139 3131 2022 202f 3e0a  ,183.31911 " />.
+00000e30: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+00000e40: 2020 2020 2073 6f64 6970 6f64 693a 7479       sodipodi:ty
+00000e50: 7065 3d22 696e 6b73 6361 7065 3a62 6f78  pe="inkscape:box
+00000e60: 3364 7369 6465 220a 2020 2020 2020 2020  3dside".        
+00000e70: 2069 643d 2270 6174 6838 3435 220a 2020   id="path845".  
+00000e80: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00000e90: 6c6c 3a23 6166 6166 6465 3b66 696c 6c2d  ll:#afafde;fill-
+00000ea0: 7275 6c65 3a65 7665 6e6f 6464 3b73 7472  rule:evenodd;str
+00000eb0: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
+00000ec0: 7769 6474 683a 3170 783b 7374 726f 6b65  width:1px;stroke
+00000ed0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00000ee0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 726f  roke-linejoin:ro
+00000ef0: 756e 643b 7374 726f 6b65 2d6f 7061 6369  und;stroke-opaci
+00000f00: 7479 3a31 220a 2020 2020 2020 2020 2069  ty:1".         i
+00000f10: 6e6b 7363 6170 653a 626f 7833 6473 6964  nkscape:box3dsid
+00000f20: 6574 7970 653d 2231 3322 0a20 2020 2020  etype="13".     
+00000f30: 2020 2020 643d 226d 2031 3630 2e33 3938      d="m 160.398
+00000f40: 332c 3139 362e 3237 3238 3720 3133 2e38  3,196.27287 13.8
+00000f50: 3835 3534 2c2d 362e 3931 3230 3520 3138  8554,-6.91205 18
+00000f60: 2e32 3938 3434 2c37 2e33 3436 3320 2d31  .29844,7.3463 -1
+00000f70: 342e 3331 3731 2c35 2e30 3234 3339 207a  4.3171,5.02439 z
+00000f80: 220a 2020 2020 2020 2020 2070 6f69 6e74  ".         point
+00000f90: 733d 2231 3734 2e32 3833 3834 2c31 3839  s="174.28384,189
+00000fa0: 2e33 3630 3832 2031 3932 2e35 3832 3238  .36082 192.58228
+00000fb0: 2c31 3936 2e37 3037 3132 2031 3738 2e32  ,196.70712 178.2
+00000fc0: 3635 3138 2c32 3031 2e37 3331 3531 2031  6518,201.73151 1
+00000fd0: 3630 2e33 3938 332c 3139 362e 3237 3238  60.3983,196.2728
+00000fe0: 3720 2220 2f3e 0a20 2020 2020 203c 7061  7 " />.      <pa
+00000ff0: 7468 0a20 2020 2020 2020 2020 736f 6469  th.         sodi
+00001000: 706f 6469 3a74 7970 653d 2269 6e6b 7363  podi:type="inksc
+00001010: 6170 653a 626f 7833 6473 6964 6522 0a20  ape:box3dside". 
+00001020: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00001030: 3834 3322 0a20 2020 2020 2020 2020 7374  843".         st
+00001040: 796c 653d 2266 696c 6c3a 2364 3764 3766  yle="fill:#d7d7f
+00001050: 663b 6669 6c6c 2d72 756c 653a 6576 656e  f;fill-rule:even
+00001060: 6f64 643b 7374 726f 6b65 3a6e 6f6e 653b  odd;stroke:none;
+00001070: 7374 726f 6b65 2d77 6964 7468 3a31 7078  stroke-width:1px
+00001080: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00001090: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+000010a0: 6a6f 696e 3a72 6f75 6e64 3b73 7472 6f6b  join:round;strok
+000010b0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+000010c0: 2020 2020 2020 696e 6b73 6361 7065 3a62        inkscape:b
+000010d0: 6f78 3364 7369 6465 7479 7065 3d22 3134  ox3dsidetype="14
+000010e0: 220a 2020 2020 2020 2020 2064 3d22 6d20  ".         d="m 
+000010f0: 3137 342e 3238 3338 342c 3137 342e 3135  174.28384,174.15
+00001100: 3439 3820 7620 3135 2e32 3035 3834 206c  498 v 15.20584 l
+00001110: 2031 382e 3239 3834 342c 372e 3334 3633   18.29844,7.3463
+00001120: 2076 202d 3132 2e38 3132 3237 207a 220a   v -12.81227 z".
+00001130: 2020 2020 2020 2020 2070 6f69 6e74 733d           points=
+00001140: 2231 3734 2e32 3833 3834 2c31 3839 2e33  "174.28384,189.3
+00001150: 3630 3832 2031 3932 2e35 3832 3238 2c31  6082 192.58228,1
+00001160: 3936 2e37 3037 3132 2031 3932 2e35 3832  96.70712 192.582
+00001170: 3238 2c31 3833 2e38 3934 3835 2031 3734  28,183.89485 174
+00001180: 2e32 3833 3834 2c31 3734 2e31 3534 3938  .28384,174.15498
+00001190: 2022 202f 3e0a 2020 2020 2020 3c70 6174   " />.      <pat
+000011a0: 680a 2020 2020 2020 2020 2073 6f64 6970  h.         sodip
+000011b0: 6f64 693a 7479 7065 3d22 696e 6b73 6361  odi:type="inksca
+000011c0: 7065 3a62 6f78 3364 7369 6465 220a 2020  pe:box3dside".  
+000011d0: 2020 2020 2020 2069 643d 2270 6174 6838         id="path8
+000011e0: 3431 220a 2020 2020 2020 2020 2073 7479  41".         sty
+000011f0: 6c65 3d22 6669 6c6c 3a23 3836 3836 6266  le="fill:#8686bf
+00001200: 3b66 696c 6c2d 7275 6c65 3a65 7665 6e6f  ;fill-rule:eveno
+00001210: 6464 3b73 7472 6f6b 653a 6e6f 6e65 3b73  dd;stroke:none;s
+00001220: 7472 6f6b 652d 7769 6474 683a 3170 783b  troke-width:1px;
+00001230: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00001240: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00001250: 6f69 6e3a 726f 756e 643b 7374 726f 6b65  oin:round;stroke
+00001260: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00001270: 2020 2020 2069 6e6b 7363 6170 653a 626f       inkscape:bo
+00001280: 7833 6473 6964 6574 7970 653d 2233 220a  x3dsidetype="3".
+00001290: 2020 2020 2020 2020 2064 3d22 6d20 3136           d="m 16
+000012a0: 302e 3339 3833 2c31 3833 2e33 3139 3131  0.3983,183.31911
+000012b0: 2031 332e 3838 3535 342c 2d39 2e31 3634   13.88554,-9.164
+000012c0: 3133 2076 2031 352e 3230 3538 3420 6c20  13 v 15.20584 l 
+000012d0: 2d31 332e 3838 3535 342c 362e 3931 3230  -13.88554,6.9120
+000012e0: 3520 7a22 0a20 2020 2020 2020 2020 706f  5 z".         po
+000012f0: 696e 7473 3d22 3137 342e 3238 3338 342c  ints="174.28384,
+00001300: 3137 342e 3135 3439 3820 3137 342e 3238  174.15498 174.28
+00001310: 3338 342c 3138 392e 3336 3038 3220 3136  384,189.36082 16
+00001320: 302e 3339 3833 2c31 3936 2e32 3732 3837  0.3983,196.27287
+00001330: 2031 3630 2e33 3938 332c 3138 332e 3331   160.3983,183.31
+00001340: 3931 3120 2220 2f3e 0a20 2020 203c 2f67  911 " />.    </g
+00001350: 3e0a 2020 2020 3c74 6578 740a 2020 2020  >.    <text.    
+00001360: 2020 2078 6d6c 3a73 7061 6365 3d22 7072     xml:space="pr
+00001370: 6573 6572 7665 220a 2020 2020 2020 2073  eserve".       s
+00001380: 7479 6c65 3d22 666f 6e74 2d73 7479 6c65  tyle="font-style
+00001390: 3a6e 6f72 6d61 6c3b 666f 6e74 2d76 6172  :normal;font-var
+000013a0: 6961 6e74 3a6e 6f72 6d61 6c3b 666f 6e74  iant:normal;font
+000013b0: 2d77 6569 6768 743a 6e6f 726d 616c 3b66  -weight:normal;f
+000013c0: 6f6e 742d 7374 7265 7463 683a 6e6f 726d  ont-stretch:norm
+000013d0: 616c 3b66 6f6e 742d 7369 7a65 3a31 3670  al;font-size:16p
+000013e0: 783b 6c69 6e65 2d68 6569 6768 743a 3132  x;line-height:12
+000013f0: 3525 3b66 6f6e 742d 6661 6d69 6c79 3a41  5%;font-family:A
+00001400: 7269 616c 3b2d 696e 6b73 6361 7065 2d66  rial;-inkscape-f
+00001410: 6f6e 742d 7370 6563 6966 6963 6174 696f  ont-specificatio
+00001420: 6e3a 4172 6961 6c3b 666f 6e74 2d76 6172  n:Arial;font-var
+00001430: 6961 6e74 2d6c 6967 6174 7572 6573 3a6e  iant-ligatures:n
+00001440: 6f72 6d61 6c3b 666f 6e74 2d76 6172 6961  ormal;font-varia
+00001450: 6e74 2d70 6f73 6974 696f 6e3a 6e6f 726d  nt-position:norm
+00001460: 616c 3b66 6f6e 742d 7661 7269 616e 742d  al;font-variant-
+00001470: 6361 7073 3a6e 6f72 6d61 6c3b 666f 6e74  caps:normal;font
+00001480: 2d76 6172 6961 6e74 2d6e 756d 6572 6963  -variant-numeric
+00001490: 3a6e 6f72 6d61 6c3b 666f 6e74 2d76 6172  :normal;font-var
+000014a0: 6961 6e74 2d61 6c74 6572 6e61 7465 733a  iant-alternates:
+000014b0: 6e6f 726d 616c 3b66 6f6e 742d 7661 7269  normal;font-vari
+000014c0: 616e 742d 6561 7374 2d61 7369 616e 3a6e  ant-east-asian:n
+000014d0: 6f72 6d61 6c3b 666f 6e74 2d66 6561 7475  ormal;font-featu
+000014e0: 7265 2d73 6574 7469 6e67 733a 6e6f 726d  re-settings:norm
+000014f0: 616c 3b66 6f6e 742d 7661 7269 6174 696f  al;font-variatio
+00001500: 6e2d 7365 7474 696e 6773 3a6e 6f72 6d61  n-settings:norma
+00001510: 6c3b 7465 7874 2d69 6e64 656e 743a 303b  l;text-indent:0;
+00001520: 7465 7874 2d61 6c69 676e 3a63 656e 7465  text-align:cente
+00001530: 723b 7465 7874 2d64 6563 6f72 6174 696f  r;text-decoratio
+00001540: 6e3a 6e6f 6e65 3b74 6578 742d 6465 636f  n:none;text-deco
+00001550: 7261 7469 6f6e 2d6c 696e 653a 6e6f 6e65  ration-line:none
+00001560: 3b74 6578 742d 6465 636f 7261 7469 6f6e  ;text-decoration
+00001570: 2d73 7479 6c65 3a73 6f6c 6964 3b74 6578  -style:solid;tex
+00001580: 742d 6465 636f 7261 7469 6f6e 2d63 6f6c  t-decoration-col
+00001590: 6f72 3a23 3030 3030 3030 3b6c 6574 7465  or:#000000;lette
+000015a0: 722d 7370 6163 696e 673a 3070 783b 776f  r-spacing:0px;wo
+000015b0: 7264 2d73 7061 6369 6e67 3a30 7078 3b74  rd-spacing:0px;t
+000015c0: 6578 742d 7472 616e 7366 6f72 6d3a 6e6f  ext-transform:no
+000015d0: 6e65 3b77 7269 7469 6e67 2d6d 6f64 653a  ne;writing-mode:
+000015e0: 6c72 2d74 623b 6469 7265 6374 696f 6e3a  lr-tb;direction:
+000015f0: 6c74 723b 7465 7874 2d6f 7269 656e 7461  ltr;text-orienta
+00001600: 7469 6f6e 3a6d 6978 6564 3b64 6f6d 696e  tion:mixed;domin
+00001610: 616e 742d 6261 7365 6c69 6e65 3a61 7574  ant-baseline:aut
+00001620: 6f3b 6261 7365 6c69 6e65 2d73 6869 6674  o;baseline-shift
+00001630: 3a62 6173 656c 696e 653b 7465 7874 2d61  :baseline;text-a
+00001640: 6e63 686f 723a 6d69 6464 6c65 3b77 6869  nchor:middle;whi
+00001650: 7465 2d73 7061 6365 3a6e 6f72 6d61 6c3b  te-space:normal;
+00001660: 7368 6170 652d 7061 6464 696e 673a 303b  shape-padding:0;
+00001670: 7368 6170 652d 6d61 7267 696e 3a30 3b69  shape-margin:0;i
+00001680: 6e6c 696e 652d 7369 7a65 3a30 3b6f 7061  nline-size:0;opa
+00001690: 6369 7479 3a31 3b76 6563 746f 722d 6566  city:1;vector-ef
+000016a0: 6665 6374 3a6e 6f6e 653b 6669 6c6c 3a23  fect:none;fill:#
+000016b0: 3030 3030 3030 3b66 696c 6c2d 6f70 6163  000000;fill-opac
+000016c0: 6974 793a 313b 7374 726f 6b65 3a6e 6f6e  ity:1;stroke:non
+000016d0: 653b 7374 726f 6b65 2d77 6964 7468 3a30  e;stroke-width:0
+000016e0: 2e39 3939 3939 3970 783b 7374 726f 6b65  .999999px;stroke
+000016f0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00001700: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00001710: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+00001720: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+00001730: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+00001740: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
+00001750: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
+00001760: 3a31 3b73 746f 702d 636f 6c6f 723a 2330  :1;stop-color:#0
+00001770: 3030 3030 303b 7374 6f70 2d6f 7061 6369  00000;stop-opaci
+00001780: 7479 3a31 220a 2020 2020 2020 2078 3d22  ty:1".       x="
+00001790: 3636 2e33 3336 3438 3722 0a20 2020 2020  66.336487".     
+000017a0: 2020 793d 2234 392e 3233 3632 3938 220a    y="49.236298".
+000017b0: 2020 2020 2020 2069 643d 2274 6578 7438         id="text8
+000017c0: 3430 220a 2020 2020 2020 2074 7261 6e73  40".       trans
+000017d0: 666f 726d 3d22 6d61 7472 6978 2830 2e32  form="matrix(0.2
+000017e0: 3634 3538 3333 332c 302c 302c 302e 3236  6458333,0,0,0.26
+000017f0: 3435 3833 3333 2c31 3538 2e39 3233 3235  458333,158.92325
+00001800: 2c31 3736 2e31 3235 3337 2922 3e3c 7473  ,176.12537)"><ts
+00001810: 7061 6e0a 2020 2020 2020 2020 2073 6f64  pan.         sod
+00001820: 6970 6f64 693a 726f 6c65 3d22 6c69 6e65  ipodi:role="line
+00001830: 220a 2020 2020 2020 2020 2069 643d 2274  ".         id="t
+00001840: 7370 616e 3833 3822 0a20 2020 2020 2020  span838".       
+00001850: 2020 783d 2236 362e 3333 3634 3837 220a    x="66.336487".
+00001860: 2020 2020 2020 2020 2079 3d22 3439 2e32           y="49.2
+00001870: 3336 3239 3822 3e24 7b66 6f6f 7d3c 2f74  36298">${foo}</t
+00001880: 7370 616e 3e3c 2f74 6578 743e 0a20 203c  span></text>.  <
+00001890: 2f67 3e0a 3c2f 7376 673e 0a              /g>.</svg>.
```

### Comparing `pyradium-0.0.8/examples/animation.svg` & `pyradium-0.0.9/examples/animation.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/examples/example.xml` & `pyradium-0.0.9/examples/example.xml`

 * *Files 3% similar despite different names*

#### Comparing `pyradium-0.0.8/examples/example.xml` & `pyradium-0.0.9/examples/example.xml`

```diff
@@ -81,14 +81,20 @@
       <li>
         <s:ac>A</s:ac>
         <s:ac>AB</s:ac>
         <s:ac>ABC</s:ac>
         <s:ac>ABCD</s:ac>
         <s:ac>ABCDE</s:ac>
       </li>
+      <li>
+        Don't confuse
+        <s:ac>MAC1</s:ac>
+        and
+        <s:ac>MAC2</s:ac>
+      </li>
     </ul>
   </slide>
   <slide>
     <s:time abs="1 min"/>
     <s:var name="heading" value="That's the second slide"/>
     <ul>
       <li>This is a test!</li>
@@ -163,21 +169,17 @@
       <s:tex>y^2 = x^3 + ax + b</s:tex>
       and that's just great.
     </p>
   </slide>
   <slide>
     <s:var name="heading" value="Long Formula"/>
     <p>This is the long form:</p>
-    <div>
-      <s:tex long="1">\sum_{i = 0}^{10} \frac{i^2}{\pi}</s:tex>
-    </div>
+    <s:tex long="1">\sum_{i = 0}^{10} \frac{i^2}{\pi}</s:tex>
     <p>While this is the short one for comparison:</p>
-    <div>
-      <s:tex>\sum_{i = 0}^{10} \frac{i^2}{\pi}</s:tex>
-    </div>
+    <s:tex>\sum_{i = 0}^{10} \frac{i^2}{\pi}</s:tex>
   </slide>
   <subsection>Code Highlighting</subsection>
   <slide>
     <s:var name="heading" value="Some Python Code"/>
     <s:code lang="python3"><![CDATA[
 			if foo == "bar":
 				print("foo was 'bar'")
@@ -266,14 +268,24 @@
       <li>
         <s:ar>light</s:ar>
         Lightning
       </li>
     </ul>
   </slide>
   <slide>
+    <s:var name="heading" value="Dashes"/>
+    <ul>
+      <li>By default dashes are replaced by endash and emdash, -- and ---</li>
+      <li>
+        But they can be verbatim as well:
+        <s:verb>-- and ---</s:verb>
+      </li>
+    </ul>
+  </slide>
+  <slide>
     <s:var name="heading" value="Symbols"/>
     <ul>
       <li>
         <s:sym>xor</s:sym>
         XOR and
         <s:sym>xmul</s:sym>
         XMUL
@@ -313,14 +325,20 @@
       </li>
     </ul>
   </slide>
   <slide>
     <s:var name="heading" value="Image Rendering"/>
     <s:img src="3dbox.svg"/>
   </slide>
+  <slide>
+    <s:var name="heading" value="Image Rendering with substitution"/>
+    <s:img src="3dbox.svg">
+      <transform cmd="replace_text" search="${foo}" replace="Works!"/>
+    </s:img>
+  </slide>
   <slide type="animation">
     <s:var name="heading" value="Image Animation"/>
     <s:var name="filename" value="animation.svg"/>
   </slide>
   <slide>
     <s:var name="heading" value="Plot Rendering"/>
     <s:plot src="histo.gnuplot"/>
```

### Comparing `pyradium-0.0.8/examples/histo.gnuplot` & `pyradium-0.0.9/examples/histo.gnuplot`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/licenses/CC-BY-4.0.txt` & `pyradium-0.0.9/licenses/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/licenses/GUST.txt` & `pyradium-0.0.9/licenses/GUST.txt`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/licenses/OFL.txt` & `pyradium-0.0.9/licenses/OFL.txt`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/Acronyms.py` & `pyradium-0.0.9/pyradium/Acronyms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #	pyradium - HTML presentation/slide show generator
-#	Copyright (C) 2021-2021 Johannes Bauer
+#	Copyright (C) 2021-2022 Johannes Bauer
 #
 #	This file is part of pyradium.
 #
 #	pyradium is free software; you can redistribute it and/or modify
 #	it under the terms of the GNU General Public License as published by
 #	the Free Software Foundation; this program is ONLY licensed under
 #	version 3 of the License, later versions are explicitly excluded.
@@ -51,15 +51,15 @@
 
 	def load_database(self, filename):
 		if filename in self._loaded_files:
 			return
 		with open(filename) as f:
 			acronyms = json.load(f)
 		for (acronym_id, acronym_data) in acronyms.items():
-			resolved_acronym = ResolvedAcronym(acronym_id = acronym_id, acronym = acronym_data.get("ac", acronym_id), text = acronym_data["text"], uri = acronym_data.get("uri"))
+			resolved_acronym = ResolvedAcronym(acronym_id = acronym_id, acronym = acronym_data.get("acronym", acronym_id), text = acronym_data["text"], uri = acronym_data.get("uri"))
 			self._acronyms[acronym_id] = resolved_acronym
 
 	def resolve(self, acronym_id):
 		if acronym_id in self._acronyms:
 			self._looked_up.add(acronym_id)
 		else:
 			if acronym_id not in self._unresolvable:
```

### Comparing `pyradium-0.0.8/pyradium/ActionDictAdd.py` & `pyradium-0.0.9/pyradium/ActionDictAdd.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/ActionDumpMetadata.py` & `pyradium-0.0.9/pyradium/ActionDumpMetadata.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/ActionHashPresentation.py` & `pyradium-0.0.9/pyradium/ActionHashPresentation.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/ActionPurge.py` & `pyradium-0.0.9/pyradium/ActionPurge.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/ActionRender.py` & `pyradium-0.0.9/pyradium/ActionRender.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/ActionServe.py` & `pyradium-0.0.9/pyradium/ActionServe.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/ActionShowStyleOpts.py` & `pyradium-0.0.9/pyradium/ActionShowStyleOpts.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/ActionSpellcheck.py` & `pyradium-0.0.9/pyradium/ActionSpellcheck.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/Agenda.py` & `pyradium-0.0.9/pyradium/Agenda.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/BaseAction.py` & `pyradium-0.0.9/pyradium/BaseAction.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/BaseDirective.py` & `pyradium-0.0.9/pyradium/BaseDirective.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/CmdlineEscape.py` & `pyradium-0.0.9/pyradium/CmdlineEscape.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/CmdlineParser.py` & `pyradium-0.0.9/pyradium/CmdlineParser.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/Controller.py` & `pyradium-0.0.9/pyradium/Controller.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/Enums.py` & `pyradium-0.0.9/pyradium/Enums.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/Exceptions.py` & `pyradium-0.0.9/pyradium/Exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,26 @@
 class UndefinedContentException(SlideException): pass
 class TemplateErrorException(SlideException): pass
 class TimeSpecificationError(SlideException): pass
 class UsageException(SlideException): pass
 
 class XMLHookRegistryException(PyRadiumException): pass
 
+class InvalidTransformationException(PyRadiumException): pass
+
 class DuplicateOrderException(PyRadiumException): pass
 class InvalidBooleanValueException(PyRadiumException): pass
 class FailedToLookupFileException(PyRadiumException): pass
 class InvalidTeXException(PyRadiumException): pass
 class UnknownSlideTypeException(PyRadiumException): pass
 
+class AcronymException(PyRadiumException): pass
+class InvalidAcronymFileException(AcronymException): pass
+class DuplicateAcronymException(AcronymException): pass
+
 class FailedToExecuteSubprocessException(PyRadiumException): pass
 
 class SpellcheckerException(PyRadiumException): pass
 
 class StyleParameterException(PyRadiumException): pass
 class InvalidStyleParameterDefinitionException(StyleParameterException): pass
 class InvalidStyleParameterValueException(StyleParameterException): pass
```

### Comparing `pyradium-0.0.8/pyradium/ExtendedJSONEncoder.py` & `pyradium-0.0.9/pyradium/ExtendedJSONEncoder.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/FileLookup.py` & `pyradium-0.0.9/pyradium/FileLookup.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/FriendlyArgumentParser.py` & `pyradium-0.0.9/pyradium/FriendlyArgumentParser.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/GenericTOC.py` & `pyradium-0.0.9/pyradium/GenericTOC.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/Logging.py` & `pyradium-0.0.9/pyradium/Logging.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/MultiCommand.py` & `pyradium-0.0.9/pyradium/MultiCommand.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/OrderedSet.py` & `pyradium-0.0.9/pyradium/OrderedSet.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/PauseRenderer.py` & `pyradium-0.0.9/pyradium/PauseRenderer.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/PrefixMatcher.py` & `pyradium-0.0.9/pyradium/PrefixMatcher.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/Presentation.py` & `pyradium-0.0.9/pyradium/Presentation.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/RenderableSlide.py` & `pyradium-0.0.9/pyradium/RenderableSlide.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/RenderedPresentation.py` & `pyradium-0.0.9/pyradium/RenderedPresentation.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/Renderer.py` & `pyradium-0.0.9/pyradium/Renderer.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/RendererCache.py` & `pyradium-0.0.9/pyradium/RendererCache.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/RenderingParameters.py` & `pyradium-0.0.9/pyradium/RenderingParameters.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/SVGTransformation.py` & `pyradium-0.0.9/pyradium/SVGTransformation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #	pyradium - HTML presentation/slide show generator
-#	Copyright (C) 2015-2021 Johannes Bauer
+#	Copyright (C) 2015-2022 Johannes Bauer
 #
 #	This file is part of pyradium.
 #
 #	pyradium is free software; you can redistribute it and/or modify
 #	it under the terms of the GNU General Public License as published by
 #	the Free Software Foundation; this program is ONLY licensed under
 #	version 3 of the License, later versions are explicitly excluded.
@@ -108,33 +108,39 @@
 
 	@property
 	def visible_layer_ids(self):
 		for layer in self._layers:
 			if layer.is_visible:
 				yield layer.layer_id
 
-
 	@property
 	def layer_ids(self):
 		for layer in self._layers:
 			yield layer.layer_id
 
 	@property
 	def layers(self):
 		return iter(self._layers)
 
-
 	def get_layer(self, layer_id):
 		return self._layers_by_id[layer_id]
 
+	def _search_replace_text(self, search, replace):
+		for text_node in XMLTools.findall_recurse(self._xml, "text"):
+			for tspan_node in XMLTools.findall(text_node, "tspan"):
+				for cdata_node in XMLTools.findall_text(tspan_node, recursive = True):
+					cdata_node.replaceWholeText(cdata_node.wholeText.replace(search, replace))
+
 	def apply(self, transformation_dict):
 		if transformation_dict["cmd"] == "show_layer":
 			self.get_layer(transformation_dict["layer_id"]).show()
 		elif transformation_dict["cmd"] == "hide_layer":
 			self.get_layer(transformation_dict["layer_id"]).hide()
+		elif transformation_dict["cmd"] == "replace_text":
+			self._search_replace_text(transformation_dict["search"], transformation_dict["replace"])
 		else:
 			raise NotImplementedError(transformation_dict["cmd"])
 
 	def apply_all(self, transformation_dicts):
 		for transformation_dict in transformation_dicts:
 			self.apply(transformation_dict)
 
@@ -149,8 +155,18 @@
 	svg = SVGTransformation("animation_l2hid.svg")
 	print(list(svg.layer_ids))
 	layer_ids = list(svg.visible_layer_ids)
 	print(layer_ids)
 	for layer_id in layer_ids:
 		svg.get_layer(layer_id).hide()
 	svg.get_layer(layer_ids[0]).show()
+	svg.apply({
+		"cmd": "replace_text",
+		"search": "MUH TEXT",
+		"replace": "This was Muh.",
+	})
+	svg.apply({
+		"cmd": "replace_text",
+		"search": "FOO TEXT",
+		"replace": "This was Foo.",
+	})
 	svg.write_file("/tmp/x.svg")
```

### Comparing `pyradium-0.0.8/pyradium/Schedule.py` & `pyradium-0.0.9/pyradium/Schedule.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/Slide.py` & `pyradium-0.0.9/pyradium/Slide.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/Spellcheck.py` & `pyradium-0.0.9/pyradium/Spellcheck.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/SpellcheckDictionary.py` & `pyradium-0.0.9/pyradium/SpellcheckDictionary.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/StyleParameters.py` & `pyradium-0.0.9/pyradium/StyleParameters.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/TOC.py` & `pyradium-0.0.9/pyradium/TOC.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/Tools.py` & `pyradium-0.0.9/pyradium/Tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #	pyradium - HTML presentation/slide show generator
-#	Copyright (C) 2015-2021 Johannes Bauer
+#	Copyright (C) 2015-2022 Johannes Bauer
 #
 #	This file is part of pyradium.
 #
 #	pyradium is free software; you can redistribute it and/or modify
 #	it under the terms of the GNU General Public License as published by
 #	the Free Software Foundation; this program is ONLY licensed under
 #	version 3 of the License, later versions are explicitly excluded.
@@ -100,14 +100,22 @@
 		return result
 
 	@classmethod
 	def findall_recurse(cls, root_node, name):
 		return cls.findall_recurse_predicate(root_node, predicate = lambda node: (node.nodeType == node.ELEMENT_NODE) and (node.tagName == name))
 
 	@classmethod
+	def findall_text(cls, root_node, recursive = False):
+		for node in root_node.childNodes:
+			if node.nodeType in [ node.TEXT_NODE, node.CDATA_SECTION_NODE ]:
+				yield node
+			elif recursive:
+				yield from cls.findall_text(node, recursive = True)
+
+	@classmethod
 	def findall(cls, root_node, name, namespace_uri = "*"):
 		result = [ ]
 		for node in root_node.childNodes:
 			if (node.nodeType == node.ELEMENT_NODE) and (node.tagName == name) and (namespace_uri in ("*", node.namespaceURI)):
 				result.append(node)
 		return result
```

### Comparing `pyradium-0.0.8/pyradium/__init__.py` & `pyradium-0.0.9/pyradium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 #	along with pyradium; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 #	Johannes Bauer <JohannesBauer@gmx.de>
 
 import pyradium.Logging
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
```

### Comparing `pyradium-0.0.8/pyradium/__main__.py` & `pyradium-0.0.9/pyradium/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #	pyradium - HTML presentation/slide show generator
-#	Copyright (C) 2015-2021 Johannes Bauer
+#	Copyright (C) 2015-2022 Johannes Bauer
 #
 #	This file is part of pyradium.
 #
 #	pyradium is free software; you can redistribute it and/or modify
 #	it under the terms of the GNU General Public License as published by
 #	the Free Software Foundation; this program is ONLY licensed under
 #	version 3 of the License, later versions are explicitly excluded.
@@ -21,14 +21,15 @@
 
 import sys
 import argparse
 import pyradium
 from .MultiCommand import MultiCommand
 from .ActionRender import ActionRender
 from .ActionServe import ActionServe
+from .ActionAcroAdd import ActionAcroAdd
 from .ActionAcroSort import ActionAcroSort
 from .ActionPurge import ActionPurge
 from .ActionHashPresentation import ActionHashPresentation
 from .ActionDumpMetadata import ActionDumpMetadata
 from .ActionSpellcheck import ActionSpellcheck
 from .ActionDictAdd import ActionDictAdd
 from .ActionShowStyleOpts import ActionShowStyleOpts
@@ -83,15 +84,20 @@
 		parser.add_argument("-v", "--verbose", action = "count", default = 0, help = "Increases verbosity. Can be specified multiple times to increase.")
 		parser.add_argument("dirname", help = "Directory that should be served.")
 	mc.register("serve", "Serve a rendered presentation over HTTP", genparser, action = ActionServe)
 
 	def genparser(parser):
 		parser.add_argument("-v", "--verbose", action = "count", default = 0, help = "Increases verbosity. Can be specified multiple times to increase.")
 		parser.add_argument("acrofile", help = "Acronym database JSON file.")
-	mc.register("acrosort", "Sort an acryonym database", genparser, action = ActionAcroSort)
+	mc.register("acroadd", "Add an acryonym to the acronym database", genparser, action = ActionAcroAdd, aliases = [ "aadd" ])
+
+	def genparser(parser):
+		parser.add_argument("-v", "--verbose", action = "count", default = 0, help = "Increases verbosity. Can be specified multiple times to increase.")
+		parser.add_argument("acrofile", help = "Acronym database JSON file.")
+	mc.register("acrosort", "Sort an acryonym database", genparser, action = ActionAcroSort, aliases = [ "asort" ])
 
 	def genparser(parser):
 		parser.add_argument("-v", "--verbose", action = "count", default = 0, help = "Increases verbosity. Can be specified multiple times to increase.")
 	mc.register("purge", "Purge the document cache", genparser, action = ActionPurge)
 
 	def genparser(parser):
 		parser.add_argument("-I", "--include-dir", metavar = "path", action = "append", default = [ ], help = "Specifies an additional include directory in which, for example, images are located which are referenced from the presentation. Can be issued multiple times.")
```

### Comparing `pyradium-0.0.8/pyradium/renderer/ExecRenderer.py` & `pyradium-0.0.9/pyradium/renderer/ExecRenderer.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/renderer/ImageRenderer.py` & `pyradium-0.0.9/pyradium/renderer/ImageRenderer.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/renderer/LatexFormulaRenderer.py` & `pyradium-0.0.9/pyradium/renderer/LatexFormulaRenderer.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/renderer/PlotRenderer.py` & `pyradium-0.0.9/pyradium/renderer/PlotRenderer.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/renderer/__init__.py` & `pyradium-0.0.9/pyradium/renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/antonio.css` & `pyradium-0.0.9/pyradium/templates/antonio/antonio.css`

 * *Files 2% similar despite different names*

```diff
@@ -245,14 +245,18 @@
 	color: #2185c5;
 }
 
 div.final_flex div.final_sub {
 	color: #677480;
 }
 
+div.texformula {
+	margin-top: 25px;
+	margin-left: 50px;
+}
 
 div.slide.quote div.flex {
 	position: relative;
 	display: flex;
 	height: 70%;
 	top: 30%;
 	width: 100%;
```

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/bar.svg` & `pyradium-0.0.9/pyradium/templates/antonio/bar.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/configuration.json` & `pyradium-0.0.9/pyradium/templates/antonio/configuration.json`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/emojis/0-puke.svg` & `pyradium-0.0.9/pyradium/templates/antonio/emojis/0-puke.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/emojis/1-bad.svg` & `pyradium-0.0.9/pyradium/templates/antonio/emojis/1-bad.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/emojis/2-good.svg` & `pyradium-0.0.9/pyradium/templates/antonio/emojis/2-good.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/emojis/3-great.svg` & `pyradium-0.0.9/pyradium/templates/antonio/emojis/3-great.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-cyrillic-ext.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-cyrillic-ext.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-cyrillic.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-cyrillic.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-greek-ext.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-greek-ext.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-greek.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-greek.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-latin-ext.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-latin-ext.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-latin.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-latin.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Bold-vietnamese.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Bold-vietnamese.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-cyrillic-ext.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-cyrillic-ext.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-cyrillic.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-cyrillic.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-greek-ext.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-greek-ext.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-greek.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-greek.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-latin-ext.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-latin-ext.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-latin.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-latin.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Light-vietnamese.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Light-vietnamese.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-cyrillic-ext.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-cyrillic-ext.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-cyrillic.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-cyrillic.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-greek-ext.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-greek-ext.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-greek.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-greek.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-latin-ext.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-latin-ext.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-latin.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-latin.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira/FiraSans-Regular-vietnamese.woff2` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira/FiraSans-Regular-vietnamese.woff2`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_fira.css` & `pyradium-0.0.9/pyradium/templates/antonio/font_fira.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_latinmodernmono/lmmono10-italic.otf` & `pyradium-0.0.9/pyradium/templates/antonio/font_latinmodernmono/lmmono10-italic.otf`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/font_latinmodernmono/lmmono10-regular.otf` & `pyradium-0.0.9/pyradium/templates/antonio/font_latinmodernmono/lmmono10-regular.otf`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/quote.svg` & `pyradium-0.0.9/pyradium/templates/antonio/quote.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/slide_feedback.html` & `pyradium-0.0.9/pyradium/templates/antonio/slide_feedback.html`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/slide_sectiontitle.html` & `pyradium-0.0.9/pyradium/templates/antonio/slide_sectiontitle.html`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/slide_toc.html` & `pyradium-0.0.9/pyradium/templates/antonio/slide_toc.html`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/template_slide.html` & `pyradium-0.0.9/pyradium/templates/antonio/template_slide.html`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/triangle1.svg` & `pyradium-0.0.9/pyradium/templates/antonio/triangle1.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/triangle2.svg` & `pyradium-0.0.9/pyradium/templates/antonio/triangle2.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/antonio/tribar.svg` & `pyradium-0.0.9/pyradium/templates/antonio/tribar.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/controller_acronym.py` & `pyradium-0.0.9/pyradium/templates/base/controller_acronym.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/controller_animation.py` & `pyradium-0.0.9/pyradium/templates/base/controller_animation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #	pyradium - HTML presentation/slide show generator
-#	Copyright (C) 2021-2021 Johannes Bauer
+#	Copyright (C) 2021-2022 Johannes Bauer
 #
 #	This file is part of pyradium.
 #
 #	pyradium is free software; you can redistribute it and/or modify
 #	it under the terms of the GNU General Public License as published by
 #	the Free Software Foundation; this program is ONLY licensed under
 #	version 3 of the License, later versions are explicitly excluded.
@@ -20,51 +20,71 @@
 #	Johannes Bauer <JohannesBauer@gmx.de>
 
 from pyradium.Controller import BaseController
 from pyradium.Exceptions import UsageException
 from pyradium.SVGTransformation import SVGTransformation
 
 class AnimationController(BaseController):
+	_VALID_ANIMATION_MODES = [ "compose", "replace" ]
+
 	def render(self):
 		filename = self.slide.get_xml_slide_var("filename")
 		if filename is None:
 			raise UsageException("Any 'animation' type slide requires a variable called 'filename' to be set.")
 		if not filename.lower().endswith(".svg"):
 			raise UsageException("Any 'animation' type slide requires an SVG input filename, but found: %s" % (filename))
 
+		animation_mode = self.slide.get_xml_slide_var("mode")
+		if animation_mode is None:
+			animation_mode = "compose"
+		if animation_mode not in self._VALID_ANIMATION_MODES:
+			raise UsageException("An 'animation' type slide needs to have a mode set to any of %s, but found: %s" % (", ".join(self._VALID_ANIMATION_MODES), animation_mode))
+
 		full_filename = self.rendered_presentation.renderer.lookup_include(filename)
 
 		# Determine the number of layers the SVG has first
 		svg = SVGTransformation(full_filename)
-		considered_layers = list(svg.visible_layer_ids)
+		if animation_mode == "compose":
+			considered_layers = list(svg.visible_layer_ids)
+		elif animation_mode == "replace":
+			considered_layers = list(svg.layer_ids)
+		else:
+			raise NotImplementedError(animation_mode)
 		svg_transforms = [ ]
 
 		# Store commands to hide all layers first
 		for layer_id in considered_layers:
 			svg_transforms.append({
 				"cmd":			"hide_layer",
 				"layer_id":		layer_id,
 			})
 
 		# Then show them one-by-one and render each
 		additional_slide_var_list = [ ]
+		previous_layer_id = None
 		renderer = self.rendered_presentation.renderer.get_custom_renderer("img")
 		for layer_id in considered_layers:
 			svg_transforms.append({
 				"cmd":			"show_layer",
 				"layer_id":		layer_id,
 			})
+			if (animation_mode == "replace") and (previous_layer_id is not None):
+				svg_transforms.append({
+					"cmd":			"hide_layer",
+					"layer_id":		previous_layer_id,
+				})
 			rendered_image = renderer.render({
 				"src":				full_filename,
 				"max_dimension":	self.rendered_presentation.renderer.rendering_params.image_max_dimension,
 				"svg_transform":	svg_transforms,
 			})
 			local_filename = "imgs/anim/%s.%s" % (rendered_image.keyhash, rendered_image.data["extension"])
 			self.rendered_presentation.add_file(local_filename, rendered_image.data["img_data"])
 			additional_slide_var_list.append({
 				"image": local_filename,
 			})
+			previous_layer_id = layer_id
 
 		if not self.rendered_presentation.renderer.rendering_params.collapse_animation:
 			yield from self.slide.emit_nocontent_slide(self.rendered_presentation, self.content_containers, additional_slide_var_list)
 		else:
 			yield from self.slide.emit_nocontent_slide(self.rendered_presentation, self.content_containers, additional_slide_var_list[-1])
```

### Comparing `pyradium-0.0.8/pyradium/templates/base/controller_toc.py` & `pyradium-0.0.9/pyradium/templates/base/controller_toc.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/cursor.svg` & `pyradium-0.0.9/pyradium/templates/base/cursor.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/index.html` & `pyradium-0.0.9/pyradium/templates/base/index.html`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/media_error.svg` & `pyradium-0.0.9/pyradium/templates/base/media_error.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/media_pause.svg` & `pyradium-0.0.9/pyradium/templates/base/media_pause.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/media_play.svg` & `pyradium-0.0.9/pyradium/templates/base/media_play.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/media_stop.svg` & `pyradium-0.0.9/pyradium/templates/base/media_stop.svg`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/pygments.css` & `pyradium-0.0.9/pyradium/templates/base/pygments.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.code_highlight .n { color: #000 }
+.code_highlight .p { color: #222 }
 .code_highlight .hll { background-color: #ffffcc }
 .code_highlight .c { color: #60a0b0; font-style: italic } /* Comment */
 /* .code_highlight .err { border: 1px solid #FF0000 } */
 /* Error */
 .code_highlight .k { color: #007020; font-weight: bold } /* Keyword */
 .code_highlight .o { color: #666666 } /* Operator */
 .code_highlight .cm { color: #60a0b0; font-style: italic } /* Comment.Multiline */
```

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium.css` & `pyradium-0.0.9/pyradium/templates/base/pyradium.css`

 * *Files 7% similar despite different names*

```diff
@@ -132,7 +132,19 @@
 }
 
 div.fillimg img {
 	max-width: 100%;
 	max-height: 100%;
 	display: block;
 }
+
+
+table {
+	border-spacing: 0px;
+	border-collapse: separate;
+}
+
+th, td {
+	padding: 5px 15px 5px 15px;
+	text-align: left;
+	border-bottom: 1px solid #ddd;
+}
```

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium.js` & `pyradium-0.0.9/pyradium/templates/base/pyradium.js`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium_feedback.js` & `pyradium-0.0.9/pyradium/templates/base/pyradium_feedback.js`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium_forms.css` & `pyradium-0.0.9/pyradium/templates/base/pyradium_forms.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium_forms.js` & `pyradium-0.0.9/pyradium/templates/base/pyradium_forms.js`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium_menu.css` & `pyradium-0.0.9/pyradium/templates/base/pyradium_menu.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium_modal.css` & `pyradium-0.0.9/pyradium/templates/base/pyradium_modal.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium_modal.js` & `pyradium-0.0.9/pyradium/templates/base/pyradium_modal.js`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium_timer.css` & `pyradium-0.0.9/pyradium/templates/base/pyradium_timer.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium_timer.js` & `pyradium-0.0.9/pyradium/templates/base/pyradium_timer.js`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium_tools.js` & `pyradium-0.0.9/pyradium/templates/base/pyradium_tools.js`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/pyradium_tooltip.css` & `pyradium-0.0.9/pyradium/templates/base/pyradium_tooltip.css`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/templates/base/timer.html` & `pyradium-0.0.9/pyradium/templates/base/timer.html`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/tests/CmdlineParserTests.py` & `pyradium-0.0.9/pyradium/tests/CmdlineParserTests.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/tests/TimeSpecificationTests.py` & `pyradium-0.0.9/pyradium/tests/TimeSpecificationTests.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/tests/__init__.py` & `pyradium-0.0.9/pyradium/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/AcronymHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/AcronymHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/ArrowHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/ArrowHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/CodeHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/CodeHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/DebugHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/DebugHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/EmoHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/EmoHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/ExecHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/ExecHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/ImgHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/PlotHook.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #	pyradium - HTML presentation/slide show generator
-#	Copyright (C) 2015-2021 Johannes Bauer
+#	Copyright (C) 2021-2021 Johannes Bauer
 #
 #	This file is part of pyradium.
 #
 #	pyradium is free software; you can redistribute it and/or modify
 #	it under the terms of the GNU General Public License as published by
 #	the Free Software Foundation; this program is ONLY licensed under
 #	version 3 of the License, later versions are explicitly excluded.
@@ -18,31 +18,31 @@
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 #	Johannes Bauer <JohannesBauer@gmx.de>
 
 from pyradium.xmlhooks.XMLHookRegistry import BaseHook, XMLHookRegistry
 
 @XMLHookRegistry.register_hook
-class ImgHook(BaseHook):
-	_TAG_NAME = "img"
+class PlotHook(BaseHook):
+	_TAG_NAME = "plot"
 
 	@classmethod
 	def handle(cls, rendered_presentation, node):
 		properties = {
 			"src":				rendered_presentation.renderer.lookup_include(node.getAttribute("src")),
 			"max_dimension":	rendered_presentation.renderer.rendering_params.image_max_dimension,
 		}
-		img_renderer = rendered_presentation.renderer.get_custom_renderer("img")
-		rendered_image = img_renderer.render(properties)
-		local_filename = "imgs/img/%s.%s" % (rendered_image.keyhash, rendered_image.data["extension"])
-		uri = "%simgs/img/%s.%s" % (rendered_presentation.renderer.rendering_params.resource_uri, rendered_image.keyhash, rendered_image.data["extension"])
+		plot_renderer = rendered_presentation.renderer.get_custom_renderer("plot")
+		rendered_plot = plot_renderer.render(properties)
+		local_filename = "imgs/plot/%s.%s" % (rendered_plot.keyhash, rendered_plot.data["extension"])
+		uri = "%simgs/plot/%s.%s" % (rendered_presentation.renderer.rendering_params.resource_uri, rendered_plot.keyhash, rendered_plot.data["extension"])
 
 		replacement_node = node.ownerDocument.createElement("div")
 		replacement_node.setAttribute("class", "fillimg")
 
 		img_node = node.ownerDocument.createElement("img")
 		img_node.setAttribute("src", uri)
 		img_node.setAttribute("class", "fill")
 		replacement_node.appendChild(img_node)
 
-		rendered_presentation.add_file(local_filename, rendered_image.data["img_data"])
+		rendered_presentation.add_file(local_filename, rendered_plot.data["img_data"])
 		return replacement_node
```

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/LinkHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/LinkHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/MonospaceHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/MonospaceHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/NoLinebreakHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/NoLinebreakHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/NoSpellcheckHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/NoSpellcheckHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/NthHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/NthHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/PlotHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/TimeHook.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #	pyradium - HTML presentation/slide show generator
-#	Copyright (C) 2021-2021 Johannes Bauer
+#	Copyright (C) 2015-2021 Johannes Bauer
 #
 #	This file is part of pyradium.
 #
 #	pyradium is free software; you can redistribute it and/or modify
 #	it under the terms of the GNU General Public License as published by
 #	the Free Software Foundation; this program is ONLY licensed under
 #	version 3 of the License, later versions are explicitly excluded.
@@ -16,33 +16,21 @@
 #	You should have received a copy of the GNU General Public License
 #	along with pyradium; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 #	Johannes Bauer <JohannesBauer@gmx.de>
 
 from pyradium.xmlhooks.XMLHookRegistry import BaseHook, XMLHookRegistry
+from pyradium.Schedule import TimeSpecification
 
 @XMLHookRegistry.register_hook
-class PlotHook(BaseHook):
-	_TAG_NAME = "plot"
+class TimeHook(BaseHook):
+	_TAG_NAME = "time"
 
 	@classmethod
 	def handle(cls, rendered_presentation, node):
-		properties = {
-			"src":				rendered_presentation.renderer.lookup_include(node.getAttribute("src")),
-			"max_dimension":	rendered_presentation.renderer.rendering_params.image_max_dimension,
-		}
-		plot_renderer = rendered_presentation.renderer.get_custom_renderer("plot")
-		rendered_plot = plot_renderer.render(properties)
-		local_filename = "imgs/plot/%s.%s" % (rendered_plot.keyhash, rendered_plot.data["extension"])
-		uri = "%simgs/plot/%s.%s" % (rendered_presentation.renderer.rendering_params.resource_uri, rendered_plot.keyhash, rendered_plot.data["extension"])
-
-		replacement_node = node.ownerDocument.createElement("div")
-		replacement_node.setAttribute("class", "fillimg")
-
-		img_node = node.ownerDocument.createElement("img")
-		img_node.setAttribute("src", uri)
-		img_node.setAttribute("class", "fill")
-		replacement_node.appendChild(img_node)
-
-		rendered_presentation.add_file(local_filename, rendered_plot.data["img_data"])
-		return replacement_node
+		abs_string = node.getAttribute("abs") if node.hasAttribute("abs") else None
+		rel_string = node.getAttribute("rel") if node.hasAttribute("rel") else None
+		time_spec = TimeSpecification.parse(abs_string = abs_string, rel_string = rel_string)
+		if rendered_presentation.schedule is not None:
+			rendered_presentation.schedule.set_slide_no(rendered_presentation.current_slide_number, time_spec)
+		return node
```

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/QuoteHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/QuoteHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/SymbolHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/SymbolHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/TerminalHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/TerminalHook.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/TexHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/TexHook.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #	pyradium - HTML presentation/slide show generator
-#	Copyright (C) 2015-2021 Johannes Bauer
+#	Copyright (C) 2015-2022 Johannes Bauer
 #
 #	This file is part of pyradium.
 #
 #	pyradium is free software; you can redistribute it and/or modify
 #	it under the terms of the GNU General Public License as published by
 #	the Free Software Foundation; this program is ONLY licensed under
 #	version 3 of the License, later versions are explicitly excluded.
@@ -42,17 +42,28 @@
 		uri = "%simgs/latex/%s.png" % (rendered_presentation.renderer.rendering_params.resource_uri, rendered_formula.keyhash)
 
 		scale_factor = 0.625 * user_scale
 		width_px = round(rendered_formula.data["info"]["width"] * scale_factor)
 		baseline_px = round(rendered_formula.data["info"]["baseline"] * scale_factor)
 		#print(properties["formula"], rendered_formula.data["info"], width_px)
 
-		replacement_node = node.ownerDocument.createElement("img")
-		replacement_node.setAttribute("src", uri)
+		# For now, always wrap in div for long formulae. Could easily add an
+		# option to override this if it's useful.
+		wrap_in_div = properties["long"]
+
+		img_node = node.ownerDocument.createElement("img")
+		img_node.setAttribute("src", uri)
 		if properties["long"]:
-			replacement_node.setAttribute("style", "width: %dpx; margin-top: 5px" % (width_px))
+			img_node.setAttribute("style", "width: %dpx; margin-top: 5px" % (width_px))
+		else:
+			img_node.setAttribute("style", "width: %dpx; margin-bottom: %dpx; margin-top: 5px" % (width_px, -baseline_px + 1))
+		img_node.setAttribute("alt", properties["formula"])
+
+		if not wrap_in_div:
+			replacement_node = img_node
 		else:
-			replacement_node.setAttribute("style", "width: %dpx; margin-bottom: %dpx; margin-top: 5px" % (width_px, -baseline_px + 1))
-		replacement_node.setAttribute("alt", properties["formula"])
+			replacement_node = node.ownerDocument.createElement("div")
+			replacement_node.setAttribute("class", "texformula")
+			replacement_node.appendChild(img_node)
 
 		rendered_presentation.add_file(local_filename, rendered_formula.data["png_data"])
 		return replacement_node
```

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/TimeHook.py` & `pyradium-0.0.9/pyradium/xmlhooks/VerbatimHook.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #	pyradium - HTML presentation/slide show generator
-#	Copyright (C) 2015-2021 Johannes Bauer
+#	Copyright (C) 2015-2022 Johannes Bauer
 #
 #	This file is part of pyradium.
 #
 #	pyradium is free software; you can redistribute it and/or modify
 #	it under the terms of the GNU General Public License as published by
 #	the Free Software Foundation; this program is ONLY licensed under
 #	version 3 of the License, later versions are explicitly excluded.
@@ -15,22 +15,16 @@
 #
 #	You should have received a copy of the GNU General Public License
 #	along with pyradium; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 #	Johannes Bauer <JohannesBauer@gmx.de>
 
-from pyradium.xmlhooks.XMLHookRegistry import BaseHook, XMLHookRegistry
-from pyradium.Schedule import TimeSpecification
+from pyradium.xmlhooks.XMLHookRegistry import InnerTextHook, XMLHookRegistry
 
 @XMLHookRegistry.register_hook
-class TimeHook(BaseHook):
-	_TAG_NAME = "time"
+class VerbatimHook(InnerTextHook):
+	_TAG_NAME = "verb"
 
 	@classmethod
-	def handle(cls, rendered_presentation, node):
-		abs_string = node.getAttribute("abs") if node.hasAttribute("abs") else None
-		rel_string = node.getAttribute("rel") if node.hasAttribute("rel") else None
-		time_spec = TimeSpecification.parse(abs_string = abs_string, rel_string = rel_string)
-		if rendered_presentation.schedule is not None:
-			rendered_presentation.schedule.set_slide_no(rendered_presentation.current_slide_number, time_spec)
-		return node
+	def handle_text(cls, text, rendered_presentation, node):
+		return list(node.childNodes)
```

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/XMLHookRegistry.py` & `pyradium-0.0.9/pyradium/xmlhooks/XMLHookRegistry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #	pyradium - HTML presentation/slide show generator
-#	Copyright (C) 2015-2021 Johannes Bauer
+#	Copyright (C) 2015-2022 Johannes Bauer
 #
 #	This file is part of pyradium.
 #
 #	pyradium is free software; you can redistribute it and/or modify
 #	it under the terms of the GNU General Public License as published by
 #	the Free Software Foundation; this program is ONLY licensed under
 #	version 3 of the License, later versions are explicitly excluded.
@@ -25,14 +25,15 @@
 from pyradium.Tools import XMLTools
 
 _log = logging.getLogger(__spec__.name)
 
 class XMLHookRegistry():
 	_HOOKS = { }
 	_SPECIAL = set([ "var", "pause", "content" ])
+	_BREAK_DESCENT_ON = set([ "s:verb", "s:term", "s:code" ])
 
 	@classmethod
 	def register_hook(cls, hook_class):
 		if hook_class._TAG_NAME is None:
 			raise XMLHookRegistryException("Hook name is not set in hook class: %s" % (hook_class))
 		if hook_class._TAG_NAME in cls._HOOKS:
 			raise XMLHookRegistryException("Duplicate hook name: %s" % (hook_class))
@@ -58,19 +59,21 @@
 							# Delete node
 							XMLTools.remove_node(node)
 						elif replace_by is node:
 							# Keep node
 							pass
 						else:
 							XMLTools.replace_node(node, replace_by)
-							if not isinstance(replace_by, list):
-								XMLTools.walk(replace_by, callback)
-							else:
-								for new_child in replace_by:
-									XMLTools.walk(new_child, callback)
+							continue_descent_with_replaced_elements = node.nodeName not in cls._BREAK_DESCENT_ON
+							if continue_descent_with_replaced_elements:
+								if not isinstance(replace_by, list):
+									XMLTools.walk(replace_by, callback)
+								else:
+									for new_child in replace_by:
+										XMLTools.walk(new_child, callback)
 					else:
 						_log.warning("Unknown hook '%s' used in source document.", hook_name)
 			elif node.nodeType == node.TEXT_NODE:
 				text = node.wholeText
 				new_text = cls._replace_text(text)
 				if text != new_text:
 					node.replaceWholeText(new_text)
```

### Comparing `pyradium-0.0.8/pyradium/xmlhooks/__init__.py` & `pyradium-0.0.9/pyradium/xmlhooks/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,7 +33,8 @@
 from .ExecHook import ExecHook
 from .MonospaceHook import MonospaceHook
 from .DebugHook import DebugHook
 from .NthHook import NthHook
 from .LinkHook import LinkHook
 from .NoSpellcheckHook import NoSpellcheckHook
 from .NoLinebreakHook import NoLinebreakHook
+from .VerbatimHook import VerbatimHook
```

### Comparing `pyradium-0.0.8/pyradium.egg-info/PKG-INFO` & `pyradium-0.0.9/pyradium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyradium
-Version: 0.0.8
+Version: 0.0.9
 Summary: Creating HTML presentations with LaTeX-ish features from XML source
 Home-page: https://github.com/johndoe31415/pyradium
 Author: Johannes Bauer
 Author-email: joe@johannes-bauer.com
 License: gpl-3.0
-Download-URL: https://github.com/johndoe31415/pyradium/archive/0.0.8.tar.gz
+Download-URL: https://github.com/johndoe31415/pyradium/archive/0.0.9.tar.gz
 Description: # pyradium
         [![Build Status](https://travis-ci.com/johndoe31415/pyradium.svg?branch=master)](https://travis-ci.com/johndoe31415/pyradium)
         
         This is a tool which takes XML input that describes a presentation and renders
         it into a presentation HTML. It borrows ideas from LaTeX-beamer but also
         combines the flexible way of creating visually appealing documents using
         HTML/CSS. it In particular, the features are:
```

### Comparing `pyradium-0.0.8/pyradium.egg-info/SOURCES.txt` & `pyradium-0.0.9/pyradium.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,17 @@
 examples/my_data.py
 examples/my_script
 examples/terminal_output.txt
 examples/sub/example_sub.xml
 licenses/CC-BY-4.0.txt
 licenses/GUST.txt
 licenses/OFL.txt
+pyradium/Acrofile.py
 pyradium/Acronyms.py
+pyradium/ActionAcroAdd.py
 pyradium/ActionAcroSort.py
 pyradium/ActionDictAdd.py
 pyradium/ActionDumpMetadata.py
 pyradium/ActionHashPresentation.py
 pyradium/ActionPurge.py
 pyradium/ActionRender.py
 pyradium/ActionServe.py
@@ -197,9 +199,10 @@
 pyradium/xmlhooks/NthHook.py
 pyradium/xmlhooks/PlotHook.py
 pyradium/xmlhooks/QuoteHook.py
 pyradium/xmlhooks/SymbolHook.py
 pyradium/xmlhooks/TerminalHook.py
 pyradium/xmlhooks/TexHook.py
 pyradium/xmlhooks/TimeHook.py
+pyradium/xmlhooks/VerbatimHook.py
 pyradium/xmlhooks/XMLHookRegistry.py
 pyradium/xmlhooks/__init__.py
```

### Comparing `pyradium-0.0.8/pyradium.py` & `pyradium-0.0.9/pyradium.py`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/serve` & `pyradium-0.0.9/serve`

 * *Files identical despite different names*

### Comparing `pyradium-0.0.8/setup.py` & `pyradium-0.0.9/setup.py`

 * *Files identical despite different names*

