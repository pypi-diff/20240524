# Comparing `tmp/QEasyWidgets-0.1.9.tar.gz` & `tmp/QEasyWidgets-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QEasyWidgets-0.1.9.tar", last modified: Sat May 18 01:46:20 2024, max compression
+gzip compressed data, was "QEasyWidgets-0.2.0.tar", last modified: Fri May 24 09:19:57 2024, max compression
```

## Comparing `QEasyWidgets-0.1.9.tar` & `QEasyWidgets-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 01:46:20.487784 QEasyWidgets-0.1.9/
--rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:12.000000 QEasyWidgets-0.1.9/LICENSE
--rw-rw-rw-   0        0        0       82 2024-04-05 05:40:54.000000 QEasyWidgets-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1908 2024-05-18 01:46:20.487784 QEasyWidgets-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 01:46:20.483498 QEasyWidgets-0.1.9/QEasyWidgets/
--rw-rw-rw-   0        0        0    23460 2024-05-18 01:45:51.000000 QEasyWidgets-0.1.9/QEasyWidgets/ComponentsCustomizer.py
--rw-rw-rw-   0        0        0    15667 2024-05-18 01:45:53.000000 QEasyWidgets-0.1.9/QEasyWidgets/QFunctions.py
--rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:06.000000 QEasyWidgets-0.1.9/QEasyWidgets/QTasks.py
--rw-rw-rw-   0        0        0    70976 2024-05-08 10:24:53.000000 QEasyWidgets-0.1.9/QEasyWidgets/Sources.py
--rw-rw-rw-   0        0        0    29202 2024-05-17 06:15:06.000000 QEasyWidgets-0.1.9/QEasyWidgets/Utils.py
--rw-rw-rw-   0        0        0    22606 2024-05-08 02:30:45.000000 QEasyWidgets-0.1.9/QEasyWidgets/WindowCustomizer.py
--rw-rw-rw-   0        0        0       22 2024-04-01 00:18:06.000000 QEasyWidgets-0.1.9/QEasyWidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 01:46:20.486325 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/
--rw-rw-rw-   0        0        0     1908 2024-05-18 01:46:20.000000 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-05-18 01:46:20.000000 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 01:46:20.000000 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-18 01:46:20.000000 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-18 01:46:20.000000 QEasyWidgets-0.1.9/QEasyWidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1135 2024-04-01 15:15:08.000000 QEasyWidgets-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-18 01:46:20.488784 QEasyWidgets-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1570 2024-05-14 15:33:05.000000 QEasyWidgets-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:19:57.480577 QEasyWidgets-0.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-12-07 09:28:12.000000 QEasyWidgets-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       82 2024-04-05 05:40:54.000000 QEasyWidgets-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1759 2024-05-24 09:19:57.480577 QEasyWidgets-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 09:19:57.477033 QEasyWidgets-0.2.0/QEasyWidgets/
+-rw-rw-rw-   0        0        0    24077 2024-05-24 09:18:44.000000 QEasyWidgets-0.2.0/QEasyWidgets/ComponentsCustomizer.py
+-rw-rw-rw-   0        0        0    16782 2024-05-24 09:18:48.000000 QEasyWidgets-0.2.0/QEasyWidgets/QFunctions.py
+-rw-rw-rw-   0        0        0     4305 2024-04-01 00:18:06.000000 QEasyWidgets-0.2.0/QEasyWidgets/QTasks.py
+-rw-rw-rw-   0        0        0    83693 2024-05-24 09:19:11.000000 QEasyWidgets-0.2.0/QEasyWidgets/Sources.py
+-rw-rw-rw-   0        0        0    29648 2024-05-23 01:55:07.000000 QEasyWidgets-0.2.0/QEasyWidgets/Utils.py
+-rw-rw-rw-   0        0        0    22606 2024-05-08 02:30:45.000000 QEasyWidgets-0.2.0/QEasyWidgets/WindowCustomizer.py
+-rw-rw-rw-   0        0        0       22 2024-04-01 00:18:06.000000 QEasyWidgets-0.2.0/QEasyWidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:19:57.479651 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/
+-rw-rw-rw-   0        0        0     1759 2024-05-24 09:19:57.000000 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-05-24 09:19:57.000000 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 09:19:57.000000 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-24 09:19:57.000000 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-24 09:19:57.000000 QEasyWidgets-0.2.0/QEasyWidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1135 2024-04-01 15:15:08.000000 QEasyWidgets-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 09:19:57.480577 QEasyWidgets-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1570 2024-05-24 09:18:36.000000 QEasyWidgets-0.2.0/setup.py
```

### Comparing `QEasyWidgets-0.1.9/LICENSE` & `QEasyWidgets-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.9/PKG-INFO` & `QEasyWidgets-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.1.9
+Version: 0.2.0
 Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PySide6
