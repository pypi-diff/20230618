# Comparing `tmp/conlay-1.0.5.tar.gz` & `tmp/conlay-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conlay-1.0.5.tar", last modified: Sun Jun 11 18:08:53 2023, max compression
+gzip compressed data, was "conlay-1.1.0.tar", last modified: Sun Jun 18 14:18:03 2023, max compression
```

## Comparing `conlay-1.0.5.tar` & `conlay-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 18:08:53.559387 conlay-1.0.5/
--rw-rw-rw-   0        0        0     1085 2023-06-09 13:08:51.000000 conlay-1.0.5/LICENSE
--rw-rw-rw-   0        0        0    22904 2023-06-11 18:08:53.557662 conlay-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    22599 2023-06-11 17:05:41.000000 conlay-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 18:08:53.549660 conlay-1.0.5/conlay/
--rw-rw-rw-   0        0        0       19 2023-06-09 13:59:21.000000 conlay-1.0.5/conlay/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-06-11 16:52:38.000000 conlay-1.0.5/conlay/main.py
-drwxrwxrwx   0        0        0        0 2023-06-11 18:08:53.556161 conlay-1.0.5/conlay.egg-info/
--rw-rw-rw-   0        0        0    22904 2023-06-11 18:08:53.000000 conlay-1.0.5/conlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-06-11 18:08:53.000000 conlay-1.0.5/conlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 18:08:53.000000 conlay-1.0.5/conlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 18:08:53.000000 conlay-1.0.5/conlay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 18:08:53.559387 conlay-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-06-11 18:08:20.000000 conlay-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-18 14:18:03.126436 conlay-1.1.0/
+-rw-rw-rw-   0        0        0     1085 2023-06-09 13:08:51.000000 conlay-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0    26811 2023-06-18 14:18:03.124436 conlay-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    26506 2023-06-18 14:05:35.000000 conlay-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-18 14:18:03.115934 conlay-1.1.0/conlay/
+-rw-rw-rw-   0        0        0       19 2023-06-09 13:59:21.000000 conlay-1.1.0/conlay/__init__.py
+-rw-rw-rw-   0        0        0    13949 2023-06-18 14:07:43.000000 conlay-1.1.0/conlay/main.py
+drwxrwxrwx   0        0        0        0 2023-06-18 14:18:03.122935 conlay-1.1.0/conlay.egg-info/
+-rw-rw-rw-   0        0        0    26811 2023-06-18 14:18:02.000000 conlay-1.1.0/conlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-06-18 14:18:03.000000 conlay-1.1.0/conlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-18 14:18:02.000000 conlay-1.1.0/conlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-18 14:18:02.000000 conlay-1.1.0/conlay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-18 14:18:03.126436 conlay-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-06-18 14:16:18.000000 conlay-1.1.0/setup.py
```

### Comparing `conlay-1.0.5/LICENSE` & `conlay-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conlay-1.0.5/PKG-INFO` & `conlay-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: conlay
-Version: 1.0.5
-Summary: A python library for creating nice layouts in the console environment
-Home-page: https://github.com/Salliii/conlay
-Author: Salliii
-Keywords: python,library,console,layout
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Conlay - Console Layout
 [![PyPi version][shields-pypi_version]][url-pypi_version]
 [![Github Issues][shields-issues]][url-issues]
 [![Github License][shields-license]][url-license]
 
 Create visually pleasing console layouts with this easy-to-use Python library. 
 
@@ -66,34 +56,37 @@
 
 ```python
 layout = Conlay()
 ```
 
 There are some attributes that can be used to modify or update the positioning, scale, color and other things. Because each <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a> is a subclass of `Conlay()`, each <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a> has the same attributes.
 
-| attribute        | description | expected type | default value |
-| :--------        | :---------- | :------------ | :------------ |
-| `relative_x`       | Relative x-position to the parent object | `int` | 0 |
-| `relative_y`       | Relative y-position to the parent object | `int` | 0 |
-| `absolute_x`       | Absolute x-position | `int` | 0 |
-| `absolute_y`       | Absolute y-position | `int` | 0 |
-| `width`            | Elements width | `int` | 0 |
-| `min_width`        | Minimal width. May limit the specified with | `int` | 0 |
-| `max_width`        | Maximal width. May limit the specified with | `int` | 0 |
-| `height`           | Elements height | `int` | 0 |
-| `min_height`       | Minimal height. May limit the specified with | `int` | 0 |
-| `max_height`       | Maximal height. May limit the specified with | `int` | 0 |
-| `zindex`           | Indicates whether an element is printed above or below other elements | `int` | 0 |
-| `padding_x`        | Specifies the padding on the x axis, which affects the absolute position of the child elements | `int` | 0 |
-| `padding_y`        | Specifies the padding on the y axis, which affects the absolute position of the child elements | `int` | 0 |
-| `text`             | Specifies the text content | `str` | n/a |
-| `background`       | Specifies whether the element should have a background or not | `bool` | False |
-| `background_color` | Specifies the background color | <a href="https://github.com/Salliii/conlay#colorbg">`Color.Bg`</a> | Color.Bg.clear |
-| `border_color`     | Specifies the border color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
-| `text_color`       | Specifies the text color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
+| attribute           | description | expected type | default value |
+| :--------           | :---------- | :------------ | :------------ |
+| `relative_x`        | Relative x-position to the parent object | `int` | 0 |
+| `relative_y`        | Relative y-position to the parent object | `int` | 0 |
+| `absolute_x`        | Absolute x-position | `int` | 0 |
+| `absolute_y`        | Absolute y-position | `int` | 0 |
+| `width`             | Elements width | `int` | 0 |
+| `min_width`         | Minimal width. May limit the specified with | `int` | 0 |
+| `max_width`         | Maximal width. May limit the specified with | `int` | 0 |
+| `height`            | Elements height | `int` | 0 |
+| `min_height`        | Minimal height. May limit the specified with | `int` | 0 |
+| `max_height`        | Maximal height. May limit the specified with | `int` | 0 |
+| `zindex`            | Indicates whether an element is printed above or below other elements | `int` | 0 |
+| `padding_x`         | Specifies the padding on the x axis, which affects the absolute position of the child elements | `int` | 0 |
+| `padding_y`         | Specifies the padding on the y axis, which affects the absolute position of the child elements | `int` | 0 |
+| `text`              | Specifies the text content | `str` | n/a |
+| `placeholder`       | Specifies the placeholder content | `str` | n/a |
+| `content`           | Stores the text content of the input element, etc. | `str` | n/a |
+| `background`        | Specifies whether the element should have a background or not | `bool` | False |
+| `background_color`  | Specifies the background color | <a href="https://github.com/Salliii/conlay#colorbg">`Color.Bg`</a> | Color.Bg.clear |
+| `border_color`      | Specifies the border color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
+| `text_color`        | Specifies the text color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
+| `placeholder_color` | Specifies the placeholder color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.rgb(150, 150, 150) |
 
 
 ### Conlay.add()
 You can use `add()` to add <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElements</a> to other <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElements</a>.
 
 Syntax:
 
