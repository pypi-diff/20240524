# Comparing `tmp/makdo-7.5.tar.gz` & `tmp/makdo-7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makdo-7.5.tar", last modified: Wed Apr 24 22:35:56 2024, max compression
+gzip compressed data, was "makdo-7.6.tar", last modified: Fri May 24 09:40:04 2024, max compression
```

## Comparing `makdo-7.5.tar` & `makdo-7.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwx------   0 say       (1000) say       (1000)        0 2024-04-24 22:35:56.419130 makdo-7.5/
--rw-------   0 say       (1000) say       (1000)    35149 2024-04-24 22:35:35.000000 makdo-7.5/LICENSE
--rw-------   0 say       (1000) say       (1000)    19384 2024-04-24 22:35:56.419130 makdo-7.5/PKG-INFO
--rw-------   0 say       (1000) say       (1000)    18997 2024-04-24 22:35:35.000000 makdo-7.5/README.txt
-drwx------   0 say       (1000) say       (1000)        0 2024-04-24 22:35:56.419130 makdo-7.5/makdo/
--rw-------   0 say       (1000) say       (1000)      137 2024-04-24 22:35:35.000000 makdo-7.5/makdo/__init__.py
--rwx------   0 say       (1000) say       (1000)   262582 2024-04-24 22:35:35.000000 makdo-7.5/makdo/makdo_docx2md.py
--rwx------   0 say       (1000) say       (1000)     4201 2024-04-24 22:35:35.000000 makdo-7.5/makdo/makdo_gui.py
--rwx------   0 say       (1000) say       (1000)   237761 2024-04-24 22:35:35.000000 makdo-7.5/makdo/makdo_md2docx.py
-drwx------   0 say       (1000) say       (1000)        0 2024-04-24 22:35:56.419130 makdo-7.5/makdo.egg-info/
--rw-------   0 say       (1000) say       (1000)    19384 2024-04-24 22:35:56.000000 makdo-7.5/makdo.egg-info/PKG-INFO
--rw-------   0 say       (1000) say       (1000)      254 2024-04-24 22:35:56.000000 makdo-7.5/makdo.egg-info/SOURCES.txt
--rw-------   0 say       (1000) say       (1000)        1 2024-04-24 22:35:56.000000 makdo-7.5/makdo.egg-info/dependency_links.txt
--rw-------   0 say       (1000) say       (1000)       32 2024-04-24 22:35:56.000000 makdo-7.5/makdo.egg-info/requires.txt
--rw-------   0 say       (1000) say       (1000)        6 2024-04-24 22:35:56.000000 makdo-7.5/makdo.egg-info/top_level.txt
--rw-------   0 say       (1000) say       (1000)       38 2024-04-24 22:35:56.419130 makdo-7.5/setup.cfg
--rw-------   0 say       (1000) say       (1000)      567 2024-04-24 22:35:35.000000 makdo-7.5/setup.py
+drwx------   0 say       (1000) say       (1000)        0 2024-05-24 09:40:04.572026 makdo-7.6/
+-rw-------   0 say       (1000) say       (1000)    35149 2024-05-24 09:39:55.000000 makdo-7.6/LICENSE
+-rw-------   0 say       (1000) say       (1000)    19412 2024-05-24 09:40:04.572026 makdo-7.6/PKG-INFO
+-rw-------   0 say       (1000) say       (1000)    19025 2024-05-24 09:39:55.000000 makdo-7.6/README.txt
+drwx------   0 say       (1000) say       (1000)        0 2024-05-24 09:40:04.568026 makdo-7.6/makdo/
+-rw-------   0 say       (1000) say       (1000)      137 2024-05-24 09:39:55.000000 makdo-7.6/makdo/__init__.py
+-rwx------   0 say       (1000) say       (1000)   266822 2024-05-24 09:39:55.000000 makdo-7.6/makdo/makdo_docx2md.py
+-rwx------   0 say       (1000) say       (1000)     4201 2024-05-24 09:39:55.000000 makdo-7.6/makdo/makdo_gui.py
+-rwx------   0 say       (1000) say       (1000)   244144 2024-05-24 09:39:55.000000 makdo-7.6/makdo/makdo_md2docx.py
+drwx------   0 say       (1000) say       (1000)        0 2024-05-24 09:40:04.572026 makdo-7.6/makdo.egg-info/
+-rw-------   0 say       (1000) say       (1000)    19412 2024-05-24 09:40:04.000000 makdo-7.6/makdo.egg-info/PKG-INFO
+-rw-------   0 say       (1000) say       (1000)      254 2024-05-24 09:40:04.000000 makdo-7.6/makdo.egg-info/SOURCES.txt
+-rw-------   0 say       (1000) say       (1000)        1 2024-05-24 09:40:04.000000 makdo-7.6/makdo.egg-info/dependency_links.txt
+-rw-------   0 say       (1000) say       (1000)       32 2024-05-24 09:40:04.000000 makdo-7.6/makdo.egg-info/requires.txt
+-rw-------   0 say       (1000) say       (1000)        6 2024-05-24 09:40:04.000000 makdo-7.6/makdo.egg-info/top_level.txt
+-rw-------   0 say       (1000) say       (1000)       38 2024-05-24 09:40:04.572026 makdo-7.6/setup.cfg
+-rw-------   0 say       (1000) say       (1000)      567 2024-05-24 09:39:55.000000 makdo-7.6/setup.py
```

### Comparing `makdo-7.5/LICENSE` & `makdo-7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `makdo-7.5/PKG-INFO` & `makdo-7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: makdo
-Version: 7.5
+Version: 7.6
 Summary: 日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します
 Home-page: https://github.com/hata48915b/makdo/
 Author: Seiichiro HATA
 Author-email: hata48915b@post.nifty.jp
 License: GPLv3+
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<!-- Time-stamp:   <2024.04.04-13:26:58-JST> -->
+<!-- Time-stamp:   <2024.04.30-11:29:18-JST> -->
 
 # MAKDO（MS Wordの互換アプリ）
 
 ![MAKDOのLOGO](https://raw.githubusercontent.com/hata48915b/makdo/main/image/md8docx.png "MAKDOのLOGO")
 
 〜〜 Markdown形式からMS Word形式へ、MS Word形式からMarkdown形式へ 〜〜
 
@@ -437,15 +437,15 @@
 
 [ライブラリのページ（PyPI）](https://pypi.org/project/makdo/)
 
 [簡易実行ファイルのページ](https://hata-o.jp/kian/index?tools#makdo)
 
 ## 名前の由来
 
-"MAKDO"は、"MAKe DOcx"です。
+"MAKDO"は、"MAKe DOcx"と"MArKDOwn"を兼ねています。
 
 "魔苦怒"は、
 「このアプリの"魔"法で、
 ナンバリング（番号付け）やインデント（字下げ）の"苦"しみや"怒"りから、
 皆様を解放したい」
 という思いで、名付けました。
```