-Requires-Dist: darkdetect
-Requires-Dist: tqdm
-Requires-Dist: psutil
-Requires-Dist: nvidia-ml-py
-Requires-Dist: PyGithub
 
 <div align = "center">
 
 # QEasyWidgets
 
 [![Releases](https://img.shields.io/github/v/release/Spr-Aachen/QEasyWidgets?color=green&label=Release&logo=Github&logoColor=white&style=for-the-badge)](https://github.com/Spr-Aachen/QEasyWidgets/releases/latest)&nbsp;
```

### Comparing `QEasyWidgets-0.1.9/QEasyWidgets/ComponentsCustomizer.py` & `QEasyWidgets-0.2.0/QEasyWidgets/ComponentsCustomizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 from .Sources import *
 
 ##############################################################################################################################
 
 class WidgetBase(QWidget):
     '''
     '''
-    Resized = Signal()
+    resized = Signal()
 
     def __init__(self,
         parent: Optional[QWidget] = None,
     ):
         super().__init__(parent)
 
     def resizeEvent(self, event: QResizeEvent) -> None:
-        self.Resized.emit()
+        self.resized.emit()
         '''
         if self.minimumSizeHint() != self.size():
             self.adjustSize()
         '''
         super().resizeEvent(event)
 
 ##############################################################################################################################
@@ -169,28 +169,47 @@
         StyleSheetBase.ScrollArea.Apply(self)
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.ScrollArea.Deregistrate(self)
 
 ##############################################################################################################################
 
+class TreeWidgetBase(QTreeWidget):
+    '''
+    '''
+    def __init__(self, parent=None):
+        super().__init__(parent=parent)
+
+        self.header().setHighlightSections(False)
+        self.header().setDefaultAlignment(Qt.AlignCenter)
+
+        self.setItemDelegate(QStyledItemDelegate(self))
+        self.setIconSize(QSize(16, 16))
+
+        StyleSheetBase.Tree.Apply(self)
+
+    def ClearDefaultStyleSheet(self) -> None:
+        StyleSheetBase.Tree.Deregistrate(self)
+
+##############################################################################################################################
+
 class LabelBase(QLabel):
     '''
     '''
-    Resized = Signal()
+    resized = Signal()
 
     def __init__(self,
         parent: Optional[QWidget] = None
     ):
         super().__init__(parent)
 
         StyleSheetBase.Label.Apply(self)
 
     def resizeEvent(self, event: QResizeEvent) -> None:
-        self.Resized.emit()
+        self.resized.emit()
         super().resizeEvent(event)
 
     def ClearDefaultStyleSheet(self) -> None:
         StyleSheetBase.Label.Deregistrate(self)
 
 ##############################################################################################################################
 
@@ -217,15 +236,15 @@
 
         widgetlayout = QGridLayout()
         widgetlayout.setContentsMargins(0, 0, 0, 0)
         widgetlayout.setSpacing(0)
         self.Widget = WidgetBase()
         self.Widget.setAttribute(Qt.WA_StyledBackground)
         self.Widget.setLayout(widgetlayout)
-        self.Widget.Resized.connect(self._resizeHeight)
+        self.Widget.resized.connect(self._resizeHeight)
 
         self.Layout = QVBoxLayout(self)
         self.Layout.setContentsMargins(0, 0, 0, 0)
         self.Layout.setSpacing(0)
         self.Layout.addWidget(self.FolderButton)
         self.Layout.addWidget(self.Widget)
 
@@ -239,15 +258,15 @@
 
     def addWidget(self, widget: QWidget, title: str):
         self.Widget.layout().addWidget(widget)
         self.FolderButton.setText(title)
         def resizeWidgetHeight():
             AdjustedHeight = widget.height()
             self.Widget.setFixedHeight(AdjustedHeight) if self.IsExpanded else None
-        widget.Resized.connect(resizeWidgetHeight) if hasattr(widget, 'Resized') else None
+        widget.resized.connect(resizeWidgetHeight) if hasattr(widget, 'resized') else None
 
     def expand(self):
         Function_SetWidgetSizeAnimation(self.Widget, TargetHeight = self.Widget.minimumSizeHint().height()).start()
         self.Label.setPixmap(QPixmap(":/ToolBox_Icon/Icons/DownArrow.png").scaled(self.Label.size(), Qt.IgnoreAspectRatio, Qt.SmoothTransformation))
         self.IsExpanded = True
 
     def collapse(self):
@@ -280,15 +299,15 @@
         page = ToolPage(self)
         page.addWidget(widget, text)
         self.Layout.addWidget(page)
         self.Pages.append(page)
         def resizeHeight():
             AdjustedHeight = page.height()
             self.setFixedHeight(AdjustedHeight)
-        page.Resized.connect(resizeHeight)
+        page.resized.connect(resizeHeight)
 
     def widget(self, index: int) -> ToolPage:
         return self.Pages[index]
 
     def setItemText(self, index: int, text: str) -> None:
         self.widget(index).setText(text)
```

### Comparing `QEasyWidgets-0.1.9/QEasyWidgets/QFunctions.py` & `QEasyWidgets-0.2.0/QEasyWidgets/QFunctions.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 class StyleSheetBase(Enum):
     '''
     '''
     Label = 'Label'
     Button = 'Button'
     ScrollArea = 'ScrollArea'
+    Tree = 'Tree'
     ToolBox = 'ToolBox'
     SpinBox = 'SpinBox'
     ComboBox = 'ComboBox'
     Edit = 'Edit'
     Player = 'Player'
     Table = 'Table'
 
@@ -116,14 +117,34 @@
                 continue
 
 
 ComponentsSignals.Signal_SetTheme.connect(Function_UpdateStyleSheet)
 
 ##############################################################################################################################
 
+class IconEngine(QIconEngine):
+    '''
+    '''
+    def __init__(self):
+        super().__init__()
+
+        self.IsIconSVG = False
+
+    def loadSVG(self, SVGString: str):
+        self.IsIconSVG = True
+        self.Icon = SVGString.encode(errors = 'replace')
+
+    def paint(self, painter: QPainter, rect: QRect, mode: QIcon.Mode, state: QIcon.State) -> None:
+        if self.IsIconSVG:
+            renderer = QSvgRenderer(self.Icon)
+            renderer.render(painter, QRectF(rect))
+        else:
+            super().paint(painter, rect, mode, state)
+
+
 class IconBase(Enum):
     '''
     '''
     Ellipsis = 'Ellipsis'
     OpenedFolder = 'OpenedFolder'
     Play = 'Play'
     Pause = 'Pause'
@@ -134,14 +155,29 @@
     def paint(self, painter: QPainter, rect: Union[QRect, QRectF], theme: Optional[str] = None):
         Prefix = 'Icons'
         IconPath = f'Icons/{theme if theme is not None else EasyTheme.THEME}/{self.value}.svg'
         IconPath = Path(f':/{Prefix}').joinpath(IconPath).as_posix()
         Renderer = QSvgRenderer(IconPath)
         Renderer.render(painter, QRectF(rect))
 
+    def create(self, theme: Optional[str] = None) -> QIcon:
+        Prefix = 'Icons'
+        IconPath = f'Icons/{theme if theme is not None else EasyTheme.THEME}/{self.value}.svg'
+        File = QFile(Path(f':/{Prefix}').joinpath(IconPath))
+        File.open(QFile.ReadOnly)
+        DomDocument = QDomDocument()
+        DomDocument.setContent(File.readAll())
+        File.close()
+
+        Engine = IconEngine()
+        Engine.loadSVG(DomDocument.toString())
+        Icon = QIcon(Engine)
+
+        return Icon
+
 
 def Function_DrawIcon(
     icon: Union[str, QIcon],
     painter: QPainter,
     rect: Union[QRect, QRectF]
 ):
     '''
```

### Comparing `QEasyWidgets-0.1.9/QEasyWidgets/QTasks.py` & `QEasyWidgets-0.2.0/QEasyWidgets/QTasks.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.9/QEasyWidgets/Sources.py` & `QEasyWidgets-0.2.0/QEasyWidgets/Sources.py`

 * *Files 10% similar despite different names*

```diff
@@ -765,14 +765,98 @@
    color: rgb(45\
 , 33, 21);\x0d\x0a    \
 background-color\
 : transparent;\x0d\x0a\
 \x09border-width: 0\
 px;\x0d\x0a\x09border-sty\
 le: solid;\x0d\x0a}\
+\x00\x00\x05\x13\
+Q\
+TreeView {\x0d\x0a\x09/*f\
+ont-size: 12px;\x0d\
+\x0a\x09text-align: ce\
+nter;*/\x0d\x0a\x09backgr\
+ound-color: tran\
+sparent;\x0d\x0a\x09borde\
+r: none;\x0d\x0a}\x0d\x0a\x0d\x0aQ\
+TreeView::item {\
+\x0d\x0a\x09background-co\
+lor: transparent\
+;\x0d\x0a\x09padding: 3px\
+;\x0d\x0a}\x0d\x0aQTreeView:\
+:item:hover {\x0d\x0a\x09\
+background-color\
+: rgba(54, 45, 3\
+3, 12);\x0d\x0a}\x0d\x0aQTre\
+eView::item:sele\
+cted {\x0d\x0a}\x0d\x0a\x0d\x0aQTr\
+eeView::branch {\
+\x0d\x0a    background\
+-color: transpar\
+ent;\x0d\x0a\x09border: n\
+one;\x0d\x0a}\x0d\x0aQTreeVi\
+ew::branch:open:\
+has-children {\x0d\x0a\
+\x09image: url(:/Tr\
+ee_Icon/Icons/Do\
+wnArrow.png);\x0d\x0a\x09\
+padding: 3px;\x0d\x0a}\
+\x0d\x0aQTreeView::bra\
+nch:closed:has-c\
+hildren {\x0d\x0a\x09imag\
+e: url(:/Tree_Ic\
+on/Icons/RightAr\
+row.png);\x0d\x0a\x09padd\
+ing: 3px;\x0d\x0a}\x0d\x0a\x0d\x0a\
+\x0d\x0aQScrollBar {\x0d\x0a\
+\x09background-colo\
+r: transparent;\x0d\
+\x0a\x09border-width: \
+1.2px;\x0d\x0a\x09border-\
+radius: 6px;\x0d\x0a\x09b\
+order-style: sol\
+id;\x0d\x0a\x09border-col\
+or: transparent;\
+\x0d\x0a\x09margin: 0px;\x0d\
+\x0a}\x0d\x0aQScrollBar:h\
+over {\x0d\x0a}\x0d\x0a\x0d\x0aQSc\
+rollBar::horizon\
+tal {\x0d\x0a\x09height: \
+9px;\x0d\x0a}\x0d\x0aQScroll\
+Bar::vertical {\x0d\
+\x0a\x09width: 9px;\x0d\x0a}\
+\x0d\x0a\x0d\x0aQScrollBar::\
+sub-line, QScrol\
+lBar::add-line {\
+\x0d\x0a\x09background-co\
+lor: transparent\
+;\x0d\x0a\x09border-width\
+: 0px;\x0d\x0a\x09border-\
+radius: 0px;\x0d\x0a\x09b\
+order-style: sol\
+id;\x0d\x0a}\x0d\x0a\x0d\x0aQScrol\
+lBar::sub-page, \
+QScrollBar::add-\
+page {\x0d\x0a\x09backgro\
+und-color: trans\
+parent;\x0d\x0a}\x0d\x0a\x0d\x0aQS\
+crollBar::handle\
+ {\x0d\x0a\x09background-\
+color: rgba(123,\
+ 123, 123, 123);\
+\x0d\x0a\x09border-width:\
+ 0px;\x0d\x0a\x09border-r\
+adius: 0px;\x0d\x0a\x09bo\
+rder-style: soli\
+d;\x0d\x0a}\x0d\x0aQScrollBa\
+r::handle:hover \
+{\x0d\x0a\x09background-c\
+olor: rgba(123, \
+123, 123, 210);\x0d\
+\x0a}\
 \x00\x00\x03\xe4\
 M\
 ediaPlayerBase Q\
 PushButton {\x0d\x0a  \
   background-col\
 or: transparent;\
 \x0d\x0a    border-wid\
@@ -1265,14 +1349,98 @@
 0, 222, 234);\x0d\x0a \
    background-co\
 lor: transparent\
 ;\x0d\x0a\x09border-width\
 : 0px;\x0d\x0a\x09border-\
 style: solid;\x0d\x0a}\
 \
+\x00\x00\x05\x16\
+Q\
+TreeView {\x0d\x0a\x09/*f\
+ont-size: 12px;\x0d\
+\x0a\x09text-align: ce\
+nter;*/\x0d\x0a\x09backgr\
+ound-color: tran\
+sparent;\x0d\x0a\x09borde\
+r: none;\x0d\x0a}\x0d\x0a\x0d\x0aQ\
+TreeView::item {\
+\x0d\x0a\x09background-co\
+lor: transparent\
+;\x0d\x0a\x09padding: 3px\
+;\x0d\x0a}\x0d\x0aQTreeView:\
+:item:hover {\x0d\x0a\x09\
+background-color\
+: rgba(201, 210,\
+ 222, 33);\x0d\x0a}\x0d\x0aQ\
+TreeView::item:s\
+elected {\x0d\x0a}\x0d\x0a\x0d\x0a\
+QTreeView::branc\
+h {\x0d\x0a    backgro\
+und-color: trans\
+parent;\x0d\x0a\x09border\
+: none;\x0d\x0a}\x0d\x0aQTre\
+eView::branch:op\
+en:has-children \
+{\x0d\x0a\x09image: url(:\
+/Tree_Icon/Icons\
+/DownArrow.png);\
+\x0d\x0a\x09padding: 3px;\
+\x0d\x0a}\x0d\x0aQTreeView::\
+branch:closed:ha\
+s-children {\x0d\x0a\x09i\
+mage: url(:/Tree\
+_Icon/Icons/Righ\
+tArrow.png);\x0d\x0a\x09p\
+adding: 3px;\x0d\x0a}\x0d\
+\x0a\x0d\x0a\x0d\x0aQScrollBar \
+{\x0d\x0a\x09background-c\
+olor: transparen\
+t;\x0d\x0a\x09border-widt\
+h: 1.2px;\x0d\x0a\x09bord\
+er-radius: 6px;\x0d\
+\x0a\x09border-style: \
+solid;\x0d\x0a\x09border-\
+color: transpare\
+nt;\x0d\x0a\x09margin: 0p\
+x;\x0d\x0a}\x0d\x0aQScrollBa\
+r:hover {\x0d\x0a}\x0d\x0a\x0d\x0a\
+QScrollBar::hori\
+zontal {\x0d\x0a\x09heigh\
+t: 9px;\x0d\x0a}\x0d\x0aQScr\
+ollBar::vertical\
+ {\x0d\x0a\x09width: 9px;\
+\x0d\x0a}\x0d\x0a\x0d\x0aQScrollBa\
+r::sub-line, QSc\
+rollBar::add-lin\
+e {\x0d\x0a\x09background\
+-color: transpar\
+ent;\x0d\x0a\x09border-wi\
+dth: 0px;\x0d\x0a\x09bord\
+er-radius: 0px;\x0d\
+\x0a\x09border-style: \
+solid;\x0d\x0a}\x0d\x0a\x0d\x0aQSc\
+rollBar::sub-pag\
+e, QScrollBar::a\
+dd-page {\x0d\x0a\x09back\
+ground-color: tr\
+ansparent;\x0d\x0a}\x0d\x0a\x0d\
+\x0aQScrollBar::han\
+dle {\x0d\x0a\x09backgrou\
+nd-color: rgba(1\
+23, 123, 123, 12\
+3);\x0d\x0a\x09border-wid\
+th: 0px;\x0d\x0a\x09borde\
+r-radius: 0px;\x0d\x0a\
+\x09border-style: s\
+olid;\x0d\x0a}\x0d\x0aQScrol\
+lBar::handle:hov\
+er {\x0d\x0a\x09backgroun\
+d-color: rgba(12\
+3, 123, 123, 210\
+);\x0d\x0a}\
 \x00\x00\x03\xf6\
 M\
 ediaPlayerBase Q\
 PushButton {\x0d\x0a  \
   background-col\
 or: transparent;\
 \x0d\x0a    border-wid\
@@ -1470,14 +1638,306 @@
 down-arrow, QDou\
 bleSpinBox::down\
 -arrow {\x0d\x0a\x09borde\
 r-image: url(:/(\
 Double)SpinBox_I\
 con/Icons/DownAr\
 row.png);\x0d\x0a}\
+\x00\x00\x09\x09\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00B\x00\x00\x00B\x08\x06\x00\x00\x00\xe3T\x00\xe8\
+\x00\x00\x00\x09pHYs\x00\x00.#\x00\x00.#\
+\x01x\xa5?v\x00\x00\x072iTXtXML\
+:com.adobe.xmp\x00\x00\
+\x00\x00\x00<?xpacket beg\
+in=\x22\xef\xbb\xbf\x22 id=\x22W5M\
+0MpCehiHzreSzNTc\
+zkc9d\x22?> <x:xmpm\
+eta xmlns:x=\x22ado\
+be:ns:meta/\x22 x:x\
+mptk=\x22Adobe XMP \
+Core 5.6-c145 79\
+.163499, 2018/08\
+/13-16:40:22    \
+    \x22> <rdf:RDF \
+xmlns:rdf=\x22http:\
+//www.w3.org/199\
+9/02/22-rdf-synt\
+ax-ns#\x22> <rdf:De\
+scription rdf:ab\
+out=\x22\x22 xmlns:xmp\
+=\x22http://ns.adob\
+e.com/xap/1.0/\x22 \
+xmlns:dc=\x22http:/\
+/purl.org/dc/ele\
+ments/1.1/\x22 xmln\
+s:photoshop=\x22htt\
+p://ns.adobe.com\
+/photoshop/1.0/\x22\
+ xmlns:xmpMM=\x22ht\
+tp://ns.adobe.co\
+m/xap/1.0/mm/\x22 x\
+mlns:stEvt=\x22http\
+://ns.adobe.com/\
+xap/1.0/sType/Re\
+sourceEvent#\x22 xm\
+p:CreatorTool=\x22A\
+dobe Photoshop C\
+C 2019 (Windows)\
+\x22 xmp:CreateDate\
+=\x222023-08-02T07:\
+57:31+08:00\x22 xmp\
+:ModifyDate=\x22202\
+4-04-11T09:01:12\
++08:00\x22 xmp:Meta\
+dataDate=\x222024-0\
+4-11T09:01:12+08\
+:00\x22 dc:format=\x22\
+image/png\x22 photo\
+shop:ColorMode=\x22\
+3\x22 photoshop:ICC\
+Profile=\x22sRGB IE\
+C61966-2.1\x22 xmpM\
+M:InstanceID=\x22xm\
+p.iid:6e5ae2d2-1\
+9d1-9743-97ec-b2\
+6dcb7372ee\x22 xmpM\
+M:DocumentID=\x22ad\
+obe:docid:photos\
+hop:82bd19bf-b85\
+9-3149-9b63-ac66\
+c1eca465\x22 xmpMM:\
+OriginalDocument\
+ID=\x22xmp.did:2171\
+225e-b130-1645-9\
+1d8-3d0a6f092812\
+\x22> <xmpMM:Histor\
+y> <rdf:Seq> <rd\
+f:li stEvt:actio\
+n=\x22created\x22 stEv\
+t:instanceID=\x22xm\
+p.iid:2171225e-b\
+130-1645-91d8-3d\
+0a6f092812\x22 stEv\
+t:when=\x222023-08-\
+02T07:57:31+08:0\
+0\x22 stEvt:softwar\
+eAgent=\x22Adobe Ph\
+otoshop CC 2019 \
+(Windows)\x22/> <rd\
+f:li stEvt:actio\
+n=\x22converted\x22 st\
+Evt:parameters=\x22\
+from application\
+/vnd.adobe.photo\
+shop to image/pn\
+g\x22/> <rdf:li stE\
+vt:action=\x22saved\
+\x22 stEvt:instance\
+ID=\x22xmp.iid:e60b\
+2233-459c-1843-b\
+df3-ac201bce0982\
+\x22 stEvt:when=\x2220\
+23-08-02T07:58:1\
+8+08:00\x22 stEvt:s\
+oftwareAgent=\x22Ad\
+obe Photoshop CC\
+ 2019 (Windows)\x22\
+ stEvt:changed=\x22\
+/\x22/> <rdf:li stE\
+vt:action=\x22saved\
+\x22 stEvt:instance\
+ID=\x22xmp.iid:6e5a\
+e2d2-19d1-9743-9\
+7ec-b26dcb7372ee\
+\x22 stEvt:when=\x2220\
+24-04-11T09:01:1\
+2+08:00\x22 stEvt:s\
+oftwareAgent=\x22Ad\
+obe Photoshop CC\
+ 2019 (Windows)\x22\
+ stEvt:changed=\x22\
+/\x22/> </rdf:Seq> \
+</xmpMM:History>\
+ </rdf:Descripti\
+on> </rdf:RDF> <\
+/x:xmpmeta> <?xp\
+acket end=\x22r\x22?>\xd6\
+\xc1YJ\x00\x00\x01}IDATx\x9c\xed\xdb;\
+R\xc3@\x10E\xd1+\x8a\xddy\x13\xa4\xac\x88\x94M\
+x}\x22\xe0%P\xb6\xa5\xf9t\xf7\xa8\xea\xdd\x94d\
+\xe6\x94-\xe3n\xd8\xf6}\xc7\xc1[\xf5\x01V\xc9\x10\
+\xca\x10\xca\x10\xca\x10\xca\x10\xca\x10\xca\x10\xca\x10\xca\x10\
+\xca\x10\xca\x10\xca\x10\xca\x10\xca\x10\xca\x10\xca\x10\xea\xfd\
+\xd9\x0f\xbe\xbe\xef\xffGW[\xf0Y\xa2\xfas\x8f\xcf\
+\x8f\xdb\xc3{\xb4\xbc\x22\xae8\xd3;}\xe6\xd6\xb7\xc6\
+\x950\x9a\xce\xda\xf3\x8c\xb8\x02F\xf3\x19{\x1f\x96+\
+ct\x9d\xed\x15\xc4\xd1\xc3qE\x8c\xa33=\xbd\xd3\
+\xd1+\xe2J\x18\xdd\x08p\xee\xadq\x05\x8c!\x048\
+\xff\x8cX\x19c\x18\x01\xda\x1e\x96+bLA\x80\xf6\
+O\x8d\x950\xa6!@\xdf\xc7\xe7\x0a\x18S\x11\xa0\xff\
+\xf7\x88J\x8c\xe9\x080\xf6\xed\xb3\x02#\x04\x01\xc6\xbf\
+\x86gb\x84!\xc0\x9cyD\x06F(\x02\xcc\x1b\xcc\
+Db\x84#\xc0\xdc\x09U\x04F\x0a\x02\xcc\x1f\xd5\xcd\
+\xc4HC\x80\x98\x99\xe5\x0c\x8cT\x04\x88\x1b\xde\x8e`\
+\xa4#@\xec\x14\xbb\x07\xa3\x04\x01\xe2\xc7\xf9-\x18e\
+\x08\x90\xb3\xd78\x83Q\x8a\x00y\x0b\x9e\x91\x8b\xa4\xec\
+S27]=\x17J[*e\xaf\xfcZ.\x96\xba\
+Y\xab\xd8}\x9e\xb9`\xfaz\xb1j\x09\xfc\xea\xa2%\
+;\xd6\xcam\xf8\xa3\x0b\x97-\x9a7\xff\xbf\xc6o\xfe\
+\xfb\x08e\x08e\x08e\x08e\x08e\x08e\x08e\x08\
+e\x08e\x08e\x08e\x08e\x08e\x08e\x08e\x08\
+e\x08\xf5\x03lL9\x83\x8c_\x1f\xe4\x00\x00\x00\x00\
+IEND\xaeB`\x82\
+\x00\x00\x08\xeb\
+\x89\
+PNG\x0d\x0a\x1a\x0a\x00\x00\x00\x0dIHDR\x00\
+\x00\x00B\x00\x00\x00B\x08\x06\x00\x00\x00\xe3T\x00\xe8\
+\x00\x00\x00\x09pHYs\x00\x00.#\x00\x00.#\
+\x01x\xa5?v\x00\x00\x072iTXtXML\
+:com.adobe.xmp\x00\x00\
+\x00\x00\x00<?xpacket beg\
+in=\x22\xef\xbb\xbf\x22 id=\x22W5M\
+0MpCehiHzreSzNTc\
+zkc9d\x22?> <x:xmpm\
+eta xmlns:x=\x22ado\
+be:ns:meta/\x22 x:x\
+mptk=\x22Adobe XMP \
+Core 5.6-c145 79\
+.163499, 2018/08\
+/13-16:40:22    \
+    \x22> <rdf:RDF \
+xmlns:rdf=\x22http:\
+//www.w3.org/199\
+9/02/22-rdf-synt\
+ax-ns#\x22> <rdf:De\
+scription rdf:ab\
+out=\x22\x22 xmlns:xmp\
+=\x22http://ns.adob\
+e.com/xap/1.0/\x22 \
+xmlns:dc=\x22http:/\
+/purl.org/dc/ele\
+ments/1.1/\x22 xmln\
+s:photoshop=\x22htt\
+p://ns.adobe.com\
+/photoshop/1.0/\x22\
+ xmlns:xmpMM=\x22ht\
+tp://ns.adobe.co\
+m/xap/1.0/mm/\x22 x\
+mlns:stEvt=\x22http\
+://ns.adobe.com/\
+xap/1.0/sType/Re\
+sourceEvent#\x22 xm\
+p:CreatorTool=\x22A\
+dobe Photoshop C\
+C 2019 (Windows)\
+\x22 xmp:CreateDate\
+=\x222023-11-03T16:\
+31:58+08:00\x22 xmp\
+:ModifyDate=\x22202\
+4-04-11T09:03:06\
++08:00\x22 xmp:Meta\
+dataDate=\x222024-0\
+4-11T09:03:06+08\
+:00\x22 dc:format=\x22\
+image/png\x22 photo\
+shop:ColorMode=\x22\
+3\x22 photoshop:ICC\
+Profile=\x22sRGB IE\
+C61966-2.1\x22 xmpM\
+M:InstanceID=\x22xm\
+p.iid:b2423aa1-5\
+138-de41-aa26-b3\
+2c134fa86d\x22 xmpM\
+M:DocumentID=\x22ad\
+obe:docid:photos\
+hop:67b9d921-412\
+d-a44a-86cb-6003\
+096e7b8e\x22 xmpMM:\
+OriginalDocument\
+ID=\x22xmp.did:21df\
+c6c4-f501-744b-8\
+7dd-5352a1652439\
+\x22> <xmpMM:Histor\
+y> <rdf:Seq> <rd\
+f:li stEvt:actio\
+n=\x22created\x22 stEv\
+t:instanceID=\x22xm\
+p.iid:21dfc6c4-f\
+501-744b-87dd-53\
+52a1652439\x22 stEv\
+t:when=\x222023-11-\
+03T16:31:58+08:0\
+0\x22 stEvt:softwar\
+eAgent=\x22Adobe Ph\
+otoshop CC 2019 \
+(Windows)\x22/> <rd\
+f:li stEvt:actio\
+n=\x22converted\x22 st\
+Evt:parameters=\x22\
+from application\
+/vnd.adobe.photo\
+shop to image/pn\
+g\x22/> <rdf:li stE\
+vt:action=\x22saved\
+\x22 stEvt:instance\
+ID=\x22xmp.iid:c334\
+6cfd-93c8-9d40-a\
+86d-42dd85e4a28f\
+\x22 stEvt:when=\x2220\
+23-11-03T16:33:0\
+6+08:00\x22 stEvt:s\
+oftwareAgent=\x22Ad\
+obe Photoshop CC\
+ 2019 (Windows)\x22\
+ stEvt:changed=\x22\
+/\x22/> <rdf:li stE\
+vt:action=\x22saved\
+\x22 stEvt:instance\
+ID=\x22xmp.iid:b242\
+3aa1-5138-de41-a\
+a26-b32c134fa86d\
+\x22 stEvt:when=\x2220\
+24-04-11T09:03:0\
+6+08:00\x22 stEvt:s\
+oftwareAgent=\x22Ad\
+obe Photoshop CC\
+ 2019 (Windows)\x22\
+ stEvt:changed=\x22\
+/\x22/> </rdf:Seq> \
+</xmpMM:History>\
+ </rdf:Descripti\
+on> </rdf:RDF> <\
+/x:xmpmeta> <?xp\
+acket end=\x22r\x22?>\x91\
+\xd9\x85\xff\x00\x00\x01_IDATx\x9c\xed\xdb\xc1\
+M\xc50\x10E\xd1\x1bDw4\xc1\x96\x8a\xd8\xd2\x04\
+\xf5\x85\x05^\xf2\xf57\xf6\xbc;b^\x01Vt\x14\
+{lgr\xdd\xf7\xcd\x04^\xd2\x0f`\xc9@\xac\x0c\
+\xc4\xca@\xac\x0c\xc4\xca\xeb\xae\x81>\xbf\xbe\xff*?\
+\xd7\xae\xf1\x1f\xe5\xe3\xfdm\xcb8\xa7\xdf\x886\xb5\xb9\
+bj\xb4\xc0\xa8Z#\xf4\x18;!\x9e\xad\x07j\x8c\
+\xddoD[\x8c\x13S\xa3%\xc6\xa95\xa2\x1d\xc6\xc9\
+\xc5\xb2\x15\xc6\xe9\xaa\xd1\x06\xa3\xa2|\xb6\xc0\xa8\xdaG\
+\xe81*\x0f]j\x8c\xea\xd3\xa7\x16#q\x0cWb\
+\xa4\xee#t\x18\xc9\x8b\x19\x15F\xfa\x86J\x83\x91\x86\
+\x00\x09\x86\x01\x02\x04\x18\x16\x08\x08c\x98  \x88a\
+\x83\x80\x10\x86\x11\x02\x02\x18V\x08(\xc60C@!\
+\x86\x1d\x02\x0a\xbe\x96A\x0f\x88\x92t\x80\xf8W;\xcb\
+Gy\x86\xb0m\xda\x98!\xca\x10\xc0\x0bQ\x8a\x00N\
+\x88r\x04\xf0AD\x10\xc0\x05\x11C\x00\x0fD\x14\x01\
+\x1c\x10q\x04\xc8C(\x10 \x0b\xa1A\x80\x1c\x84\x0a\
+\x012\x10:\x04\xa8\x87P\x22@-\x84\x16\x01<}\
+\x96Q\x04pt\xde\xc6\x11 \xdf\x8b\xad@\x80\xb3\x10\
+m\x10\xe0\x1cD+\x048\x03\xd1\x0e\x01\xf6C\xb4D\
+\x80\xbd\x10m\x11\xc0\xd3g\x19\x8f\xa1\xf3V\x91t/\
+\xb6&\xd7\xfc\x1b\xfe\x9b\xf4\x0d\x95&\x03\xb12\x10+\
+\x03\xb12\x10+? \xf1:\x7fc\xc8\x19\xfc\x00\x00\
+\x00\x00IEND\xaeB`\x82\
 \x00\x00\x01X\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 width=\x2216\
 \x22 height=\x2216\x22 fi\
 ll=\x22rgb(54, 45, \
@@ -2443,14 +2903,18 @@
 \x02$\xe0^\
 \x00C\
 \x00o\x00m\x00b\x00o\x00B\x00o\x00x\x00_\x00I\x00c\x00o\x00n\
 \x00\x05\
 \x00O\xa6S\
 \x00I\
 \x00c\x00o\x00n\x00s\
+\x00\x09\
+\x0b\xb3Q^\
+\x00T\
+\x00r\x00e\x00e\x00_\x00I\x00c\x00o\x00n\
 \x00\x03\
 \x00\x00V\x83\
 \x00Q\
 \x00S\x00S\
 \x00\x0c\
 \x0d\xcf;~\
 \x00T\
@@ -2507,14 +2971,18 @@
 \x0d\xa0/\xc3\
 \x00S\
 \x00c\x00r\x00o\x00l\x00l\x00A\x00r\x00e\x00a\x00.\x00q\x00s\x00s\
 \x00\x09\
 \x08\xbf\xfcC\
 \x00L\
 \x00a\x00b\x00e\x00l\x00.\x00q\x00s\x00s\
+\x00\x08\
+\x08\xb8S\xc3\
+\x00T\
+\x00r\x00e\x00e\x00.\x00q\x00s\x00s\
 \x00\x0a\
 \x0f\xcf\xbd\xa3\
 \x00P\
 \x00l\x00a\x00y\x00e\x00r\x00.\x00q\x00s\x00s\
 \x00\x0a\
 \x03S\x07\xa3\
 \x00D\
@@ -2523,14 +2991,18 @@
 \x09(\xecC\
 \x00T\
 \x00a\x00b\x00l\x00e\x00.\x00q\x00s\x00s\
 \x00\x0b\
 \x09\xdf\xb8\xe3\
 \x00S\
 \x00p\x00i\x00n\x00B\x00o\x00x\x00.\x00q\x00s\x00s\
+\x00\x0e\
+\x06\xd9PG\
+\x00R\
+\x00i\x00g\x00h\x00t\x00A\x00r\x00r\x00o\x00w\x00.\x00p\x00n\x00g\
 \x00\x08\
 \x02\x8cP'\
 \x00P\
 \x00l\x00a\x00y\x00.\x00s\x00v\x00g\
 \x00\x05\
 \x00[Z\xc7\
 \x00X\
@@ -2558,135 +3030,147 @@
 \x00\x0b\
 \x09\xd2\xc6g\
 \x00U\
 \x00p\x00A\x00r\x00r\x00o\x00w\x00.\x00p\x00n\x00g\
 "
 
 qt_resource_struct = b"\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x05\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x06\x00\x00\x00\x01\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x00v\x00\x02\x00\x00\x00\x01\x00\x00\x00&\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00^\x00\x02\x00\x00\x00\x01\x00\x00\x00\x22\
+\x00\x00\x00N\x00\x02\x00\x00\x00\x01\x00\x00\x00\x15\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00N\x00\x02\x00\x00\x00\x01\x00\x00\x00\x11\
+\x00\x00\x00.\x00\x02\x00\x00\x00\x01\x00\x00\x00\x12\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00.\x00\x02\x00\x00\x00\x01\x00\x00\x00\x0e\
+\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x0f\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x0b\
+\x00\x00\x00^\x00\x02\x00\x00\x00\x01\x00\x00\x00\x0c\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00j\x00\x02\x00\x00\x00\x01\x00\x00\x00\x06\
+\x00\x00\x00\x82\x00\x02\x00\x00\x00\x01\x00\x00\x00\x07\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00N\x00\x02\x00\x00\x00\x04\x00\x00\x00\x07\
+\x00\x00\x00N\x00\x02\x00\x00\x00\x04\x00\x00\x00\x08\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x0a\xd7\
+\x00\x00\x00\xe0\x00\x00\x00\x00\x00\x01\x00\x00\x0a\xd7\
 \x00\x00\x01\x8fK\xdfE\x9c\
-\x00\x00\x00\xa8\x00\x00\x00\x00\x00\x01\x00\x00\x09\x0d\
+\x00\x00\x00\xc0\x00\x00\x00\x00\x00\x01\x00\x00\x09\x0d\
 \x00\x00\x01\x8fK\xdf\xf1\xcd\
-\x00\x00\x00\xea\x00\x00\x00\x00\x00\x01\x00\x00\x13\xe0\
+\x00\x00\x01\x02\x00\x00\x00\x00\x00\x01\x00\x00\x13\xe0\
 \x00\x00\x01\x8e\xca\xac8 \
-\x00\x00\x00\x88\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x00\xa0\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
+\x00\x00\x01\x8e\xca\xacO\x90\
+\x00\x00\x00N\x00\x02\x00\x00\x00\x02\x00\x00\x00\x0d\
+\x00\x00\x00\x00\x00\x00\x00\x00\
+\x00\x00\x02\x90\x00\x00\x00\x00\x00\x01\x00\x00k\x10\
+\x00\x00\x01\x8e\xca\xae\x0c\xe0\
+\x00\x00\x00\xa0\x00\x00\x00\x00\x00\x01\x00\x00b\x03\
 \x00\x00\x01\x8e\xca\xacO\x90\
-\x00\x00\x00N\x00\x02\x00\x00\x00\x02\x00\x00\x00\x0c\
+\x00\x00\x00N\x00\x02\x00\x00\x00\x02\x00\x00\x00\x10\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x03\x1c\x00\x00\x00\x00\x00\x01\x00\x00\x88\x18\
+\x00\x00\x03l\x00\x00\x00\x00\x00\x01\x00\x00\xa4E\
 \x00\x00\x01\x8e\xca\xad9\xf0\
-\x00\x00\x00\x88\x00\x00\x00\x00\x00\x01\x00\x00\x7f\x0b\
+\x00\x00\x00\xa0\x00\x00\x00\x00\x00\x01\x00\x00\x9b8\
 \x00\x00\x01\x8e\xca\xacO\x90\
-\x00\x00\x00N\x00\x02\x00\x00\x00\x02\x00\x00\x00\x0f\
+\x00\x00\x00N\x00\x02\x00\x00\x00\x02\x00\x00\x00\x13\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x03\x1c\x00\x00\x00\x00\x00\x01\x00\x00v\x02\
+\x00\x00\x03l\x00\x00\x00\x00\x00\x01\x00\x00\x92/\
 \x00\x00\x01\x8e\xca\xad9\xf0\
-\x00\x00\x00\x88\x00\x00\x00\x00\x00\x01\x00\x00l\xf5\
+\x00\x00\x00\xa0\x00\x00\x00\x00\x00\x01\x00\x00\x89\x22\
 \x00\x00\x01\x8e\xca\xacO\x90\
-\x00\x00\x00N\x00\x02\x00\x00\x00\x02\x00\x00\x00\x12\
+\x00\x00\x00N\x00\x02\x00\x00\x00\x02\x00\x00\x00\x16\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\x0a\x00\x02\x00\x00\x00\x07\x00\x00\x00\x1b\
+\x00\x00\x01\x22\x00\x02\x00\x00\x00\x07\x00\x00\x00\x1f\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\x18\x00\x02\x00\x00\x00\x07\x00\x00\x00\x14\
+\x00\x00\x010\x00\x02\x00\x00\x00\x07\x00\x00\x00\x18\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x02x\x00\x00\x00\x00\x00\x01\x00\x00Y.\
+\x00\x00\x02\xc8\x00\x00\x00\x00\x00\x01\x00\x00u[\
 \x00\x00\x01\x8f>\x86Q\xd3\
-\x00\x00\x02b\x00\x00\x00\x00\x00\x01\x00\x00W\xd2\
+\x00\x00\x02\xb2\x00\x00\x00\x00\x00\x01\x00\x00s\xff\
 \x00\x00\x01\x8f>\x87\xf7h\
-\x00\x00\x02\xdc\x00\x00\x00\x00\x00\x01\x00\x00_#\
+\x00\x00\x03,\x00\x00\x00\x00\x00\x01\x00\x00{P\
 \x00\x00\x01\x8f\x04\xb5\x94\x80\
-\x00\x00\x02\x88\x00\x00\x00\x00\x00\x01\x00\x00Zi\
+\x00\x00\x02\xd8\x00\x00\x00\x00\x00\x01\x00\x00v\x96\
 \x00\x00\x01\x8f>\x87\xe3:\
-\x00\x00\x02\xfa\x00\x00\x00\x00\x00\x01\x00\x00`:\
+\x00\x00\x03J\x00\x00\x00\x00\x00\x01\x00\x00|g\
 \x00\x00\x01\x8f>\x86\xa2\x90\
-\x00\x00\x02\xc6\x00\x00\x00\x00\x00\x01\x00\x00^;\
+\x00\x00\x03\x16\x00\x00\x00\x00\x00\x01\x00\x00zh\
 \x00\x00\x01\x8f>\x86\xc1v\
-\x00\x00\x02\xae\x00\x00\x00\x00\x00\x01\x00\x00\x5c\xdb\
+\x00\x00\x02\xfe\x00\x00\x00\x00\x00\x01\x00\x00y\x08\
 \x00\x00\x01\x8f>\x87\xeb#\
-\x00\x00\x02x\x00\x00\x00\x00\x00\x01\x00\x00c\xb8\
+\x00\x00\x02\xc8\x00\x00\x00\x00\x00\x01\x00\x00\x7f\xe5\
 \x00\x00\x01\x8f9\x0d\xd2\xe4\
-\x00\x00\x02b\x00\x00\x00\x00\x00\x01\x00\x00bY\
+\x00\x00\x02\xb2\x00\x00\x00\x00\x00\x01\x00\x00~\x86\
 \x00\x00\x01\x8f>\x87\x9fd\
-\x00\x00\x02\xdc\x00\x00\x00\x00\x00\x01\x00\x00i\xb9\
+\x00\x00\x03,\x00\x00\x00\x00\x00\x01\x00\x00\x85\xe6\
 \x00\x00\x01\x8f\x04\xb5u@\
-\x00\x00\x02\x88\x00\x00\x00\x00\x00\x01\x00\x00d\xf6\
+\x00\x00\x02\xd8\x00\x00\x00\x00\x00\x01\x00\x00\x81#\
 \x00\x00\x01\x8f>\x87\x8b\xbb\
-\x00\x00\x02\xfa\x00\x00\x00\x00\x00\x01\x00\x00j\xd3\
+\x00\x00\x03J\x00\x00\x00\x00\x00\x01\x00\x00\x87\x00\
 \x00\x00\x01\x8f9\x0d\xba\x13\
-\x00\x00\x02\xc6\x00\x00\x00\x00\x00\x01\x00\x00h\xce\
+\x00\x00\x03\x16\x00\x00\x00\x00\x00\x01\x00\x00\x84\xfb\
 \x00\x00\x01\x8f9\x0d\xa5\xc5\
-\x00\x00\x02\xae\x00\x00\x00\x00\x00\x01\x00\x00gk\
+\x00\x00\x02\xfe\x00\x00\x00\x00\x00\x01\x00\x00\x83\x98\
 \x00\x00\x01\x8f>\x87\x95\xc9\
-\x00\x00\x00^\x00\x02\x00\x00\x00\x02\x00\x00\x00#\
+\x00\x00\x00v\x00\x02\x00\x00\x00\x02\x00\x00\x00'\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\x0a\x00\x02\x00\x00\x00\x0c\x00\x00\x001\
+\x00\x00\x01\x22\x00\x02\x00\x00\x00\x0d\x00\x00\x006\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\x18\x00\x02\x00\x00\x00\x0c\x00\x00\x00%\
+\x00\x00\x010\x00\x02\x00\x00\x00\x0d\x00\x00\x00)\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\xa2\x00\x01\x00\x00\x00\x01\x00\x00'\x83\
+\x00\x00\x01\xba\x00\x01\x00\x00\x00\x01\x00\x00'\x83\
 \x00\x00\x01\x8e\xfe\x80\xfc\xd0\
-\x00\x00\x02\x14\x00\x00\x00\x00\x00\x01\x00\x001\xe6\
+\x00\x00\x02B\x00\x00\x00\x00\x00\x01\x00\x006\xfd\
 \x00\x00\x01\x8f\x15#{p\
-\x00\x00\x01B\x00\x00\x00\x00\x00\x01\x00\x00\x1f\xee\
+\x00\x00\x01Z\x00\x00\x00\x00\x00\x01\x00\x00\x1f\xee\
 \x00\x00\x01\x8e\xb2\xe6_\x90\
-\x00\x00\x01\xe2\x00\x00\x00\x00\x00\x01\x00\x00-\x0c\
+\x00\x00\x02\x12\x00\x00\x00\x00\x00\x01\x00\x00-\xfe\
+\x00\x00\x01\x8f\x9fN\xec\xe6\
+\x00\x00\x01\xfa\x00\x00\x00\x00\x00\x01\x00\x00-\x0c\
 \x00\x00\x01\x8f\x14+\x9eP\
-\x00\x00\x02.\x00\x01\x00\x00\x00\x01\x00\x004g\
+\x00\x00\x02\x5c\x00\x01\x00\x00\x00\x01\x00\x009~\
 \x00\x00\x01\x8e\xcdo\x9d\xe0\
-\x00\x00\x01V\x00\x00\x00\x00\x00\x01\x00\x00!\x07\
+\x00\x00\x01n\x00\x00\x00\x00\x00\x01\x00\x00!\x07\
 \x00\x00\x01\x8fW\xbb>\xb7\
-\x00\x00\x02F\x00\x00\x00\x00\x00\x01\x00\x006#\
+\x00\x00\x02t\x00\x00\x00\x00\x00\x01\x00\x00;:\
 \x00\x00\x01\x8e\xfe\x81;P\
-\x00\x00\x01\x8c\x00\x00\x00\x00\x00\x01\x00\x00$\xca\
+\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00$\xca\
 \x00\x00\x01\x8fW\x1d\x9d\xf9\
-\x00\x00\x01r\x00\x00\x00\x00\x00\x01\x00\x00#D\
+\x00\x00\x01\x8a\x00\x00\x00\x00\x00\x01\x00\x00#D\
 \x00\x00\x01\x8e\xfe\x8c\xeb\x80\
-\x00\x00\x01(\x00\x00\x00\x00\x00\x01\x00\x00\x1c\xc1\
+\x00\x00\x01@\x00\x00\x00\x00\x00\x01\x00\x00\x1c\xc1\
 \x00\x00\x01\x8fA\xc8+\xf8\
-\x00\x00\x01\xc0\x00\x00\x00\x00\x00\x01\x00\x00)\xa3\
+\x00\x00\x01\xd8\x00\x00\x00\x00\x00\x01\x00\x00)\xa3\
 \x00\x00\x01\x8e\xd7\x95e \
-\x00\x00\x01\xfa\x00\x00\x00\x00\x00\x01\x00\x00-\xfe\
+\x00\x00\x02(\x00\x00\x00\x00\x00\x01\x00\x003\x15\
 \x00\x00\x01\x8e\xb2\xe6\x86\xa0\
-\x00\x00\x01\xa2\x00\x01\x00\x00\x00\x01\x00\x00E\x0e\
+\x00\x00\x01\xba\x00\x01\x00\x00\x00\x01\x00\x00J%\
 \x00\x00\x01\x8e\xfe\x81\x99\x10\
-\x00\x00\x02\x14\x00\x00\x00\x00\x00\x01\x00\x00Oy\
+\x00\x00\x02B\x00\x00\x00\x00\x00\x01\x00\x00Y\xaa\
 \x00\x00\x01\x8f\x15#T`\
-\x00\x00\x01B\x00\x00\x00\x00\x00\x01\x00\x00=d\
+\x00\x00\x01Z\x00\x00\x00\x00\x00\x01\x00\x00B{\
 \x00\x00\x01\x8cC\x9b+\xe0\
-\x00\x00\x01\xe2\x00\x00\x00\x00\x00\x01\x00\x00J\x8a\
+\x00\x00\x02\x12\x00\x00\x00\x00\x00\x01\x00\x00P\x96\
+\x00\x00\x01\x8f\x9fN\xec\xe6\
+\x00\x00\x01\xfa\x00\x00\x00\x00\x00\x01\x00\x00O\xa1\
 \x00\x00\x01\x8f\x14-k@\
-\x00\x00\x02.\x00\x01\x00\x00\x00\x01\x00\x00Q\xfd\
+\x00\x00\x02\x5c\x00\x01\x00\x00\x00\x01\x00\x00\x5c.\
 \x00\x00\x01\x8e\xd7\x97\x12\xd0\
-\x00\x00\x01V\x00\x00\x00\x00\x00\x01\x00\x00>\x80\
+\x00\x00\x01n\x00\x00\x00\x00\x00\x01\x00\x00C\x97\
 \x00\x00\x01\x8fW\xbb\xcb0\
-\x00\x00\x02F\x00\x00\x00\x00\x00\x01\x00\x00S\xc1\
+\x00\x00\x02t\x00\x00\x00\x00\x00\x01\x00\x00]\xf2\
 \x00\x00\x01\x8e\xfe\x81r\x00\
-\x00\x00\x01\x8c\x00\x00\x00\x00\x00\x01\x00\x00BI\
+\x00\x00\x01\xa4\x00\x00\x00\x00\x00\x01\x00\x00G`\
 \x00\x00\x01\x8fW\x1d\xae\xe1\
-\x00\x00\x01r\x00\x00\x00\x00\x00\x01\x00\x00@\xc3\
+\x00\x00\x01\x8a\x00\x00\x00\x00\x00\x01\x00\x00E\xda\
 \x00\x00\x01\x8f4\x12\xb0C\
-\x00\x00\x01(\x00\x00\x00\x00\x00\x01\x00\x00:.\
+\x00\x00\x01@\x00\x00\x00\x00\x00\x01\x00\x00?E\
 \x00\x00\x01\x8fA\xc8D \
-\x00\x00\x01\xc0\x00\x00\x00\x00\x00\x01\x00\x00G'\
+\x00\x00\x01\xd8\x00\x00\x00\x00\x00\x01\x00\x00L>\
 \x00\x00\x01\x8e\xd7\x97\x12\xd0\
-\x00\x00\x01\xfa\x00\x00\x00\x00\x00\x01\x00\x00K\x7f\
+\x00\x00\x02(\x00\x00\x00\x00\x00\x01\x00\x00U\xb0\
 \x00\x00\x01\x8dg\xd5\xfe0\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
```

### Comparing `QEasyWidgets-0.1.9/QEasyWidgets/Utils.py` & `QEasyWidgets-0.2.0/QEasyWidgets/Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import io
 import shutil
 import psutil
 import signal
 import shlex
 import subprocess
 import collections
+import inspect
 import hashlib
 import urllib
 import platform
 import win32gui
 import win32con
 import win32api
 import win32print
@@ -391,14 +392,24 @@
     URLList = re.compile(r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+').findall(RawString(String))
     URL = URLList[0]
 
     return URL
 
 #############################################################################################################
 
+def GetClassFromMethod(Method):
+    '''
+    Modules = list(inspect.getmodule(Method).__dict__.values())
+    Modules = [Module for Module in Modules if str(Module).startswith("<class '__main__.")]
+    return Modules[-1]
+    '''
+    return inspect.getmodule(Method).__dict__[Method.__qualname__.split('.')[0]]
+
+#############################################################################################################
+
 def RunEvents(
     Events: Union[list, dict]
 ):
     '''
     '''
     if isinstance(Events, list):
         for Event in Events:
```

### Comparing `QEasyWidgets-0.1.9/QEasyWidgets/WindowCustomizer.py` & `QEasyWidgets-0.2.0/QEasyWidgets/WindowCustomizer.py`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.9/QEasyWidgets.egg-info/PKG-INFO` & `QEasyWidgets-0.2.0/QEasyWidgets.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 Metadata-Version: 2.1
 Name: QEasyWidgets
-Version: 0.1.9
+Version: 0.2.0
 Summary: A simple widget library based on PySide6
 Home-page: https://github.com/Spr-Aachen/QEasyWidgets
 Author: Spr_Aachen
 Author-email: 2835946988@qq.com
 License: GPLv3
 Project-URL: Source Code, https://github.com/Spr-Aachen/QEasyWidgets
 Project-URL: Bug Tracker, https://github.com/Spr-Aachen/QEasyWidgets/issues
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: PySide6
-Requires-Dist: darkdetect
-Requires-Dist: tqdm
-Requires-Dist: psutil
-Requires-Dist: nvidia-ml-py
-Requires-Dist: PyGithub
 
 <div align = "center">
 
 # QEasyWidgets
 
 [![Releases](https://img.shields.io/github/v/release/Spr-Aachen/QEasyWidgets?color=green&label=Release&logo=Github&logoColor=white&style=for-the-badge)](https://github.com/Spr-Aachen/QEasyWidgets/releases/latest)&nbsp;
```

### Comparing `QEasyWidgets-0.1.9/README.md` & `QEasyWidgets-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `QEasyWidgets-0.1.9/setup.py` & `QEasyWidgets-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open('./README.md', encoding = 'utf-8') as f:
     LongDescription = f.read()
 
 ##############################################################################################################################
 
 setup(
     name = "QEasyWidgets",
-    version = '0.1.9',
+    version = '0.2.0',
     description = 'A simple widget library based on PySide6',
     long_description = LongDescription,
     long_description_content_type = 'text/markdown',
     license = 'GPLv3',
     author = "Spr_Aachen",
     author_email = '2835946988@qq.com',
     url = 'https://github.com/Spr-Aachen/QEasyWidgets',
```