@@ -436,14 +429,153 @@
 
 >
 ```
 
 
 
 
+## Input()
+The `Input()` class is a subclass of the <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a> class and is used to create a input field.
+
+Syntax:
+
+```python
+element = Input(x, y, text, length, border)
+```
+
+| argument | description | expected type |
+| :------- | :---------- | :------------ |
+| `x`      | Relative x-position to its parent element | `int` |
+| `y`      | Relative y-position to its parent element | `int` |
+| `text`   | Text content | `str` |
+| `length` | expected input length | `int` |
+| `border` | Borders character set | <a href="https://github.com/Salliii/conlay#border">Border()</a> or one of its subclasses such as <a href="https://github.com/Salliii/conlay#bold">Bold()</a> or <a href="https://github.com/Salliii/conlay#thin">Thin()</a> |
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = Input(0, 0, "input:", 10, Thin())
+layout.add(input_element)
+
+layout.print()
+```
+
+Console output:
+
+```
+╭────────────────╮
+│input:          │
+╰────────────────╯
+
+
+>
+```
+
+after you've entered a text, you can get it with the element.content variable
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = Input(0, 0, "input:", 10, Thin())
+layout.add(input_element)
+
+layout.print()
+
+print(input_element.content)
+```
+
+
+
+
+## ThinInput()
+The `ThinInput()` class is a subclass of the <a href="https://github.com/Salliii/conlay#input">Input()</a> class and is used to create a simple input field with a <a href="https://github.com/Salliii/conlay#thin">Thin()</a> Border.
+
+Syntax:
+
+```python
+element = ThinInput(x, y, text, length)
+```
+
+| argument | description | expected type |
+| :------- | :---------- | :------------ |
+| `x`      | Relative x-position to its parent element | `int` |
+| `y`      | Relative y-position to its parent element | `int` |
+| `text`   | Text content | `str` |
+| `length` | expected input length | `int` |
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = ThinInput(0, 0, "input:", 10)
+layout.add(input_element)
+
+layout.print()
+```
+
+Console output:
+
+```
+╭────────────────╮
+│input:          │
+╰────────────────╯
+
+
+>
+```
+
+
+
+
+## BoldInput()
+The `BoldInput()` class is a subclass of the <a href="https://github.com/Salliii/conlay#input">Input()</a> class and is used to create a simple input field with a <a href="https://github.com/Salliii/conlay#bold">Bold()</a> Border.
+
+Syntax:
+
+```python
+element = BoldInput(x, y, text, length)
+```
+
+| argument | description | expected type |
+| :------- | :---------- | :------------ |
+| `x`      | Relative x-position to its parent element | `int` |
+| `y`      | Relative y-position to its parent element | `int` |
+| `text`   | Text content | `str` |
+| `length` | expected input length | `int` |
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = BoldInput(0, 0, "input:", 10)
+layout.add(input_element)
+
+layout.print()
+```
+
+Console output:
+
+```
+┏━━━━━━━━━━━━━━━━┓
+┃input:          ┃
+┗━━━━━━━━━━━━━━━━┛
+
+
+>
+```
+
+
+
+
 ## Cursor
 The `Cursor` class provides a few functions for simple <a href="https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797">Ansi Escape</a> cursor actions.
 
 
 ### Cursor.setPosition()
 Set the cursor to a specific position. The <a href="https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797">Ansi Escape Sequence</a> used for this command is `\x1b[<y>;<x>H`.
 
@@ -705,14 +837,17 @@
 - <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a>
 - <a href="https://github.com/Salliii/conlay#box">Box()</a>
 - <a href="https://github.com/Salliii/conlay#thinbox">ThinBox()</a>
 - <a href="https://github.com/Salliii/conlay#boldbox">BoldBox()</a>
 - <a href="https://github.com/Salliii/conlay#label">Label()</a>
 - <a href="https://github.com/Salliii/conlay#thinlabel">ThinLabel()</a>
 - <a href="https://github.com/Salliii/conlay#boldlabel">BoldLabel()</a>
+- <a href="https://github.com/Salliii/conlay#input">Input()</a>
+- <a href="https://github.com/Salliii/conlay#thininput">ThinInput()</a>
+- <a href="https://github.com/Salliii/conlay#boldinput">BoldInput()</a>
 
 ##### Cursor & Console
 - <a href="https://github.com/Salliii/conlay#cursor">Cursor</a>
   - <a href="https://github.com/Salliii/conlay#cursorsetposition">_setPosition()_</a>
   - <a href="https://github.com/Salliii/conlay#cursorshifthorizontal">_shiftHorizontal()_</a>
   - <a href="https://github.com/Salliii/conlay#cursorshiftvertical">_shiftVertical()_</a>
   - <a href="https://github.com/Salliii/conlay#cursorhide">_hide()_</a>
@@ -749,8 +884,8 @@
 [shields-pypi_version]: https://img.shields.io/pypi/v/conlay?label=PyPi%20Version&style=for-the-badge
 [shields-issues]: https://img.shields.io/github/issues/Salliii/conlay?style=for-the-badge
 [shields-license]: https://img.shields.io/github/license/Salliii/conlay?style=for-the-badge
 
 <!-- url -->
 [url-pypi_version]: https://pypi.org/project/conlay/
 [url-issues]: https://github.com/Salliii/conlay/issues
-[url-license]: https://github.com/Salliii/conlay/blob/main/LICENSE
+[url-license]: https://github.com/Salliii/conlay/blob/main/LICENSE
```

#### html2text {}

```diff
@@ -1,19 +1,15 @@
-Metadata-Version: 2.1 Name: conlay Version: 1.0.5 Summary: A python library for
-creating nice layouts in the console environment Home-page: https://github.com/
-Salliii/conlay Author: Salliii Keywords: python,library,console,layout
-Description-Content-Type: text/markdown License-File: LICENSE # Conlay -
-Console Layout [![PyPi version][shields-pypi_version]][url-pypi_version] [!
-[Github Issues][shields-issues]][url-issues] [![Github License][shields-
-license]][url-license] Create visually pleasing console layouts with this easy-
-to-use Python library. ## Installing Install using pip ```bash pip install
-conlay ``` or install it from PyPi ## Example ```python from conlay import *
-layout = Conlay() blank_box = BoldBox(0, 0, 30, 5) layout.add(blank_box) label
-= ThinLabel(0, 0, "this is a test") blank_box.add(label) layout.print() ```
-Console output: ```
+# Conlay - Console Layout [![PyPi version][shields-pypi_version]][url-
+pypi_version] [![Github Issues][shields-issues]][url-issues] [![Github License]
+[shields-license]][url-license] Create visually pleasing console layouts with
+this easy-to-use Python library. ## Installing Install using pip ```bash pip
+install conlay ``` or install it from PyPi ## Example ```python from conlay
+import * layout = Conlay() blank_box = BoldBox(0, 0, 30, 5) layout.add
+(blank_box) label = ThinLabel(0, 0, "this is a test") blank_box.add(label)
+layout.print() ``` Console output: ```
 ââââââââââââââââââââââââââââââ
 ââ­âââââââââââââââ® â ââthis is a testâ
 â ââ°âââââââââââââââ¯ â
 ââââââââââââââââââââââââââââââ
 > ``` ## Conlay() `Conlay()` is the core class within the library. It generates
 and prints out the layout. ```python layout = Conlay() ``` There are some
 attributes that can be used to modify or update the positioning, scale, color
@@ -29,38 +25,41 @@
 height | `int` | 0 | | `min_height` | Minimal height. May limit the specified
 with | `int` | 0 | | `max_height` | Maximal height. May limit the specified
 with | `int` | 0 | | `zindex` | Indicates whether an element is printed above
 or below other elements | `int` | 0 | | `padding_x` | Specifies the padding on
 the x axis, which affects the absolute position of the child elements | `int` |
 0 | | `padding_y` | Specifies the padding on the y axis, which affects the
 absolute position of the child elements | `int` | 0 | | `text` | Specifies the
-text content | `str` | n/a | | `background` | Specifies whether the element
+text content | `str` | n/a | | `placeholder` | Specifies the placeholder
+content | `str` | n/a | | `content` | Stores the text content of the input
+element, etc. | `str` | n/a | | `background` | Specifies whether the element
 should have a background or not | `bool` | False | | `background_color` |
 Specifies the background color | `Color.Bg` | Color.Bg.clear | | `border_color`
 | Specifies the border color | `Color.Fg` | Color.Fg.clear | | `text_color` |
-Specifies the text color | `Color.Fg` | Color.Fg.clear | ### Conlay.add() You
-can use `add()` to add LayoutElements to other LayoutElements. Syntax:
-```python parent.add(child) ``` | argument | description | expected type | | :-
------- | :---------- | :------------ | | `child` | child element |
-LayoutElements() or one of its subclasses such as Box(), Label(), etc. |
-Example: ```python # add a LayoutElement to the main layout layout = Conlay()
-layout.add(ThinBox(...)) # add a LayoutElement to another LayoutElement BoldBox
-(...).add(ThinLabel(...)) ``` ### Conlay.print() You have to call `print()` to
-generate and print out the layout. Syntax: ```python layout.print() ```
-Example: ```python layout = Conlay() ... layout.print() ``` ## LayoutElement()
-The `LayoutElement()` class serves as a superclass for all other layout
-elements such as Box(), Label(), etc. Syntax: ```python element = LayoutElement
-(x, y, w, h, border) ``` | argument | description | expected type | | :------
-- | :---------- | :------------ | | `x` | Relative x-position to its parent
-element | `int` | | `y` | Relative y-position to its parent element | `int` | |
-`w` | Elements width | `int` | | `h` | Elements height | `int` | | `border` |
-Borders character set | Border() or one of its subclasses such as Bold() or
-Thin() | Example: ```python from conlay import * layout = Conlay() element =
-LayoutElement(0, 0, 30, 5, Thin()) layout.add(element) layout.print() ```
-Console output: ```
+Specifies the text color | `Color.Fg` | Color.Fg.clear | | `placeholder_color`
+| Specifies the placeholder color | `Color.Fg` | Color.Fg.rgb(150, 150, 150) |
+### Conlay.add() You can use `add()` to add LayoutElements to other
+LayoutElements. Syntax: ```python parent.add(child) ``` | argument |
+description | expected type | | :------- | :---------- | :------------ | |
+`child` | child element | LayoutElements() or one of its subclasses such as Box
+(), Label(), etc. | Example: ```python # add a LayoutElement to the main layout
+layout = Conlay() layout.add(ThinBox(...)) # add a LayoutElement to another
+LayoutElement BoldBox(...).add(ThinLabel(...)) ``` ### Conlay.print() You have
+to call `print()` to generate and print out the layout. Syntax: ```python
+layout.print() ``` Example: ```python layout = Conlay() ... layout.print() ```
+## LayoutElement() The `LayoutElement()` class serves as a superclass for all
+other layout elements such as Box(), Label(), etc. Syntax: ```python element =
+LayoutElement(x, y, w, h, border) ``` | argument | description | expected type
+| | :------- | :---------- | :------------ | | `x` | Relative x-position to its
+parent element | `int` | | `y` | Relative y-position to its parent element |
+`int` | | `w` | Elements width | `int` | | `h` | Elements height | `int` | |
+`border` | Borders character set | Border() or one of its subclasses such as
+Bold() or Thin() | Example: ```python from conlay import * layout = Conlay()
+element = LayoutElement(0, 0, 30, 5, Thin()) layout.add(element) layout.print()
+``` Console output: ```
 â­âââââââââââââââââââââââââââââ®
 â â â â â â
 â°âââââââââââââââââââââââââââââ¯
 > ``` ## Box() The `Box()` class is a subclass of the LayoutElement() class and
 is used to create a simple box. Syntax: ```python element = Box(x, y, w, h,
 border) ``` | argument | description | expected type | | :------- | :---------
 - | :------------ | | `x` | Relative x-position to its parent element | `int` |