### Comparing `makdo-7.5/README.txt` & `makdo-7.6/README.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- Time-stamp:   <2024.04.04-13:26:58-JST> -->
+<!-- Time-stamp:   <2024.04.30-11:29:18-JST> -->
 
 # MAKDO（MS Wordの互換アプリ）
 
 ![MAKDOのLOGO](https://raw.githubusercontent.com/hata48915b/makdo/main/image/md8docx.png "MAKDOのLOGO")
 
 〜〜 Markdown形式からMS Word形式へ、MS Word形式からMarkdown形式へ 〜〜
 
@@ -425,15 +425,15 @@
 
 [ライブラリのページ（PyPI）](https://pypi.org/project/makdo/)
 
 [簡易実行ファイルのページ](https://hata-o.jp/kian/index?tools#makdo)
 
 ## 名前の由来
 
-"MAKDO"は、"MAKe DOcx"です。
+"MAKDO"は、"MAKe DOcx"と"MArKDOwn"を兼ねています。
 
 "魔苦怒"は、
 「このアプリの"魔"法で、
 ナンバリング（番号付け）やインデント（字下げ）の"苦"しみや"怒"りから、
 皆様を解放したい」
 という思いで、名付けました。
```

### Comparing `makdo-7.5/makdo/makdo_docx2md.py` & `makdo-7.6/makdo/makdo_docx2md.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 # Name:         docx2md.py
 # Version:      v07 Furuichibashi
-# Time-stamp:   <2024.04.04-08:36:04-JST>
+# Time-stamp:   <2024.05.19-12:27:22-JST>
 
 # docx2md.py
 # Copyright (C) 2022-2024  Seiichiro HATA
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -140,20 +140,20 @@
     parser.add_argument(
         '-L', '--line-number',
         action='store_true',
         help='行番号を出力します')
     parser.add_argument(
         '-m', '--mincho-font',
         type=str,
-        metavar='FONT_NAME',
+        metavar='FONT_NAME or ASCII_FONT_NAME/KANJI_FONT_NAME',
         help='明朝フォント')
     parser.add_argument(
         '-g', '--gothic-font',
         type=str,
-        metavar='FONT_NAME',
+        metavar='FONT_NAME or ASCII_FONT_NAME/KANJI_FONT_NAME',
         help='ゴシックフォント')
     parser.add_argument(
         '-i', '--ivs-font',
         type=str,
         metavar='FONT_NAME',
         help='異字体（IVS）フォント')
     # parser.add_argument(
@@ -243,41 +243,40 @@
 
 DEFAULT_HEADER_STRING = ''
 
 DEFAULT_PAGE_NUMBER = ': n :'
 
 DEFAULT_LINE_NUMBER = False
 
-DEFAULT_MINCHO_FONT = 'ＭＳ 明朝'
+DEFAULT_MINCHO_FONT = 'Times New Roman / ＭＳ 明朝'
 DEFAULT_GOTHIC_FONT = 'ＭＳ ゴシック'
 DEFAULT_IVS_FONT = 'IPAmj明朝'  # IPAmjMincho
 DEFAULT_MATH_FONT = 'Cambria Math'
 # DEFAULT_MATH_FONT = 'Liberation Serif'
 DEFAULT_FONT_SIZE = 12.0
 TABLE_FONT_SCALE = 0.8
 
 MS_FONTS = [
-    ['ＭＳ 明朝',
-     'ＭＳ明朝',
-     'ＭＳ 明朝;MS Mincho',
-     'MS Mincho;ＭＳ 明朝',
+    ['ＭＳ 明朝', 'ＭＳ明朝',
+     'ＭＳ 明朝;MS Mincho', 'MS Mincho;ＭＳ 明朝',
      'Mincho;MS Mincho'],
-    ['ＭＳゴシック',
-     'ＭＳ ゴシック;MS Gothic',
-     'MS Gothic;ＭＳ ゴシック',
+    ['ＭＳ ゴシック', 'ＭＳゴシック',
+     'ＭＳ ゴシック;MS Gothic', 'MS Gothic;ＭＳ ゴシック',
      'Gothic;MS Gothic'],
-    ['ＭＳ Ｐ明朝',
-     'ＭＳＰ明朝',
-     'ＭＳ Ｐ明朝;MS PMincho',
-     'MS PMincho;ＭＳ Ｐ明朝'
+    ['ＭＳ Ｐ明朝', 'ＭＳＰ明朝',
+     'ＭＳ Ｐ明朝;MS PMincho', 'MS PMincho;ＭＳ Ｐ明朝'
      'PMincho;MS PMincho'],
-    ['ＭＳ Ｐゴシック',
-     'ＭＳ Ｐゴシック;MS PGothic',
-     'MS PGothic; ＭＳ Ｐゴシック',
+    ['ＭＳ Ｐゴシック', 'ＭＳＰゴシック',
+     'ＭＳ Ｐゴシック;MS PGothic', 'MS PGothic; ＭＳ Ｐゴシック',
      'PGothic;MS PGothic'],
+    ['游明朝', 'Yu Mincho'],
+    ['游ゴシック', 'Yu Gothic'],
+    ['ヒラギノ明朝', 'Hiragino Mincho'],
+    ['ヒラギノ角ゴ', 'Hiragino Kaku Gothic'],
+    ['ヒラギノ丸ゴ', 'Hiragino Maru Gothic'],
 ]
 
 DEFAULT_LINE_SPACING = 2.14  # (2.0980+2.1812)/2=2.1396
 
 DEFAULT_SPACE_BEFORE = ''
 DEFAULT_SPACE_AFTER = ''
 TABLE_SPACE_BEFORE = 0.45
@@ -1496,18 +1495,18 @@
                 has_two_or_more_sections = True
         if not has_two_or_more_sections:
             while re.match(NOT_ESCAPED + 'M', Form.page_number):
                 Form.page_number \
                     = re.sub(NOT_ESCAPED + 'M', '\\1N', Form.page_number)
         elif re.match(NOT_ESCAPED + '(N|M)', Form.page_number):
             msg = '※ 警告: ' \
-                + '"<Page>"を含む場合、' \
+                + '"<Pgbr>"を含む場合、' \
                 + 'Libreofficeでは総ページ番号を適切に表示できません'
             # msg = 'warning: ' \
-            #     + 'If "<Page>" is present, ' \
+            #     + 'If "<Pgbr>" is present, ' \
             #     + 'Libreoffice can\'t display total page numbers properly'
             sys.stderr.write(msg + '\n\n')
 
     def _configure_by_document_xml(self, xml_lines):
         width_x = -1.0
         height_x = -1.0
         top_x = -1.0
@@ -1618,62 +1617,81 @@
     def _configure_by_styles_xml(self, xml_lines):
         xml_body = XML.get_body('w:styles', xml_lines)
         xml_blocks = XML.get_blocks(xml_body)
         sb = ['0.0', '0.0', '0.0', '0.0', '0.0', '0.0']
         sa = ['0.0', '0.0', '0.0', '0.0', '0.0', '0.0']
         for xb in xml_blocks:
             name = ''
-            font = ''
+            afnt = ''
+            kfnt = ''
             sz_x = -1.0
             f_it = False
             f_bd = False
             f_sk = False
             f_ul = ''
             f_cl = ''
             f_hc = ''
             alig = ''
             ls_x = -1.0
             ase = -1
             asn = -1
             for xl in xb:
                 name = XML.get_value('w:name', 'w:val', name, xl)
-                font = XML.get_value('w:rFonts', 'w:ascii', font, xl)
-                font = XML.get_value('w:rFonts', 'w:eastAsia', font, xl)
-                # font = XML.get_value('w:rFonts', '*', font, xl)
+                afnt = XML.get_value('w:rFonts', 'w:ascii', afnt, xl)
+                kfnt = XML.get_value('w:rFonts', 'w:eastAsia', kfnt, xl)
                 sz_x = XML.get_value('w:sz', 'w:val', sz_x, xl)
                 f_it = XML.is_this_tag('w:i', f_it, xl)
                 f_bd = XML.is_this_tag('w:b', f_bd, xl)
                 f_sk = XML.is_this_tag('w:strike', f_sk, xl)
                 f_ul = XML.get_value('w:u', 'w:val', f_ul, xl)
                 f_cl = XML.get_value('w:color', 'w:val', f_cl, xl)
                 f_hc = XML.get_value('w:highlight', 'w:val', f_hc, xl)
                 alig = XML.get_value('w:jc', 'w:val', alig, xl)
                 ls_x = XML.get_value('w:spacing', 'w:line', ls_x, xl)
                 ase = XML.get_value('w:autoSpaceDE', 'w:val', ase, xl)
                 asn = XML.get_value('w:autoSpaceDN', 'w:val', asn, xl)
             if name == 'makdo':
                 # MINCHO FONT
-                Form.mincho_font = font
+                if afnt != '' and kfnt != '':
+                    if afnt == kfnt:
+                        Form.mincho_font = afnt
+                    else:
+                        Form.mincho_font = afnt + ' / ' + kfnt
+                elif afnt != '' and kfnt == '':
+                    Form.mincho_font = afnt
+                elif afnt == '' and kfnt != '':
+                    Form.mincho_font = kfnt
                 # FONT SIZE
                 if sz_x > 0:
                     Form.font_size = round(sz_x / 2, 1)
                 # LINE SPACING
                 if ls_x > 0:
                     Form.line_spacing = round(ls_x / 20 / Form.font_size, 2)
                 # AUTO SPACE
                 if ase == 0 and asn == 0:
                     Form.auto_space = False
                 else:
                     Form.auto_space = True
             elif name == 'makdo-g':
                 # GOTHIC FONT
-                Form.gothic_font = font
+                if afnt != '' and kfnt != '':
+                    if afnt == kfnt:
+                        Form.gothic_font = afnt
+                    else:
+                        Form.gothic_font = afnt + ' / ' + kfnt
+                elif afnt != '' and kfnt == '':
+                    Form.gothic_font = afnt
+                elif afnt == '' and kfnt != '':
+                    Form.gothic_font = kfnt
             elif name == 'makdo-i':
                 # IVS FONT
-                Form.ivs_font = font
+                if kfnt != '':
+                    Form.ivs_font = kfnt
+                elif afnt != '':
+                    Form.ivs_font = afnt
             else:
                 for i in range(6):
                     if name != 'makdo-' + str(i + 1):
                         continue
                     for xl in xb:
                         sb[i] \
                             = XML.get_value('w:spacing', 'w:before', sb[i], xl)
@@ -2167,16 +2185,22 @@
         else:
             cfgs += '行番号: 無\n'
         cfgs += '\n'
 
         cfgs += \
             '# 明朝体とゴシック体と異字体（IVS）のフォントを指定できます。'
         cfgs += '\n'
-        cfgs += '明朝体: ' + cls.mincho_font + '\n'
-        cfgs += 'ゴシ体: ' + cls.gothic_font + '\n'
+        if '/' in cls.mincho_font:
+            cfgs += '明朝体: ' + cls.mincho_font + '\n'
+        else:
+            cfgs += '明朝体: = / ' + cls.mincho_font + '\n'
+        if '/' in cls.gothic_font:
+            cfgs += 'ゴシ体: ' + cls.gothic_font + '\n'
+        else:
+            cfgs += 'ゴシ体: = / ' + cls.gothic_font + '\n'
         cfgs += '異字体: ' + cls.ivs_font + '\n'
         cfgs += '\n'
 
         cfgs += \
             '# 基本の文字の大きさをポイント単位で指定できます。'
         cfgs += '\n'
         cfgs += '文字サ: ' + str(round(cls.font_size, 1)) + ' pt\n'
@@ -2648,14 +2672,17 @@
                         paragraphs[-1].md_text = '<Pgbr>'
                     if paragraphs[-1].md_lines_text == '<pgbr>':
                         paragraphs[-1].md_lines_text = '<Pgbr>'
                     if paragraphs[-1].text_to_write == '<pgbr>':
                         paragraphs[-1].text_to_write = '<Pgbr>'
                     if paragraphs[-1].text_to_write_with_reviser == '<pgbr>':
                         paragraphs[-1].text_to_write_with_reviser = '<Pgbr>'
+                    # ATTACHED PAGE BREAK
+                    if paragraphs[-1].attached_pagebreak == 'pgbr':
+                        paragraphs[-1].attached_pagebreak = 'Pgbr'
                 continue
             p = rp.get_paragraph()
             paragraphs.append(p)
         # self.paragraphs = paragraphs
         return paragraphs
 
     def modify_paragraphs(self):
@@ -3347,14 +3374,15 @@
     def __init__(self, xml_lines):
         # DECLARATION
         self.raw_paragraph_number = -1
         self.has_removed = False
         self.xml_lines = []
         self.raw_class = ''
         self.horizontal_line = ''  # 'top'|'bottom'|'textbox'
+        self.attached_pagebreak = ''  # 'pgbr' | 'Pgbr'
         self.chars_data = []
         self.images = {}
         self.raw_text = ''
         self.head_space = ''
         self.tail_space = ''
         self.raw_text_del = ''
         self.raw_text_ins = ''
@@ -3366,14 +3394,15 @@
         # SUBSTITUTION
         RawParagraph.raw_paragraph_number += 1
         self.raw_paragraph_number = RawParagraph.raw_paragraph_number
         self.xml_lines = xml_lines
         self.raw_class = self._get_raw_class(self.xml_lines)
         self.horizontal_line \
             = self._get_horizontal_line(self.raw_class, self.xml_lines)
+        self.attached_pagebreak = self.get_attached_pagebreak(self.xml_lines)
         self.chars_data, self.images \
             = self._get_chars_data_and_images(self.raw_class, self.xml_lines)
         self.raw_text = self._get_raw_text(self.chars_data)
         self.head_space, self.raw_text \
             = self._separate_head_space(self.raw_text,
                                         '->', '<-', '\\+>', '<\\+')
         rts, rrt \
@@ -3415,14 +3444,21 @@
                 return 'bottom'
             res = '^<v:rect( .*)? style="width:0;height:1.5pt"( .*)?>$'
             if re.match(res, xl):
                 # HORIZONTAL LINE (TEXTBOX)
                 return 'textbox'
         return ''
 
+    @staticmethod
+    def get_attached_pagebreak(xml_lines):
+        for xl in xml_lines:
+            if re.match('^<w:br w:type=[\'"]page[\'"]/>$', xl):
+                return 'pgbr'
+        return ''
+
     @classmethod
     def _get_chars_data_and_images(cls, raw_class, xml_lines, type='normal'):
         if raw_class != 'w:tbl':
             font_size = Form.font_size
         else:
             font_size = Form.font_size * TABLE_FONT_SCALE
         chars_data = []
@@ -3537,22 +3573,32 @@
                 continue
             elif re.match('^</w:ruby>$', xl):
                 chars_data.append(CharsDatum([], '>$', []))
                 ruby = ''
                 continue
             # FONT
             if re.match('^<w:rFonts .*>$', xl):
-                font = ''
-                font = XML.get_value('w:rFonts', 'w:ascii', font, xl)
-                font = XML.get_value('w:rFonts', 'w:eastAsia', font, xl)
+                afnt = XML.get_value('w:rFonts', 'w:ascii', '', xl)
+                kfnt = XML.get_value('w:rFonts', 'w:eastAsia', '', xl)
                 # SYMPTOMATIC TREATMENT
                 for mfs in MS_FONTS:
-                    for mf in mfs:
-                        if font == mf:
-                            font = mfs[0]
+                    if afnt in mfs:
+                        afnt = mfs[0]
+                    if kfnt in mfs:
+                        kfnt = mfs[0]
+                font = ''
+                if afnt != '' and kfnt != '':
+                    if afnt == kfnt:
+                        font = afnt
+                    else:
+                        font = afnt + ' / ' + kfnt
+                elif afnt != '' and kfnt == '':
+                    font = afnt
+                elif afnt == '' and kfnt != '':
+                    font = kfnt
                 if font != '':
                     if font == Form.mincho_font:
                         pass
                     elif font == Form.gothic_font:
                         cd.append_fds('`', '`')
                     else:
                         cd.append_fds('@' + font + '@', '@' + font + '@')
@@ -4362,17 +4408,25 @@
     def _convert_ivs(raw_text):
         ivs_font = Form.ivs_font
         res = '^(.*[^\\\\0-9])([0-9]+);'
         while re.match(res, raw_text, flags=re.DOTALL):
             raw_text = re.sub(res, '\\1\\\\\\2;', raw_text, flags=re.DOTALL)
         ivs_beg = int('0xE0100', 16)
         ivs_end = int('0xE01EF', 16)
-        res = '^(.*)@' + ivs_font + '@' + \
-            '(.)([' + chr(ivs_beg) + '-' + chr(ivs_end) + '])' + \
-            '@' + ivs_font + '@(.*)$'
+        #
+        res = '^(.*)(@' + ivs_font + '@)' + \
+            '(.[' + chr(ivs_beg) + '-' + chr(ivs_end) + '])' + \
+            '(.*)$'
+        while re.match(res, raw_text):
+            raw_text = re.sub(res, '\\1\\3\\2\\4', raw_text)
+        #
+        res = '@' + ivs_font + '@@' + ivs_font + '@'
+        raw_text = re.sub(res, '', raw_text)
+        #
+        res = '^(.*)(.)([' + chr(ivs_beg) + '-' + chr(ivs_end) + '])(.*)$'
         while re.match(res, raw_text, flags=re.DOTALL):
             t1 = re.sub(res, '\\1', raw_text, flags=re.DOTALL)
             t2 = re.sub(res, '\\2', raw_text, flags=re.DOTALL)
             t3 = re.sub(res, '\\3', raw_text, flags=re.DOTALL)
             t4 = re.sub(res, '\\4', raw_text, flags=re.DOTALL)
             ivs_n = ord(t3) - ivs_beg
             raw_text = t1 + t2 + str(ivs_n) + ';' + t4
@@ -4615,14 +4669,15 @@
     def __init__(self, raw_paragraph):
         # RECEIVED
         self.raw_paragraph_number = raw_paragraph.raw_paragraph_number
         self.has_removed = raw_paragraph.has_removed
         self.xml_lines = raw_paragraph.xml_lines
         self.raw_class = raw_paragraph.raw_class
         self.horizontal_line = raw_paragraph.horizontal_line
+        self.attached_pagebreak = raw_paragraph.attached_pagebreak
         self.chars_data = raw_paragraph.chars_data
         self.raw_text = raw_paragraph.raw_text
         self.head_space = raw_paragraph.head_space
         self.tail_space = raw_paragraph.tail_space
         self.raw_text_del = raw_paragraph.raw_text_del
         self.raw_text_ins = raw_paragraph.raw_text_ins
         self.raw_text_doi = raw_paragraph.raw_text_doi
@@ -4705,14 +4760,24 @@
         return proper_depth
 
     def _get_revisers_and_md_text(self, raw_text):
         numbering_revisers = []
         head_font_revisers, tail_font_revisers, raw_text \
             = Paragraph._get_font_revisers_and_md_text(raw_text)
         md_text = self._get_md_text(raw_text)
+        # PREFORMATTED
+        if self.paragraph_class == 'preformatted':
+            if '`' in head_font_revisers:
+                head_font_revisers.remove('`')
+            else:
+                head_font_revisers.append('`')
+            if '`' in tail_font_revisers:
+                tail_font_revisers.remove('`')
+            else:
+                tail_font_revisers.append('`')
         return numbering_revisers, head_font_revisers, tail_font_revisers, \
             md_text
 
     @staticmethod
     def _get_font_revisers_and_md_text(raw_text):
         head_font_revisers = []
         tail_font_revisers = []
@@ -5158,14 +5223,16 @@
         numbering_revisers = self.numbering_revisers
         length_revisers = self.length_revisers
         head_font_revisers = self.head_font_revisers
         tail_font_revisers = self.tail_font_revisers
         text_to_write = self.text_to_write
         pre_text_to_write = self.pre_text_to_write
         post_text_to_write = self.post_text_to_write
+        paragraph_class = self.paragraph_class
+        attached_pagebreak = self.attached_pagebreak
         # LEFT SYMBOL
         has_left_sharp = False
         has_left_colon = False
         if re.match('^# (.|\n)*$', text_to_write):
             text_to_write = re.sub('^# ', '', text_to_write)
             has_left_sharp = True
         elif re.match('^: (.|\n)*$', text_to_write):
@@ -5198,14 +5265,20 @@
         for rev in reversed(tail_font_revisers):
             ttwwr += rev
         # RIGHT SYMBOL
         if has_right_colon:
             ttwwr += ' :'
         if post_text_to_write != '':
             ttwwr += '\n' + post_text_to_write
+        # PAGE BREAK
+        if paragraph_class != 'pagebreak':
+            if attached_pagebreak == 'pgbr':
+                ttwwr += '\n\n<pgbr>'
+            if attached_pagebreak == 'Pgbr':
+                ttwwr += '\n\n<Pgbr>'
         text_to_write_with_reviser = ttwwr
         # self.text_to_write_with_reviser = text_to_write_with_reviser
         return text_to_write_with_reviser
 
     @classmethod
     def _split_into_lines(cls, md_text):
         md_lines_text = ''
@@ -6094,19 +6167,30 @@
         m_size = Form.font_size
         t_size = m_size * TABLE_FONT_SCALE
         xml_lines = self.xml_lines
         is_in_row = False
         is_in_cel = False
         tab = []
         wid = []
+        hei = []
         for xl in xml_lines:
-            res = '^<w:gridCol w:w=[\'"]([0-9]+)[\'"]/>$'
-            if re.match(res, xl):
-                w = round((float(re.sub(res, '\\1', xl)) / t_size / 10) - 4)
+            if re.match('^<w:gridCol(?: .*)?/>$', xl):
+                res = '^<(?:.* )?w:w=.*[\'"]([0-9]+)[\'"](?: .*)?/>$'
+                w = 0
+                if re.match(res, xl):
+                    wt = re.sub(res, '\\1', xl)
+                    w = round((float(wt) / t_size / 10) - 4)
                 wid.append(w)
+            if re.match('^<w:trHeight(?: .*)?/>$', xl):
+                h = 0
+                res = '^<(?:.* )?w:val=.*[\'"]([0-9]+)[\'"](?: .*)?/>$'
+                if re.match(res, xl):
+                    ht = re.sub(res, '\\1', xl)
+                    h = round((float(ht) / t_size / 10) - 2)
+                hei.append(h)
             if is_in_cel:
                 cell.append(xl)
             if re.match('<w:tr( .*)?>', xl):
                 row = []
                 is_in_row = True
             elif xl == '<w:tc>':
                 cell = []
@@ -6172,18 +6256,16 @@
                     elif re.match('<w:jc w:val=[\'"]right[\'"]/>', xml):
                         tmp.append('-' * (wid[j] - 1) + ':')
                         break
                 else:
                     tmp.append(':' + '-' * (wid[j] - 1))
                 # NIL OR DOUBLE LINE
                 if col_line[j] == 'nil':
-                    tmp[-1] = re.sub('-', '', tmp[-1], 1)
-                    tmp[-1] += '_'
+                    tmp[-1] += '^'
                 elif col_line[j] == 'double':
-                    tmp[-1] = re.sub('-', '', tmp[-1], 1)
                     tmp[-1] += '='
             ali.append(tmp)
         # GET MD TEXT
         md_text = ''
         is_in_head = True
         for i, row in enumerate(tab):
             if is_in_head:
@@ -6216,20 +6298,29 @@
                     raw_text = re.sub('(\\s+\\\\)$', '\\1 ', raw_text)
                 else:
                     raw_text = re.sub('^\\\\', '', raw_text)
                     raw_text = re.sub('\\\\$', '', raw_text)
                 raw_text = re.sub('\\|', '\\\\|', raw_text)
                 raw_text = re.sub('\n', '<br>', raw_text)
                 md_text += '|' + raw_text + '|'
-            md_text += '\n'
+            # HEIGHT
+            if hei[i] > 0:
+                for xml in cell:
+                    if re.match('<w:vAlign w:val=[\'"]top[\'"]/>', xml):
+                        md_text += ':' + '-' * (hei[i] - 1)
+                    elif re.match('<w:vAlign w:val=[\'"]center[\'"]/>', xml):
+                        md_text += ':' + '-' * (hei[i] - 2) + ':'
+                    elif re.match('<w:vAlign w:val=[\'"]bottom[\'"]/>', xml):
+                        md_text += '-' * (hei[i] - 1) + ':'
             # NIL OR DOUBLE LINE
             if row_line[i] == 'double':
-                md_text += '=\n'
+                md_text += '='
             elif row_line[i] == 'nil':
-                md_text += '_\n'
+                md_text += '^'
+            md_text += '\n'
         tmp_text = ''
         for line in md_text.split('\n'):
             if re.match('^\\|.*\\|$', line):
                 line = re.sub('^\\|', '', line)
                 line = re.sub('\\|$', '', line)
                 line = line.replace('||', '|')
                 line = '|' + line + '|'
@@ -6628,15 +6719,18 @@
     """A class to handle pagebreak paragraph"""
 
     paragraph_class = 'pagebreak'
 
     @classmethod
     def is_this_class(cls, raw_paragraph):
         rp = raw_paragraph
+        rp_text = rp.raw_text
         rp_xl = rp.xml_lines
+        if rp_text != '':
+            return False
         for xl in rp_xl:
             if re.match('^<w:br w:type=[\'"]page[\'"]/>$', xl):
                 return True
         return False
 
     def _get_md_text(self, raw_text):
         md_text = '<pgbr>'
```

### Comparing `makdo-7.5/makdo/makdo_gui.py` & `makdo-7.6/makdo/makdo_gui.py`

 * *Files identical despite different names*

### Comparing `makdo-7.5/makdo/makdo_md2docx.py` & `makdo-7.6/makdo/makdo_md2docx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 # Name:         md2docx.py
 # Version:      v07 Furuichibashi
-# Time-stamp:   <2024.04.02-12:24:28-JST>
+# Time-stamp:   <2024.05.21-05:34:51-JST>
 
 # md2docx.py
 # Copyright (C) 2022-2024  Seiichiro HATA
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -156,20 +156,20 @@
     parser.add_argument(
         '-L', '--line-number',
         action='store_true',
         help='行番号を出力します')
     parser.add_argument(
         '-m', '--mincho-font',
         type=str,
-        metavar='FONT_NAME',
+        metavar='FONT_NAME or ASCII_FONT_NAME/KANJI_FONT_NAME',
         help='明朝フォント')
     parser.add_argument(
         '-g', '--gothic-font',
         type=str,
-        metavar='FONT_NAME',
+        metavar='FONT_NAME or ASCII_FONT_NAME/KANJI_FONT_NAME',
         help='ゴシックフォント')
     parser.add_argument(
         '-i', '--ivs-font',
         type=str,
         metavar='FONT_NAME',
         help='異字体（IVS）フォント')
     # parser.add_argument(
@@ -341,19 +341,20 @@
 
 DEFAULT_HEADER_STRING = ''
 
 DEFAULT_PAGE_NUMBER = ': n :'
 
 DEFAULT_LINE_NUMBER = False
 
-DEFAULT_MINCHO_FONT = 'ＭＳ 明朝'
+DEFAULT_MINCHO_FONT = 'Times New Roman / ＭＳ 明朝'
 DEFAULT_GOTHIC_FONT = 'ＭＳ ゴシック'
 DEFAULT_IVS_FONT = 'IPAmj明朝'  # IPAmjMincho
 DEFAULT_MATH_FONT = 'Cambria Math'
 # DEFAULT_MATH_FONT = 'Liberation Serif'
+DEFAULT_LINE_NUMBER_FONT = 'Calibri'
 DEFAULT_FONT_SIZE = 12.0
 TABLE_FONT_SCALE = 0.8
 
 DEFAULT_LINE_SPACING = 2.14  # (2.0980+2.1812)/2=2.1396
 
 DEFAULT_SPACE_BEFORE = ''
 DEFAULT_SPACE_AFTER = ''
@@ -1082,23 +1083,26 @@
         ms_sec.page_width = Cm(PAPER_WIDTH[Form.paper_size])
         ms_sec.top_margin = Cm(Form.top_margin)
         ms_sec.bottom_margin = Cm(Form.bottom_margin)
         ms_sec.left_margin = Cm(Form.left_margin)
         ms_sec.right_margin = Cm(Form.right_margin)
         ms_sec.header_distance = Cm(1.0)
         ms_sec.footer_distance = Cm(1.0)
-        ms_doc.styles['Normal'].font.size = Pt(m_size / 2)  # line number
+        # NORMAL (LINE NUMBER)
+        ms_doc.styles['Normal'].font.size = Pt(m_size / 2)
+        XML.set_font(ms_doc.styles['Normal'], DEFAULT_LINE_NUMBER_FONT)
+        # LIST
         ms_doc.styles['List Bullet'].font.size = Pt(m_size)
         ms_doc.styles['List Bullet 2'].font.size = Pt(m_size)
         ms_doc.styles['List Bullet 3'].font.size = Pt(m_size)
         ms_doc.styles['List Number'].font.size = Pt(m_size)
         ms_doc.styles['List Number 2'].font.size = Pt(m_size)
         ms_doc.styles['List Number 3'].font.size = Pt(m_size)
         # HEADER
-        # ms_doc.styles['Header'].font.name = self.mincho_font
+        # XML.set_font(ms_doc.styles['Header'], Form.mincho_font)
         # ms_doc.styles['Header'].font.size = Pt(m_size)
         if Form.header_string != '':
             # MDLINE
             ml = MdLine(-1, Form.header_string)
             # RAWPARAGRAPH
             pn = RawParagraph.raw_paragraph_number
             rp = RawParagraph([ml])
@@ -1117,16 +1121,16 @@
             elif p.alignment == 'center':
                 ms_par.alignment = WD_PARAGRAPH_ALIGNMENT.CENTER
             else:
                 ms_par.alignment = WD_PARAGRAPH_ALIGNMENT.LEFT
             p.write_text(ms_par, p.chars_state, p.text_to_write_with_reviser)
             Paragraph.bridge_chars_state.initialize()
         # FOOTER
-        # ms_doc.styles['Footer'].font.name = self.mincho_font  # page number
-        # ms_doc.styles['Footer'].font.size = Pt(m_size)        # page number
+        # XML.set_font(ms_doc.styles['Footer'], Form.mincho_font)
+        # ms_doc.styles['Footer'].font.size = Pt(m_size)
         if Form.page_number != '':
             # MDLINE
             ml = MdLine(-1, Form.page_number)
             # RAWPARAGRAPH
             pn = RawParagraph.raw_paragraph_number
             rp = RawParagraph([ml])
             RawParagraph.raw_paragraph_number = pn
@@ -1146,14 +1150,35 @@
             else:
                 ms_par.alignment = WD_PARAGRAPH_ALIGNMENT.LEFT
             p.write_text(ms_par, p.chars_state, p.text_to_write_with_reviser,
                          'footer')
             Paragraph.bridge_chars_state.initialize()
         # LINE NUMBER
         if Form.line_number:
+            # MS WORD
+            # if 'line number' not in ms_doc.styles:
+            #     ms_doc.styles.add_style('line number',
+            #                             WD_STYLE_TYPE.CHARACTER)
+            # XML.set_font(ms_doc.styles['line number'],
+            #              DEFAULT_LINE_NUMBER_FONT)
+            # ms_doc.styles['line number'].font.size = Pt(m_size / 2)
+            # LIBREOFFICE (ENGLISH)
+            if 'Line Numbering' not in ms_doc.styles:
+                ms_doc.styles.add_style('Line Numbering',
+                                        WD_STYLE_TYPE.CHARACTER)
+            XML.set_font(ms_doc.styles['Line Numbering'],
+                         DEFAULT_LINE_NUMBER_FONT)
+            ms_doc.styles['Line Numbering'].font.size = Pt(m_size / 2)
+            # LIBREOFFICE (JAPANESE)
+            if '行番号付け' not in ms_doc.styles:
+                ms_doc.styles.add_style('行番号付け',
+                                        WD_STYLE_TYPE.CHARACTER)
+            XML.set_font(ms_doc.styles['行番号付け'],
+                         DEFAULT_LINE_NUMBER_FONT)
+            ms_doc.styles['行番号付け'].font.size = Pt(m_size / 2)
             opts = {}
             opts['w:countBy'] = '5'
             opts['w:restart'] = 'newPage'
             opts['w:distance'] = '567'  # 567≒20*72/2.54=1cm
             XML.add_tag(ms_doc.sections[0]._sectPr, 'w:lnNumType', opts)
         self.make_styles(ms_doc)
         return ms_doc
@@ -1161,30 +1186,30 @@
     def make_styles(self, ms_doc):
         m_size = Form.font_size
         s_size = m_size * 0.8
         l_size = m_size * 1.2
         line_spacing = Form.line_spacing
         # NORMAL
         ms_doc.styles.add_style('makdo', WD_STYLE_TYPE.PARAGRAPH)
-        ms_doc.styles['makdo'].font.name = Form.mincho_font
+        XML.set_font(ms_doc.styles['makdo'], Form.mincho_font)
         ms_doc.styles['makdo'].font.size = Pt(m_size)
         ms_doc.styles['makdo'].paragraph_format.line_spacing \
             = Pt(line_spacing * m_size)
         if not Form.auto_space:
             ms_ppr = ms_doc.styles['makdo']._element.get_or_add_pPr()
             # KANJI<->ENGLISH
             XML.add_tag(ms_ppr, 'w:autoSpaceDE', {'w:val': '0'})
             # KANJI<->NUMBER
             XML.add_tag(ms_ppr, 'w:autoSpaceDN', {'w:val': '0'})
         # GOTHIC
         ms_doc.styles.add_style('makdo-g', WD_STYLE_TYPE.PARAGRAPH)
-        ms_doc.styles['makdo-g'].font.name = Form.gothic_font
+        XML.set_font(ms_doc.styles['makdo-g'], Form.gothic_font)
         # IVS
         ms_doc.styles.add_style('makdo-i', WD_STYLE_TYPE.PARAGRAPH)
-        ms_doc.styles['makdo-i'].font.name = Form.ivs_font
+        XML.set_font(ms_doc.styles['makdo-i'], Form.ivs_font)
         # TABLE
         ms_doc.styles.add_style('makdo-t', WD_STYLE_TYPE.PARAGRAPH)
         ms_doc.styles['makdo-t'].font.size = Pt(s_size)
         ms_doc.styles['makdo-t'].paragraph_format.line_spacing = Pt(l_size)
         # ALIGNMENT
         # ms_doc.styles.add_style('makdo-a', WD_STYLE_TYPE.PARAGRAPH)
         # SECTION
@@ -1205,23 +1230,24 @@
         ms_doc.styles['makdo-h'].font.size = Pt(m_size * 0.5)
         # MATH
         ms_doc.styles.add_style('makdo-m', WD_STYLE_TYPE.PARAGRAPH)
         # ms_doc.styles['makdo-m'].font.name = DEFAULT_MATH_FONT
         ms_doc.styles['makdo-m'].font.size = Pt(m_size)
         # REMARKS
         ms_doc.styles.add_style('makdo-r', WD_STYLE_TYPE.PARAGRAPH)
-        ms_doc.styles['makdo-r'].paragraph_format.line_spacing = 0
+        ms_doc.styles['makdo-r'].paragraph_format.line_spacing = Pt(10.5)
         ms_doc.styles['makdo-r'].paragraph_format.space_before = Pt(10.5)
         ms_doc.styles['makdo-r'].paragraph_format.space_after = Pt(10.5)
+        text_width = PAPER_WIDTH[Form.paper_size] \
+            - Form.left_margin - Form.right_margin
+        half_width = text_width / 2
         ms_doc.styles['makdo-r'].paragraph_format.first_line_indent = 0
         ms_doc.styles['makdo-r'].paragraph_format.left_indent = 0
-        ms_doc.styles['makdo-r'].paragraph_format.right_indent = 0
-        ms_doc.styles['makdo-r'].font.name = Form.gothic_font
-        ms_doc.styles['makdo-r'].element.rPr.rFonts.set(ns.qn('w:eastAsia'),
-                                                        Form.gothic_font)
+        ms_doc.styles['makdo-r'].paragraph_format.right_indent = Cm(half_width)
+        XML.set_font(ms_doc.styles['makdo-r'], Form.gothic_font)
         ms_doc.styles['makdo-r'].font.size = Pt(10.5)
         ms_doc.styles['makdo-r'].font.color.rgb = RGBColor(255, 255, 0)
         ms_doc.styles['makdo-r'].font.highlight_color = WD_COLOR_INDEX.BLUE
 
 
 class MdFile:
 
@@ -2011,15 +2037,16 @@
         size = round(chars_state.font_size * chars_state.font_scale, 1)
         oe1 = XML.add_tag(oe0, 'w:rPr', {})
         # FONT
         if chars_state.is_preformatted:
             font = chars_state.gothic_font
         else:
             font = chars_state.mincho_font
-        opt = {'w:ascii': font, 'w:hAnsi': font, 'w:eastAsia': font}
+        af, kf = XML.get_ascii_and_kanji_font(font)
+        opt = {'w:ascii': af, 'w:hAnsi': af, 'w:eastAsia': kf}
         oe2 = XML.add_tag(oe1, 'w:rFonts', opt)
         # ITALIC
         if chars_state.is_italic:
             oe2 = XML.add_tag(oe1, 'w:i', {})
         # BOLD
         if chars_state.is_bold:
             oe2 = XML.add_tag(oe1, 'w:b', {})
@@ -2048,14 +2075,36 @@
         # SUBSCRIPT
         if chars_state.sub_or_sup == 'sub':
             oe2 = XML.add_tag(oe1, 'w:vertAlign', {'w:val': 'subscript'})
         # SUPERSCRIPT
         if chars_state.sub_or_sup == 'sup':
             oe2 = XML.add_tag(oe1, 'w:vertAlign', {'w:val': 'superscript'})
 
+    @staticmethod
+    def set_font(style_or_run, font):
+        af, kf = XML.get_ascii_and_kanji_font(font)
+        style_or_run.font.name = af
+        style_or_run.element.rPr.rFonts.set(ns.qn('w:eastAsia'), kf)
+        # style_or_run._element.rPr.rFonts.set(ns.qn('w:eastAsia'), kf)
+
+    @staticmethod
+    def get_ascii_and_kanji_font(font):
+        fs = (font + '/').split('/')
+        af = fs[0]
+        af = re.sub('^\\s+', '', af)
+        af = re.sub('\\s+$', '', af)
+        kf = fs[1]
+        kf = re.sub('^\\s+', '', kf)
+        kf = re.sub('\\s+$', '', kf)
+        if af == '' or af == '=':
+            return kf, kf
+        if kf == '' or kf == '=':
+            return af, af
+        return af, kf
+
 
 class Math:
 
     """A class to write math expressions"""
 
     symbols = {
         '\\alpha': 'α', '\\beta': 'β', '\\gamma': 'γ', '\\delta': 'δ',
@@ -3230,14 +3279,23 @@
                     p.length_docx['space after'] = 0.0
                     if mx > 0:
                         p_next.length_docx['space before'] \
                             = mx + TABLE_SPACE_AFTER
                     else:
                         p_next.length_docx['space before'] \
                             = mn + TABLE_SPACE_AFTER
+        # SEARCH FOR ATTACHED PAGEBREAK
+        exception = ['empty', 'blank', 'table', 'pagebreak', 'horizontalline',
+                     'remarks']
+        for i, p in enumerate(paragraphs):
+            if i > 0:
+                p_prev = paragraphs[i - 1]
+            if p.paragraph_class == 'pagebreak':
+                if p_prev.paragraph_class not in exception:
+                    p.is_attached_pagebreak = True
         return self.paragraphs
 
     def write_property(self, ms_doc):
         host = socket.gethostname()
         if host is None:
             host = '-'
         hh = self._get_hash(host)
@@ -4366,18 +4424,21 @@
             # .[0-9]+; (IVS (IDEOGRAPHIC VARIATION SEQUENCE))
             ivsn = re.sub(res_ivs, '\\3', unit)
             ivsc = re.sub(res_ivs, '\\2', unit)
             unit = re.sub(res_ivs, '\\1', unit)
             ivsu = int('0xE0100', 16) + int(ivsn)
             if int(ivsu) <= int('0xE01EF', 16):
                 unit = XML.write_unit(ms_par._p, chars_state, unit)
-                save_name = chars_state.mincho_font
-                chars_state.mincho_font = chars_state.ivs_font
+                is_mincho_font = False
+                if chars_state.mincho_font == Form.mincho_font:
+                    is_mincho_font = True
+                    chars_state.mincho_font = chars_state.ivs_font
                 unit = XML.write_unit(ms_par._p, chars_state, ivsc + chr(ivsu))
-                chars_state.mincho_font = save_name
+                if is_mincho_font:
+                    chars_state.mincho_font = Form.mincho_font
         elif re.match(res_foc, unit):
             # "^.*^" (FONT COLOR)
             col = re.sub(res_foc, '\\2', unit)
             if col == '':
                 col = 'FFFFFF'
             elif re.match('^([0-9A-F])([0-9A-F])([0-9A-F])$', col):
                 col = re.sub('^([0-9A-F])([0-9A-F])([0-9A-F])$',
@@ -4793,229 +4854,280 @@
 
 
 class ParagraphTable(Paragraph):
 
     """A class to handle table paragraph"""
 
     paragraph_class = 'table'
-    res_feature = '^\\|.*\\|$'
+    res_feature = '^\\|.*\\|(:?-*:?)?(\\^+|=+)?$'
 
     def write_paragraph(self, ms_doc):
+        md_lines = self.md_lines
         chars_state = self.chars_state
         m_size = Form.font_size
         t_size = m_size * TABLE_FONT_SCALE
-        tab = self._get_table_data(self.md_lines)
-        # NIL OR DOUBLE LINE
-        row_line, col_line, tab = self._get_row_and_col_line(tab)
-        conf_row, ali_list, wid_list = self._get_table_alignment_and_width(tab)
-        if conf_row >= 0:
-            tab.pop(conf_row)
+        # GET DATA
+        tab, conf_line_place, \
+            col_alig_list, col_widt_list, col_rule_list, \
+            row_alig_list, row_heig_list, row_rule_list \
+            = self._get_tab_and_place_and_list(md_lines)
+        cal, cwl, crl = col_alig_list, col_widt_list, col_rule_list
+        tab, col_alig_mtrx, col_widt_mtrx, col_rule_mtrx \
+            = self._get_col_data(tab, conf_line_place, cal, cwl, crl)
+        ral, rhl, rrl = row_alig_list, row_heig_list, row_rule_list
+        tab, row_alig_mtrx, row_heig_mtrx, row_rule_mtrx \
+            = self._get_row_data(tab, conf_line_place, ral, rhl, rrl)
+        # hori_alig_list = col_alig_list
+        hori_leng_list = col_widt_list
+        hori_rule_list = col_rule_list
+        # vert_alig_list = row_alig_list
+        vert_leng_list = row_heig_list
+        vert_rule_list = row_rule_list
+        hori_alig_mtrx = col_alig_mtrx
+        # hori_leng_mtrx = col_widt_mtrx
+        # hori_rule_mtrx = col_rule_mtrx
+        vert_alig_mtrx = row_alig_mtrx
+        # vert_leng_mtrx = row_heig_mtrx
+        # vert_rule_mtrx = row_rule_mtrx
+        # MAKE TABLE
         row = len(tab)
         col = len(tab[0])
         ms_tab = ms_doc.add_table(row, col, style='Table Grid')
+        ms_tab.alignment = WD_TABLE_ALIGNMENT.CENTER
         # ms_tab.autofit = True
+        # SET LENGTH AND ALIGNMENT
         for i in range(len(tab)):
             ms_tab.rows[i].height_rule = WD_ROW_HEIGHT_RULE.AUTO
+            if vert_leng_list[i] > 0:
+                ms_tab.rows[i].height = Pt(t_size * (vert_leng_list[i] + 1))
         for j in range(len(tab[0])):
-            ms_tab.columns[j].width = Pt((wid_list[j] + 2) * t_size)
-        ms_tab.alignment = WD_TABLE_ALIGNMENT.CENTER
+            if hori_leng_list[j] > 0:
+                ms_tab.columns[j].width = Pt(t_size * (hori_leng_list[j] + 2))
+        # SET CELLS
         for i in range(len(tab)):
-            # ms_tab.rows[i].height = Pt(1.5 * m_size)
             for j in range(len(tab[i])):
-                cell = tab[i][j]
-                if re.match('^\\s*:\\s(.*)\\s:\\s*$', cell):
-                    cell = re.sub('^\\s*:\\s(.*)\\s:\\s*$', '\\1', cell)
-                    cel_ali = WD_TABLE_ALIGNMENT.CENTER
-                elif re.match('^\\s*:\\s(.*)$', cell):
-                    cell = re.sub('\\s*:\\s(.*)', '\\1', cell)
-                    cel_ali = WD_TABLE_ALIGNMENT.LEFT
-                elif re.match('^(.*)\\s:\\s*$', cell):
-                    cell = re.sub('^(.*)\\s:\\s*$', '\\1', cell)
-                    cel_ali = WD_TABLE_ALIGNMENT.RIGHT
-                elif i < conf_row:
-                    cel_ali = WD_TABLE_ALIGNMENT.CENTER
-                else:
-                    cel_ali = ali_list[j]
-                if cel_ali == WD_TABLE_ALIGNMENT.LEFT:
-                    cell = re.sub('\\s+$', '', cell)
-                elif cel_ali == WD_TABLE_ALIGNMENT.CENTER:
-                    cell = re.sub('^\\s+', '', cell)
-                    cell = re.sub('\\s+$', '', cell)
-                elif cel_ali == WD_TABLE_ALIGNMENT.RIGHT:
-                    cell = re.sub('^\\s+', '', cell)
+                # ALIGNMENT
                 ms_cell = ms_tab.cell(i, j)
-                ms_cell.width = Pt((wid_list[j] + 2) * t_size)
-                ms_cell.vertical_alignment = WD_ALIGN_VERTICAL.CENTER
+                ms_cell.horizontal_alignment = hori_alig_mtrx[i][j]
+                ms_cell.vertical_alignment = vert_alig_mtrx[i][j]
+                # ms_cell.width = Pt(t_size * (hori_leng_mtrx[i][j] + 2))
+                # ms_cell.height = Pt(t_size * (vert_leng_mtrx[i][j] + 1))
                 ms_par = ms_cell.paragraphs[0]
                 ms_par.style = 'makdo-t'
+                # TEXT
+                cell = tab[i][j]
                 # WORD WRAP (英単語の途中で改行する)
                 ms_ppr = ms_par._p.get_or_add_pPr()
                 XML.add_tag(ms_ppr, 'w:wordWrap', {'w:val': '0'})
                 chars_state.font_size = t_size
                 self.write_text(ms_par, chars_state, cell)
                 chars_state.font_size = m_size
                 ms_fmt = ms_par.paragraph_format
-                ms_fmt.alignment = cel_ali
-                # NIL OR DOUBLE LINE
+                ms_fmt.alignment = hori_alig_mtrx[i][j]
+                # RULE
                 ms_tcpr = ms_cell._tc.get_or_add_tcPr()
                 ms_tcbr = XML.add_tag(ms_tcpr, 'w:tcBorders')
-                if i > 0 and row_line[i - 1] == 'nil':
+                if i > 0 and vert_rule_list[i - 1] == '^':
                     XML.add_tag(ms_tcbr, 'w:top', {'w:val': 'nil'})
-                if row_line[i] == 'nil':
+                if vert_rule_list[i] == '^':
                     XML.add_tag(ms_tcbr, 'w:bottom', {'w:val': 'nil'})
-                if row_line[i] == 'double':
+                if i > 0 and vert_rule_list[i - 1] == '=':
+                    XML.add_tag(ms_tcbr, 'w:top', {'w:val': 'double'})
+                if vert_rule_list[i] == '=':
                     XML.add_tag(ms_tcbr, 'w:bottom', {'w:val': 'double'})
-                if j > 0 and col_line[j - 1] == 'nil':
+                if j > 0 and hori_rule_list[j - 1] == '^':
                     XML.add_tag(ms_tcbr, 'w:left', {'w:val': 'nil'})
-                if col_line[j] == 'nil':
+                if hori_rule_list[j] == '^':
                     XML.add_tag(ms_tcbr, 'w:right', {'w:val': 'nil'})
-                if col_line[j] == 'double':
+                if j > 0 and hori_rule_list[j - 1] == '=':
+                    XML.add_tag(ms_tcbr, 'w:left', {'w:val': 'double'})
+                if hori_rule_list[j] == '=':
                     XML.add_tag(ms_tcbr, 'w:right', {'w:val': 'double'})
 
+    def _get_tab_and_place_and_list(self, md_lines):
+        tab_lines = self._get_tab_lines(md_lines)
+        tab, conf_line_place, \
+            col_alig_list, col_widt_list, col_rule_list, \
+            row_alig_list, row_heig_list, row_rule_list \
+            = self._get_tab_data(tab_lines)
+        return tab, conf_line_place, \
+            col_alig_list, col_widt_list, col_rule_list, \
+            row_alig_list, row_heig_list, row_rule_list
+
     @staticmethod
-    def _get_table_data(md_lines):
-        tab = []
-        line = ''
+    def _get_tab_lines(md_lines):
+        tab_lines = []
+        tab_line = ''
         for ml in md_lines:
-            if re.match('^\\\\?$', ml.text):
+            tab_line += re.sub('^\\s*', '', ml.text)
+            if re.match(NOT_ESCAPED + '\\\\$', tab_line):
+                tab_line = re.sub('\\s*\\\\$', '', tab_line)
                 continue
-            if re.match('^.*\\\\$', line):
-                line = re.sub('\\\\$', '', line)
-                line += re.sub('^\\s*', '', ml.text)
-            else:
-                line += ml.text
-            if re.match('^.*\\\\$', line):
+            tab_lines.append(tab_line)
+            tab_line = ''
+        return tab_lines
+
+    @staticmethod
+    def _get_tab_data(tab_lines):
+        tab = []
+        conf_line_place = -1.0
+        col_alig_list, col_widt_list, col_rule_list = [], [], []
+        row_alig_list, row_heig_list, row_rule_list = [], [], []
+        for tl in tab_lines:
+            if conf_line_place == -1 and \
+               re.match('^(\\|\\s*(:?-*:?)?(\\^+|=+)?\\s*)+\\|$', tl) and \
+               not re.match('^\\|+$', tl):
+                conf_line_place = float(len(tab)) - 0.5
+                tl = re.sub('^\\|(.*)\\|$', '\\1', tl)
+                for c in tl.split('|'):
+                    # COL RULE
+                    if re.match('^.*\\^$', c):
+                        col_rule_list.append('^')
+                    elif re.match('^.*=$', c):
+                        col_rule_list.append('=')
+                    else:
+                        col_rule_list.append('')
+                    c = re.sub('(\\^+|=+)$', '', c)
+                    # COL WIDTH
+                    col_widt_list.append(float(len(c)) / 2)
+                    # COL ALIGN
+                    if re.match('^:-*:$', c):
+                        col_alig_list.append(WD_TABLE_ALIGNMENT.CENTER)
+                    elif re.match('^-*:$', c):
+                        col_alig_list.append(WD_TABLE_ALIGNMENT.RIGHT)
+                    elif re.match('^:?-+$', c) or c == '':
+                        col_alig_list.append(WD_TABLE_ALIGNMENT.LEFT)
                 continue
-            line = re.sub('^\\|', '', line)
-            line = re.sub('\\|$', '', line)
-            # SPLIT BY '|' NOT '\\|'
-            tmp_col = line.split('|')
-            col = []
-            for c in tmp_col:
-                if len(col) > 0 and re.match(NOT_ESCAPED + '\\\\$', col[-1]):
-                    col[-1] += '|' + c
-                else:
-                    col.append(c)
-            if len(col) > 0 and re.match(NOT_ESCAPED + '\\\\$', col[-1]):
-                col[-1] += '|'
-            tab.append(col)
-            line = ''
-            # NIL OR DOUBLE LINE
-            if re.match('^_+$', ml.text):
-                if len(tab[-1]) == 1:
-                    tab.pop(-1)
-                else:
-                    tab[-1].pop(-1)
-                tab.append(['_'])
-            elif re.match('^=+$', ml.text):
-                if len(tab[-1]) == 1:
-                    tab.pop(-1)
-                else:
-                    tab[-1].pop(-1)
-                tab.append(['='])
-        m = 0
-        for rw in tab:
-            if m < len(rw) - 1:
-                m = len(rw) - 1
-        for rw in tab:
-            while len(rw) - 1 < m:
-                rw.append('')
-        # for i in range(len(tab)):
-        #     for j in range(len(tab[i])):
-        #         tab[i][j] = re.sub('^\\s+', '', tab[i][j])
-        #         tab[i][j] = re.sub('\\s+$', '', tab[i][j])
-        return tab
-
-    # FOR NIL OR DOUBLE LINE
-    @staticmethod
-    def _get_row_and_col_line(tab):
-        row_line = []
-        col_line = []
-        has_conf_row = False
+            if tl != '':
+                if not re.match('^(:?-*:?)?(\\^+|=+)?$', tl):
+                    row_rule_list.append('')
+                    row_heig_list.append(0.0)
+                    row_alig_list.append(WD_ALIGN_VERTICAL.CENTER)
+                c = ''
+                res = '^(.*?)\\s*((?::?-+|:-*:|-*:)?(?:\\^+|=+)?)\\s*\\|?$'
+                if re.match(res, tl):
+                    c = re.sub(res, '\\2', tl)
+                    tl = re.sub(res, '\\1', tl)
+                # ROW RULE
+                if re.match('^.*\\^+$', c):
+                    row_rule_list[-1] = '^'
+                    c = re.sub('\\^+$', '', c)
+                elif re.match('^.*=+$', c):
+                    row_rule_list[-1] = '='
+                    c = re.sub('=+$', '', c)
+                # ROW HEIGHT
+                if c != '':
+                    row_heig_list[-1] = float(len(c)) / 2
+                # ROW ALIGN
+                if re.match('^:-*:$', c) or c == '':
+                    row_alig_list[-1] = WD_ALIGN_VERTICAL.CENTER
+                elif re.match('^-*:$', c):
+                    row_alig_list[-1] = WD_ALIGN_VERTICAL.BOTTOM
+                elif re.match('^:?-+$', c):
+                    row_alig_list[-1] = WD_ALIGN_VERTICAL.TOP
+            if tl != '':
+                # TAB
+                cells = []
+                cell = ''
+                tl = re.sub('^\\|', '', tl)
+                tl = re.sub('\\|$', '', tl)
+                for c in tl.split('|'):
+                    cell += c
+                    if re.match(NOT_ESCAPED + '\\\\$', cell):
+                        cell = re.sub('\\\\$', '', cell) + '|'
+                    else:
+                        cells.append(cell)
+                        cell = ''
+                tab.append(cells)
+        # FOR SHORTAGE
+        max_row = 0
+        for row in tab:
+            if max_row < len(row):
+                max_row = len(row)
+        for row in tab:
+            while len(row) < max_row:
+                row.append('')
+            while len(col_alig_list) < max_row:
+                col_alig_list.append(WD_TABLE_ALIGNMENT.LEFT)
+            while len(col_widt_list) < max_row:
+                col_widt_list.append(0.0)
+            while len(col_rule_list) < max_row:
+                col_rule_list.append('')
+        # WIDTH
+        max_width = [0.0 for j in range(len(tab[0]))]
         for i in range(len(tab)):
-            # ROW
             for j in range(len(tab[i])):
-                if j == 0 and not re.match('^(_+|=+)$', tab[i][j]):
-                    break
-                if j > 0 and tab[i][j] != '':
-                    break
-            else:
-                if re.match('^_+$', tab[i][0]):
-                    row_line[-1] = 'nil'
-                else:
-                    row_line[-1] = 'double'
-                tab[i] = '^|remove|$'
-                continue
-            # COLUMN
-            for j in range(len(tab[i])):
-                if has_conf_row:
-                    break
-                if not re.match('^ *:?-*:? *(_|=)?$', tab[i][j]):
-                    break
-            else:
-                for k in range(len(tab[i])):
-                    if re.match('^.*_$', tab[i][k]):
-                        tab[i][k] = re.sub(':_$', '-:', tab[i][k])
-                        tab[i][k] = re.sub('_$', '-', tab[i][k])
-                        col_line.append('nil')
-                    elif re.match('^.*=$', tab[i][k]):
-                        tab[i][k] = re.sub(':=$', '-:', tab[i][k])
-                        tab[i][k] = re.sub('=$', '-', tab[i][k])
-                        col_line.append('double')
-                    else:
-                        col_line.append('')
-                has_conf_row = True
-                continue
-            row_line.append('')
-        # COLUMN (IF NO CONFIG LINE)
-        if col_line == []:
-            m = 0
-            for t in tab:
-                n = len(t)
-                if m < n:
-                    m = n
-            col_line = ['' for x in range(m)]
-        while '^|remove|$' in tab:
-            tab.remove('^|remove|$')
-        return row_line, col_line, tab
+                line = ''
+                for t in tab[i][j].split('<br>'):
+                    if re.match(NOT_ESCAPED + '\\\\$', t):
+                        line += re.sub('\\\\$', '', t) + '<br>'
+                        continue
+                    line += t
+                    line = re.sub('^\\s*:\\s(.*)$', '\\1', line)
+                    line = re.sub(NOT_ESCAPED + '\\s:\\s*$', '\\1', line)
+                    for fd in FONT_DECORATORS + ['<>']:
+                        while re.match(NOT_ESCAPED + fd, line):
+                            line = re.sub(NOT_ESCAPED + fd, '\\1', line)
+                    w = get_real_width(line) / 2
+                    if max_width[j] < w:
+                        max_width[j] = w
+                    line = ''
+        for j in range(len(col_alig_list)):
+            if col_widt_list[j] == 0:
+                col_widt_list[j] = max_width[j]
+        # RETURN
+        return tab, conf_line_place, \
+            col_alig_list, col_widt_list, col_rule_list, \
+            row_alig_list, row_heig_list, row_rule_list
 
     @staticmethod
-    def _get_table_alignment_and_width(tab):
-        conf_row = -1
+    def _get_col_data(tab, conf_line_place,
+                      col_alig_list, col_widt_list, col_rule_list):
+        col_alig_mtrx, col_widt_mtrx, col_rule_mtrx = [], [], []
         for i in range(len(tab)):
+            ca, cw, cr = [], [], []
             for j in range(len(tab[i])):
-                if not re.match('^ *:?-*:? *(_|=)?$', tab[i][j]):
-                    break
-            else:
-                conf_row = i
-                break
-        ali_list = []
-        wid_list = []
-        if conf_row >= 0:
-            for s in tab[conf_row]:
-                s = s.replace(' ', '')
-                if re.match('^:-*:$', s):
-                    ali_list.append(WD_TABLE_ALIGNMENT.CENTER)
-                elif re.match('^-+:$', s):
-                    ali_list.append(WD_TABLE_ALIGNMENT.RIGHT)
-                else:
-                    ali_list.append(WD_TABLE_ALIGNMENT.LEFT)
-                wid_list.append(float(len(s)) / 2)
-        else:
-            for i in range(len(tab)):
-                while len(ali_list) < len(tab[i]):
-                    ali_list.append(WD_TABLE_ALIGNMENT.LEFT)
-                while len(wid_list) < len(tab[i]):
-                    wid_list.append(0.0)
-                for j in range(len(tab[i])):
-                    s = tab[i][j]
-                    w = float(get_real_width(s)) / 2
-                    if wid_list[j] < w:
-                        wid_list[j] = w
-        return conf_row, ali_list, wid_list
+                ca.append(col_alig_list[j])
+                cw.append(col_widt_list[j])
+                cr.append(col_rule_list[j])
+            col_alig_mtrx.append(ca)
+            col_widt_mtrx.append(cw)
+            col_rule_mtrx.append(cr)
+        # ALIGNMENT
+        for i in range(len(tab)):
+            for j in range(len(tab[i])):
+                cell = tab[i][j]
+                if re.match('^\\s*:\\s', cell) and \
+                   re.match(NOT_ESCAPED + '\\s:\\s*$', cell):
+                    col_alig_mtrx[i][j] = WD_TABLE_ALIGNMENT.CENTER
+                    tab[i][j] = re.sub('^\\s*:\\s(.*)\\s:\\s*$', '\\1', cell)
+                elif re.match('^\\s*:\\s', cell):
+                    col_alig_mtrx[i][j] = WD_TABLE_ALIGNMENT.LEFT
+                    tab[i][j] = re.sub('^\\s*:\\s(.*)$', '\\1', cell)
+                elif re.match(NOT_ESCAPED + '\\s:\\s*$', cell):
+                    col_alig_mtrx[i][j] = WD_TABLE_ALIGNMENT.RIGHT
+                    tab[i][j] = re.sub('^(.*)\\s:\\s*$', '\\1', cell)
+                elif conf_line_place > 0 and i < conf_line_place:
+                    col_alig_mtrx[i][j] = WD_TABLE_ALIGNMENT.CENTER
+        return tab, col_alig_mtrx, col_widt_mtrx, col_rule_mtrx
+
+    @staticmethod
+    def _get_row_data(tab, conf_line_place,
+                      row_alig_list, row_heig_list, row_rule_list):
+        row_alig_mtrx, row_heig_mtrx, row_rule_mtrx = [], [], []
+        for i in range(len(tab)):
+            ra, rh, rr = [], [], []
+            for j in range(len(tab[i])):
+                ra.append(row_alig_list[i])
+                rh.append(row_heig_list[i])
+                rr.append(row_rule_list[i])
+            row_alig_mtrx.append(ra)
+            row_heig_mtrx.append(rh)
+            row_rule_mtrx.append(rr)
+        return tab, row_alig_mtrx, row_heig_mtrx, row_rule_mtrx
 
 
 class ParagraphImage(Paragraph):
 
     """A class to handle image paragraph"""
 
     paragraph_class = 'image'
@@ -5065,15 +5177,15 @@
                     ms_doc.add_picture(path, height=Cm(cm_h))
                 else:
                     ms_doc.add_picture(path)
                 ms_doc.paragraphs[-1].alignment = WD_ALIGN_PARAGRAPH.CENTER
                 # CAPTION
                 if capt != '':
                     ms_run = ms_doc.paragraphs[-1].add_run('\n' + capt)
-                    ms_run.font.name = self.chars_state.mincho_font
+                    XML.set_font(ms_run, self.chars_state.mincho_font)
                     ms_run.font.size = Pt(self.chars_state.font_size)
             except BaseException:
                 e = ms_doc.paragraphs[-1]._element
                 e.getparent().remove(e)
                 ms_par = self._get_ms_par(ms_doc)
                 ms_par.add_run(text)
                 ms_par.alignment = WD_ALIGN_PARAGRAPH.CENTER
@@ -5409,17 +5521,26 @@
 class ParagraphPagebreak(Paragraph):
 
     """A class to handle preformatted paragraph"""
 
     paragraph_class = 'pagebreak'
     res_feature = '^(?:<div style="break-.*: page;"></div>|<pgbr/?>|<Pgbr/?>)$'
 
+    def __init__(self, raw_paragraph):
+        super().__init__(raw_paragraph)
+        self.is_attached_pagebreak = False
+
     def write_paragraph(self, ms_doc):
+        is_attached_pagebreak = self.is_attached_pagebreak
         ttw = self.text_to_write
-        ms_doc.add_page_break()
+        if is_attached_pagebreak:
+            ms_run = XML.add_tag(ms_doc.paragraphs[-1]._p, 'w:r')
+            XML.add_tag(ms_run, 'w:br', {'w:type': 'page'})
+        else:
+            ms_doc.add_page_break()
         if re.match('<Pgbr/?>', ttw):
             ms_doc.add_section(WD_SECTION.NEW_PAGE)
             XML.add_tag(ms_doc.sections[-1]._sectPr,
                         'w:pgNumType', {'w:start': '1'})
 
 
 class ParagraphHorizontalLine(Paragraph):
```

### Comparing `makdo-7.5/makdo.egg-info/PKG-INFO` & `makdo-7.6/makdo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: makdo
-Version: 7.5
+Version: 7.6
 Summary: 日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します
 Home-page: https://github.com/hata48915b/makdo/
 Author: Seiichiro HATA
 Author-email: hata48915b@post.nifty.jp
 License: GPLv3+
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<!-- Time-stamp:   <2024.04.04-13:26:58-JST> -->
+<!-- Time-stamp:   <2024.04.30-11:29:18-JST> -->
 
 # MAKDO（MS Wordの互換アプリ）
 
 ![MAKDOのLOGO](https://raw.githubusercontent.com/hata48915b/makdo/main/image/md8docx.png "MAKDOのLOGO")
 
 〜〜 Markdown形式からMS Word形式へ、MS Word形式からMarkdown形式へ 〜〜
 
@@ -437,15 +437,15 @@
 
 [ライブラリのページ（PyPI）](https://pypi.org/project/makdo/)
 
 [簡易実行ファイルのページ](https://hata-o.jp/kian/index?tools#makdo)
 
 ## 名前の由来
 
-"MAKDO"は、"MAKe DOcx"です。
+"MAKDO"は、"MAKe DOcx"と"MArKDOwn"を兼ねています。
 
 "魔苦怒"は、
 「このアプリの"魔"法で、
 ナンバリング（番号付け）やインデント（字下げ）の"苦"しみや"怒"りから、
 皆様を解放したい」
 という思いで、名付けました。
```

### Comparing `makdo-7.5/setup.py` & `makdo-7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='makdo',
-    version='07.05',
+    version='07.06',
     description='日本の公用文書（司法文書、行政文書）をMarkdown形式とMicrosoft Word形式との間で変換します',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Seiichiro HATA',
     author_email='hata48915b@post.nifty.jp',
     url='https://github.com/hata48915b/makdo/',
     license='GPLv3+',
```