@@ -119,17 +118,52 @@
 BoldLabel(x, y, text) ``` | argument | description | expected type | | :------
 - | :---------- | :------------ | | `x` | Relative x-position to its parent
 element | `int` | | `y` | Relative y-position to its parent element | `int` | |
 `text` | Text content | `str` | ```python from conlay import * layout = Conlay
 () boldlabel = BoldLabel(0, 0, "this is a test") layout.add(boldlabel)
 layout.print() ``` Console output: ```
 ââââââââââââââââ âthis is a testâ
-ââââââââââââââââ > ``` ## Cursor The `Cursor`
-class provides a few functions for simple Ansi_Escape cursor actions. ###
-Cursor.setPosition() Set the cursor to a specific position. The Ansi_Escape
+ââââââââââââââââ > ``` ## Input() The `Input()`
+class is a subclass of the LayoutElement() class and is used to create a input
+field. Syntax: ```python element = Input(x, y, text, length, border) ``` |
+argument | description | expected type | | :------- | :---------- | :----------
+-- | | `x` | Relative x-position to its parent element | `int` | | `y` |
+Relative y-position to its parent element | `int` | | `text` | Text content |
+`str` | | `length` | expected input length | `int` | | `border` | Borders
+character set | Border() or one of its subclasses such as Bold() or Thin() |
+```python from conlay import * layout = Conlay() input_element = Input(0, 0,
+"input:", 10, Thin()) layout.add(input_element) layout.print() ``` Console
+output: ``` â­âââââââââââââââââ® âinput:
+â â°âââââââââââââââââ¯ > ``` after you've
+entered a text, you can get it with the element.content variable ```python from
+conlay import * layout = Conlay() input_element = Input(0, 0, "input:", 10,
+Thin()) layout.add(input_element) layout.print() print(input_element.content)
+``` ## ThinInput() The `ThinInput()` class is a subclass of the Input() class
+and is used to create a simple input field with a Thin() Border. Syntax:
+```python element = ThinInput(x, y, text, length) ``` | argument | description
+| expected type | | :------- | :---------- | :------------ | | `x` | Relative
+x-position to its parent element | `int` | | `y` | Relative y-position to its
+parent element | `int` | | `text` | Text content | `str` | | `length` |
+expected input length | `int` | ```python from conlay import * layout = Conlay
+() input_element = ThinInput(0, 0, "input:", 10) layout.add(input_element)
+layout.print() ``` Console output: ```
+â­âââââââââââââââââ® âinput: â
+â°âââââââââââââââââ¯ > ``` ## BoldInput() The
+`BoldInput()` class is a subclass of the Input() class and is used to create a
+simple input field with a Bold() Border. Syntax: ```python element = BoldInput
+(x, y, text, length) ``` | argument | description | expected type | | :------
+- | :---------- | :------------ | | `x` | Relative x-position to its parent
+element | `int` | | `y` | Relative y-position to its parent element | `int` | |
+`text` | Text content | `str` | | `length` | expected input length | `int` |
+```python from conlay import * layout = Conlay() input_element = BoldInput(0,
+0, "input:", 10) layout.add(input_element) layout.print() ``` Console output:
+``` ââââââââââââââââââ âinput: â
+ââââââââââââââââââ > ``` ## Cursor The
+`Cursor` class provides a few functions for simple Ansi_Escape cursor actions.
+### Cursor.setPosition() Set the cursor to a specific position. The Ansi_Escape
 Sequence used for this command is `\x1b[;H`. Syntax: ```python
 Cursor.setPosition(x, y) ``` Example: ```python Cursor.setPosition(10, 5) ```
 ### Cursor.shiftHorizontal() Move the cursor along the X axis. The Ansi_Escape
 Sequence used for this command is `\x1b[D` and `\x1b[C`. Syntax: ```python
 Cursor.shiftHorizontal(x) ``` Example: ```python # move the cursor 10 collumns
 to the right Cursor.shiftHorizontal(10) # move the cursor 5 collumns to the
 left Cursor.shiftHorizontal(-5) ``` ### Cursor.shiftVertical() Move the cursor
@@ -191,19 +225,19 @@
 `bottom_right` | `\u251B` | ## Bold() The `Bold()` class is a subclass of
 Border() and serves as a character set and defines the required bold Unicode
 characters. | class attributes | unicode characters | | :--------------- | :---
 -------------- | | `vertical` | `\u2502` | | `horizontal` | `\u2500` | |
 `top_left` | `\u256D` | | `top_right` | `\u256E` | | `bottom_left` | `\u2570` |
 | `bottom_right` | `\u256F` | ## Summary - Conlay() - _add()_ - _print()_ #####
 Elements - LayoutElement() - Box() - ThinBox() - BoldBox() - Label() -
-ThinLabel() - BoldLabel() ##### Cursor & Console - Cursor - _setPosition()_ -
-_shiftHorizontal()_ - _shiftVertical()_ - _hide()_ - _show()_ - Console -
-_reset()_ - _clear()_ - _eraseLineToEnd()_ - _eraseLineFromStart()_ -
-_eraseLine()_ ##### Coloring - Color - Bg - _rgb()_ - Fg - _rgb()_ ##### Border
-& Border Types - Border - Bold - Thin ## License Licensed under the MIT
-License.  [shields-pypi_version]: https://img.shields.io/pypi/v/
-conlay?label=PyPi%20Version&style=for-the-badge [shields-issues]: https://
-img.shields.io/github/issues/Salliii/conlay?style=for-the-badge [shields-
-license]: https://img.shields.io/github/license/Salliii/conlay?style=for-the-
-badge  [url-pypi_version]: https://pypi.org/project/conlay/ [url-issues]:
-https://github.com/Salliii/conlay/issues [url-license]: https://github.com/
-Salliii/conlay/blob/main/LICENSE
+ThinLabel() - BoldLabel() - Input() - ThinInput() - BoldInput() ##### Cursor &
+Console - Cursor - _setPosition()_ - _shiftHorizontal()_ - _shiftVertical()_ -
+_hide()_ - _show()_ - Console - _reset()_ - _clear()_ - _eraseLineToEnd()_ -
+_eraseLineFromStart()_ - _eraseLine()_ ##### Coloring - Color - Bg - _rgb()_ -
+Fg - _rgb()_ ##### Border & Border Types - Border - Bold - Thin ## License
+Licensed under the MIT_License.  [shields-pypi_version]: https://
+img.shields.io/pypi/v/conlay?label=PyPi%20Version&style=for-the-badge [shields-
+issues]: https://img.shields.io/github/issues/Salliii/conlay?style=for-the-
+badge [shields-license]: https://img.shields.io/github/license/Salliii/
+conlay?style=for-the-badge  [url-pypi_version]: https://pypi.org/project/
+conlay/ [url-issues]: https://github.com/Salliii/conlay/issues [url-license]:
+https://github.com/Salliii/conlay/blob/main/LICENSE
```

### Comparing `conlay-1.0.5/README.md` & `conlay-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: conlay
+Version: 1.1.0
+Summary: A python library for creating nice layouts in the console environment
+Home-page: https://github.com/Salliii/conlay
+Author: Salliii
+Keywords: python,library,console,layout
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Conlay - Console Layout
 [![PyPi version][shields-pypi_version]][url-pypi_version]
 [![Github Issues][shields-issues]][url-issues]
 [![Github License][shields-license]][url-license]
 
 Create visually pleasing console layouts with this easy-to-use Python library. 
 
@@ -56,34 +66,37 @@
 
 ```python
 layout = Conlay()
 ```
 
 There are some attributes that can be used to modify or update the positioning, scale, color and other things. Because each <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a> is a subclass of `Conlay()`, each <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a> has the same attributes.
 
-| attribute        | description | expected type | default value |
-| :--------        | :---------- | :------------ | :------------ |
-| `relative_x`       | Relative x-position to the parent object | `int` | 0 |
-| `relative_y`       | Relative y-position to the parent object | `int` | 0 |
-| `absolute_x`       | Absolute x-position | `int` | 0 |
-| `absolute_y`       | Absolute y-position | `int` | 0 |
-| `width`            | Elements width | `int` | 0 |
-| `min_width`        | Minimal width. May limit the specified with | `int` | 0 |
-| `max_width`        | Maximal width. May limit the specified with | `int` | 0 |
-| `height`           | Elements height | `int` | 0 |
-| `min_height`       | Minimal height. May limit the specified with | `int` | 0 |
-| `max_height`       | Maximal height. May limit the specified with | `int` | 0 |
-| `zindex`           | Indicates whether an element is printed above or below other elements | `int` | 0 |
-| `padding_x`        | Specifies the padding on the x axis, which affects the absolute position of the child elements | `int` | 0 |
-| `padding_y`        | Specifies the padding on the y axis, which affects the absolute position of the child elements | `int` | 0 |
-| `text`             | Specifies the text content | `str` | n/a |
-| `background`       | Specifies whether the element should have a background or not | `bool` | False |
-| `background_color` | Specifies the background color | <a href="https://github.com/Salliii/conlay#colorbg">`Color.Bg`</a> | Color.Bg.clear |
-| `border_color`     | Specifies the border color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
-| `text_color`       | Specifies the text color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
+| attribute           | description | expected type | default value |
+| :--------           | :---------- | :------------ | :------------ |
+| `relative_x`        | Relative x-position to the parent object | `int` | 0 |
+| `relative_y`        | Relative y-position to the parent object | `int` | 0 |
+| `absolute_x`        | Absolute x-position | `int` | 0 |
+| `absolute_y`        | Absolute y-position | `int` | 0 |
+| `width`             | Elements width | `int` | 0 |
+| `min_width`         | Minimal width. May limit the specified with | `int` | 0 |
+| `max_width`         | Maximal width. May limit the specified with | `int` | 0 |
+| `height`            | Elements height | `int` | 0 |
+| `min_height`        | Minimal height. May limit the specified with | `int` | 0 |
+| `max_height`        | Maximal height. May limit the specified with | `int` | 0 |
+| `zindex`            | Indicates whether an element is printed above or below other elements | `int` | 0 |
+| `padding_x`         | Specifies the padding on the x axis, which affects the absolute position of the child elements | `int` | 0 |
+| `padding_y`         | Specifies the padding on the y axis, which affects the absolute position of the child elements | `int` | 0 |
+| `text`              | Specifies the text content | `str` | n/a |
+| `placeholder`       | Specifies the placeholder content | `str` | n/a |
+| `content`           | Stores the text content of the input element, etc. | `str` | n/a |
+| `background`        | Specifies whether the element should have a background or not | `bool` | False |
+| `background_color`  | Specifies the background color | <a href="https://github.com/Salliii/conlay#colorbg">`Color.Bg`</a> | Color.Bg.clear |
+| `border_color`      | Specifies the border color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
+| `text_color`        | Specifies the text color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
+| `placeholder_color` | Specifies the placeholder color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.rgb(150, 150, 150) |
 
 
 ### Conlay.add()
 You can use `add()` to add <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElements</a> to other <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElements</a>.
 
 Syntax:
 
@@ -426,14 +439,153 @@
 
 >
 ```
 
 
 
 
+## Input()
+The `Input()` class is a subclass of the <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a> class and is used to create a input field.
+
+Syntax:
+
+```python
+element = Input(x, y, text, length, border)
+```
+
+| argument | description | expected type |
+| :------- | :---------- | :------------ |
+| `x`      | Relative x-position to its parent element | `int` |
+| `y`      | Relative y-position to its parent element | `int` |
+| `text`   | Text content | `str` |
+| `length` | expected input length | `int` |
+| `border` | Borders character set | <a href="https://github.com/Salliii/conlay#border">Border()</a> or one of its subclasses such as <a href="https://github.com/Salliii/conlay#bold">Bold()</a> or <a href="https://github.com/Salliii/conlay#thin">Thin()</a> |
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = Input(0, 0, "input:", 10, Thin())
+layout.add(input_element)
+
+layout.print()
+```
+
+Console output:
+
+```
+╭────────────────╮
+│input:          │
+╰────────────────╯
+
+
+>
+```
+
+after you've entered a text, you can get it with the element.content variable
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = Input(0, 0, "input:", 10, Thin())
+layout.add(input_element)
+
+layout.print()
+
+print(input_element.content)
+```
+
+
+
+
+## ThinInput()
+The `ThinInput()` class is a subclass of the <a href="https://github.com/Salliii/conlay#input">Input()</a> class and is used to create a simple input field with a <a href="https://github.com/Salliii/conlay#thin">Thin()</a> Border.
+
+Syntax:
+
+```python
+element = ThinInput(x, y, text, length)
+```
+
+| argument | description | expected type |
+| :------- | :---------- | :------------ |
+| `x`      | Relative x-position to its parent element | `int` |
+| `y`      | Relative y-position to its parent element | `int` |
+| `text`   | Text content | `str` |
+| `length` | expected input length | `int` |
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = ThinInput(0, 0, "input:", 10)
+layout.add(input_element)
+
+layout.print()
+```
+
+Console output:
+
+```
+╭────────────────╮
+│input:          │
+╰────────────────╯
+
+
+>
+```
+
+
+
+
+## BoldInput()
+The `BoldInput()` class is a subclass of the <a href="https://github.com/Salliii/conlay#input">Input()</a> class and is used to create a simple input field with a <a href="https://github.com/Salliii/conlay#bold">Bold()</a> Border.
+
+Syntax:
+
+```python
+element = BoldInput(x, y, text, length)
+```
+
+| argument | description | expected type |
+| :------- | :---------- | :------------ |
+| `x`      | Relative x-position to its parent element | `int` |
+| `y`      | Relative y-position to its parent element | `int` |
+| `text`   | Text content | `str` |
+| `length` | expected input length | `int` |
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = BoldInput(0, 0, "input:", 10)
+layout.add(input_element)
+
+layout.print()
+```
+
+Console output:
+
+```
+┏━━━━━━━━━━━━━━━━┓
+┃input:          ┃
+┗━━━━━━━━━━━━━━━━┛
+
+
+>
+```
+
+
+
+
 ## Cursor
 The `Cursor` class provides a few functions for simple <a href="https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797">Ansi Escape</a> cursor actions.
 
 
 ### Cursor.setPosition()
 Set the cursor to a specific position. The <a href="https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797">Ansi Escape Sequence</a> used for this command is `\x1b[<y>;<x>H`.
 
@@ -695,14 +847,17 @@
 - <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a>
 - <a href="https://github.com/Salliii/conlay#box">Box()</a>
 - <a href="https://github.com/Salliii/conlay#thinbox">ThinBox()</a>
 - <a href="https://github.com/Salliii/conlay#boldbox">BoldBox()</a>
 - <a href="https://github.com/Salliii/conlay#label">Label()</a>
 - <a href="https://github.com/Salliii/conlay#thinlabel">ThinLabel()</a>
 - <a href="https://github.com/Salliii/conlay#boldlabel">BoldLabel()</a>
+- <a href="https://github.com/Salliii/conlay#input">Input()</a>
+- <a href="https://github.com/Salliii/conlay#thininput">ThinInput()</a>
+- <a href="https://github.com/Salliii/conlay#boldinput">BoldInput()</a>
 
 ##### Cursor & Console
 - <a href="https://github.com/Salliii/conlay#cursor">Cursor</a>
   - <a href="https://github.com/Salliii/conlay#cursorsetposition">_setPosition()_</a>
   - <a href="https://github.com/Salliii/conlay#cursorshifthorizontal">_shiftHorizontal()_</a>
   - <a href="https://github.com/Salliii/conlay#cursorshiftvertical">_shiftVertical()_</a>
   - <a href="https://github.com/Salliii/conlay#cursorhide">_hide()_</a>
@@ -739,8 +894,8 @@
 [shields-pypi_version]: https://img.shields.io/pypi/v/conlay?label=PyPi%20Version&style=for-the-badge
 [shields-issues]: https://img.shields.io/github/issues/Salliii/conlay?style=for-the-badge
 [shields-license]: https://img.shields.io/github/license/Salliii/conlay?style=for-the-badge
 
 <!-- url -->
 [url-pypi_version]: https://pypi.org/project/conlay/
 [url-issues]: https://github.com/Salliii/conlay/issues
-[url-license]: https://github.com/Salliii/conlay/blob/main/LICENSE
+[url-license]: https://github.com/Salliii/conlay/blob/main/LICENSE
```

#### html2text {}

```diff
@@ -1,15 +1,19 @@
-# Conlay - Console Layout [![PyPi version][shields-pypi_version]][url-
-pypi_version] [![Github Issues][shields-issues]][url-issues] [![Github License]
-[shields-license]][url-license] Create visually pleasing console layouts with
-this easy-to-use Python library. ## Installing Install using pip ```bash pip
-install conlay ``` or install it from PyPi ## Example ```python from conlay
-import * layout = Conlay() blank_box = BoldBox(0, 0, 30, 5) layout.add
-(blank_box) label = ThinLabel(0, 0, "this is a test") blank_box.add(label)
-layout.print() ``` Console output: ```
+Metadata-Version: 2.1 Name: conlay Version: 1.1.0 Summary: A python library for
+creating nice layouts in the console environment Home-page: https://github.com/
+Salliii/conlay Author: Salliii Keywords: python,library,console,layout
+Description-Content-Type: text/markdown License-File: LICENSE # Conlay -
+Console Layout [![PyPi version][shields-pypi_version]][url-pypi_version] [!
+[Github Issues][shields-issues]][url-issues] [![Github License][shields-
+license]][url-license] Create visually pleasing console layouts with this easy-
+to-use Python library. ## Installing Install using pip ```bash pip install
+conlay ``` or install it from PyPi ## Example ```python from conlay import *
+layout = Conlay() blank_box = BoldBox(0, 0, 30, 5) layout.add(blank_box) label
+= ThinLabel(0, 0, "this is a test") blank_box.add(label) layout.print() ```
+Console output: ```
 ââââââââââââââââââââââââââââââ
 ââ­âââââââââââââââ® â ââthis is a testâ
 â ââ°âââââââââââââââ¯ â
 ââââââââââââââââââââââââââââââ
 > ``` ## Conlay() `Conlay()` is the core class within the library. It generates
 and prints out the layout. ```python layout = Conlay() ``` There are some
 attributes that can be used to modify or update the positioning, scale, color
@@ -25,38 +29,41 @@
 height | `int` | 0 | | `min_height` | Minimal height. May limit the specified
 with | `int` | 0 | | `max_height` | Maximal height. May limit the specified
 with | `int` | 0 | | `zindex` | Indicates whether an element is printed above
 or below other elements | `int` | 0 | | `padding_x` | Specifies the padding on
 the x axis, which affects the absolute position of the child elements | `int` |
 0 | | `padding_y` | Specifies the padding on the y axis, which affects the
 absolute position of the child elements | `int` | 0 | | `text` | Specifies the
-text content | `str` | n/a | | `background` | Specifies whether the element
+text content | `str` | n/a | | `placeholder` | Specifies the placeholder
+content | `str` | n/a | | `content` | Stores the text content of the input
+element, etc. | `str` | n/a | | `background` | Specifies whether the element
 should have a background or not | `bool` | False | | `background_color` |
 Specifies the background color | `Color.Bg` | Color.Bg.clear | | `border_color`
 | Specifies the border color | `Color.Fg` | Color.Fg.clear | | `text_color` |
-Specifies the text color | `Color.Fg` | Color.Fg.clear | ### Conlay.add() You
-can use `add()` to add LayoutElements to other LayoutElements. Syntax:
-```python parent.add(child) ``` | argument | description | expected type | | :-
------- | :---------- | :------------ | | `child` | child element |
-LayoutElements() or one of its subclasses such as Box(), Label(), etc. |
-Example: ```python # add a LayoutElement to the main layout layout = Conlay()
-layout.add(ThinBox(...)) # add a LayoutElement to another LayoutElement BoldBox
-(...).add(ThinLabel(...)) ``` ### Conlay.print() You have to call `print()` to
-generate and print out the layout. Syntax: ```python layout.print() ```
-Example: ```python layout = Conlay() ... layout.print() ``` ## LayoutElement()
-The `LayoutElement()` class serves as a superclass for all other layout
-elements such as Box(), Label(), etc. Syntax: ```python element = LayoutElement
-(x, y, w, h, border) ``` | argument | description | expected type | | :------
-- | :---------- | :------------ | | `x` | Relative x-position to its parent
-element | `int` | | `y` | Relative y-position to its parent element | `int` | |
-`w` | Elements width | `int` | | `h` | Elements height | `int` | | `border` |
-Borders character set | Border() or one of its subclasses such as Bold() or
-Thin() | Example: ```python from conlay import * layout = Conlay() element =
-LayoutElement(0, 0, 30, 5, Thin()) layout.add(element) layout.print() ```
-Console output: ```
+Specifies the text color | `Color.Fg` | Color.Fg.clear | | `placeholder_color`
+| Specifies the placeholder color | `Color.Fg` | Color.Fg.rgb(150, 150, 150) |
+### Conlay.add() You can use `add()` to add LayoutElements to other
+LayoutElements. Syntax: ```python parent.add(child) ``` | argument |
+description | expected type | | :------- | :---------- | :------------ | |
+`child` | child element | LayoutElements() or one of its subclasses such as Box
+(), Label(), etc. | Example: ```python # add a LayoutElement to the main layout
+layout = Conlay() layout.add(ThinBox(...)) # add a LayoutElement to another
+LayoutElement BoldBox(...).add(ThinLabel(...)) ``` ### Conlay.print() You have
+to call `print()` to generate and print out the layout. Syntax: ```python
+layout.print() ``` Example: ```python layout = Conlay() ... layout.print() ```
+## LayoutElement() The `LayoutElement()` class serves as a superclass for all
+other layout elements such as Box(), Label(), etc. Syntax: ```python element =
+LayoutElement(x, y, w, h, border) ``` | argument | description | expected type
+| | :------- | :---------- | :------------ | | `x` | Relative x-position to its
+parent element | `int` | | `y` | Relative y-position to its parent element |
+`int` | | `w` | Elements width | `int` | | `h` | Elements height | `int` | |
+`border` | Borders character set | Border() or one of its subclasses such as
+Bold() or Thin() | Example: ```python from conlay import * layout = Conlay()
+element = LayoutElement(0, 0, 30, 5, Thin()) layout.add(element) layout.print()
+``` Console output: ```
 â­âââââââââââââââââââââââââââââ®
 â â â â â â
 â°âââââââââââââââââââââââââââââ¯
 > ``` ## Box() The `Box()` class is a subclass of the LayoutElement() class and
 is used to create a simple box. Syntax: ```python element = Box(x, y, w, h,
 border) ``` | argument | description | expected type | | :------- | :---------
 - | :------------ | | `x` | Relative x-position to its parent element | `int` |
@@ -115,17 +122,52 @@
 BoldLabel(x, y, text) ``` | argument | description | expected type | | :------
 - | :---------- | :------------ | | `x` | Relative x-position to its parent
 element | `int` | | `y` | Relative y-position to its parent element | `int` | |
 `text` | Text content | `str` | ```python from conlay import * layout = Conlay
 () boldlabel = BoldLabel(0, 0, "this is a test") layout.add(boldlabel)
 layout.print() ``` Console output: ```
 ââââââââââââââââ âthis is a testâ
-ââââââââââââââââ > ``` ## Cursor The `Cursor`
-class provides a few functions for simple Ansi_Escape cursor actions. ###
-Cursor.setPosition() Set the cursor to a specific position. The Ansi_Escape
+ââââââââââââââââ > ``` ## Input() The `Input()`
+class is a subclass of the LayoutElement() class and is used to create a input
+field. Syntax: ```python element = Input(x, y, text, length, border) ``` |
+argument | description | expected type | | :------- | :---------- | :----------
+-- | | `x` | Relative x-position to its parent element | `int` | | `y` |
+Relative y-position to its parent element | `int` | | `text` | Text content |
+`str` | | `length` | expected input length | `int` | | `border` | Borders
+character set | Border() or one of its subclasses such as Bold() or Thin() |
+```python from conlay import * layout = Conlay() input_element = Input(0, 0,
+"input:", 10, Thin()) layout.add(input_element) layout.print() ``` Console
+output: ``` â­âââââââââââââââââ® âinput:
+â â°âââââââââââââââââ¯ > ``` after you've
+entered a text, you can get it with the element.content variable ```python from
+conlay import * layout = Conlay() input_element = Input(0, 0, "input:", 10,
+Thin()) layout.add(input_element) layout.print() print(input_element.content)
+``` ## ThinInput() The `ThinInput()` class is a subclass of the Input() class
+and is used to create a simple input field with a Thin() Border. Syntax:
+```python element = ThinInput(x, y, text, length) ``` | argument | description
+| expected type | | :------- | :---------- | :------------ | | `x` | Relative
+x-position to its parent element | `int` | | `y` | Relative y-position to its
+parent element | `int` | | `text` | Text content | `str` | | `length` |
+expected input length | `int` | ```python from conlay import * layout = Conlay
+() input_element = ThinInput(0, 0, "input:", 10) layout.add(input_element)
+layout.print() ``` Console output: ```
+â­âââââââââââââââââ® âinput: â
+â°âââââââââââââââââ¯ > ``` ## BoldInput() The
+`BoldInput()` class is a subclass of the Input() class and is used to create a
+simple input field with a Bold() Border. Syntax: ```python element = BoldInput
+(x, y, text, length) ``` | argument | description | expected type | | :------
+- | :---------- | :------------ | | `x` | Relative x-position to its parent
+element | `int` | | `y` | Relative y-position to its parent element | `int` | |
+`text` | Text content | `str` | | `length` | expected input length | `int` |
+```python from conlay import * layout = Conlay() input_element = BoldInput(0,
+0, "input:", 10) layout.add(input_element) layout.print() ``` Console output:
+``` ââââââââââââââââââ âinput: â
+ââââââââââââââââââ > ``` ## Cursor The
+`Cursor` class provides a few functions for simple Ansi_Escape cursor actions.
+### Cursor.setPosition() Set the cursor to a specific position. The Ansi_Escape
 Sequence used for this command is `\x1b[;H`. Syntax: ```python
 Cursor.setPosition(x, y) ``` Example: ```python Cursor.setPosition(10, 5) ```
 ### Cursor.shiftHorizontal() Move the cursor along the X axis. The Ansi_Escape
 Sequence used for this command is `\x1b[D` and `\x1b[C`. Syntax: ```python
 Cursor.shiftHorizontal(x) ``` Example: ```python # move the cursor 10 collumns
 to the right Cursor.shiftHorizontal(10) # move the cursor 5 collumns to the
 left Cursor.shiftHorizontal(-5) ``` ### Cursor.shiftVertical() Move the cursor
@@ -187,19 +229,19 @@
 `bottom_right` | `\u251B` | ## Bold() The `Bold()` class is a subclass of
 Border() and serves as a character set and defines the required bold Unicode
 characters. | class attributes | unicode characters | | :--------------- | :---
 -------------- | | `vertical` | `\u2502` | | `horizontal` | `\u2500` | |
 `top_left` | `\u256D` | | `top_right` | `\u256E` | | `bottom_left` | `\u2570` |
 | `bottom_right` | `\u256F` | ## Summary - Conlay() - _add()_ - _print()_ #####
 Elements - LayoutElement() - Box() - ThinBox() - BoldBox() - Label() -
-ThinLabel() - BoldLabel() ##### Cursor & Console - Cursor - _setPosition()_ -
-_shiftHorizontal()_ - _shiftVertical()_ - _hide()_ - _show()_ - Console -
-_reset()_ - _clear()_ - _eraseLineToEnd()_ - _eraseLineFromStart()_ -
-_eraseLine()_ ##### Coloring - Color - Bg - _rgb()_ - Fg - _rgb()_ ##### Border
-& Border Types - Border - Bold - Thin ## License Licensed under the MIT
-License.  [shields-pypi_version]: https://img.shields.io/pypi/v/
-conlay?label=PyPi%20Version&style=for-the-badge [shields-issues]: https://
-img.shields.io/github/issues/Salliii/conlay?style=for-the-badge [shields-
-license]: https://img.shields.io/github/license/Salliii/conlay?style=for-the-
-badge  [url-pypi_version]: https://pypi.org/project/conlay/ [url-issues]:
-https://github.com/Salliii/conlay/issues [url-license]: https://github.com/
-Salliii/conlay/blob/main/LICENSE
+ThinLabel() - BoldLabel() - Input() - ThinInput() - BoldInput() ##### Cursor &
+Console - Cursor - _setPosition()_ - _shiftHorizontal()_ - _shiftVertical()_ -
+_hide()_ - _show()_ - Console - _reset()_ - _clear()_ - _eraseLineToEnd()_ -
+_eraseLineFromStart()_ - _eraseLine()_ ##### Coloring - Color - Bg - _rgb()_ -
+Fg - _rgb()_ ##### Border & Border Types - Border - Bold - Thin ## License
+Licensed under the MIT_License.  [shields-pypi_version]: https://
+img.shields.io/pypi/v/conlay?label=PyPi%20Version&style=for-the-badge [shields-
+issues]: https://img.shields.io/github/issues/Salliii/conlay?style=for-the-
+badge [shields-license]: https://img.shields.io/github/license/Salliii/
+conlay?style=for-the-badge  [url-pypi_version]: https://pypi.org/project/
+conlay/ [url-issues]: https://github.com/Salliii/conlay/issues [url-license]:
+https://github.com/Salliii/conlay/blob/main/LICENSE
```

### Comparing `conlay-1.0.5/conlay/main.py` & `conlay-1.1.0/conlay/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,25 +36,27 @@
 
 
 
 
 class Color:
     """ color set """
 
+    clear = "\x1b[0m"
+
     class Bg:
         """ background color set """
 
         # clear background color
         clear = "\x1b[49m"
 
         # function that returns a properly formatted ansi escape code for the background color
         def rgb(r:int, g:int, b:int) -> str:
             return "\x1b[48;2;{r};{g};{b}m".format(r=r, g=g, b=b)
         
-        # default color set
+        # default bg color set
         black = rgb(0, 0, 0)
         white = rgb(255, 255, 255)
         red = rgb(205, 49, 49)
         green = rgb(13, 188, 121)
         blue = rgb(36, 114, 200)
         yellow = rgb(229, 229, 16)
         purple = rgb(188, 63, 188)
@@ -67,15 +69,15 @@
         # clear background color
         clear = "\x1b[49m"
 
         # function that returns a properly formatted ansi escape code for the foreground color
         def rgb(r:int, g:int, b:int) -> str:
             return "\x1b[38;2;{r};{g};{b}m".format(r=r, g=g, b=b)
         
-        # default color set
+        # default fg color set
         black = rgb(0, 0, 0)
         white = rgb(255, 255, 255)
         red = rgb(205, 49, 49)
         green = rgb(13, 188, 121)
         blue = rgb(36, 114, 200)
         yellow = rgb(229, 229, 16)
         purple = rgb(188, 63, 188)
@@ -198,18 +200,21 @@
         self.height = int()
         self.min_height = int()
         self.max_height = int()
         self.zindex = int()
         self.padding_x = int()
         self.padding_y = int()
         self.text = str()
+        self.placeholder = str()
+        self.content = str()
         self.background = bool()
         self.background_color = Color.Bg.clear
         self.border_color = Color.Fg.clear
         self.text_color = Color.Fg.clear
+        self.placeholder_color = Color.Fg.rgb(150, 150, 150)
 
 
     def __sort_childs_by_zindex__(self, reverse=False) -> list:
         """ sort child list by elements zindex attribute """
         
         return list(sorted(self.childs, key=lambda child: child.zindex, reverse=reverse))
     
@@ -318,76 +323,151 @@
         # set cursor position
         Cursor.setPosition(0, self.__get_final_cursor_position__())
 
 
 
 
 class LayoutElement(Conlay):
+    """ main class for each layout element """
+
     def __init__(self, x:int, y:int, w:int, h:int, border:Border) -> None:
         super().__init__()
 
+        # class attributes
         self.relative_x = x + 1
         self.relative_y = y + 1
         self.width = w
         self.height = h
         self.border = border
 
 
 
 
 class Box(LayoutElement):
+    """ layout element to create a simple box """
+
     def __init__(self, x:int, y:int, w:int, h:int, border:Border) -> None:
         super().__init__(x, y, w, h, border)
 
     
     def __preprint__(self) -> int:
         return 1
     
 
-    def __pastprint__(self) -> int:
+    def __print__(self) -> int:
         return 1
 
 
 class ThinBox(Box):
+    """ layout element to create a thin box """
+
     def __init__(self, x:int, y:int, w:int, h:int) -> None:
         super().__init__(x, y, w, h, Thin())
 
 
 class BoldBox(Box):
+    """ layout element to create a bold box """
+
     def __init__(self, x:int, y:int, w:int, h:int) -> None:
         super().__init__(x, y, w, h, Bold())
 
 
 
 
 class Label(LayoutElement):
+    """ layout element to create a simple label """
+
     def __init__(self, x:int, y:int, text:str, border:Border) -> None:
+
+        # calculates width and height depending on the text content 
         w = len(max(text.split("\n"), key=len))
         h = len(text.split("\n"))
 
         super().__init__(x, y, w, h, border)
 
+        # set text content
         self.text = text
 
 
     def __preprint__(self) -> int:
+        # calculate width and height depending on its padding
         self.width = self.width + self.padding_x * 2 + 2
         self.height = self.height + self.padding_y * 2 + 2
 
         return 1
 
 
     def __print__(self) -> int:
+        # print text content
         Cursor.setPosition(self.absolute_x + 1 + self.padding_x, self.absolute_y + 1 + self.padding_y)
-        print(self.text, end="")
+        print(self.text_color + self.text, end=Color.clear)
 
         return 1
 
 
 class ThinLabel(Label):
+    """ layout element to create a thin label """
+
     def __init__(self, x:int, y:int, text:str) -> None:
         super().__init__(x, y, text, Thin())
 
 
 class BoldLabel(Label):
+    """ layout element to create a bold label """
+
     def __init__(self, x:int, y:int, text:str) -> None:
-        super().__init__(x, y, text, Bold())
+        super().__init__(x, y, text, Bold())
+
+
+
+
+class Input(LayoutElement):
+    """ layout element to create a simple input element """
+
+    def __init__(self, x:int, y:int, text:str, length:int, border:Border) -> None:
+
+        # calculates width and height depending on the text content and the input length
+        w = len(" ".join(text.split("\n"))) + length
+        h = len(text.split("\n"))
+
+        super().__init__(x, y, w, h, border)
+
+        # set text content
+        self.text = " ".join(text.split("\n"))
+
+
+    def __preprint__(self) -> int:
+        # calculate width and height depending on its padding
+        self.width = self.width + self.padding_x * 2 + 2
+        self.height = self.height + self.padding_y * 2 + 2
+
+        return 1
+
+
+    def __print__(self) -> int:
+        # print text content
+        Cursor.setPosition(self.absolute_x + 1 + self.padding_x, self.absolute_y + 1 + self.padding_y)
+        print(self.text_color + self.text, end=Color.clear)
+
+        # print placeholder content
+        Cursor.setPosition(self.absolute_x + 1 + self.padding_x + len(self.text), self.absolute_y + 1 + self.padding_y)
+        print(self.placeholder_color + self.placeholder, end=Color.clear)
+
+        # print input
+        Cursor.setPosition(self.absolute_x + 1 + self.padding_x + len(self.text), self.absolute_y + 1 + self.padding_y)
+        self.content = input()
+
+        return 1
+
+
+class ThinInput(Input):
+    """ layout element to create a thin input """
+
+    def __init__(self, x:int, y:int, text:str, length:int) -> None:
+        super().__init__(x, y, text, length, Thin())
+
+
+class BoldInput(Input):
+    """ layout element to create a bold input """
+
+    def __init__(self, x:int, y:int, text:str, length:int) -> None:
+        super().__init__(x, y, text, length, Bold())
```

### Comparing `conlay-1.0.5/conlay.egg-info/PKG-INFO` & `conlay-1.1.0/conlay.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conlay
-Version: 1.0.5
+Version: 1.1.0
 Summary: A python library for creating nice layouts in the console environment
 Home-page: https://github.com/Salliii/conlay
 Author: Salliii
 Keywords: python,library,console,layout
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -66,34 +66,37 @@
 
 ```python
 layout = Conlay()
 ```
 
 There are some attributes that can be used to modify or update the positioning, scale, color and other things. Because each <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a> is a subclass of `Conlay()`, each <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a> has the same attributes.
 
-| attribute        | description | expected type | default value |
-| :--------        | :---------- | :------------ | :------------ |
-| `relative_x`       | Relative x-position to the parent object | `int` | 0 |
-| `relative_y`       | Relative y-position to the parent object | `int` | 0 |
-| `absolute_x`       | Absolute x-position | `int` | 0 |
-| `absolute_y`       | Absolute y-position | `int` | 0 |
-| `width`            | Elements width | `int` | 0 |
-| `min_width`        | Minimal width. May limit the specified with | `int` | 0 |
-| `max_width`        | Maximal width. May limit the specified with | `int` | 0 |
-| `height`           | Elements height | `int` | 0 |
-| `min_height`       | Minimal height. May limit the specified with | `int` | 0 |
-| `max_height`       | Maximal height. May limit the specified with | `int` | 0 |
-| `zindex`           | Indicates whether an element is printed above or below other elements | `int` | 0 |
-| `padding_x`        | Specifies the padding on the x axis, which affects the absolute position of the child elements | `int` | 0 |
-| `padding_y`        | Specifies the padding on the y axis, which affects the absolute position of the child elements | `int` | 0 |
-| `text`             | Specifies the text content | `str` | n/a |
-| `background`       | Specifies whether the element should have a background or not | `bool` | False |
-| `background_color` | Specifies the background color | <a href="https://github.com/Salliii/conlay#colorbg">`Color.Bg`</a> | Color.Bg.clear |
-| `border_color`     | Specifies the border color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
-| `text_color`       | Specifies the text color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
+| attribute           | description | expected type | default value |
+| :--------           | :---------- | :------------ | :------------ |
+| `relative_x`        | Relative x-position to the parent object | `int` | 0 |
+| `relative_y`        | Relative y-position to the parent object | `int` | 0 |
+| `absolute_x`        | Absolute x-position | `int` | 0 |
+| `absolute_y`        | Absolute y-position | `int` | 0 |
+| `width`             | Elements width | `int` | 0 |
+| `min_width`         | Minimal width. May limit the specified with | `int` | 0 |
+| `max_width`         | Maximal width. May limit the specified with | `int` | 0 |
+| `height`            | Elements height | `int` | 0 |
+| `min_height`        | Minimal height. May limit the specified with | `int` | 0 |
+| `max_height`        | Maximal height. May limit the specified with | `int` | 0 |
+| `zindex`            | Indicates whether an element is printed above or below other elements | `int` | 0 |
+| `padding_x`         | Specifies the padding on the x axis, which affects the absolute position of the child elements | `int` | 0 |
+| `padding_y`         | Specifies the padding on the y axis, which affects the absolute position of the child elements | `int` | 0 |
+| `text`              | Specifies the text content | `str` | n/a |
+| `placeholder`       | Specifies the placeholder content | `str` | n/a |
+| `content`           | Stores the text content of the input element, etc. | `str` | n/a |
+| `background`        | Specifies whether the element should have a background or not | `bool` | False |
+| `background_color`  | Specifies the background color | <a href="https://github.com/Salliii/conlay#colorbg">`Color.Bg`</a> | Color.Bg.clear |
+| `border_color`      | Specifies the border color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
+| `text_color`        | Specifies the text color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.clear |
+| `placeholder_color` | Specifies the placeholder color | <a href="https://github.com/Salliii/conlay#colorfg">`Color.Fg`</a> | Color.Fg.rgb(150, 150, 150) |
 
 
 ### Conlay.add()
 You can use `add()` to add <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElements</a> to other <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElements</a>.
 
 Syntax:
 
@@ -436,14 +439,153 @@
 
 >
 ```
 
 
 
 
+## Input()
+The `Input()` class is a subclass of the <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a> class and is used to create a input field.
+
+Syntax:
+
+```python
+element = Input(x, y, text, length, border)
+```
+
+| argument | description | expected type |
+| :------- | :---------- | :------------ |
+| `x`      | Relative x-position to its parent element | `int` |
+| `y`      | Relative y-position to its parent element | `int` |
+| `text`   | Text content | `str` |
+| `length` | expected input length | `int` |
+| `border` | Borders character set | <a href="https://github.com/Salliii/conlay#border">Border()</a> or one of its subclasses such as <a href="https://github.com/Salliii/conlay#bold">Bold()</a> or <a href="https://github.com/Salliii/conlay#thin">Thin()</a> |
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = Input(0, 0, "input:", 10, Thin())
+layout.add(input_element)
+
+layout.print()
+```
+
+Console output:
+
+```
+╭────────────────╮
+│input:          │
+╰────────────────╯
+
+
+>
+```
+
+after you've entered a text, you can get it with the element.content variable
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = Input(0, 0, "input:", 10, Thin())
+layout.add(input_element)
+
+layout.print()
+
+print(input_element.content)
+```
+
+
+
+
+## ThinInput()
+The `ThinInput()` class is a subclass of the <a href="https://github.com/Salliii/conlay#input">Input()</a> class and is used to create a simple input field with a <a href="https://github.com/Salliii/conlay#thin">Thin()</a> Border.
+
+Syntax:
+
+```python
+element = ThinInput(x, y, text, length)
+```
+
+| argument | description | expected type |
+| :------- | :---------- | :------------ |
+| `x`      | Relative x-position to its parent element | `int` |
+| `y`      | Relative y-position to its parent element | `int` |
+| `text`   | Text content | `str` |
+| `length` | expected input length | `int` |
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = ThinInput(0, 0, "input:", 10)
+layout.add(input_element)
+
+layout.print()
+```
+
+Console output:
+
+```
+╭────────────────╮
+│input:          │
+╰────────────────╯
+
+
+>
+```
+
+
+
+
+## BoldInput()
+The `BoldInput()` class is a subclass of the <a href="https://github.com/Salliii/conlay#input">Input()</a> class and is used to create a simple input field with a <a href="https://github.com/Salliii/conlay#bold">Bold()</a> Border.
+
+Syntax:
+
+```python
+element = BoldInput(x, y, text, length)
+```
+
+| argument | description | expected type |
+| :------- | :---------- | :------------ |
+| `x`      | Relative x-position to its parent element | `int` |
+| `y`      | Relative y-position to its parent element | `int` |
+| `text`   | Text content | `str` |
+| `length` | expected input length | `int` |
+
+```python
+from conlay import *
+
+layout = Conlay()
+
+input_element = BoldInput(0, 0, "input:", 10)
+layout.add(input_element)
+
+layout.print()
+```
+
+Console output:
+
+```
+┏━━━━━━━━━━━━━━━━┓
+┃input:          ┃
+┗━━━━━━━━━━━━━━━━┛
+
+
+>
+```
+
+
+
+
 ## Cursor
 The `Cursor` class provides a few functions for simple <a href="https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797">Ansi Escape</a> cursor actions.
 
 
 ### Cursor.setPosition()
 Set the cursor to a specific position. The <a href="https://gist.github.com/fnky/458719343aabd01cfb17a3a4f7296797">Ansi Escape Sequence</a> used for this command is `\x1b[<y>;<x>H`.
 
@@ -705,14 +847,17 @@
 - <a href="https://github.com/Salliii/conlay#layoutelement">LayoutElement()</a>
 - <a href="https://github.com/Salliii/conlay#box">Box()</a>
 - <a href="https://github.com/Salliii/conlay#thinbox">ThinBox()</a>
 - <a href="https://github.com/Salliii/conlay#boldbox">BoldBox()</a>
 - <a href="https://github.com/Salliii/conlay#label">Label()</a>
 - <a href="https://github.com/Salliii/conlay#thinlabel">ThinLabel()</a>
 - <a href="https://github.com/Salliii/conlay#boldlabel">BoldLabel()</a>
+- <a href="https://github.com/Salliii/conlay#input">Input()</a>
+- <a href="https://github.com/Salliii/conlay#thininput">ThinInput()</a>
+- <a href="https://github.com/Salliii/conlay#boldinput">BoldInput()</a>
 
 ##### Cursor & Console
 - <a href="https://github.com/Salliii/conlay#cursor">Cursor</a>
   - <a href="https://github.com/Salliii/conlay#cursorsetposition">_setPosition()_</a>
   - <a href="https://github.com/Salliii/conlay#cursorshifthorizontal">_shiftHorizontal()_</a>
   - <a href="https://github.com/Salliii/conlay#cursorshiftvertical">_shiftVertical()_</a>
   - <a href="https://github.com/Salliii/conlay#cursorhide">_hide()_</a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: conlay Version: 1.0.5 Summary: A python library for
+Metadata-Version: 2.1 Name: conlay Version: 1.1.0 Summary: A python library for
 creating nice layouts in the console environment Home-page: https://github.com/
 Salliii/conlay Author: Salliii Keywords: python,library,console,layout
 Description-Content-Type: text/markdown License-File: LICENSE # Conlay -
 Console Layout [![PyPi version][shields-pypi_version]][url-pypi_version] [!
 [Github Issues][shields-issues]][url-issues] [![Github License][shields-
 license]][url-license] Create visually pleasing console layouts with this easy-
 to-use Python library. ## Installing Install using pip ```bash pip install
@@ -29,38 +29,41 @@
 height | `int` | 0 | | `min_height` | Minimal height. May limit the specified
 with | `int` | 0 | | `max_height` | Maximal height. May limit the specified
 with | `int` | 0 | | `zindex` | Indicates whether an element is printed above
 or below other elements | `int` | 0 | | `padding_x` | Specifies the padding on
 the x axis, which affects the absolute position of the child elements | `int` |
 0 | | `padding_y` | Specifies the padding on the y axis, which affects the
 absolute position of the child elements | `int` | 0 | | `text` | Specifies the
-text content | `str` | n/a | | `background` | Specifies whether the element
+text content | `str` | n/a | | `placeholder` | Specifies the placeholder
+content | `str` | n/a | | `content` | Stores the text content of the input
+element, etc. | `str` | n/a | | `background` | Specifies whether the element
 should have a background or not | `bool` | False | | `background_color` |
 Specifies the background color | `Color.Bg` | Color.Bg.clear | | `border_color`
 | Specifies the border color | `Color.Fg` | Color.Fg.clear | | `text_color` |
-Specifies the text color | `Color.Fg` | Color.Fg.clear | ### Conlay.add() You
-can use `add()` to add LayoutElements to other LayoutElements. Syntax:
-```python parent.add(child) ``` | argument | description | expected type | | :-
------- | :---------- | :------------ | | `child` | child element |
-LayoutElements() or one of its subclasses such as Box(), Label(), etc. |
-Example: ```python # add a LayoutElement to the main layout layout = Conlay()
-layout.add(ThinBox(...)) # add a LayoutElement to another LayoutElement BoldBox
-(...).add(ThinLabel(...)) ``` ### Conlay.print() You have to call `print()` to
-generate and print out the layout. Syntax: ```python layout.print() ```
-Example: ```python layout = Conlay() ... layout.print() ``` ## LayoutElement()
-The `LayoutElement()` class serves as a superclass for all other layout
-elements such as Box(), Label(), etc. Syntax: ```python element = LayoutElement
-(x, y, w, h, border) ``` | argument | description | expected type | | :------
-- | :---------- | :------------ | | `x` | Relative x-position to its parent
-element | `int` | | `y` | Relative y-position to its parent element | `int` | |
-`w` | Elements width | `int` | | `h` | Elements height | `int` | | `border` |
-Borders character set | Border() or one of its subclasses such as Bold() or
-Thin() | Example: ```python from conlay import * layout = Conlay() element =
-LayoutElement(0, 0, 30, 5, Thin()) layout.add(element) layout.print() ```
-Console output: ```
+Specifies the text color | `Color.Fg` | Color.Fg.clear | | `placeholder_color`
+| Specifies the placeholder color | `Color.Fg` | Color.Fg.rgb(150, 150, 150) |
+### Conlay.add() You can use `add()` to add LayoutElements to other
+LayoutElements. Syntax: ```python parent.add(child) ``` | argument |
+description | expected type | | :------- | :---------- | :------------ | |
+`child` | child element | LayoutElements() or one of its subclasses such as Box
+(), Label(), etc. | Example: ```python # add a LayoutElement to the main layout
+layout = Conlay() layout.add(ThinBox(...)) # add a LayoutElement to another
+LayoutElement BoldBox(...).add(ThinLabel(...)) ``` ### Conlay.print() You have
+to call `print()` to generate and print out the layout. Syntax: ```python
+layout.print() ``` Example: ```python layout = Conlay() ... layout.print() ```
+## LayoutElement() The `LayoutElement()` class serves as a superclass for all
+other layout elements such as Box(), Label(), etc. Syntax: ```python element =
+LayoutElement(x, y, w, h, border) ``` | argument | description | expected type
+| | :------- | :---------- | :------------ | | `x` | Relative x-position to its
+parent element | `int` | | `y` | Relative y-position to its parent element |
+`int` | | `w` | Elements width | `int` | | `h` | Elements height | `int` | |
+`border` | Borders character set | Border() or one of its subclasses such as
+Bold() or Thin() | Example: ```python from conlay import * layout = Conlay()
+element = LayoutElement(0, 0, 30, 5, Thin()) layout.add(element) layout.print()
+``` Console output: ```
 â­âââââââââââââââââââââââââââââ®
 â â â â â â
 â°âââââââââââââââââââââââââââââ¯
 > ``` ## Box() The `Box()` class is a subclass of the LayoutElement() class and
 is used to create a simple box. Syntax: ```python element = Box(x, y, w, h,
 border) ``` | argument | description | expected type | | :------- | :---------
 - | :------------ | | `x` | Relative x-position to its parent element | `int` |
@@ -119,17 +122,52 @@
 BoldLabel(x, y, text) ``` | argument | description | expected type | | :------
 - | :---------- | :------------ | | `x` | Relative x-position to its parent
 element | `int` | | `y` | Relative y-position to its parent element | `int` | |
 `text` | Text content | `str` | ```python from conlay import * layout = Conlay
 () boldlabel = BoldLabel(0, 0, "this is a test") layout.add(boldlabel)
 layout.print() ``` Console output: ```
 ââââââââââââââââ âthis is a testâ
-ââââââââââââââââ > ``` ## Cursor The `Cursor`
-class provides a few functions for simple Ansi_Escape cursor actions. ###
-Cursor.setPosition() Set the cursor to a specific position. The Ansi_Escape
+ââââââââââââââââ > ``` ## Input() The `Input()`
+class is a subclass of the LayoutElement() class and is used to create a input
+field. Syntax: ```python element = Input(x, y, text, length, border) ``` |
+argument | description | expected type | | :------- | :---------- | :----------
+-- | | `x` | Relative x-position to its parent element | `int` | | `y` |
+Relative y-position to its parent element | `int` | | `text` | Text content |
+`str` | | `length` | expected input length | `int` | | `border` | Borders
+character set | Border() or one of its subclasses such as Bold() or Thin() |
+```python from conlay import * layout = Conlay() input_element = Input(0, 0,
+"input:", 10, Thin()) layout.add(input_element) layout.print() ``` Console
+output: ``` â­âââââââââââââââââ® âinput:
+â â°âââââââââââââââââ¯ > ``` after you've
+entered a text, you can get it with the element.content variable ```python from
+conlay import * layout = Conlay() input_element = Input(0, 0, "input:", 10,
+Thin()) layout.add(input_element) layout.print() print(input_element.content)
+``` ## ThinInput() The `ThinInput()` class is a subclass of the Input() class
+and is used to create a simple input field with a Thin() Border. Syntax:
+```python element = ThinInput(x, y, text, length) ``` | argument | description
+| expected type | | :------- | :---------- | :------------ | | `x` | Relative
+x-position to its parent element | `int` | | `y` | Relative y-position to its
+parent element | `int` | | `text` | Text content | `str` | | `length` |
+expected input length | `int` | ```python from conlay import * layout = Conlay
+() input_element = ThinInput(0, 0, "input:", 10) layout.add(input_element)
+layout.print() ``` Console output: ```
+â­âââââââââââââââââ® âinput: â
+â°âââââââââââââââââ¯ > ``` ## BoldInput() The
+`BoldInput()` class is a subclass of the Input() class and is used to create a
+simple input field with a Bold() Border. Syntax: ```python element = BoldInput
+(x, y, text, length) ``` | argument | description | expected type | | :------
+- | :---------- | :------------ | | `x` | Relative x-position to its parent
+element | `int` | | `y` | Relative y-position to its parent element | `int` | |
+`text` | Text content | `str` | | `length` | expected input length | `int` |
+```python from conlay import * layout = Conlay() input_element = BoldInput(0,
+0, "input:", 10) layout.add(input_element) layout.print() ``` Console output:
+``` ââââââââââââââââââ âinput: â
+ââââââââââââââââââ > ``` ## Cursor The
+`Cursor` class provides a few functions for simple Ansi_Escape cursor actions.
+### Cursor.setPosition() Set the cursor to a specific position. The Ansi_Escape
 Sequence used for this command is `\x1b[;H`. Syntax: ```python
 Cursor.setPosition(x, y) ``` Example: ```python Cursor.setPosition(10, 5) ```
 ### Cursor.shiftHorizontal() Move the cursor along the X axis. The Ansi_Escape
 Sequence used for this command is `\x1b[D` and `\x1b[C`. Syntax: ```python
 Cursor.shiftHorizontal(x) ``` Example: ```python # move the cursor 10 collumns
 to the right Cursor.shiftHorizontal(10) # move the cursor 5 collumns to the
 left Cursor.shiftHorizontal(-5) ``` ### Cursor.shiftVertical() Move the cursor
@@ -191,19 +229,19 @@
 `bottom_right` | `\u251B` | ## Bold() The `Bold()` class is a subclass of
 Border() and serves as a character set and defines the required bold Unicode
 characters. | class attributes | unicode characters | | :--------------- | :---
 -------------- | | `vertical` | `\u2502` | | `horizontal` | `\u2500` | |
 `top_left` | `\u256D` | | `top_right` | `\u256E` | | `bottom_left` | `\u2570` |
 | `bottom_right` | `\u256F` | ## Summary - Conlay() - _add()_ - _print()_ #####
 Elements - LayoutElement() - Box() - ThinBox() - BoldBox() - Label() -
-ThinLabel() - BoldLabel() ##### Cursor & Console - Cursor - _setPosition()_ -
-_shiftHorizontal()_ - _shiftVertical()_ - _hide()_ - _show()_ - Console -
-_reset()_ - _clear()_ - _eraseLineToEnd()_ - _eraseLineFromStart()_ -
-_eraseLine()_ ##### Coloring - Color - Bg - _rgb()_ - Fg - _rgb()_ ##### Border
-& Border Types - Border - Bold - Thin ## License Licensed under the MIT
-License.  [shields-pypi_version]: https://img.shields.io/pypi/v/
-conlay?label=PyPi%20Version&style=for-the-badge [shields-issues]: https://
-img.shields.io/github/issues/Salliii/conlay?style=for-the-badge [shields-
-license]: https://img.shields.io/github/license/Salliii/conlay?style=for-the-
-badge  [url-pypi_version]: https://pypi.org/project/conlay/ [url-issues]:
-https://github.com/Salliii/conlay/issues [url-license]: https://github.com/
-Salliii/conlay/blob/main/LICENSE
+ThinLabel() - BoldLabel() - Input() - ThinInput() - BoldInput() ##### Cursor &
+Console - Cursor - _setPosition()_ - _shiftHorizontal()_ - _shiftVertical()_ -
+_hide()_ - _show()_ - Console - _reset()_ - _clear()_ - _eraseLineToEnd()_ -
+_eraseLineFromStart()_ - _eraseLine()_ ##### Coloring - Color - Bg - _rgb()_ -
+Fg - _rgb()_ ##### Border & Border Types - Border - Bold - Thin ## License
+Licensed under the MIT_License.  [shields-pypi_version]: https://
+img.shields.io/pypi/v/conlay?label=PyPi%20Version&style=for-the-badge [shields-
+issues]: https://img.shields.io/github/issues/Salliii/conlay?style=for-the-
+badge [shields-license]: https://img.shields.io/github/license/Salliii/
+conlay?style=for-the-badge  [url-pypi_version]: https://pypi.org/project/
+conlay/ [url-issues]: https://github.com/Salliii/conlay/issues [url-license]:
+https://github.com/Salliii/conlay/blob/main/LICENSE
```

### Comparing `conlay-1.0.5/setup.py` & `conlay-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = "1.0.5"
+VERSION = "1.1.0"
 
 with open("README.md", "r", encoding="utf-8") as readme:
     DESC_LONG = readme.read()
 
 
 setuptools.setup(
     name="conlay",
```

