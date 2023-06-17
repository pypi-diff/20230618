# Comparing `tmp/docx2python-2.7.2.tar.gz` & `tmp/docx2python-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx2python-2.7.2.tar", max compression
+gzip compressed data, was "docx2python-2.7.3.tar", max compression
```

## Comparing `docx2python-2.7.2.tar` & `docx2python-2.7.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      240 2023-01-19 19:29:25.943561 docx2python-2.7.2/docx2python/__init__.py
--rw-r--r--   0        0        0     4977 2023-06-14 22:17:55.360593 docx2python-2.7.2/docx2python/attribute_register.py
--rw-r--r--   0        0        0     5272 2023-01-19 19:29:25.944712 docx2python-2.7.2/docx2python/bullets_and_numbering.py
--rw-r--r--   0        0        0     9246 2023-05-03 15:35:58.417678 docx2python-2.7.2/docx2python/depth_collector.py
--rw-r--r--   0        0        0     6857 2023-04-27 14:43:36.300114 docx2python-2.7.2/docx2python/docx_context.py
--rw-r--r--   0        0        0     8410 2023-01-27 18:14:24.180137 docx2python-2.7.2/docx2python/docx_output.py
--rw-r--r--   0        0        0    16656 2023-01-23 22:13:46.338596 docx2python-2.7.2/docx2python/docx_reader.py
--rw-r--r--   0        0        0    10473 2023-06-16 01:58:00.213479 docx2python-2.7.2/docx2python/docx_text.py
--rw-r--r--   0        0        0     3244 2023-01-19 19:29:25.947556 docx2python-2.7.2/docx2python/forms.py
--rw-r--r--   0        0        0     9725 2023-01-19 19:29:25.947999 docx2python-2.7.2/docx2python/iterators.py
--rw-r--r--   0        0        0     1939 2023-01-23 22:13:46.340597 docx2python-2.7.2/docx2python/main.py
--rw-r--r--   0        0        0     5291 2023-01-19 19:29:25.949121 docx2python-2.7.2/docx2python/merge_runs.py
--rw-r--r--   0        0        0     2942 2023-06-14 22:17:55.361917 docx2python-2.7.2/docx2python/namespace.py
--rw-r--r--   0        0        0     3587 2023-01-19 19:29:25.949556 docx2python-2.7.2/docx2python/numbering_formats.py
--rw-r--r--   0        0        0        0 2023-02-03 22:08:10.380704 docx2python-2.7.2/docx2python/py.typed
--rw-r--r--   0        0        0    10053 2023-01-23 22:13:46.340597 docx2python-2.7.2/docx2python/text_runs.py
--rw-r--r--   0        0        0     4525 2023-04-27 14:43:36.301404 docx2python-2.7.2/docx2python/utilities.py
--rw-r--r--   0        0        0     1097 2023-01-19 19:29:25.942725 docx2python-2.7.2/LICENSE.txt
--rw-r--r--   0        0        0     1486 2023-06-16 02:38:10.617710 docx2python-2.7.2/pyproject.toml
--rw-r--r--   0        0        0    13515 2023-06-16 01:42:45.207612 docx2python-2.7.2/README.md
--rw-r--r--   0        0        0    13730 1970-01-01 00:00:00.000000 docx2python-2.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-17 22:58:58.043164 docx2python-2.7.3/LICENSE.txt
+-rw-r--r--   0        0        0    13157 2023-06-17 22:58:58.043164 docx2python-2.7.3/README.md
+-rw-r--r--   0        0        0      229 2023-06-17 22:58:58.043164 docx2python-2.7.3/docx2python/__init__.py
+-rw-r--r--   0        0        0     4832 2023-06-17 22:58:58.043164 docx2python-2.7.3/docx2python/attribute_register.py
+-rw-r--r--   0        0        0     5116 2023-06-17 22:58:58.043164 docx2python-2.7.3/docx2python/bullets_and_numbering.py
+-rw-r--r--   0        0        0     8968 2023-06-17 22:58:58.043164 docx2python-2.7.3/docx2python/depth_collector.py
+-rw-r--r--   0        0        0     6656 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/docx_context.py
+-rw-r--r--   0        0        0     8148 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/docx_output.py
+-rw-r--r--   0        0        0    16197 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/docx_reader.py
+-rw-r--r--   0        0        0    10181 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/docx_text.py
+-rw-r--r--   0        0        0     3155 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/forms.py
+-rw-r--r--   0        0        0     9416 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/iterators.py
+-rw-r--r--   0        0        0     1887 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/main.py
+-rw-r--r--   0        0        0     5137 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/merge_runs.py
+-rw-r--r--   0        0        0     2861 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/namespace.py
+-rw-r--r--   0        0        0     3456 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/numbering_formats.py
+-rw-r--r--   0        0        0        0 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/py.typed
+-rw-r--r--   0        0        0     9754 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/text_runs.py
+-rw-r--r--   0        0        0     4394 2023-06-17 22:58:58.047164 docx2python-2.7.3/docx2python/utilities.py
+-rw-r--r--   0        0        0     1426 2023-06-17 22:58:58.047164 docx2python-2.7.3/pyproject.toml
+-rw-r--r--   0        0        0    13730 1970-01-01 00:00:00.000000 docx2python-2.7.3/PKG-INFO
```

### Comparing `docx2python-2.7.2/docx2python/attribute_register.py` & `docx2python-2.7.3/docx2python/attribute_register.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-""" The tags and attributes docx2python knows how to handle.
-
-:author: Shay Hill
-:created: 3/18/2021
-
-A lot of the information in a docx file isn't text or text attributes. Docx files
-record spelling errors, revision history, etc. Docx2Python will ignore (by design)
-much of this.
-"""
-from enum import Enum
-from typing import Callable, Iterator, NamedTuple, Optional
-
-from lxml.etree import _Element as EtreeElement  # type: ignore
-
-from .namespace import qn
-
-
-class HtmlFormatter(NamedTuple):
-    """
-    The information needed to group and format html tags.
-
-    If a text run has multiple span attributes, Docx2Python does not open multiple
-    span elements.
-
-    ``<span style="font-size:12"><span style="font-weight:bold"> ...``
-
-    Instead, these elements are first grouped by self.container, then by
-    self.property, then printed all together.
-
-    ``<span style="font-size:12;font-weight:bold">``
-
-    This makes a more-readable text extraction, but it does involve passing these
-    HtmlFormatter instances around A LOT.
-
-    Formatting in the xml file will appear as child elements of an rPr or pPr element:
-
-    ``<w:sz w:val="32"/>``
-
-    self.formatter will be a function that takes the element tag name (here ``sz``)
-    and element ``w:val`` attribute (here ``"32"``).
-    """
-
-    formatter: Callable[[str, str], str] = lambda tag, val: tag
-    container: Optional[str] = None  # e.g., 'span'
-    property_: Optional[str] = None  # e.g., 'style'
-
-
-# An HtmlFormatter instance for every xml format Docx2Python recognizes.
-# This mapping can be extended from outside by
-#
-#     import docx2python
-#     docx2python.attribute_register.xml2html_formatter[xml_format] =
-#         docx2python.attribute_register.HtmlFormatter(args)
-XML2HTML_FORMATTER = {
-    "b": HtmlFormatter(),
-    "i": HtmlFormatter(),
-    "u": HtmlFormatter(),
-    "strike": HtmlFormatter(lambda tag, val: "s"),
-    "vertAlign": HtmlFormatter(lambda tag, val: val[:3]),  # subscript and superscript
-    "smallCaps": HtmlFormatter(
-        lambda tag, val: "font-variant:small-caps", "span", "style"
-    ),
-    "caps": HtmlFormatter(lambda tag, val: "text-transform:uppercase", "span", "style"),
-    "highlight": HtmlFormatter(
-        lambda tag, val: f"background-color:{val}", "span", "style"
-    ),
-    "sz": HtmlFormatter(lambda tag, val: f"font-size:{val}pt", "span", "style"),
-    "color": HtmlFormatter(lambda tag, val: f"color:{val}", "span", "style"),
-    "Heading1": HtmlFormatter(lambda tag, val: "h1"),
-    "Heading2": HtmlFormatter(lambda tag, val: "h2"),
-    "Heading3": HtmlFormatter(lambda tag, val: "h3"),
-    "Heading4": HtmlFormatter(lambda tag, val: "h4"),
-    "Heading5": HtmlFormatter(lambda tag, val: "h5"),
-    "Heading6": HtmlFormatter(lambda tag, val: "h6"),
-}
-
-
-class Tags(str, Enum):
-    """
-    These are the tags that provoke some action in docx2python.
-    """
-
-    BODY = qn("w:body")
-    BR = qn("w:br")
-    DOCUMENT = qn("w:document")
-    ENDNOTE = qn("w:endnote")
-    ENDNOTE_REFERENCE = qn("w:endnoteReference")
-    FOOTNOTE = qn("w:footnote")
-    FOOTNOTE_REFERENCE = qn("w:footnoteReference")
-    FORM_CHECKBOX = qn("w:checkBox")
-    FORM_DDLIST = qn("w:ddList")  # drop-down form
-    HYPERLINK = qn("w:hyperlink")
-    IMAGE = qn("a:blip")
-    IMAGE_ALT = qn("wp:docPr")
-    IMAGEDATA = qn("v:imagedata")
-    MATH = qn("m:oMath")
-    PARAGRAPH = qn("w:p")
-    PAR_PROPERTIES = qn("w:pPr")
-    RUN = qn("w:r")
-    RUN_PROPERTIES = qn("w:rPr")
-    SYM = qn("w:sym")
-    TAB = qn("w:tab")
-    TABLE = qn("w:tbl")
-    TABLE_CELL = qn("w:tc")
-    TABLE_ROW = qn("w:tr")
-    TEXT = qn("w:t")
-    TEXT_MATH = qn("m:t")
-
-
-# elem.attrib key for relationship ids. These can find the information they reference by
-# ``file_instance.rels[elem.attrib[RELS_ID]]``
-RELS_ID = qn("r:id")
-
-_CONTENT_TAGS = set(Tags) - {Tags.RUN_PROPERTIES, Tags.PAR_PROPERTIES}
-
-
-def has_content(tree: EtreeElement) -> Optional[str]:
-    """
-    Does the element have any descendent content elements?
-
-    :param tree: xml element
-    :return: first content tag found or None if no content tags are found
-
-    This is to check for text in any skipped elements.
-
-    Docx2Python ignores spell check, revision, and other elements. This function checks
-    that no content (paragraphs, run, text, link, ...) is contained in children of any
-    ignored elements.
-
-    If no content is found, the element can be safely ignored going forward.
-    """
-
-    def iter_content(tree_: EtreeElement) -> Iterator[str]:
-        """Yield all content elements in tree
-
-        :param tree_: xml element
-        :yield: child content elements
-        :return: None
-        """
-        if tree_.tag in _CONTENT_TAGS:
-            yield tree_.tag
-        for branch in tree_:
-            yield from iter_content(branch)
-
-    return next(iter_content(tree), None)
+""" The tags and attributes docx2python knows how to handle.
+
+:author: Shay Hill
+:created: 3/18/2021
+
+A lot of the information in a docx file isn't text or text attributes. Docx files
+record spelling errors, revision history, etc. Docx2Python will ignore (by design)
+much of this.
+"""
+from enum import Enum
+from typing import Callable, Iterator, NamedTuple, Optional
+
+from lxml.etree import _Element as EtreeElement  # type: ignore
+
+from .namespace import qn
+
+
+class HtmlFormatter(NamedTuple):
+    """
+    The information needed to group and format html tags.
+
+    If a text run has multiple span attributes, Docx2Python does not open multiple
+    span elements.
+
+    ``<span style="font-size:12"><span style="font-weight:bold"> ...``
+
+    Instead, these elements are first grouped by self.container, then by
+    self.property, then printed all together.
+
+    ``<span style="font-size:12;font-weight:bold">``
+
+    This makes a more-readable text extraction, but it does involve passing these
+    HtmlFormatter instances around A LOT.
+
+    Formatting in the xml file will appear as child elements of an rPr or pPr element:
+
+    ``<w:sz w:val="32"/>``
+
+    self.formatter will be a function that takes the element tag name (here ``sz``)
+    and element ``w:val`` attribute (here ``"32"``).
+    """
+
+    formatter: Callable[[str, str], str] = lambda tag, val: tag
+    container: Optional[str] = None  # e.g., 'span'
+    property_: Optional[str] = None  # e.g., 'style'
+
+
+# An HtmlFormatter instance for every xml format Docx2Python recognizes.
+# This mapping can be extended from outside by
+#
+#     import docx2python
+#     docx2python.attribute_register.xml2html_formatter[xml_format] =
+#         docx2python.attribute_register.HtmlFormatter(args)
+XML2HTML_FORMATTER = {
+    "b": HtmlFormatter(),
+    "i": HtmlFormatter(),
+    "u": HtmlFormatter(),
+    "strike": HtmlFormatter(lambda tag, val: "s"),
+    "vertAlign": HtmlFormatter(lambda tag, val: val[:3]),  # subscript and superscript
+    "smallCaps": HtmlFormatter(
+        lambda tag, val: "font-variant:small-caps", "span", "style"
+    ),
+    "caps": HtmlFormatter(lambda tag, val: "text-transform:uppercase", "span", "style"),
+    "highlight": HtmlFormatter(
+        lambda tag, val: f"background-color:{val}", "span", "style"
+    ),
+    "sz": HtmlFormatter(lambda tag, val: f"font-size:{val}pt", "span", "style"),
+    "color": HtmlFormatter(lambda tag, val: f"color:{val}", "span", "style"),
+    "Heading1": HtmlFormatter(lambda tag, val: "h1"),
+    "Heading2": HtmlFormatter(lambda tag, val: "h2"),
+    "Heading3": HtmlFormatter(lambda tag, val: "h3"),
+    "Heading4": HtmlFormatter(lambda tag, val: "h4"),
+    "Heading5": HtmlFormatter(lambda tag, val: "h5"),
+    "Heading6": HtmlFormatter(lambda tag, val: "h6"),
+}
+
+
+class Tags(str, Enum):
+    """
+    These are the tags that provoke some action in docx2python.
+    """
+
+    BODY = qn("w:body")
+    BR = qn("w:br")
+    DOCUMENT = qn("w:document")
+    ENDNOTE = qn("w:endnote")
+    ENDNOTE_REFERENCE = qn("w:endnoteReference")
+    FOOTNOTE = qn("w:footnote")
+    FOOTNOTE_REFERENCE = qn("w:footnoteReference")
+    FORM_CHECKBOX = qn("w:checkBox")
+    FORM_DDLIST = qn("w:ddList")  # drop-down form
+    HYPERLINK = qn("w:hyperlink")
+    IMAGE = qn("a:blip")
+    IMAGE_ALT = qn("wp:docPr")
+    IMAGEDATA = qn("v:imagedata")
+    MATH = qn("m:oMath")
+    PARAGRAPH = qn("w:p")
+    PAR_PROPERTIES = qn("w:pPr")
+    RUN = qn("w:r")
+    RUN_PROPERTIES = qn("w:rPr")
+    SYM = qn("w:sym")
+    TAB = qn("w:tab")
+    TABLE = qn("w:tbl")
+    TABLE_CELL = qn("w:tc")
+    TABLE_ROW = qn("w:tr")
+    TEXT = qn("w:t")
+    TEXT_MATH = qn("m:t")
+
+
+# elem.attrib key for relationship ids. These can find the information they reference by
+# ``file_instance.rels[elem.attrib[RELS_ID]]``
+RELS_ID = qn("r:id")
+
+_CONTENT_TAGS = set(Tags) - {Tags.RUN_PROPERTIES, Tags.PAR_PROPERTIES}
+
+
+def has_content(tree: EtreeElement) -> Optional[str]:
+    """
+    Does the element have any descendent content elements?
+
+    :param tree: xml element
+    :return: first content tag found or None if no content tags are found
+
+    This is to check for text in any skipped elements.
+
+    Docx2Python ignores spell check, revision, and other elements. This function checks
+    that no content (paragraphs, run, text, link, ...) is contained in children of any
+    ignored elements.
+
+    If no content is found, the element can be safely ignored going forward.
+    """
+
+    def iter_content(tree_: EtreeElement) -> Iterator[str]:
+        """Yield all content elements in tree
+
+        :param tree_: xml element
+        :yield: child content elements
+        :return: None
+        """
+        if tree_.tag in _CONTENT_TAGS:
+            yield tree_.tag
+        for branch in tree_:
+            yield from iter_content(branch)
+
+    return next(iter_content(tree), None)
```

### Comparing `docx2python-2.7.2/docx2python/bullets_and_numbering.py` & `docx2python-2.7.3/docx2python/bullets_and_numbering.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-""" Generate bullet and numbered-list strings.
-
-:author: Shay Hill
-:created: 11/15/2021
-
-Docx xml files do not track explicit numbering values. Each numbered paragraph has ::
-
-    <w:ilvl w:val="0"/>   # indentation level
-    <w:numId w:val="9"/>  # index to a list [by ilvl] of numbered-list formats
-
-Docx2Python keeps track of current numbering value, and increments these values as
-numbered paragraphs are encountered. If extracting partial text, the numbers may be
-incorrect, because all paragraphs in a numbered-list format may not be encountered
-during the extraction.
-"""
-from __future__ import annotations
-
-import warnings
-from collections import defaultdict
-from typing import Callable
-
-from lxml.etree import _Element as EtreeElement  # type: ignore
-
-from docx2python import numbering_formats as nums
-from docx2python.namespace import qn
-
-
-def _get_bullet_function(numFmt: str) -> Callable[[int], str]:
-    """Select a bullet or numbering format function from xml numFmt.
-
-    :param numFmt: xml numFmt (e.g., decimal, lowerLetter)
-    :return: a function that takes an int and returns a string. If numFmt is not
-        recognized, treat numbers as bullets.
-    """
-    numFmt2bullet_function: dict[str, Callable[[int], str]] = {
-        "decimal": nums.decimal,
-        "lowerLetter": nums.lower_letter,
-        "upperLetter": nums.upper_letter,
-        "lowerRoman": nums.lower_roman,
-        "upperRoman": nums.upper_roman,
-        "bullet": nums.bullet,
-    }
-    try:
-        retval_: Callable[[int], str] = numFmt2bullet_function[numFmt]
-        return retval_
-    except KeyError:
-        warnings.warn(
-            f"{numFmt} numbering format not implemented, "
-            + f"substituting '{nums.bullet()}'"
-        )
-        return nums.bullet
-
-
-def _new_list_counter() -> defaultdict[str, defaultdict[str, int]]:
-    """
-    A counter, starting at zero, for each numId
-
-    :return: {
-        a_numId: 0,
-        b_numId: 0
-    }
-
-    This is what you need to keep track of where every nested list is at.
-    """
-    return defaultdict(lambda: defaultdict(lambda: 0))
-
-
-def _increment_list_counter(ilvl2count: defaultdict[str, int], ilvl: str) -> int:
-    """
-    Increase counter at ilvl, reset counter at deeper levels.
-
-    :param ilvl2count: context['numId2count']
-    :param ilvl: string representing an integer
-    :return: updated count at ilvl.
-        updates context['numId2count'] by reference
-
-    On a numbered list, the count for sub-lists should reset when a parent list
-    increases, e.g.,
-
-    1. top-level list
-        a. sublist
-        b. sublist continues
-    2. back to top-level list
-        a. sublist counter has been reset
-
-    List counters are defaultdicts, so we can reset sublist counters by deleting
-    them.
-    """
-    ilvl2count[ilvl] += 1
-    deeper_levels = [x for x in ilvl2count.keys() if x > ilvl]
-    for level in deeper_levels:
-        del ilvl2count[level]
-    return ilvl2count[ilvl]
-
-
-class BulletGenerator:
-    """
-    Keep track of list counters and generate bullet strings.
-    """
-
-    def __init__(self, numId2numFmts: dict[str, list[str]]) -> None:
-        """
-        Set numId2numFmts. Initiate counters.
-        """
-        self.numId2numFmts = numId2numFmts
-        self.numId2count = _new_list_counter()
-
-    def get_bullet(self, paragraph: EtreeElement) -> str:
-        """
-        Get bullet string if paragraph is numbered. (e.g, '--  ' or '1)  ')
-
-        :param paragraph: <w:p> xml element
-        :return: specified 'bullet' string or '' if paragraph is not numbered
-
-        <w:p>
-            <w:pPr>
-                <w:numPr>
-                    <w:ilvl w:val="0"/>
-                    <w:numId w:val="9"/>
-                </w:numPr>
-            </wpPr>
-            <w:r>
-                <w:t>this text in numbered or bulleted list
-                </w:t>
-            </w:r>
-        </w:p>
-
-        bullet preceded by one tab for every indentation level.
-        """
-        try:
-            pPr = next(paragraph.iterfind(qn("w:pPr")))
-            numPr = next(pPr.iterfind(qn("w:numPr")))
-            numId = next(numPr.iterfind(qn("w:numId"))).attrib[qn("w:val")]
-            ilvl = next(numPr.iterfind(qn("w:ilvl"))).attrib[qn("w:val")]
-            try:
-                numFmt = self.numId2numFmts[str(numId)][int(ilvl)]
-            except IndexError:
-                # give up and put a bullet
-                numFmt = "bullet"
-        except (StopIteration, KeyError):
-            # not a numbered paragraph
-            return ""
-
-        def format_bullet(bullet: str) -> str:
-            """Indent, format and pad the bullet or number string.
-
-            :param bullet: any kind of list-item string (bullet, number, Roman, ...)
-            :return: formatted bullet string
-            """
-            if bullet != nums.bullet():
-                bullet += ")"
-            return "\t" * int(ilvl) + bullet + "\t"
-
-        number = _increment_list_counter(self.numId2count[numId], str(ilvl))
-        get_unformatted_bullet_str = _get_bullet_function(numFmt)
-        return format_bullet(get_unformatted_bullet_str(number))
+""" Generate bullet and numbered-list strings.
+
+:author: Shay Hill
+:created: 11/15/2021
+
+Docx xml files do not track explicit numbering values. Each numbered paragraph has ::
+
+    <w:ilvl w:val="0"/>   # indentation level
+    <w:numId w:val="9"/>  # index to a list [by ilvl] of numbered-list formats
+
+Docx2Python keeps track of current numbering value, and increments these values as
+numbered paragraphs are encountered. If extracting partial text, the numbers may be
+incorrect, because all paragraphs in a numbered-list format may not be encountered
+during the extraction.
+"""
+from __future__ import annotations
+
+import warnings
+from collections import defaultdict
+from typing import Callable
+
+from lxml.etree import _Element as EtreeElement  # type: ignore
+
+from docx2python import numbering_formats as nums
+from docx2python.namespace import qn
+
+
+def _get_bullet_function(numFmt: str) -> Callable[[int], str]:
+    """Select a bullet or numbering format function from xml numFmt.
+
+    :param numFmt: xml numFmt (e.g., decimal, lowerLetter)
+    :return: a function that takes an int and returns a string. If numFmt is not
+        recognized, treat numbers as bullets.
+    """
+    numFmt2bullet_function: dict[str, Callable[[int], str]] = {
+        "decimal": nums.decimal,
+        "lowerLetter": nums.lower_letter,
+        "upperLetter": nums.upper_letter,
+        "lowerRoman": nums.lower_roman,
+        "upperRoman": nums.upper_roman,
+        "bullet": nums.bullet,
+    }
+    try:
+        retval_: Callable[[int], str] = numFmt2bullet_function[numFmt]
+        return retval_
+    except KeyError:
+        warnings.warn(
+            f"{numFmt} numbering format not implemented, "
+            + f"substituting '{nums.bullet()}'"
+        )
+        return nums.bullet
+
+
+def _new_list_counter() -> defaultdict[str, defaultdict[str, int]]:
+    """
+    A counter, starting at zero, for each numId
+
+    :return: {
+        a_numId: 0,
+        b_numId: 0
+    }
+
+    This is what you need to keep track of where every nested list is at.
+    """
+    return defaultdict(lambda: defaultdict(lambda: 0))
+
+
+def _increment_list_counter(ilvl2count: defaultdict[str, int], ilvl: str) -> int:
+    """
+    Increase counter at ilvl, reset counter at deeper levels.
+
+    :param ilvl2count: context['numId2count']
+    :param ilvl: string representing an integer
+    :return: updated count at ilvl.
+        updates context['numId2count'] by reference
+
+    On a numbered list, the count for sub-lists should reset when a parent list
+    increases, e.g.,
+
+    1. top-level list
+        a. sublist
+        b. sublist continues
+    2. back to top-level list
+        a. sublist counter has been reset
+
+    List counters are defaultdicts, so we can reset sublist counters by deleting
+    them.
+    """
+    ilvl2count[ilvl] += 1
+    deeper_levels = [x for x in ilvl2count.keys() if x > ilvl]
+    for level in deeper_levels:
+        del ilvl2count[level]
+    return ilvl2count[ilvl]
+
+
+class BulletGenerator:
+    """
+    Keep track of list counters and generate bullet strings.
+    """
+
+    def __init__(self, numId2numFmts: dict[str, list[str]]) -> None:
+        """
+        Set numId2numFmts. Initiate counters.
+        """
+        self.numId2numFmts = numId2numFmts
+        self.numId2count = _new_list_counter()
+
+    def get_bullet(self, paragraph: EtreeElement) -> str:
+        """
+        Get bullet string if paragraph is numbered. (e.g, '--  ' or '1)  ')
+
+        :param paragraph: <w:p> xml element
+        :return: specified 'bullet' string or '' if paragraph is not numbered
+
+        <w:p>
+            <w:pPr>
+                <w:numPr>
+                    <w:ilvl w:val="0"/>
+                    <w:numId w:val="9"/>
+                </w:numPr>
+            </wpPr>
+            <w:r>
+                <w:t>this text in numbered or bulleted list
+                </w:t>
+            </w:r>
+        </w:p>
+
+        bullet preceded by one tab for every indentation level.
+        """
+        try:
+            pPr = next(paragraph.iterfind(qn("w:pPr")))
+            numPr = next(pPr.iterfind(qn("w:numPr")))
+            numId = next(numPr.iterfind(qn("w:numId"))).attrib[qn("w:val")]
+            ilvl = next(numPr.iterfind(qn("w:ilvl"))).attrib[qn("w:val")]
+            try:
+                numFmt = self.numId2numFmts[str(numId)][int(ilvl)]
+            except IndexError:
+                # give up and put a bullet
+                numFmt = "bullet"
+        except (StopIteration, KeyError):
+            # not a numbered paragraph
+            return ""
+
+        def format_bullet(bullet: str) -> str:
+            """Indent, format and pad the bullet or number string.
+
+            :param bullet: any kind of list-item string (bullet, number, Roman, ...)
+            :return: formatted bullet string
+            """
+            if bullet != nums.bullet():
+                bullet += ")"
+            return "\t" * int(ilvl) + bullet + "\t"
+
+        number = _increment_list_counter(self.numId2count[numId], str(ilvl))
+        get_unformatted_bullet_str = _get_bullet_function(numFmt)
+        return format_bullet(get_unformatted_bullet_str(number))
```

### Comparing `docx2python-2.7.2/docx2python/depth_collector.py` & `docx2python-2.7.3/docx2python/depth_collector.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-"""Collect xml text in a nested list
-
-:author: Shay Hill
-:created: 6/26/2019
-
-::
-
-    [  # tables
-        [  # table
-            [  # row
-                [  # cell
-                    [  # paragraph
-                        ""  # text run
-                    ]
-                ]
-            ]
-        ]
-    ]
-
-Text in table cells and text outside of a table must be captured at depth=5. To keep
-track of this, these few methods will put text where it needs to be.
-
-The package will recursively descend into elements in the docx file, so the point at
-which a table, row, cell, paragraph, or text run begins and ends is known. Drop and
-raise the caret when these items are opened or closed in the xml. Insert text when
-found.
-
-Shorthand for this package. Instances of this class should not escape the package.
-Pass out of package with depth_collector_instance.tree.
-"""
-
-from __future__ import annotations
-
-from contextlib import suppress
-from dataclasses import dataclass, field
-from typing import Any, Iterable
-
-from .text_runs import html_close, html_open
-
-
-@dataclass
-class Run:
-    """A text run. Html styles and text content"""
-
-    html_style: list[str] = field(default_factory=list)
-    text: str = field(default="")
-
-    def __str__(self) -> str:
-        """Return any text content in the run
-
-        :return: text content or "" if none
-        """
-        if self.text:
-            return html_open(self.html_style) + self.text + html_close(self.html_style)
-        return ""
-
-
-@dataclass
-class Par:
-    """A text paragraph. Html styles and a list of run strings"""
-
-    html_style: list[str]
-    runs: list[Run] = field(default_factory=list)
-
-    @property
-    def strings(self) -> list[str]:
-        """Return a list of strings from the runs
-
-        :return: a string for each run with text content
-        """
-        return [x for x in (str(y) for y in self.runs) if x]
-
-
-class CaretDepthError(Exception):
-    """Caller attempted to raise or lower DepthCollector caret out of range"""
-
-
-class DepthCollector:
-    """Insert items into a tree at a consistent depth."""
-
-    def __init__(self, item_depth: int) -> None:
-        """
-        Record item depth and initiate data container.
-
-        :param item_depth: content will only appear at this depth, though empty lists
-            may appear above. I.e., this is how many brackets to open before inserting
-            an item. E.g., item_depth = 3 => [[['item']]].
-        """
-        # TODO: factor out item_depth
-        self.item_depth = item_depth
-        self._par_depth = 4
-
-        self._rightmost_branches: list[Any] = [[]]
-
-        self.open_pars: list[Par] = []
-        self.orphan_runs: list[Run] = []
-
-    def view_branch(self, address: Iterable[int]) -> Any:
-        """Return the item at the given address
-
-        :param address: a tuple of indices to the item to be returned
-        :return: the item at the address
-        """
-        branch = self._rightmost_branches
-        for i in address:
-            branch = branch[i]
-        return branch
-
-    @staticmethod
-    def _get_run_strings(runs: list[Run]) -> list[str]:
-        """Return a string for each run in the current open paragraph. Ignore ""
-
-        :param runs: list of runs
-        :return: a string for each run with text content
-        """
-        return [x for x in (str(x) for x in runs) if x]
-
-    def commence_paragraph(self, html_style: list[str] | None = None) -> Par:
-        """Gather any cached runs and open a new paragraph.
-
-        :param html_style: html style to apply to the paragraph
-        :return: the new paragraph
-        """
-        html_style = html_style or []
-        new_par = Par(html_style, self.orphan_runs + [Run([], html_open(html_style))])
-        self.orphan_runs = []
-        self.open_pars.append(new_par)
-        return new_par
-
-    def conclude_paragraph(self) -> None:
-        """Close the current paragraph and add it to the tree."""
-        old_par = self.open_pars.pop()
-        old_par.runs.append(Run([], html_close(old_par.html_style)))
-        self.insert(old_par.strings)
-
-    def commence_run(self, html_style: list[str] | None = None) -> None:
-        """Open a new run and add it to the current paragraph.
-
-        :param html_style: html style to apply to the run
-        """
-        self._open_runs.append(Run(html_style or []))
-
-    def conclude_run(self) -> None:
-        """Close the current run and add it to the current paragraph."""
-        self.commence_run()
-
-    @property
-    def tree(self) -> list[str | list[str]]:
-        """All collected items.
-
-        :return: a nested list of _par_depth + 1 levels
-        """
-        return self._rightmost_branches[0]
-
-    @property
-    def caret(self) -> list[str | list[str]]:
-        """Lowest open child.
-
-        :return: the list where new content will be appended
-        """
-        return self._rightmost_branches[-1]
-
-    @property
-    def caret_depth(self) -> int:
-        """Depth of the lowest open child.
-
-        :return: from 0 to _par_depth, the depth of the last-closed element in the
-            tree.
-        """
-        return len(self._rightmost_branches)
-
-    @property
-    def _open_runs(self) -> list[Run]:
-        """Runs in the current paragraph.
-
-        :return: a list of runs
-        """
-        with suppress(IndexError):
-            return self.open_pars[-1].runs
-        return self.orphan_runs
-
-    @property
-    def _open_run(self) -> Run:
-        """The last run in the current paragraph.
-
-        :return: a run
-        """
-        if not self._open_runs:
-            self._open_runs.append(Run())
-        return self._open_runs[-1]
-
-    def _drop_caret(self) -> None:
-        """Create a new branch under caret.
-
-        :raise CaretDepthError: if caret is already at the maximum depth
-        :return: None
-        """
-        if self.caret_depth >= self.item_depth:
-            raise CaretDepthError("will not lower caret beneath item_depth")
-        self._rightmost_branches[-1].append([])
-        self._rightmost_branches.append(self._rightmost_branches[-1][-1])
-
-    def _raise_caret(self) -> None:
-        """Close branch at caret and move up to parent.
-
-        :raise CaretDepthError: if there is no outside list to which to ascend
-        """
-        if self.caret_depth == 1:
-            raise CaretDepthError("will not raise caret above root")
-        self._rightmost_branches = self._rightmost_branches[:-1]
-
-    def set_caret(self, depth: None | int) -> None:
-        """
-        Set caret at given depth.
-
-        :param depth: depth level for caret (between 1 and item_depth inclusive)
-            another at the same depth. This is how consecutive paragraphs avoid being
-            merged into one paragraph. You'll want this true for every element except
-            text runs. :depth: == None means the element (perhaps ``body``) does not
-            effect depth (see details in docx_text._get_elem_depth).
-        """
-        if depth is None:
-            return
-        while self.caret_depth < depth:
-            self._drop_caret()
-        while self.caret_depth > depth:
-            self._raise_caret()
-
-    def insert(self, item: list[str]) -> None:
-        """Add item at self._par_depth. Add branches if necessary to reach depth.
-
-        :param item: list of strings to insert at caret
-
-        This dumps the contents of the most recently closed paragraph into the
-        _rightmost_branches collector.
-        """
-        self.set_caret(self._par_depth)
-        self._rightmost_branches[-1].append(item)
-
-    def add_text_into_open_run(self, item: str) -> None:
-        """
-        Add item into previous run.
-
-        :param item: string to insert into previous run
-
-        This is for tags and other text that appears between run tags. All entries to
-        ``add_text_into_open_run`` will be merged together.
-        """
-        self._open_run.text += item
-
-    def insert_text_as_new_run(self, item: str, styled: bool = False) -> None:
-        """
-        Close previous run, cache style, open and close new run, re-open cached style.
-
-        :param item: string to insert into new run
-        :param styled: True if item has associated html styles
-
-        This is for items like links that may be inside a run element with other text.
-
-        Paraphrased in html:
-
-            <run><b>some text<a href="">link</a>other text</b></run>
-
-        Starts with an open run
-            <run><b>some text
-
-        Then hits the link. We'll make this a run inside the actual run
-
-            <run><b>some text</b></run>  # close this open run
-            <run><a href="">link</a></run>  # add link as a new run
-            <run><b>  # open a new run with the same style as the aborted first run
-        """
-        open_style = self._open_run.html_style
-        if styled:
-            self._open_runs.append(Run(open_style, item))
-        else:
-            self._open_runs.append(Run([], item))
-        self._open_runs.append(Run(open_style))
+"""Collect xml text in a nested list
+
+:author: Shay Hill
+:created: 6/26/2019
+
+::
+
+    [  # tables
+        [  # table
+            [  # row
+                [  # cell
+                    [  # paragraph
+                        ""  # text run
+                    ]
+                ]
+            ]
+        ]
+    ]
+
+Text in table cells and text outside of a table must be captured at depth=5. To keep
+track of this, these few methods will put text where it needs to be.
+
+The package will recursively descend into elements in the docx file, so the point at
+which a table, row, cell, paragraph, or text run begins and ends is known. Drop and
+raise the caret when these items are opened or closed in the xml. Insert text when
+found.
+
+Shorthand for this package. Instances of this class should not escape the package.
+Pass out of package with depth_collector_instance.tree.
+"""
+
+from __future__ import annotations
+
+from contextlib import suppress
+from dataclasses import dataclass, field
+from typing import Any, Iterable
+
+from .text_runs import html_close, html_open
+
+
+@dataclass
+class Run:
+    """A text run. Html styles and text content"""
+
+    html_style: list[str] = field(default_factory=list)
+    text: str = field(default="")
+
+    def __str__(self) -> str:
+        """Return any text content in the run
+
+        :return: text content or "" if none
+        """
+        if self.text:
+            return html_open(self.html_style) + self.text + html_close(self.html_style)
+        return ""
+
+
+@dataclass
+class Par:
+    """A text paragraph. Html styles and a list of run strings"""
+
+    html_style: list[str]
+    runs: list[Run] = field(default_factory=list)
+
+    @property
+    def strings(self) -> list[str]:
+        """Return a list of strings from the runs
+
+        :return: a string for each run with text content
+        """
+        return [x for x in (str(y) for y in self.runs) if x]
+
+
+class CaretDepthError(Exception):
+    """Caller attempted to raise or lower DepthCollector caret out of range"""
+
+
+class DepthCollector:
+    """Insert items into a tree at a consistent depth."""
+
+    def __init__(self, item_depth: int) -> None:
+        """
+        Record item depth and initiate data container.
+
+        :param item_depth: content will only appear at this depth, though empty lists
+            may appear above. I.e., this is how many brackets to open before inserting
+            an item. E.g., item_depth = 3 => [[['item']]].
+        """
+        # TODO: factor out item_depth
+        self.item_depth = item_depth
+        self._par_depth = 4
+
+        self._rightmost_branches: list[Any] = [[]]
+
+        self.open_pars: list[Par] = []
+        self.orphan_runs: list[Run] = []
+
+    def view_branch(self, address: Iterable[int]) -> Any:
+        """Return the item at the given address
+
+        :param address: a tuple of indices to the item to be returned
+        :return: the item at the address
+        """
+        branch = self._rightmost_branches
+        for i in address:
+            branch = branch[i]
+        return branch
+
+    @staticmethod
+    def _get_run_strings(runs: list[Run]) -> list[str]:
+        """Return a string for each run in the current open paragraph. Ignore ""
+
+        :param runs: list of runs
+        :return: a string for each run with text content
+        """
+        return [x for x in (str(x) for x in runs) if x]
+
+    def commence_paragraph(self, html_style: list[str] | None = None) -> Par:
+        """Gather any cached runs and open a new paragraph.
+
+        :param html_style: html style to apply to the paragraph
+        :return: the new paragraph
+        """
+        html_style = html_style or []
+        new_par = Par(html_style, self.orphan_runs + [Run([], html_open(html_style))])
+        self.orphan_runs = []
+        self.open_pars.append(new_par)
+        return new_par
+
+    def conclude_paragraph(self) -> None:
+        """Close the current paragraph and add it to the tree."""
+        old_par = self.open_pars.pop()
+        old_par.runs.append(Run([], html_close(old_par.html_style)))
+        self.insert(old_par.strings)
+
+    def commence_run(self, html_style: list[str] | None = None) -> None:
+        """Open a new run and add it to the current paragraph.
+
+        :param html_style: html style to apply to the run
+        """
+        self._open_runs.append(Run(html_style or []))
+
+    def conclude_run(self) -> None:
+        """Close the current run and add it to the current paragraph."""
+        self.commence_run()
+
+    @property
+    def tree(self) -> list[str | list[str]]:
+        """All collected items.
+
+        :return: a nested list of _par_depth + 1 levels
+        """
+        return self._rightmost_branches[0]
+
+    @property
+    def caret(self) -> list[str | list[str]]:
+        """Lowest open child.
+
+        :return: the list where new content will be appended
+        """
+        return self._rightmost_branches[-1]
+
+    @property
+    def caret_depth(self) -> int:
+        """Depth of the lowest open child.
+
+        :return: from 0 to _par_depth, the depth of the last-closed element in the
+            tree.
+        """
+        return len(self._rightmost_branches)
+
+    @property
+    def _open_runs(self) -> list[Run]:
+        """Runs in the current paragraph.
+
+        :return: a list of runs
+        """
+        with suppress(IndexError):
+            return self.open_pars[-1].runs
+        return self.orphan_runs
+
+    @property
+    def _open_run(self) -> Run:
+        """The last run in the current paragraph.
+
+        :return: a run
+        """
+        if not self._open_runs:
+            self._open_runs.append(Run())
+        return self._open_runs[-1]
+
+    def _drop_caret(self) -> None:
+        """Create a new branch under caret.
+
+        :raise CaretDepthError: if caret is already at the maximum depth
+        :return: None
+        """
+        if self.caret_depth >= self.item_depth:
+            raise CaretDepthError("will not lower caret beneath item_depth")
+        self._rightmost_branches[-1].append([])
+        self._rightmost_branches.append(self._rightmost_branches[-1][-1])
+
+    def _raise_caret(self) -> None:
+        """Close branch at caret and move up to parent.
+
+        :raise CaretDepthError: if there is no outside list to which to ascend
+        """
+        if self.caret_depth == 1:
+            raise CaretDepthError("will not raise caret above root")
+        self._rightmost_branches = self._rightmost_branches[:-1]
+
+    def set_caret(self, depth: None | int) -> None:
+        """
+        Set caret at given depth.
+
+        :param depth: depth level for caret (between 1 and item_depth inclusive)
+            another at the same depth. This is how consecutive paragraphs avoid being
+            merged into one paragraph. You'll want this true for every element except
+            text runs. :depth: == None means the element (perhaps ``body``) does not
+            effect depth (see details in docx_text._get_elem_depth).
+        """
+        if depth is None:
+            return
+        while self.caret_depth < depth:
+            self._drop_caret()
+        while self.caret_depth > depth:
+            self._raise_caret()
+
+    def insert(self, item: list[str]) -> None:
+        """Add item at self._par_depth. Add branches if necessary to reach depth.
+
+        :param item: list of strings to insert at caret
+
+        This dumps the contents of the most recently closed paragraph into the
+        _rightmost_branches collector.
+        """
+        self.set_caret(self._par_depth)
+        self._rightmost_branches[-1].append(item)
+
+    def add_text_into_open_run(self, item: str) -> None:
+        """
+        Add item into previous run.
+
+        :param item: string to insert into previous run
+
+        This is for tags and other text that appears between run tags. All entries to
+        ``add_text_into_open_run`` will be merged together.
+        """
+        self._open_run.text += item
+
+    def insert_text_as_new_run(self, item: str, styled: bool = False) -> None:
+        """
+        Close previous run, cache style, open and close new run, re-open cached style.
+
+        :param item: string to insert into new run
+        :param styled: True if item has associated html styles
+
+        This is for items like links that may be inside a run element with other text.
+
+        Paraphrased in html:
+
+            <run><b>some text<a href="">link</a>other text</b></run>
+
+        Starts with an open run
+            <run><b>some text
+
+        Then hits the link. We'll make this a run inside the actual run
+
+            <run><b>some text</b></run>  # close this open run
+            <run><a href="">link</a></run>  # add link as a new run
+            <run><b>  # open a new run with the same style as the aborted first run
+        """
+        open_style = self._open_run.html_style
+        if styled:
+            self._open_runs.append(Run(open_style, item))
+        else:
+            self._open_runs.append(Run([], item))
+        self._open_runs.append(Run(open_style))
```

### Comparing `docx2python-2.7.2/docx2python/docx_context.py` & `docx2python-2.7.3/docx2python/docx_context.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-""" Content from files that aren't ``word/document.xml``
-
-:author: Shay Hill
-:created: 6/26/2019
-
-Most of the "meat" in a docx file is in ``word/document.xml``. These functions retrieve
-numbering formats, images, and font styles from *other* files in a decompressed docx.
-"""
-from __future__ import annotations
-
-import re
-import zipfile
-
-from lxml import etree
-from lxml.etree import _Element as EtreeElement  # type: ignore
-
-from .namespace import qn
-
-
-def collect_numFmts(numFmts_root: EtreeElement) -> dict[str, list[str]]:
-    """
-    Collect abstractNum bullet formats into a dictionary
-
-    :param numFmts_root: Root element of ``word/numbering.xml``.
-    :return: numId mapped to numFmts (by ilvl)
-
-    :background:
-
-    ``word/numbering.xml`` will have two sections.
-
-    **SECTION 1** - Some abstractNum elements defining numbering formats for multiple
-    indentation levels::
-
-        <w:abstractNum w:abstractNumId="0">
-            <w:lvl w:ilvl="0"><w:numFmt w:val="decimal"/></w:lvl>
-            <w:lvl w:ilvl="1"><w:numFmt w:val="lowerLetter"/></w:lvl>
-            ...
-        </w:abstractNum>
-
-    **SECTION 2** - Some num elements, each referencing an abstractNum. Multiple nums
-    may reference the same abstractNum, but each will maintain a separate count (i.e.,
-    each numbered paragraph will start from 1, even if it shares a style with another
-    paragraph.)::
-
-        <w:num w:numId="1">
-            <w:abstractNumId w:val="0"/>
-        </w:num>
-        <w:num w:numId="2">
-            <w:abstractNumId w:val="5"/>
-        </w:num>
-
-    **E.g, Given**: *above*
-
-    **E.g., Returns**::
-
-        {
-            # -----ilvl=0------ilvl=1------ilvl=2---
-            "1": ["decimal", "lowerLetter", ...],
-            "2": ...
-        }
-    """
-    abstractNumId2numFmts: dict[str, list[str]] = {}
-
-    for abstractNum in numFmts_root.findall(qn("w:abstractNum")):
-        id_ = str(abstractNum.attrib[qn("w:abstractNumId")])
-        abstractNumId2numFmts[id_] = []
-        for lvl in abstractNum.findall(qn("w:lvl")):
-            numFmt = lvl.find(qn("w:numFmt"))
-            if numFmt is not None:
-                abstractNumId2numFmts[id_].append(str(numFmt.attrib[qn("w:val")]))
-
-    numId2numFmts: dict[str, list[str]] = {}
-    num: EtreeElement
-    for num in (x for x in numFmts_root.findall(qn("w:num"))):
-        numId = num.attrib[qn("w:numId")]
-        abstractNumId = num.find(qn("w:abstractNumId"))
-        if abstractNumId is None:
-            continue
-        abstractNumIdval = abstractNumId.attrib.get(qn("w:val"))
-        numId2numFmts[str(numId)] = abstractNumId2numFmts[str(abstractNumIdval)]
-
-    return numId2numFmts
-
-
-def collect_rels(zipf: zipfile.ZipFile) -> dict[str, list[dict[str, str]]]:
-    """
-    Map file to relId to attrib
-
-    :param zipf: created by ``zipfile.ZipFile("docx_filename")``
-    :return: a deep dictionary ``{filename: list of Relationships``
-
-    Each rel in list of Relationships is::
-
-        {
-            "Id": "rId1",
-            "Type": "http...",
-            "Target": "path to file in docx"
-        }
-
-    There are several rels files:
-
-    ``_rels/.rels``: rels related to entire structure.  The identity of
-        ``word/document.xml`` is here. (It might be called ``word/document2.xml`` or
-        something else. Checking here is the best way to make sure.)
-
-    ``word/_rels/document.xml.rels``: images, headers, etc. referenced by
-        ``word/document.xml``
-
-    ``word/_rels/header1.xml.rels``: images, etc. for ``header1.xml``
-
-    ...
-
-    Get everything from everywhere. Map ``_rels/.rels`` to ``'rels'`` and everything
-    else to e.g., ``'document'`` or ``'header'``. RelIds are **not** unique between
-    these files.
-
-    **E.g, Given**::
-
-    # one of several files
-
-        <?xml version="1.0" encoding="UTF-8" standalone="yes"?>
-        <Relationships xmlns="http://schemas.../relationships">
-            <Relationship Id="rId3" Type="http://schemas... \
-                /extended-properties" Target="docProps/app.xml"/>
-            <Relationship Id="rId2" Type="http://schemas... \
-                /core-properties" Target="docProps/core.xml"/>
-            <Relationship Id="rId1" Type="http://schemas... \
-                /officeDocument" Target="word/document.xml"/>
-            <Relationship Id="rId4" Type="http://schemas... \
-                /custom-properties" Target="docProps/custom.xml"/>
-        </Relationships>
-
-    **Returns**::
-
-        {
-            "filename": [
-                {
-                    "Id": "rId3",
-                    "Type": "http://schemas.../extended-properties",
-                    "Target": "docProps/app.xml",
-                },
-                {
-                    "Id": "rId2",
-                    "Type": "http://schemas.../core-properties",
-                    "Target": "docProps/core.xml",
-                },
-            ]
-        }
-    """
-    path2rels: dict[str, list[dict[str, str]]] = {}
-    for rels in (x for x in zipf.namelist() if x[-5:] == ".rels"):
-        path2rels[rels] = [
-            {str(y): str(z) for y, z in x.attrib.items()}
-            for x in etree.fromstring(zipf.read(rels))
-        ]
-    return path2rels
-
-
-def collect_docProps(root: EtreeElement) -> dict[str, str | None]:
-    """
-    Get author, modified, etc. from core-properties (should be docProps/core.xml)
-
-    :param root: root of the XML tree
-    :return: document property names mapped to values
-
-    **E.g., Given**::
-
-        <cp:coreProperties xmlns:cp="http://schemas.openxmlformats...">
-            <dc:title>SG-DOP-5009 - Operate ROMAR swarf unit
-            </dc:title>
-            <dc:creator>Shay Hill
-            </dc:creator>
-            <cp:lastModifiedBy>Shay Hill
-            </cp:lastModifiedBy>
-            <cp:revision>6
-            </cp:revision>
-            <cp:lastPrinted>2017-11-17T15:47:00Z
-            </cp:lastPrinted>
-            <dcterms:created xsi:type="dcterms:W3CDTF">2019-01-10T07:21:00Z
-            </dcterms:created>
-            <dcterms:modified xsi:type="dcterms:W3CDTF">2019-01-11T11:41:00Z
-            </dcterms:modified>
-        </cp:coreProperties>
-
-    **E.g., Returns**::
-
-        {
-            "title": "SG-DOP-5009 - Operate ROMAR swarf unit",
-            "creator": "Shay Hill",
-            "lastModifiedBy": "Shay Hill",
-            "revision": "6",
-            ...
-        }
-    """
-    docProp2text: dict[str, str | None] = {}
-    capture_tag_name = re.compile(r"{.+}(?P<tag_name>\w+)")
-    for dc in root:
-        tag_match = re.match(capture_tag_name, dc.tag)
-        if tag_match:
-            docProp2text[tag_match.group("tag_name")] = dc.text
-    return docProp2text
+""" Content from files that aren't ``word/document.xml``
+
+:author: Shay Hill
+:created: 6/26/2019
+
+Most of the "meat" in a docx file is in ``word/document.xml``. These functions retrieve
+numbering formats, images, and font styles from *other* files in a decompressed docx.
+"""
+from __future__ import annotations
+
+import re
+import zipfile
+
+from lxml import etree
+from lxml.etree import _Element as EtreeElement  # type: ignore
+
+from .namespace import qn
+
+
+def collect_numFmts(numFmts_root: EtreeElement) -> dict[str, list[str]]:
+    """
+    Collect abstractNum bullet formats into a dictionary
+
+    :param numFmts_root: Root element of ``word/numbering.xml``.
+    :return: numId mapped to numFmts (by ilvl)
+
+    :background:
+
+    ``word/numbering.xml`` will have two sections.
+
+    **SECTION 1** - Some abstractNum elements defining numbering formats for multiple
+    indentation levels::
+
+        <w:abstractNum w:abstractNumId="0">
+            <w:lvl w:ilvl="0"><w:numFmt w:val="decimal"/></w:lvl>
+            <w:lvl w:ilvl="1"><w:numFmt w:val="lowerLetter"/></w:lvl>
+            ...
+        </w:abstractNum>
+
+    **SECTION 2** - Some num elements, each referencing an abstractNum. Multiple nums
+    may reference the same abstractNum, but each will maintain a separate count (i.e.,
+    each numbered paragraph will start from 1, even if it shares a style with another
+    paragraph.)::
+
+        <w:num w:numId="1">
+            <w:abstractNumId w:val="0"/>
+        </w:num>
+        <w:num w:numId="2">
+            <w:abstractNumId w:val="5"/>
+        </w:num>
+
+    **E.g, Given**: *above*
+
+    **E.g., Returns**::
+
+        {
+            # -----ilvl=0------ilvl=1------ilvl=2---
+            "1": ["decimal", "lowerLetter", ...],
+            "2": ...
+        }
+    """
+    abstractNumId2numFmts: dict[str, list[str]] = {}
+
+    for abstractNum in numFmts_root.findall(qn("w:abstractNum")):
+        id_ = str(abstractNum.attrib[qn("w:abstractNumId")])
+        abstractNumId2numFmts[id_] = []
+        for lvl in abstractNum.findall(qn("w:lvl")):
+            numFmt = lvl.find(qn("w:numFmt"))
+            if numFmt is not None:
+                abstractNumId2numFmts[id_].append(str(numFmt.attrib[qn("w:val")]))
+
+    numId2numFmts: dict[str, list[str]] = {}
+    num: EtreeElement
+    for num in (x for x in numFmts_root.findall(qn("w:num"))):
+        numId = num.attrib[qn("w:numId")]
+        abstractNumId = num.find(qn("w:abstractNumId"))
+        if abstractNumId is None:
+            continue
+        abstractNumIdval = abstractNumId.attrib.get(qn("w:val"))
+        numId2numFmts[str(numId)] = abstractNumId2numFmts[str(abstractNumIdval)]
+
+    return numId2numFmts
+
+
+def collect_rels(zipf: zipfile.ZipFile) -> dict[str, list[dict[str, str]]]:
+    """
+    Map file to relId to attrib
+
+    :param zipf: created by ``zipfile.ZipFile("docx_filename")``
+    :return: a deep dictionary ``{filename: list of Relationships``
+
+    Each rel in list of Relationships is::
+
+        {
+            "Id": "rId1",
+            "Type": "http...",
+            "Target": "path to file in docx"
+        }
+
+    There are several rels files:
+
+    ``_rels/.rels``: rels related to entire structure.  The identity of
+        ``word/document.xml`` is here. (It might be called ``word/document2.xml`` or
+        something else. Checking here is the best way to make sure.)
+
+    ``word/_rels/document.xml.rels``: images, headers, etc. referenced by
+        ``word/document.xml``
+
+    ``word/_rels/header1.xml.rels``: images, etc. for ``header1.xml``
+
+    ...
+
+    Get everything from everywhere. Map ``_rels/.rels`` to ``'rels'`` and everything
+    else to e.g., ``'document'`` or ``'header'``. RelIds are **not** unique between
+    these files.
+
+    **E.g, Given**::
+
+    # one of several files
+
+        <?xml version="1.0" encoding="UTF-8" standalone="yes"?>
+        <Relationships xmlns="http://schemas.../relationships">
+            <Relationship Id="rId3" Type="http://schemas... \
+                /extended-properties" Target="docProps/app.xml"/>
+            <Relationship Id="rId2" Type="http://schemas... \
+                /core-properties" Target="docProps/core.xml"/>
+            <Relationship Id="rId1" Type="http://schemas... \
+                /officeDocument" Target="word/document.xml"/>
+            <Relationship Id="rId4" Type="http://schemas... \
+                /custom-properties" Target="docProps/custom.xml"/>
+        </Relationships>
+
+    **Returns**::
+
+        {
+            "filename": [
+                {
+                    "Id": "rId3",
+                    "Type": "http://schemas.../extended-properties",
+                    "Target": "docProps/app.xml",
+                },
+                {
+                    "Id": "rId2",
+                    "Type": "http://schemas.../core-properties",
+                    "Target": "docProps/core.xml",
+                },
+            ]
+        }
+    """
+    path2rels: dict[str, list[dict[str, str]]] = {}
+    for rels in (x for x in zipf.namelist() if x[-5:] == ".rels"):
+        path2rels[rels] = [
+            {str(y): str(z) for y, z in x.attrib.items()}
+            for x in etree.fromstring(zipf.read(rels))
+        ]
+    return path2rels
+
+
+def collect_docProps(root: EtreeElement) -> dict[str, str | None]:
+    """
+    Get author, modified, etc. from core-properties (should be docProps/core.xml)
+
+    :param root: root of the XML tree
+    :return: document property names mapped to values
+
+    **E.g., Given**::
+
+        <cp:coreProperties xmlns:cp="http://schemas.openxmlformats...">
+            <dc:title>SG-DOP-5009 - Operate ROMAR swarf unit
+            </dc:title>
+            <dc:creator>Shay Hill
+            </dc:creator>
+            <cp:lastModifiedBy>Shay Hill
+            </cp:lastModifiedBy>
+            <cp:revision>6
+            </cp:revision>
+            <cp:lastPrinted>2017-11-17T15:47:00Z
+            </cp:lastPrinted>
+            <dcterms:created xsi:type="dcterms:W3CDTF">2019-01-10T07:21:00Z
+            </dcterms:created>
+            <dcterms:modified xsi:type="dcterms:W3CDTF">2019-01-11T11:41:00Z
+            </dcterms:modified>
+        </cp:coreProperties>
+
+    **E.g., Returns**::
+
+        {
+            "title": "SG-DOP-5009 - Operate ROMAR swarf unit",
+            "creator": "Shay Hill",
+            "lastModifiedBy": "Shay Hill",
+            "revision": "6",
+            ...
+        }
+    """
+    docProp2text: dict[str, str | None] = {}
+    capture_tag_name = re.compile(r"{.+}(?P<tag_name>\w+)")
+    for dc in root:
+        tag_match = re.match(capture_tag_name, dc.tag)
+        if tag_match:
+            docProp2text[tag_match.group("tag_name")] = dc.text
+    return docProp2text
```

### Comparing `docx2python-2.7.2/docx2python/docx_output.py` & `docx2python-2.7.3/docx2python/docx_output.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,262 +1,262 @@
-"""Output format for extracted docx content.
-
-:author: Shay Hill
-:created: 7/5/2019
-
-Holds runs in a 5-deep nested list (paragraphs are lists of text runs [strings])::
-
-    [  # tables
-        [  # table
-            [  # row
-                [  # cell
-                    [  # paragraph
-                        "run 1 ",  # text run
-                        "run 2 ",  # text run
-                        "run 3"  # text run
-                    ]
-                ]
-            ]
-        ]
-    ]
-
-_runs properties (e.g., ``header_runs``) return text in this format.
-
-Also returns a 4-deep nested list (paragraphs are strings)::
-
-    [  # tables
-        [  # table
-            [  # row
-                [  # cell
-                    "run 1 run 2 run 3"  # paragraph
-                ]
-            ]
-        ]
-    ]
-
-This is the format for default (no trailing "_runs", e.g ``header``) properties.
-
-"""
-from copy import deepcopy
-from dataclasses import dataclass
-from typing import Any, Dict, Optional
-from warnings import warn
-
-from .docx_context import collect_docProps
-from .docx_reader import DocxReader
-from .docx_text import TablesList
-from .iterators import enum_at_depth, get_html_map, iter_at_depth
-
-
-@dataclass
-class DocxContent:
-    """Holds return values for docx content."""
-
-    docx_reader: DocxReader
-    docx2python_kwargs: Dict[str, Any]
-
-    def close(self):
-        """Close the zipfile opened by DocxReader"""
-        self.docx_reader.close()
-
-    def __enter__(self) -> "DocxContent":
-        """Do nothing. The zipfile will open itself when needed.
-
-        :return: self"""
-        return self
-
-    def __exit__(
-        self,
-        exc_type: Any,  # None | Type[Exception], but py <= 3.9 doesn't like it.
-        exc_value: Any,  # None | Exception, but py <= 3.9 doesn't like it.
-        exc_traceback: Any,  # None | TracebackType, but py <= 3.9 doesn't like it.
-    ):
-        """Close the zipfile opened by DocxReader
-
-        :param exc_type: Python internal use
-        :param exc_value: Python internal use
-        :param exc_traceback: Python internal use
-        """
-        self.close()
-
-    def __getattr__(self, name: str) -> Any:
-        """
-        Create depth-four paragraph tables form depth-five run tables.
-
-        :param name: name of an internal docx xml file
-        :return: extracted text from named file with runs joined together into
-            paragraphs.
-        :raise AttributeError: if "name" file cannot be found
-
-        Docx2Python v1 joined runs into paragraphs [[[str]]] earlier in the code.
-        Docx2Python v2 exposes runs [[[[str]]]] to the user, but still returns
-        paragraphs by default.
-        """
-        if name in {"header", "footer", "body", "footnotes", "endnotes"}:
-            runs = deepcopy(getattr(self, name + "_runs"))
-            for (i, j, k, l), paragraph in enum_at_depth(runs, 4):
-                runs[i][j][k][l] = "".join(paragraph)
-            return runs
-        raise AttributeError(f"no attribute {name}")
-
-    def _get_runs(self, type_: str) -> TablesList:
-        """Get text runs for an internal document type.
-
-        :param type_: this package looks for any of
-            ("header", "officeDocument", "footer", "footnotes", "endnotes")
-            You can try others.
-        :return: text runs [[[[str]]]]
-        """
-        content: TablesList = []
-        for file in self.docx_reader.files_of_type(type_):
-            content += file.content
-        return content
-
-    @property
-    def header_runs(self) -> TablesList:
-        """Get text runs for header files.
-
-        :return: text runs [[[[str]]]]
-        """
-        return self._get_runs("header")
-
-    @property
-    def footer_runs(self) -> TablesList:
-        """Get text runs for footer files.
-
-        :return: text runs [[[[str]]]]
-        """
-        return self._get_runs("footer")
-
-    @property
-    def officeDocument_runs(self) -> TablesList:
-        """Get text runs for the main officeDocument file.
-
-        :return: text runs [[[[str]]]]
-        """
-        return self._get_runs("officeDocument")
-
-    @property
-    def body_runs(self) -> TablesList:
-        """Get text runs for the main officeDocument file.
-
-        :return: text runs [[[[str]]]]
-
-        This is an alias for officeDocument_runs.
-        """
-        return self.officeDocument_runs
-
-    @property
-    def footnotes_runs(self) -> TablesList:
-        """Get text runs for footnotes files.
-
-        :return: text runs [[[[str]]]]
-        """
-        return self._get_runs("footnotes")
-
-    @property
-    def endnotes_runs(self) -> TablesList:
-        """Get text runs for endnotes files.
-
-        :return: text runs [[[[str]]]]
-        """
-        return self._get_runs("endnotes")
-
-    @property
-    def images(self) -> Dict[str, bytes]:
-        """Get bytestring of all images in the document.
-
-        :return: dict {image_name: image_bytes}
-        """
-        return self.docx_reader.pull_image_files(
-            self.docx2python_kwargs["image_folder"]
-        )
-
-    @property
-    def document(self) -> TablesList:
-        """All docx "tables" concatenated.
-
-        :return: text paragraphs [[[str]]]
-        """
-        return self.header + self.body + self.footer + self.footnotes + self.endnotes
-
-    @property
-    def document_runs(self) -> TablesList:
-        """All docx x_runs properties concatenated.
-
-        :return: text runs [[[[str]]]]
-        """
-        return (
-            self.header_runs
-            + self.body_runs
-            + self.footer_runs
-            + self.footnotes_runs
-            + self.endnotes_runs
-        )
-
-    @property
-    def text(self) -> str:
-        """All docx paragraphs, "\n\n" joined.
-
-        :return: all docx paragraphs, "\n\n" joined
-        """
-        if self.docx2python_kwargs["paragraph_styles"] is True:
-            # Paragraph descriptors have been inserted as the first run of each
-            # paragraph. Take them out.
-            pars = ["".join(x[1:]) for x in iter_at_depth(self.document_runs, 4)]
-            return "\n\n".join(pars)
-        return "\n\n".join(iter_at_depth(self.document, 4))
-
-    @property
-    def html_map(self) -> str:
-        """A visual mapping of docx content.
-
-        :return: html to show all strings with index tuples
-        """
-        return get_html_map(self.document)
-
-    @property
-    def properties(self) -> Dict[str, Optional[str]]:
-        """Document core-properties as a dictionary.
-
-        :return: document core-properties as a dictionary
-
-        Docx files created with Google docs won't have core-properties. If the file
-        `core-properties` is missing, return an empty dict.
-        """
-        warn(
-            "DocxContent.properties is deprecated and will be removed in some future "
-            + "version. Use DocxContent.core_properties.",
-            FutureWarning,
-        )
-        return self.core_properties
-
-    @property
-    def core_properties(self) -> Dict[str, Optional[str]]:
-        """Document core-properties as a dictionary.
-
-        :return: document core-properties as a dictionary
-
-        Docx files created with Google docs won't have core-properties. If the file
-        `core-properties` is missing, return an empty dict.
-        """
-        try:
-            docProps = next(iter(self.docx_reader.files_of_type("core-properties")))
-            return collect_docProps(docProps.root_element)
-        except StopIteration:
-            warn(
-                "Could not find core-properties file (should be in docProps/core.xml) "
-                + "in DOCX, so returning an empty core_properties dictionary. Docx "
-                + "files created in Google Docs do not have a core-properties file, "
-                + "so this may be expected."
-            )
-            return {}
-
-    def save_images(self, image_folder: str) -> Dict[str, bytes]:
-        """Write images to hard drive.
-
-        :param image_folder: folder to write images to
-        :return: dictionary of image names and image data
-
-        If the image folder does not exist, it will not be created.
-        """
-        return self.docx_reader.pull_image_files(image_folder)
+"""Output format for extracted docx content.
+
+:author: Shay Hill
+:created: 7/5/2019
+
+Holds runs in a 5-deep nested list (paragraphs are lists of text runs [strings])::
+
+    [  # tables
+        [  # table
+            [  # row
+                [  # cell
+                    [  # paragraph
+                        "run 1 ",  # text run
+                        "run 2 ",  # text run
+                        "run 3"  # text run
+                    ]
+                ]
+            ]
+        ]
+    ]
+
+_runs properties (e.g., ``header_runs``) return text in this format.
+
+Also returns a 4-deep nested list (paragraphs are strings)::
+
+    [  # tables
+        [  # table
+            [  # row
+                [  # cell
+                    "run 1 run 2 run 3"  # paragraph
+                ]
+            ]
+        ]
+    ]
+
+This is the format for default (no trailing "_runs", e.g ``header``) properties.
+
+"""
+from copy import deepcopy
+from dataclasses import dataclass
+from typing import Any, Dict, Optional
+from warnings import warn
+
+from .docx_context import collect_docProps
+from .docx_reader import DocxReader
+from .docx_text import TablesList
+from .iterators import enum_at_depth, get_html_map, iter_at_depth
+
+
+@dataclass
+class DocxContent:
+    """Holds return values for docx content."""
+
+    docx_reader: DocxReader
+    docx2python_kwargs: Dict[str, Any]
+
+    def close(self):
+        """Close the zipfile opened by DocxReader"""
+        self.docx_reader.close()
+
+    def __enter__(self) -> "DocxContent":
+        """Do nothing. The zipfile will open itself when needed.
+
+        :return: self"""
+        return self
+
+    def __exit__(
+        self,
+        exc_type: Any,  # None | Type[Exception], but py <= 3.9 doesn't like it.
+        exc_value: Any,  # None | Exception, but py <= 3.9 doesn't like it.
+        exc_traceback: Any,  # None | TracebackType, but py <= 3.9 doesn't like it.
+    ):
+        """Close the zipfile opened by DocxReader
+
+        :param exc_type: Python internal use
+        :param exc_value: Python internal use
+        :param exc_traceback: Python internal use
+        """
+        self.close()
+
+    def __getattr__(self, name: str) -> Any:
+        """
+        Create depth-four paragraph tables form depth-five run tables.
+
+        :param name: name of an internal docx xml file
+        :return: extracted text from named file with runs joined together into
+            paragraphs.
+        :raise AttributeError: if "name" file cannot be found
+
+        Docx2Python v1 joined runs into paragraphs [[[str]]] earlier in the code.
+        Docx2Python v2 exposes runs [[[[str]]]] to the user, but still returns
+        paragraphs by default.
+        """
+        if name in {"header", "footer", "body", "footnotes", "endnotes"}:
+            runs = deepcopy(getattr(self, name + "_runs"))
+            for (i, j, k, l), paragraph in enum_at_depth(runs, 4):
+                runs[i][j][k][l] = "".join(paragraph)
+            return runs
+        raise AttributeError(f"no attribute {name}")
+
+    def _get_runs(self, type_: str) -> TablesList:
+        """Get text runs for an internal document type.
+
+        :param type_: this package looks for any of
+            ("header", "officeDocument", "footer", "footnotes", "endnotes")
+            You can try others.
+        :return: text runs [[[[str]]]]
+        """
+        content: TablesList = []
+        for file in self.docx_reader.files_of_type(type_):
+            content += file.content
+        return content
+
+    @property
+    def header_runs(self) -> TablesList:
+        """Get text runs for header files.
+
+        :return: text runs [[[[str]]]]
+        """
+        return self._get_runs("header")
+
+    @property
+    def footer_runs(self) -> TablesList:
+        """Get text runs for footer files.
+
+        :return: text runs [[[[str]]]]
+        """
+        return self._get_runs("footer")
+
+    @property
+    def officeDocument_runs(self) -> TablesList:
+        """Get text runs for the main officeDocument file.
+
+        :return: text runs [[[[str]]]]
+        """
+        return self._get_runs("officeDocument")
+
+    @property
+    def body_runs(self) -> TablesList:
+        """Get text runs for the main officeDocument file.
+
+        :return: text runs [[[[str]]]]
+
+        This is an alias for officeDocument_runs.
+        """
+        return self.officeDocument_runs
+
+    @property
+    def footnotes_runs(self) -> TablesList:
+        """Get text runs for footnotes files.
+
+        :return: text runs [[[[str]]]]
+        """
+        return self._get_runs("footnotes")
+
+    @property
+    def endnotes_runs(self) -> TablesList:
+        """Get text runs for endnotes files.
+
+        :return: text runs [[[[str]]]]
+        """
+        return self._get_runs("endnotes")
+
+    @property
+    def images(self) -> Dict[str, bytes]:
+        """Get bytestring of all images in the document.
+
+        :return: dict {image_name: image_bytes}
+        """
+        return self.docx_reader.pull_image_files(
+            self.docx2python_kwargs["image_folder"]
+        )
+
+    @property
+    def document(self) -> TablesList:
+        """All docx "tables" concatenated.
+
+        :return: text paragraphs [[[str]]]
+        """
+        return self.header + self.body + self.footer + self.footnotes + self.endnotes
+
+    @property
+    def document_runs(self) -> TablesList:
+        """All docx x_runs properties concatenated.
+
+        :return: text runs [[[[str]]]]
+        """
+        return (
+            self.header_runs
+            + self.body_runs
+            + self.footer_runs
+            + self.footnotes_runs
+            + self.endnotes_runs
+        )
+
+    @property
+    def text(self) -> str:
+        """All docx paragraphs, "\n\n" joined.
+
+        :return: all docx paragraphs, "\n\n" joined
+        """
+        if self.docx2python_kwargs["paragraph_styles"] is True:
+            # Paragraph descriptors have been inserted as the first run of each
+            # paragraph. Take them out.
+            pars = ["".join(x[1:]) for x in iter_at_depth(self.document_runs, 4)]
+            return "\n\n".join(pars)
+        return "\n\n".join(iter_at_depth(self.document, 4))
+
+    @property
+    def html_map(self) -> str:
+        """A visual mapping of docx content.
+
+        :return: html to show all strings with index tuples
+        """
+        return get_html_map(self.document)
+
+    @property
+    def properties(self) -> Dict[str, Optional[str]]:
+        """Document core-properties as a dictionary.
+
+        :return: document core-properties as a dictionary
+
+        Docx files created with Google docs won't have core-properties. If the file
+        `core-properties` is missing, return an empty dict.
+        """
+        warn(
+            "DocxContent.properties is deprecated and will be removed in some future "
+            + "version. Use DocxContent.core_properties.",
+            FutureWarning,
+        )
+        return self.core_properties
+
+    @property
+    def core_properties(self) -> Dict[str, Optional[str]]:
+        """Document core-properties as a dictionary.
+
+        :return: document core-properties as a dictionary
+
+        Docx files created with Google docs won't have core-properties. If the file
+        `core-properties` is missing, return an empty dict.
+        """
+        try:
+            docProps = next(iter(self.docx_reader.files_of_type("core-properties")))
+            return collect_docProps(docProps.root_element)
+        except StopIteration:
+            warn(
+                "Could not find core-properties file (should be in docProps/core.xml) "
+                + "in DOCX, so returning an empty core_properties dictionary. Docx "
+                + "files created in Google Docs do not have a core-properties file, "
+                + "so this may be expected."
+            )
+            return {}
+
+    def save_images(self, image_folder: str) -> Dict[str, bytes]:
+        """Write images to hard drive.
+
+        :param image_folder: folder to write images to
+        :return: dictionary of image names and image data
+
+        If the image folder does not exist, it will not be created.
+        """
+        return self.docx_reader.pull_image_files(image_folder)
```

### Comparing `docx2python-2.7.2/docx2python/docx_reader.py` & `docx2python-2.7.3/docx2python/docx_reader.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,459 +1,459 @@
-""" Hold and decode docx internal xml files.
-
-:author: Shay Hill
-:created: 3/18/2021
-
-See the docx file structure in ``README_DOCX_FILE_STRUCTURE.md``. Each file in that
-structure can be stored as a ``File`` instance, though not all will be stored through
-the typical docx2python progression.
-
-The ``File`` class is designed to hold and decode xml files with content (text).
-Several of the xml files in a docx do not contain content. These contain numbering
-formats, font information, rId-lookup tables, and other. ``File`` instances will hold
-these as well, though they will not have ``rels`` or ``content`` attributes. Will
-return an empty dictionary or empty list if asked.
-
-Some of these non-content files are shared between between . The substance of these
-files is accessible through the ``DocxContent`` class. This class holds file
-instances and decodes shared non-content in a docx file structure.
-"""
-
-from __future__ import annotations
-
-import copy
-import os
-import pathlib
-import zipfile
-from contextlib import suppress
-from dataclasses import dataclass
-from io import BytesIO
-from operator import attrgetter
-from pathlib import Path
-from typing import Any
-from warnings import warn
-
-from lxml import etree
-from lxml.etree import _Element as EtreeElement  # type: ignore
-
-from .attribute_register import XML2HTML_FORMATTER
-from .docx_context import collect_numFmts, collect_rels
-from .docx_text import get_text
-from .merge_runs import merge_elems
-
-CONTENT_FILE_TYPES = {"officeDocument", "header", "footer", "footnotes", "endnotes"}
-
-
-@dataclass
-class File:
-    """The attribute dict of a file in the docx, plus cached data
-
-    The docx lists internal files in various _rels files. Each will be specified with a
-    dict of, e.g.::
-
-        {
-            'Id': 'rId8',
-            'Type': 'http://schemas.openxmlformats.org/.../relationships/header',
-            'Target': 'header1.xml'
-        }
-
-    This isn't quite enough to infer the structure of the docx. You'll also need to
-    know the directory where each attribute dict was found::
-
-        'dir': 'word/_rels'
-
-    That's the starting point for these instances. Other attributes are inferred or
-    created at runtime.
-    """
-
-    def __init__(self, context: DocxReader, attribute_dict: dict[str, str]) -> None:
-        """
-        Point to container DocxContext instance and store attributes as properties.
-
-        :param context: The DocxContent object holding this instance
-        :param attribute_dict: Attributes of this file found in the rels, plus 'dir' as
-            described above.
-        """
-        self.context = context
-        self.Id = str(attribute_dict["Id"])
-        self.Type = os.path.basename(attribute_dict["Type"])
-        self.Target = attribute_dict["Target"]
-        self.dir = attribute_dict["dir"]
-
-        # cached_properties
-        self.__path: None | str = None
-        self.__rels_path: None | str = None
-        self.__rels: None | dict[str, str] = None
-        self.__root_element: None | EtreeElement = None
-
-    def __repr__(self) -> str:
-        """File with self.path
-
-        :return: String representation
-        """
-        return f"File({self.path})"
-
-    @property
-    def path(self) -> str:
-        """Infer path/to/xml/file from instance attributes
-
-        :return: path to xml file
-
-        This will take the information in a file specification (from one of the rels
-        files, e.g., {Id:'  ', Type:'  ' Target:'  ', dir:'  '}) and infer a path to
-        the specified xml file.
-
-        E.g.,
-        from     self.dir = '_rels'       self.Target = 'word/document.xml
-                    dirname ''          +       dirname 'word/'
-                                        +       filename =   'document.xml'
-        return `word/document`
-
-        E.g.,
-        from     self.dir = 'word/_rels'       self.Target = 'header1.xml
-                    dirname 'word'      +            dirname ''
-                                        +       filename =   'header1.xml'
-        return `word/header1.xml`
-        """
-        if self.__path is not None:
-            return self.__path
-
-        dirs = [os.path.dirname(x) for x in (self.dir, self.Target)]
-        dirname = "/".join([x for x in dirs if x])
-        filename = os.path.basename(self.Target)
-        self.__path = "/".join([dirname, filename])
-        return self.__path
-
-    @property
-    def _rels_path(self) -> str:
-        """Infer path/to/rels from instance attributes.
-
-        :return: path to rels (which may not exist)
-
-        Every content file (``document.xml``, ``header1.xml``, ...) will have its own
-        ``.rels`` file--if any relationships are defined.
-
-        The path inferred here may not exist.
-
-        E.g.,
-        from     self.dir = '_rels'       self.Target = 'word/document.xml
-                    dirname ''          +       dirname 'word/'
-                                        +       filename =   'document.xml'
-        return `word/_rels/document.xml.rels`
-
-        E.g.,
-        from     self.dir = 'word/_rels'       self.Target = 'header1.xml
-                    dirname 'word'      +            dirname ''
-                                        +       filename =   'header1.xml'
-        return `word/_rels/header1.xml.rels`
-        """
-        if self.__rels_path is not None:
-            return self.__rels_path
-        dirname, filename = os.path.split(self.path)
-        self.__rels_path = "/".join([dirname, "_rels", filename + ".rels"])
-        return self.__rels_path
-
-    @property
-    def rels(self) -> dict[str, str]:
-        """rIds mapped to values
-
-        :return: dict of rIds mapped to values
-
-        Each content file.xml will have a file.xml.rels file--if relationships are
-        defined. Inside file.xml, values defined in the file.xml.rels file may be
-        referenced by their rId numbers.
-
-        :return: Contents of the file.xml.rels file with reference rId numbers. These
-        refer to values defined in the file.xml.rels file:
-
-        E.g.::
-
-        {
-            "rId3": "webSettings.xml",
-            "rId2": "settings.xml",
-            "rId1": "styles.xml",
-            "rId6": "theme/theme1.xml",
-            "rId5": "fontTable.xml",
-            "rId4": "https://www.shayallenhill.com/",
-        }
-
-        Not every xml file with have a rels file. Return an empty dictionary if the
-        rels file is not found.
-        """
-        if self.__rels is not None:
-            return self.__rels
-
-        try:
-            unzipped = self.context.zipf.read(self._rels_path)
-            tree = etree.fromstring(unzipped)
-            self.__rels = {str(x.attrib["Id"]): str(x.attrib["Target"]) for x in tree}
-        except KeyError:
-            self.__rels = {}
-        return self.__rels
-
-    @property
-    def root_element(self) -> EtreeElement:
-        """Root element of the file.
-
-        :return: Root element of the file.
-
-        Try to merge consecutive, duplicate (except text) elements in content files.
-        See documentation for ``merge_elems``. Warn if ``merge_elems`` fails.
-        (I don't think it will fail).
-        """
-        if self.__root_element is not None:
-            return self.__root_element
-
-        root = etree.fromstring(self.context.zipf.read(self.path))
-        if self.Type in CONTENT_FILE_TYPES:
-            root_ = copy.copy(root)
-            try:
-                merge_elems(self, root)
-            except Exception as ex:
-                warn(
-                    "Attempt to merge consecutive elements in "
-                    + f"{self.context.docx_filename} {self.path} resulted in "
-                    + f"{repr(ex)}. Moving on."
-                )
-                self.__root_element = root_
-        self.__root_element = root
-        return self.__root_element
-
-    @property
-    def content(self) -> list[list[list[list[str]]]]:
-        """Text extracted into a 5-layer-deep nested list of strings.
-
-        :return: Text extracted into a 5-layer-deep nested list of strings.
-        """
-        return get_text(self)
-
-    def get_content(
-        self, root: EtreeElement | None = None
-    ) -> list[list[list[list[str]]]]:
-        """
-        The same content as property 'content' with optional given root.
-
-        :param root: Extract content of file from root down.
-            If root is not given, return full content of file.
-        :return: Text extracted into a 5-layer-deep nested list of strings.
-        """
-        return get_text(self, root)
-
-
-@dataclass
-class DocxReader:
-    """
-    Hold File instances and decode information shared between them (e.g., numFmts)
-    """
-
-    def __init__(
-        self,
-        docx_filename: Path | str | BytesIO,
-        html: bool = False,
-        paragraph_styles: bool = False,
-        duplicate_merged_cells: bool = False,
-    ):
-        self.docx_filename = docx_filename
-        self.do_pStyle = paragraph_styles
-        self.duplicate_merged_cells = duplicate_merged_cells
-
-        if html:
-            self.xml2html_format = XML2HTML_FORMATTER
-        else:
-            self.xml2html_format = {}
-
-        # cached properties and a flag (__closed)
-        self.__zipf: None | zipfile.ZipFile = None
-        self.__files: None | list[File] = None
-        self.__numId2NumFmts: None | dict[str, list[str]] = None
-        self.__closed = False
-
-    @property
-    def zipf(self) -> zipfile.ZipFile:
-        """
-        Entire docx unzipped into bytes.
-
-        :return: Entire docx unzipped into bytes.
-        :raise ValueError: If DocxReader instance has been closed
-        """
-        if self.__closed:
-            raise ValueError("DocxReader instance has been closed.")
-        if self.__zipf is None:
-            self.__zipf = zipfile.ZipFile(self.docx_filename)
-            return self.__zipf
-        assert self.__zipf is not None
-        return self.__zipf
-
-    def close(self):
-        """Close the zipfile, set __closed flag to True."""
-        if self.__zipf is not None and self.__zipf.fp:
-            self.__zipf.close()
-        self.__closed = True
-
-    def __enter__(self) -> DocxReader:
-        """Do nothing. The zipfile will open itself when needed.
-
-        :return: self
-        """
-        return self
-
-    def __exit__(
-        self,
-        exc_type: Any,  # None | Type[Exception], but py <= 3.9 doesn't like it.
-        exc_value: Any,  # None | Exception, but py <= 3.9 doesn't like it.
-        exc_traceback: Any,  # None | TracebackType, but py <= 3.9 doesn't like it.
-    ):
-        """Close the zipfile.
-
-        :param exc_type: Python internal use
-        :param exc_value: Python internal use
-        :param exc_traceback: Python internal use
-        """
-        self.close()
-
-    @property
-    def files(self) -> list[File]:
-        """
-        Instantiate a File instance for every content file.
-
-        :return: List of File instances, one per content file.
-        """
-        if self.__files is not None:
-            return self.__files
-
-        files: list[File] = []
-        for k, v in collect_rels(self.zipf).items():
-            files += [File(self, {**x, "dir": os.path.dirname(k)}) for x in v]
-        self.__files = files
-        return self.__files
-
-    @property
-    def numId2numFmts(self) -> dict[str, list[str]]:
-        """
-        numId referenced in xml to list of numFmt per indentation level
-
-        :return: numId referenced in xml to list of numFmt per indentation level
-
-        See docstring for collect_numFmts
-
-        Returns an empty dictionary if word/numbering.xml cannot be found.
-        Ultimately, this will result in any lists (there should NOT be any lists if
-        there is no word/numbering.xml) being "numbered" with "--".
-        """
-        if self.__numId2NumFmts is not None:
-            return self.__numId2NumFmts
-
-        try:
-            numFmts_root = etree.fromstring(self.zipf.read("word/numbering.xml"))
-            self.__numId2NumFmts = collect_numFmts(numFmts_root)
-        except KeyError:
-            self.__numId2NumFmts = {}
-        return self.__numId2NumFmts
-
-    def file_of_type(self, type_: str) -> File:
-        """
-        Return file instance attrib Type='http://.../type_'. Warn if more than one.
-
-        :param type_: this package looks for any of
-            ("header", "officeDocument", "footer", "footnotes", "endnotes")
-            You can try others.
-        :return: File instance of the requested type
-        :raise KeyError: if no file of the requested type is found
-        """
-        files_of_type = self.files_of_type(type_)
-        if len(files_of_type) > 1:
-            warn("Multiple files of type '{type_}' found. Returning first.")
-        try:
-            return files_of_type[0]
-        except IndexError as exc:
-            raise KeyError(
-                f"There is no item of type '{type_}' "
-                + "in the {self.docx_filename} archive"
-            ) from exc
-
-    def files_of_type(self, type_: str | None = None) -> list[File]:
-        """
-        File instances with attrib Type='http://.../type_'
-
-        :param type_: this package looks for any of
-            ("header", "officeDocument", "footer", "footnotes", "endnotes")
-            You can try others. If argument is None (default), returns all content file
-            types.
-        :return: File instances of the requested type, sorted by path
-        """
-        if type_ is None:
-            types = CONTENT_FILE_TYPES
-        else:
-            types = {type_}
-
-        return sorted(
-            (x for x in self.files if x.Type in types), key=attrgetter("path")
-        )
-
-    def content_files(self) -> list[File]:
-        """
-        Content files (contain displayed text) inside the docx.
-
-        :return: File instances of context files, sorted by path
-        """
-        return self.files_of_type()
-
-    def save(self, filename: Path | str) -> None:
-        """
-        Save the (presumably altered) xml.
-
-        :param filename: path to output file (presumably *.docx)
-
-        xml (root_element) attributes are cached, so these can be altered and saved.
-        This allows saving a copy of the input docx after the ``merge_elems`` operation.
-        Also allows some light editing like search and replace.
-        """
-        content_files = [x for x in self.files if x.Type in CONTENT_FILE_TYPES]
-        with zipfile.ZipFile(f"{filename}", mode="w") as zout:
-            _copy_but(self.zipf, zout, {x.path for x in content_files})
-            for file in content_files:
-                zout.writestr(file.path, etree.tostring(file.root_element))
-
-    def pull_image_files(self, image_directory: str | None = None) -> dict[str, bytes]:
-        """
-        Copy images from zip file.
-
-        :param image_directory: optional destination for copied images
-        :return: Image names mapped to images in binary format.
-
-            To write these to disc::
-
-                with open(key, 'wb') as file:
-                    file.write(value)
-
-        :side effects: Given an optional image_directory, will write the images out
-        to file.
-        """
-        images: dict[str, bytes] = {}
-        for image in self.files_of_type("image"):
-            with suppress(KeyError):
-                images[os.path.basename(image.Target)] = self.zipf.read(image.path)
-        if image_directory is not None:
-            pathlib.Path(image_directory).mkdir(parents=True, exist_ok=True)
-            for file, image_bytes in images.items():
-                with open(os.path.join(image_directory, file), "wb") as image_copy:
-                    _ = image_copy.write(image_bytes)
-        return images
-
-
-def _copy_but(
-    in_zip: zipfile.ZipFile,
-    out_zip: zipfile.ZipFile,
-    exclusions: set[str] | None = None,
-) -> None:
-    """
-    Copy every file in a docx except those listed in exclusions.
-
-    :param in_zip: zipfile of origin xml file
-    :param out_zip: zipfile of destination xml file
-    :param exclusions: filenames you don't want to copy (e.g., 'document.xml')
-    """
-    exclusions = exclusions or set()
-    for item in in_zip.infolist():
-        if item.filename not in exclusions:
-            buffer = in_zip.read(item.filename)
-            out_zip.writestr(item, buffer)
+""" Hold and decode docx internal xml files.
+
+:author: Shay Hill
+:created: 3/18/2021
+
+See the docx file structure in ``README_DOCX_FILE_STRUCTURE.md``. Each file in that
+structure can be stored as a ``File`` instance, though not all will be stored through
+the typical docx2python progression.
+
+The ``File`` class is designed to hold and decode xml files with content (text).
+Several of the xml files in a docx do not contain content. These contain numbering
+formats, font information, rId-lookup tables, and other. ``File`` instances will hold
+these as well, though they will not have ``rels`` or ``content`` attributes. Will
+return an empty dictionary or empty list if asked.
+
+Some of these non-content files are shared between between . The substance of these
+files is accessible through the ``DocxContent`` class. This class holds file
+instances and decodes shared non-content in a docx file structure.
+"""
+
+from __future__ import annotations
+
+import copy
+import os
+import pathlib
+import zipfile
+from contextlib import suppress
+from dataclasses import dataclass
+from io import BytesIO
+from operator import attrgetter
+from pathlib import Path
+from typing import Any
+from warnings import warn
+
+from lxml import etree
+from lxml.etree import _Element as EtreeElement  # type: ignore
+
+from .attribute_register import XML2HTML_FORMATTER
+from .docx_context import collect_numFmts, collect_rels
+from .docx_text import get_text
+from .merge_runs import merge_elems
+
+CONTENT_FILE_TYPES = {"officeDocument", "header", "footer", "footnotes", "endnotes"}
+
+
+@dataclass
+class File:
+    """The attribute dict of a file in the docx, plus cached data
+
+    The docx lists internal files in various _rels files. Each will be specified with a
+    dict of, e.g.::
+
+        {
+            'Id': 'rId8',
+            'Type': 'http://schemas.openxmlformats.org/.../relationships/header',
+            'Target': 'header1.xml'
+        }
+
+    This isn't quite enough to infer the structure of the docx. You'll also need to
+    know the directory where each attribute dict was found::
+
+        'dir': 'word/_rels'
+
+    That's the starting point for these instances. Other attributes are inferred or
+    created at runtime.
+    """
+
+    def __init__(self, context: DocxReader, attribute_dict: dict[str, str]) -> None:
+        """
+        Point to container DocxContext instance and store attributes as properties.
+
+        :param context: The DocxContent object holding this instance
+        :param attribute_dict: Attributes of this file found in the rels, plus 'dir' as
+            described above.
+        """
+        self.context = context
+        self.Id = str(attribute_dict["Id"])
+        self.Type = os.path.basename(attribute_dict["Type"])
+        self.Target = attribute_dict["Target"]
+        self.dir = attribute_dict["dir"]
+
+        # cached_properties
+        self.__path: None | str = None
+        self.__rels_path: None | str = None
+        self.__rels: None | dict[str, str] = None
+        self.__root_element: None | EtreeElement = None
+
+    def __repr__(self) -> str:
+        """File with self.path
+
+        :return: String representation
+        """
+        return f"File({self.path})"
+
+    @property
+    def path(self) -> str:
+        """Infer path/to/xml/file from instance attributes
+
+        :return: path to xml file
+
+        This will take the information in a file specification (from one of the rels
+        files, e.g., {Id:'  ', Type:'  ' Target:'  ', dir:'  '}) and infer a path to
+        the specified xml file.
+
+        E.g.,
+        from     self.dir = '_rels'       self.Target = 'word/document.xml
+                    dirname ''          +       dirname 'word/'
+                                        +       filename =   'document.xml'
+        return `word/document`
+
+        E.g.,
+        from     self.dir = 'word/_rels'       self.Target = 'header1.xml
+                    dirname 'word'      +            dirname ''
+                                        +       filename =   'header1.xml'
+        return `word/header1.xml`
+        """
+        if self.__path is not None:
+            return self.__path
+
+        dirs = [os.path.dirname(x) for x in (self.dir, self.Target)]
+        dirname = "/".join([x for x in dirs if x])
+        filename = os.path.basename(self.Target)
+        self.__path = "/".join([dirname, filename])
+        return self.__path
+
+    @property
+    def _rels_path(self) -> str:
+        """Infer path/to/rels from instance attributes.
+
+        :return: path to rels (which may not exist)
+
+        Every content file (``document.xml``, ``header1.xml``, ...) will have its own
+        ``.rels`` file--if any relationships are defined.
+
+        The path inferred here may not exist.
+
+        E.g.,
+        from     self.dir = '_rels'       self.Target = 'word/document.xml
+                    dirname ''          +       dirname 'word/'
+                                        +       filename =   'document.xml'
+        return `word/_rels/document.xml.rels`
+
+        E.g.,
+        from     self.dir = 'word/_rels'       self.Target = 'header1.xml
+                    dirname 'word'      +            dirname ''
+                                        +       filename =   'header1.xml'
+        return `word/_rels/header1.xml.rels`
+        """
+        if self.__rels_path is not None:
+            return self.__rels_path
+        dirname, filename = os.path.split(self.path)
+        self.__rels_path = "/".join([dirname, "_rels", filename + ".rels"])
+        return self.__rels_path
+
+    @property
+    def rels(self) -> dict[str, str]:
+        """rIds mapped to values
+
+        :return: dict of rIds mapped to values
+
+        Each content file.xml will have a file.xml.rels file--if relationships are
+        defined. Inside file.xml, values defined in the file.xml.rels file may be
+        referenced by their rId numbers.
+
+        :return: Contents of the file.xml.rels file with reference rId numbers. These
+        refer to values defined in the file.xml.rels file:
+
+        E.g.::
+
+        {
+            "rId3": "webSettings.xml",
+            "rId2": "settings.xml",
+            "rId1": "styles.xml",
+            "rId6": "theme/theme1.xml",
+            "rId5": "fontTable.xml",
+            "rId4": "https://www.shayallenhill.com/",
+        }
+
+        Not every xml file with have a rels file. Return an empty dictionary if the
+        rels file is not found.
+        """
+        if self.__rels is not None:
+            return self.__rels
+
+        try:
+            unzipped = self.context.zipf.read(self._rels_path)
+            tree = etree.fromstring(unzipped)
+            self.__rels = {str(x.attrib["Id"]): str(x.attrib["Target"]) for x in tree}
+        except KeyError:
+            self.__rels = {}
+        return self.__rels
+
+    @property
+    def root_element(self) -> EtreeElement:
+        """Root element of the file.
+
+        :return: Root element of the file.
+
+        Try to merge consecutive, duplicate (except text) elements in content files.
+        See documentation for ``merge_elems``. Warn if ``merge_elems`` fails.
+        (I don't think it will fail).
+        """
+        if self.__root_element is not None:
+            return self.__root_element
+
+        root = etree.fromstring(self.context.zipf.read(self.path))
+        if self.Type in CONTENT_FILE_TYPES:
+            root_ = copy.copy(root)
+            try:
+                merge_elems(self, root)
+            except Exception as ex:
+                warn(
+                    "Attempt to merge consecutive elements in "
+                    + f"{self.context.docx_filename} {self.path} resulted in "
+                    + f"{repr(ex)}. Moving on."
+                )
+                self.__root_element = root_
+        self.__root_element = root
+        return self.__root_element
+
+    @property
+    def content(self) -> list[list[list[list[str]]]]:
+        """Text extracted into a 5-layer-deep nested list of strings.
+
+        :return: Text extracted into a 5-layer-deep nested list of strings.
+        """
+        return get_text(self)
+
+    def get_content(
+        self, root: EtreeElement | None = None
+    ) -> list[list[list[list[str]]]]:
+        """
+        The same content as property 'content' with optional given root.
+
+        :param root: Extract content of file from root down.
+            If root is not given, return full content of file.
+        :return: Text extracted into a 5-layer-deep nested list of strings.
+        """
+        return get_text(self, root)
+
+
+@dataclass
+class DocxReader:
+    """
+    Hold File instances and decode information shared between them (e.g., numFmts)
+    """
+
+    def __init__(
+        self,
+        docx_filename: Path | str | BytesIO,
+        html: bool = False,
+        paragraph_styles: bool = False,
+        duplicate_merged_cells: bool = False,
+    ):
+        self.docx_filename = docx_filename
+        self.do_pStyle = paragraph_styles
+        self.duplicate_merged_cells = duplicate_merged_cells
+
+        if html:
+            self.xml2html_format = XML2HTML_FORMATTER
+        else:
+            self.xml2html_format = {}
+
+        # cached properties and a flag (__closed)
+        self.__zipf: None | zipfile.ZipFile = None
+        self.__files: None | list[File] = None
+        self.__numId2NumFmts: None | dict[str, list[str]] = None
+        self.__closed = False
+
+    @property
+    def zipf(self) -> zipfile.ZipFile:
+        """
+        Entire docx unzipped into bytes.
+
+        :return: Entire docx unzipped into bytes.
+        :raise ValueError: If DocxReader instance has been closed
+        """
+        if self.__closed:
+            raise ValueError("DocxReader instance has been closed.")
+        if self.__zipf is None:
+            self.__zipf = zipfile.ZipFile(self.docx_filename)
+            return self.__zipf
+        assert self.__zipf is not None
+        return self.__zipf
+
+    def close(self):
+        """Close the zipfile, set __closed flag to True."""
+        if self.__zipf is not None and self.__zipf.fp:
+            self.__zipf.close()
+        self.__closed = True
+
+    def __enter__(self) -> DocxReader:
+        """Do nothing. The zipfile will open itself when needed.
+
+        :return: self
+        """
+        return self
+
+    def __exit__(
+        self,
+        exc_type: Any,  # None | Type[Exception], but py <= 3.9 doesn't like it.
+        exc_value: Any,  # None | Exception, but py <= 3.9 doesn't like it.
+        exc_traceback: Any,  # None | TracebackType, but py <= 3.9 doesn't like it.
+    ):
+        """Close the zipfile.
+
+        :param exc_type: Python internal use
+        :param exc_value: Python internal use
+        :param exc_traceback: Python internal use
+        """
+        self.close()
+
+    @property
+    def files(self) -> list[File]:
+        """
+        Instantiate a File instance for every content file.
+
+        :return: List of File instances, one per content file.
+        """
+        if self.__files is not None:
+            return self.__files
+
+        files: list[File] = []
+        for k, v in collect_rels(self.zipf).items():
+            files += [File(self, {**x, "dir": os.path.dirname(k)}) for x in v]
+        self.__files = files
+        return self.__files
+
+    @property
+    def numId2numFmts(self) -> dict[str, list[str]]:
+        """
+        numId referenced in xml to list of numFmt per indentation level
+
+        :return: numId referenced in xml to list of numFmt per indentation level
+
+        See docstring for collect_numFmts
+
+        Returns an empty dictionary if word/numbering.xml cannot be found.
+        Ultimately, this will result in any lists (there should NOT be any lists if
+        there is no word/numbering.xml) being "numbered" with "--".
+        """
+        if self.__numId2NumFmts is not None:
+            return self.__numId2NumFmts
+
+        try:
+            numFmts_root = etree.fromstring(self.zipf.read("word/numbering.xml"))
+            self.__numId2NumFmts = collect_numFmts(numFmts_root)
+        except KeyError:
+            self.__numId2NumFmts = {}
+        return self.__numId2NumFmts
+
+    def file_of_type(self, type_: str) -> File:
+        """
+        Return file instance attrib Type='http://.../type_'. Warn if more than one.
+
+        :param type_: this package looks for any of
+            ("header", "officeDocument", "footer", "footnotes", "endnotes")
+            You can try others.
+        :return: File instance of the requested type
+        :raise KeyError: if no file of the requested type is found
+        """
+        files_of_type = self.files_of_type(type_)
+        if len(files_of_type) > 1:
+            warn("Multiple files of type '{type_}' found. Returning first.")
+        try:
+            return files_of_type[0]
+        except IndexError as exc:
+            raise KeyError(
+                f"There is no item of type '{type_}' "
+                + "in the {self.docx_filename} archive"
+            ) from exc
+
+    def files_of_type(self, type_: str | None = None) -> list[File]:
+        """
+        File instances with attrib Type='http://.../type_'
+
+        :param type_: this package looks for any of
+            ("header", "officeDocument", "footer", "footnotes", "endnotes")
+            You can try others. If argument is None (default), returns all content file
+            types.
+        :return: File instances of the requested type, sorted by path
+        """
+        if type_ is None:
+            types = CONTENT_FILE_TYPES
+        else:
+            types = {type_}
+
+        return sorted(
+            (x for x in self.files if x.Type in types), key=attrgetter("path")
+        )
+
+    def content_files(self) -> list[File]:
+        """
+        Content files (contain displayed text) inside the docx.
+
+        :return: File instances of context files, sorted by path
+        """
+        return self.files_of_type()
+
+    def save(self, filename: Path | str) -> None:
+        """
+        Save the (presumably altered) xml.
+
+        :param filename: path to output file (presumably *.docx)
+
+        xml (root_element) attributes are cached, so these can be altered and saved.
+        This allows saving a copy of the input docx after the ``merge_elems`` operation.
+        Also allows some light editing like search and replace.
+        """
+        content_files = [x for x in self.files if x.Type in CONTENT_FILE_TYPES]
+        with zipfile.ZipFile(f"{filename}", mode="w") as zout:
+            _copy_but(self.zipf, zout, {x.path for x in content_files})
+            for file in content_files:
+                zout.writestr(file.path, etree.tostring(file.root_element))
+
+    def pull_image_files(self, image_directory: str | None = None) -> dict[str, bytes]:
+        """
+        Copy images from zip file.
+
+        :param image_directory: optional destination for copied images
+        :return: Image names mapped to images in binary format.
+
+            To write these to disc::
+
+                with open(key, 'wb') as file:
+                    file.write(value)
+
+        :side effects: Given an optional image_directory, will write the images out
+        to file.
+        """
+        images: dict[str, bytes] = {}
+        for image in self.files_of_type("image"):
+            with suppress(KeyError):
+                images[os.path.basename(image.Target)] = self.zipf.read(image.path)
+        if image_directory is not None:
+            pathlib.Path(image_directory).mkdir(parents=True, exist_ok=True)
+            for file, image_bytes in images.items():
+                with open(os.path.join(image_directory, file), "wb") as image_copy:
+                    _ = image_copy.write(image_bytes)
+        return images
+
+
+def _copy_but(
+    in_zip: zipfile.ZipFile,
+    out_zip: zipfile.ZipFile,
+    exclusions: set[str] | None = None,
+) -> None:
+    """
+    Copy every file in a docx except those listed in exclusions.
+
+    :param in_zip: zipfile of origin xml file
+    :param out_zip: zipfile of destination xml file
+    :param exclusions: filenames you don't want to copy (e.g., 'document.xml')
+    """
+    exclusions = exclusions or set()
+    for item in in_zip.infolist():
+        if item.filename not in exclusions:
+            buffer = in_zip.read(item.filename)
+            out_zip.writestr(item, buffer)
```

### Comparing `docx2python-2.7.2/docx2python/docx_text.py` & `docx2python-2.7.3/docx2python/docx_text.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,292 +1,292 @@
-"""Extract text from docx content files.
-
-:author: Shay Hill
-:created: 6/6/2019
-
-Content in the extracted docx is found in the ``word`` folder:
-    ``word/document.html``
-    ``word/header1.html``
-    ``word/footer1.html``
-"""
-from __future__ import annotations
-
-from contextlib import suppress
-from typing import TYPE_CHECKING, List, Sequence, cast
-
-from lxml.etree import _Element as EtreeElement  # type: ignore
-
-from .attribute_register import Tags
-from .bullets_and_numbering import BulletGenerator
-from .depth_collector import DepthCollector, Run
-from .forms import get_checkBox_entry, get_ddList_entry
-from .iterators import iter_at_depth
-from .namespace import qn
-from .text_runs import (
-    gather_Pr,
-    get_paragraph_formatting,
-    get_pStyle,
-    get_run_formatting,
-)
-
-if TYPE_CHECKING:
-    from docx_reader import File
-
-TablesList = List[List[List[List[str]]]]
-
-
-def _get_elem_depth(tree: EtreeElement) -> int | None:
-    """What depth is this element in a nested list, relative to paragraphs (depth 4)?
-
-    :param tree: element in a docx content xml (header, footer, officeDocument, etc.)
-
-    :return: 4 - recursion depth;
-        None if no paragraphs are found or if descending into nest would cause a
-        false start (e.g., Tags.DOCUMENT or Tags.BODY which often have A paragraph (but
-        not the next paragraph) at one or two levels down.
-
-    Typically, the docx is a table of tables::
-
-        [  # entire document
-            [  # table
-                [  # table row
-                    [  # table cell
-                        [  # paragraph
-                            "",  # run
-                            "",  # run
-                            "",  # run
-                        ]
-                    ]
-                ]
-            ]
-        ]
-
-    But this isn't always the case. Instead of looking explicitly for tables,
-    table rows, and table cells, look inside elements for paragraphs to determine
-    depth in the nested list.
-
-    E.g., given a table row element with a paragraph two levels in, return 2.
-    So, depth of element will be 4 - 2 = 3.
-
-    document = depth 0
-    table = depth 1
-    table row = depth 2
-    table cell = depth 3
-    paragraph = depth 4
-    below paragraph = depth 5
-
-    There will only ever be one document list, so the min depth returned is 1
-    """
-
-    if tree.tag in {Tags.DOCUMENT, Tags.BODY}:
-        return None
-
-    def search_at_depth(tree_: Sequence[EtreeElement], _depth: int = 0) -> int | None:
-        """Width-first recursive search for Tags.PARAGRAPH
-
-        :param tree_: a sequence of elements which may contain a paragraph
-        :return: depth of the first paragraph found, or None if no paragraph found
-        """
-        if not tree_:
-            return None
-        if any(x.tag == Tags.PARAGRAPH for x in tree_):
-            return max(4 - _depth, 1)
-        grandchildren = [list(x) for x in tree_]
-        return search_at_depth([x for y in grandchildren for x in y], _depth + 1)
-
-    return search_at_depth([tree])
-
-
-def get_paragraphs(file: File, root: EtreeElement) -> list[str]:
-    """Return a list of paragraphs from the document
-
-    :param file: an internal file element (e.g., header, footer, document))
-    :param root: the root element of the document
-    :return: a list of paragraphs
-    """
-    all_paragraphs: list[str] = []
-    for branch in root:
-        all_paragraphs += list(iter_at_depth(get_text(file, branch), 5))
-    return all_paragraphs
-
-
-def merged_text_tree(file: File, root: EtreeElement) -> str:
-    """Return a string of all text in the document
-
-    :param file: an internal file element (e.g., header, footer, document))
-    :param root: the root element of the document
-    :return: a string of all text in the document
-    """
-    return "".join(get_paragraphs(file, root))
-
-
-def get_text(file: File, root: EtreeElement | None = None) -> TablesList:
-    """Xml as a string to a list of cell strings.
-
-    :param file: File instance from which text will be extracted.
-    :param root: Optionally extract content from a single element.
-        If None, root_element of file will be used.
-    :return: A 5-deep nested list of strings.
-
-    Sorts the text into the DepthCollector instance, five-levels deep
-
-    ``[table][row][cell][paragraph][run]`` is a string
-
-    Joins the runs before returning, so return list will be
-
-    ``[table][row][cell][paragraph]`` is a string
-
-    If you'd like to extend or edit this package, this function is probably where you
-    want to do it. Nothing tricky here except keeping track of the text formatting.
-    """
-    root = root if root is not None else file.root_element
-    bullets = BulletGenerator(file.context.numId2numFmts)
-    # numId2count = _new_list_counter()
-    tables = DepthCollector(5)
-
-    xml2html = file.context.xml2html_format
-
-    def branches(tree: EtreeElement) -> None:
-        """
-        Recursively iterate over tree. Add text when found.
-
-        :param tree: An Element from an xml file (etree)
-        :effect: Adds text cells to outer variable `tables`.
-        """
-        do_descend = True
-
-        tree_depth = _get_elem_depth(tree)
-        tables.set_caret(tree_depth)
-
-        # queue up tags before opening any paragraphs or runs
-        if tree.tag == Tags.PARAGRAPH:
-            par = tables.commence_paragraph(get_paragraph_formatting(tree, xml2html))
-            if file.context.do_pStyle:
-                par.runs.insert(0, Run([], get_pStyle(tree) or "None"))
-            tables.insert_text_as_new_run(bullets.get_bullet(tree))
-
-        elif tree.tag == Tags.RUN:
-            tables.commence_run(get_run_formatting(tree, xml2html))
-
-        elif tree.tag in {Tags.TEXT, Tags.TEXT_MATH}:
-            # oddly enough, these don't all contain text
-            text = tree.text if tree.text is not None else ""
-            if xml2html:
-                text = text.replace("&", "&amp;")
-                text = text.replace("<", "&lt;")
-                text = text.replace(">", "&gt;")
-            tables.add_text_into_open_run(text)
-
-        elif tree.tag == Tags.MATH:
-            # read equations
-            text = "".join(str(x) for x in tree.itertext())
-            do_descend = False
-            tables.insert_text_as_new_run(f"<latex>{text}</latex>")
-
-        elif tree.tag == Tags.BR:
-            tables.add_text_into_open_run("\n")
-
-        elif tree.tag == Tags.SYM:
-            font = str(tree.attrib.get(qn("w:font")))
-            char = str(tree.attrib.get(qn("w:char")))
-            if char:
-                tables.add_text_into_open_run(
-                    f"<span style=font-family:{font}>&#x0{char[1:]};</span>"
-                )
-
-        elif tree.tag == Tags.FOOTNOTE:
-            footnote_type = str(tree.attrib.get(qn("w:type"), "")).lower()
-            if "separator" not in footnote_type:
-                tables.insert_text_as_new_run(
-                    f"footnote{str(tree.attrib[qn('w:id')])})\t"
-                )
-
-        elif tree.tag == Tags.ENDNOTE:
-            endnote_type = str(tree.attrib.get(qn("w:type"), "")).lower()
-            if "separator" not in endnote_type:
-                tables.insert_text_as_new_run(
-                    f"endnote{str(tree.attrib[qn('w:id')])})\t"
-                )
-
-        elif tree.tag == Tags.HYPERLINK:
-            # look for an href, ignore internal references (anchors)
-            text = merged_text_tree(file, tree)
-            do_descend = False
-            try:
-                rId = tree.attrib[qn("r:id")]
-                link = file.rels[rId]
-                tables.insert_text_as_new_run(f'<a href="{link}">{text}</a>')
-            except KeyError:
-                tables.insert_text_as_new_run(text)
-
-        if tree.tag == Tags.FORM_CHECKBOX:
-            tables.insert_text_as_new_run(get_checkBox_entry(tree))
-
-        elif tree.tag == Tags.FORM_DDLIST:
-            tables.insert_text_as_new_run(get_ddList_entry(tree))
-
-        elif tree.tag == Tags.FOOTNOTE_REFERENCE:
-            tables.insert_text_as_new_run(
-                f"----footnote{str(tree.attrib[qn('w:id')])}----"
-            )
-
-        elif tree.tag == Tags.ENDNOTE_REFERENCE:
-            tables.insert_text_as_new_run(
-                f"----endnote{str(tree.attrib[qn('w:id')])}----"
-            )
-
-        elif tree.tag == Tags.IMAGE:
-            with suppress(KeyError):
-                rId = tree.attrib[qn("r:embed")]
-                image = file.rels[rId]
-                tables.insert_text_as_new_run(f"----{image}----")
-
-        elif tree.tag == Tags.IMAGE_ALT:
-            with suppress(KeyError):
-                description = tree.attrib["descr"]
-                tables.insert_text_as_new_run(f"----Image alt text---->{description}<")
-
-        elif tree.tag == Tags.IMAGEDATA:
-            with suppress(KeyError):
-                rId = tree.attrib[qn("r:id")]
-                image = file.rels[rId]
-                tables.insert_text_as_new_run(f"----{image}----")
-
-        elif tree.tag == Tags.TAB:
-            tables.insert_text_as_new_run("\t")
-
-        if do_descend:
-            for branch in tree:
-                branches(branch)
-
-        if tree.tag == Tags.PARAGRAPH:
-            tables.conclude_paragraph()
-
-        elif tree.tag == Tags.TABLE_CELL and file.context.duplicate_merged_cells:
-            pr = gather_Pr(tree)
-
-            if pr.get("vMerge", "Not None") is None:
-                tables.set_caret(tree_depth)
-                cell_idx = len(tables.caret) - 1
-                assert isinstance(tree_depth, int)
-                prev_row_cell = tables.view_branch((tree_depth - 2, -2, cell_idx))
-                tables.caret[-1] = prev_row_cell
-
-            grid_span = pr.get("gridSpan", 1)
-            assert grid_span is not None
-            for _ in range(int(grid_span) - 1):
-                tables.set_caret(tree_depth)
-                tables.caret.append(tables.caret[-1])
-
-        elif tree.tag == Tags.RUN:
-            tables.conclude_run()
-
-        tables.set_caret(tree_depth)
-
-    branches(root)
-
-    if tables.orphan_runs:
-        _ = tables.commence_paragraph()
-    if tables.open_pars:
-        tables.conclude_paragraph()
-
-    return cast(TablesList, tables.tree)
+"""Extract text from docx content files.
+
+:author: Shay Hill
+:created: 6/6/2019
+
+Content in the extracted docx is found in the ``word`` folder:
+    ``word/document.html``
+    ``word/header1.html``
+    ``word/footer1.html``
+"""
+from __future__ import annotations
+
+from contextlib import suppress
+from typing import TYPE_CHECKING, List, Sequence, cast
+
+from lxml.etree import _Element as EtreeElement  # type: ignore
+
+from .attribute_register import Tags
+from .bullets_and_numbering import BulletGenerator
+from .depth_collector import DepthCollector, Run
+from .forms import get_checkBox_entry, get_ddList_entry
+from .iterators import iter_at_depth
+from .namespace import qn
+from .text_runs import (
+    gather_Pr,
+    get_paragraph_formatting,
+    get_pStyle,
+    get_run_formatting,
+)
+
+if TYPE_CHECKING:
+    from docx_reader import File
+
+TablesList = List[List[List[List[str]]]]
+
+
+def _get_elem_depth(tree: EtreeElement) -> int | None:
+    """What depth is this element in a nested list, relative to paragraphs (depth 4)?
+
+    :param tree: element in a docx content xml (header, footer, officeDocument, etc.)
+
+    :return: 4 - recursion depth;
+        None if no paragraphs are found or if descending into nest would cause a
+        false start (e.g., Tags.DOCUMENT or Tags.BODY which often have A paragraph (but
+        not the next paragraph) at one or two levels down.
+
+    Typically, the docx is a table of tables::
+
+        [  # entire document
+            [  # table
+                [  # table row
+                    [  # table cell
+                        [  # paragraph
+                            "",  # run
+                            "",  # run
+                            "",  # run
+                        ]
+                    ]
+                ]
+            ]
+        ]
+
+    But this isn't always the case. Instead of looking explicitly for tables,
+    table rows, and table cells, look inside elements for paragraphs to determine
+    depth in the nested list.
+
+    E.g., given a table row element with a paragraph two levels in, return 2.
+    So, depth of element will be 4 - 2 = 3.
+
+    document = depth 0
+    table = depth 1
+    table row = depth 2
+    table cell = depth 3
+    paragraph = depth 4
+    below paragraph = depth 5
+
+    There will only ever be one document list, so the min depth returned is 1
+    """
+
+    if tree.tag in {Tags.DOCUMENT, Tags.BODY}:
+        return None
+
+    def search_at_depth(tree_: Sequence[EtreeElement], _depth: int = 0) -> int | None:
+        """Width-first recursive search for Tags.PARAGRAPH
+
+        :param tree_: a sequence of elements which may contain a paragraph
+        :return: depth of the first paragraph found, or None if no paragraph found
+        """
+        if not tree_:
+            return None
+        if any(x.tag == Tags.PARAGRAPH for x in tree_):
+            return max(4 - _depth, 1)
+        grandchildren = [list(x) for x in tree_]
+        return search_at_depth([x for y in grandchildren for x in y], _depth + 1)
+
+    return search_at_depth([tree])
+
+
+def get_paragraphs(file: File, root: EtreeElement) -> list[str]:
+    """Return a list of paragraphs from the document
+
+    :param file: an internal file element (e.g., header, footer, document))
+    :param root: the root element of the document
+    :return: a list of paragraphs
+    """
+    all_paragraphs: list[str] = []
+    for branch in root:
+        all_paragraphs += list(iter_at_depth(get_text(file, branch), 5))
+    return all_paragraphs
+
+
+def merged_text_tree(file: File, root: EtreeElement) -> str:
+    """Return a string of all text in the document
+
+    :param file: an internal file element (e.g., header, footer, document))
+    :param root: the root element of the document
+    :return: a string of all text in the document
+    """
+    return "".join(get_paragraphs(file, root))
+
+
+def get_text(file: File, root: EtreeElement | None = None) -> TablesList:
+    """Xml as a string to a list of cell strings.
+
+    :param file: File instance from which text will be extracted.
+    :param root: Optionally extract content from a single element.
+        If None, root_element of file will be used.
+    :return: A 5-deep nested list of strings.
+
+    Sorts the text into the DepthCollector instance, five-levels deep
+
+    ``[table][row][cell][paragraph][run]`` is a string
+
+    Joins the runs before returning, so return list will be
+
+    ``[table][row][cell][paragraph]`` is a string
+
+    If you'd like to extend or edit this package, this function is probably where you
+    want to do it. Nothing tricky here except keeping track of the text formatting.
+    """
+    root = root if root is not None else file.root_element
+    bullets = BulletGenerator(file.context.numId2numFmts)
+    # numId2count = _new_list_counter()
+    tables = DepthCollector(5)
+
+    xml2html = file.context.xml2html_format
+
+    def branches(tree: EtreeElement) -> None:
+        """
+        Recursively iterate over tree. Add text when found.
+
+        :param tree: An Element from an xml file (etree)
+        :effect: Adds text cells to outer variable `tables`.
+        """
+        do_descend = True
+
+        tree_depth = _get_elem_depth(tree)
+        tables.set_caret(tree_depth)
+
+        # queue up tags before opening any paragraphs or runs
+        if tree.tag == Tags.PARAGRAPH:
+            par = tables.commence_paragraph(get_paragraph_formatting(tree, xml2html))
+            if file.context.do_pStyle:
+                par.runs.insert(0, Run([], get_pStyle(tree) or "None"))
+            tables.insert_text_as_new_run(bullets.get_bullet(tree))
+
+        elif tree.tag == Tags.RUN:
+            tables.commence_run(get_run_formatting(tree, xml2html))
+
+        elif tree.tag in {Tags.TEXT, Tags.TEXT_MATH}:
+            # oddly enough, these don't all contain text
+            text = tree.text if tree.text is not None else ""
+            if xml2html:
+                text = text.replace("&", "&amp;")
+                text = text.replace("<", "&lt;")
+                text = text.replace(">", "&gt;")
+            tables.add_text_into_open_run(text)
+
+        elif tree.tag == Tags.MATH:
+            # read equations
+            text = "".join(str(x) for x in tree.itertext())
+            do_descend = False
+            tables.insert_text_as_new_run(f"<latex>{text}</latex>")
+
+        elif tree.tag == Tags.BR:
+            tables.add_text_into_open_run("\n")
+
+        elif tree.tag == Tags.SYM:
+            font = str(tree.attrib.get(qn("w:font")))
+            char = str(tree.attrib.get(qn("w:char")))
+            if char:
+                tables.add_text_into_open_run(
+                    f"<span style=font-family:{font}>&#x0{char[1:]};</span>"
+                )
+
+        elif tree.tag == Tags.FOOTNOTE:
+            footnote_type = str(tree.attrib.get(qn("w:type"), "")).lower()
+            if "separator" not in footnote_type:
+                tables.insert_text_as_new_run(
+                    f"footnote{str(tree.attrib[qn('w:id')])})\t"
+                )
+
+        elif tree.tag == Tags.ENDNOTE:
+            endnote_type = str(tree.attrib.get(qn("w:type"), "")).lower()
+            if "separator" not in endnote_type:
+                tables.insert_text_as_new_run(
+                    f"endnote{str(tree.attrib[qn('w:id')])})\t"
+                )
+
+        elif tree.tag == Tags.HYPERLINK:
+            # look for an href, ignore internal references (anchors)
+            text = merged_text_tree(file, tree)
+            do_descend = False
+            try:
+                rId = tree.attrib[qn("r:id")]
+                link = file.rels[rId]
+                tables.insert_text_as_new_run(f'<a href="{link}">{text}</a>')
+            except KeyError:
+                tables.insert_text_as_new_run(text)
+
+        if tree.tag == Tags.FORM_CHECKBOX:
+            tables.insert_text_as_new_run(get_checkBox_entry(tree))
+
+        elif tree.tag == Tags.FORM_DDLIST:
+            tables.insert_text_as_new_run(get_ddList_entry(tree))
+
+        elif tree.tag == Tags.FOOTNOTE_REFERENCE:
+            tables.insert_text_as_new_run(
+                f"----footnote{str(tree.attrib[qn('w:id')])}----"
+            )
+
+        elif tree.tag == Tags.ENDNOTE_REFERENCE:
+            tables.insert_text_as_new_run(
+                f"----endnote{str(tree.attrib[qn('w:id')])}----"
+            )
+
+        elif tree.tag == Tags.IMAGE:
+            with suppress(KeyError):
+                rId = tree.attrib[qn("r:embed")]
+                image = file.rels[rId]
+                tables.insert_text_as_new_run(f"----{image}----")
+
+        elif tree.tag == Tags.IMAGE_ALT:
+            with suppress(KeyError):
+                description = tree.attrib["descr"]
+                tables.insert_text_as_new_run(f"----Image alt text---->{description}<")
+
+        elif tree.tag == Tags.IMAGEDATA:
+            with suppress(KeyError):
+                rId = tree.attrib[qn("r:id")]
+                image = file.rels[rId]
+                tables.insert_text_as_new_run(f"----{image}----")
+
+        elif tree.tag == Tags.TAB:
+            tables.insert_text_as_new_run("\t")
+
+        if do_descend:
+            for branch in tree:
+                branches(branch)
+
+        if tree.tag == Tags.PARAGRAPH:
+            tables.conclude_paragraph()
+
+        elif tree.tag == Tags.TABLE_CELL and file.context.duplicate_merged_cells:
+            pr = gather_Pr(tree)
+
+            if pr.get("vMerge", "Not None") is None:
+                tables.set_caret(tree_depth)
+                cell_idx = len(tables.caret) - 1
+                assert isinstance(tree_depth, int)
+                prev_row_cell = tables.view_branch((tree_depth - 2, -2, cell_idx))
+                tables.caret[-1] = prev_row_cell
+
+            grid_span = pr.get("gridSpan", 1)
+            assert grid_span is not None
+            for _ in range(int(grid_span) - 1):
+                tables.set_caret(tree_depth)
+                tables.caret.append(tables.caret[-1])
+
+        elif tree.tag == Tags.RUN:
+            tables.conclude_run()
+
+        tables.set_caret(tree_depth)
+
+    branches(root)
+
+    if tables.orphan_runs:
+        _ = tables.commence_paragraph()
+    if tables.open_pars:
+        tables.conclude_paragraph()
+
+    return cast(TablesList, tables.tree)
```

### Comparing `docx2python-2.7.2/docx2python/forms.py` & `docx2python-2.7.3/docx2python/forms.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-""" Form checkboxes, dropdowns, and other non-text elements visible in Word.
-
-:author: Shay Hill
-:created: 6/17/2020
-
-Word represents some special characters as non-text elements (e.g., checkBox). These
-functions examine these elements to infer suitable text replacements.
-
-This file references "\u2610" and "\u2612" a few times. These are open and
-crossed-out checkboxes. Pypi doesn't like them in my file, so I have to reference
-them by their escape sequences.
-"""
-
-from contextlib import suppress
-from typing import Union
-
-from lxml.etree import _Element as EtreeElement  # type: ignore
-
-from .namespace import qn
-
-
-def get_checkBox_entry(checkBox: EtreeElement) -> str:
-    """Create text representation for a checkBox element.
-
-    :param checkBox: a checkBox xml element
-    :return:
-        1. attempt to get ``checked.w:val`` and return "\u2610" or "\u2612"
-        2. attempt to get ``default.w:val`` and return "\u2610" or "\u2612"
-        3. return ``--checkbox failed--``
-
-    Docx xml has at least two types of checkbox elements::
-
-        1. ``checkBox`` can only be checked when the form is locked. These do not
-        contain a text element, so this function is needed to select one from the
-        ``w:checked`` or ``w:default`` sub-elements.
-
-        2. ``checkbox`` can be checked any time. Prints text as "\u2610" or "\u2612".
-        Docx2Python can safely ignore this second type, as there will be a <w:t>
-        element inside with a checkbox character.
-
-    <w:checkBox>
-        <w:sizeAuto/>
-        <w:default w:val="1"/>
-        <w:checked w:val="0"/>
-    </w:checkBox>
-
-    If the ``checked`` attribute is absent, return the default
-    If the ``checked`` attribute is present, but not w:val is given, return unchecked
-    """
-
-    def get_wval() -> Union[str, None]:
-        """Get the value of the ``w:val`` attribute of the ``checked`` element.
-
-        :return: the value of the ``w:val`` attribute of the ``checked`` element
-        """
-        with suppress(StopIteration):
-            checked = next(checkBox.iterfind(qn("w:checked")))
-            return str(checked.attrib.get(qn("w:val")) or "1")
-        with suppress(StopIteration, KeyError):
-            default = next(checkBox.iterfind(qn("w:default")))
-            return str(default.attrib[qn("w:val")])
-        return None
-
-    return {"0": "\u2610", "1": "\u2612", None: "----checkbox failed----"}[get_wval()]
-
-
-def get_ddList_entry(ddList: EtreeElement) -> str:
-    """Get only the selected string of a dropdown list.
-
-    :param ddList: a dropdown-list element
-    :return: w:listEntry value of input element.
-
-    <w:ddList>
-        <w:result w:val="1"/>
-        <w:listEntry w:val="selection 1"/>
-        <w:listEntry w:val="selection 2"/>
-    </w:ddList>
-
-    <w:result w:val="0"/> might be missing when selection is "0"
-    """
-    list_entries = [
-        x.attrib.get(qn("w:val")) for x in ddList.findall(qn("w:listEntry"))
-    ]
-    try:
-        result = next(ddList.iterfind(qn("w:result")))
-        list_index = int(result.attrib[qn("w:val")])
-    except (StopIteration, KeyError):
-        list_index = 0
-    return str(list_entries[list_index])
+""" Form checkboxes, dropdowns, and other non-text elements visible in Word.
+
+:author: Shay Hill
+:created: 6/17/2020
+
+Word represents some special characters as non-text elements (e.g., checkBox). These
+functions examine these elements to infer suitable text replacements.
+
+This file references "\u2610" and "\u2612" a few times. These are open and
+crossed-out checkboxes. Pypi doesn't like them in my file, so I have to reference
+them by their escape sequences.
+"""
+
+from contextlib import suppress
+from typing import Union
+
+from lxml.etree import _Element as EtreeElement  # type: ignore
+
+from .namespace import qn
+
+
+def get_checkBox_entry(checkBox: EtreeElement) -> str:
+    """Create text representation for a checkBox element.
+
+    :param checkBox: a checkBox xml element
+    :return:
+        1. attempt to get ``checked.w:val`` and return "\u2610" or "\u2612"
+        2. attempt to get ``default.w:val`` and return "\u2610" or "\u2612"
+        3. return ``--checkbox failed--``
+
+    Docx xml has at least two types of checkbox elements::
+
+        1. ``checkBox`` can only be checked when the form is locked. These do not
+        contain a text element, so this function is needed to select one from the
+        ``w:checked`` or ``w:default`` sub-elements.
+
+        2. ``checkbox`` can be checked any time. Prints text as "\u2610" or "\u2612".
+        Docx2Python can safely ignore this second type, as there will be a <w:t>
+        element inside with a checkbox character.
+
+    <w:checkBox>
+        <w:sizeAuto/>
+        <w:default w:val="1"/>
+        <w:checked w:val="0"/>
+    </w:checkBox>
+
+    If the ``checked`` attribute is absent, return the default
+    If the ``checked`` attribute is present, but not w:val is given, return unchecked
+    """
+
+    def get_wval() -> Union[str, None]:
+        """Get the value of the ``w:val`` attribute of the ``checked`` element.
+
+        :return: the value of the ``w:val`` attribute of the ``checked`` element
+        """
+        with suppress(StopIteration):
+            checked = next(checkBox.iterfind(qn("w:checked")))
+            return str(checked.attrib.get(qn("w:val")) or "1")
+        with suppress(StopIteration, KeyError):
+            default = next(checkBox.iterfind(qn("w:default")))
+            return str(default.attrib[qn("w:val")])
+        return None
+
+    return {"0": "\u2610", "1": "\u2612", None: "----checkbox failed----"}[get_wval()]
+
+
+def get_ddList_entry(ddList: EtreeElement) -> str:
+    """Get only the selected string of a dropdown list.
+
+    :param ddList: a dropdown-list element
+    :return: w:listEntry value of input element.
+
+    <w:ddList>
+        <w:result w:val="1"/>
+        <w:listEntry w:val="selection 1"/>
+        <w:listEntry w:val="selection 2"/>
+    </w:ddList>
+
+    <w:result w:val="0"/> might be missing when selection is "0"
+    """
+    list_entries = [
+        x.attrib.get(qn("w:val")) for x in ddList.findall(qn("w:listEntry"))
+    ]
+    try:
+        result = next(ddList.iterfind(qn("w:result")))
+        list_index = int(result.attrib[qn("w:val")])
+    except (StopIteration, KeyError):
+        list_index = 0
+    return str(list_entries[list_index])
```

### Comparing `docx2python-2.7.2/docx2python/iterators.py` & `docx2python-2.7.3/docx2python/iterators.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,309 +1,309 @@
-"""Iterate over extracted docx content.
-
-:author: Shay Hill
-:created: 6/28/2019
-
-This package extracts docx text as::
-
-    [  # tables
-        [  # table
-            [  # row
-                [  # cell
-                    ""  # paragraph
-                ]
-            ]
-        ]
-    ]
-
-These functions help manipulate that deep nest without deep indentation.
-
-"""
-
-from __future__ import annotations
-
-from typing import Any, Iterable, Iterator, List, NamedTuple, Sequence, cast
-
-TablesList = List[List[List[List[Any]]]]
-
-
-class IndexedItem(NamedTuple):
-    """The address (indices in a nested list) of an item and the item itself."""
-
-    index: tuple[int, ...]
-    value: Any
-
-
-def enum_at_depth(nested: Sequence[Any], depth: int) -> Iterator[IndexedItem]:
-    """Enumerate over a nested sequence at depth.
-
-    :param nested: a (nested) sequence
-    :param depth: depth of iteration
-
-        * ``1`` => ``((i,), nested[i])``
-        * ``2`` => ``((i, j), nested[:][j])``
-        * ``3`` => ``((i, j, k), nested[:][:][k])``
-        * ...
-
-    :return: tuples (tuple "address", item)
-    :raise ValueError: if depth is less than 1
-
-    >>> sequence = [
-    ...     [[["a", "b"], ["c"]], [["d", "e"]]],
-    ...     [[["f"], ["g", "h"]]]
-    ... ]
-
-    >>> for x in enum_at_depth(sequence, 1): print(x)
-    IndexedItem(index=(0,), value=[[['a', 'b'], ['c']], [['d', 'e']]])
-    IndexedItem(index=(1,), value=[[['f'], ['g', 'h']]])
-
-    >>> for x in enum_at_depth(sequence, 2): print(x)
-    IndexedItem(index=(0, 0), value=[['a', 'b'], ['c']])
-    IndexedItem(index=(0, 1), value=[['d', 'e']])
-    IndexedItem(index=(1, 0), value=[['f'], ['g', 'h']])
-
-    >>> for x in enum_at_depth(sequence, 3): print(x)
-    IndexedItem(index=(0, 0, 0), value=['a', 'b'])
-    IndexedItem(index=(0, 0, 1), value=['c'])
-    IndexedItem(index=(0, 1, 0), value=['d', 'e'])
-    IndexedItem(index=(1, 0, 0), value=['f'])
-    IndexedItem(index=(1, 0, 1), value=['g', 'h'])
-
-    >>> for x in enum_at_depth(sequence, 4): print(x)
-    IndexedItem(index=(0, 0, 0, 0), value='a')
-    IndexedItem(index=(0, 0, 0, 1), value='b')
-    IndexedItem(index=(0, 0, 1, 0), value='c')
-    IndexedItem(index=(0, 1, 0, 0), value='d')
-    IndexedItem(index=(0, 1, 0, 1), value='e')
-    IndexedItem(index=(1, 0, 0, 0), value='f')
-    IndexedItem(index=(1, 0, 1, 0), value='g')
-    IndexedItem(index=(1, 0, 1, 1), value='h')
-
-    >>> list(enum_at_depth(sequence, 5))
-    Traceback (most recent call last):
-    ...
-    TypeError: will not iterate over sequence item
-
-    This error is analogous to the ``TypeError: 'int' object is not iterable`` you
-    would see if attempting to enumerate over a non-iterable. In this case,
-    you've attempted to enumerate over an item that *may* be iterable, but is not of
-    the same type as the ``nested`` sequence argument. This type checking is how we
-    can safely descend into a nested list of strings.
-    """
-    if depth < 1:
-        raise ValueError("depth argument must be >= 1")
-    argument_type = type(nested)
-
-    def enumerate_next_depth(enumd: Iterable[IndexedItem]) -> Iterator[IndexedItem]:
-        """
-        Descend into a nested sequence, enumerating along descent
-
-        :param enumd: tuples (tuple of indices, sequences)
-        :return: updated index tuples with items from each sequence.
-        :raises TypeError: if the sequence is not of the same type as the ``nested``.
-            This will happen if you try to iterate into a string in a list of
-            strings.
-        """
-        for index_tuple, sequence in enumd:
-            if not isinstance(sequence, argument_type):
-                raise TypeError("will not iterate over sequence item")
-            for i, item in enumerate(sequence):
-                yield IndexedItem(index_tuple + (i,), item)
-
-    depth_n: Iterator[IndexedItem]
-    depth_n = (IndexedItem((i,), x) for i, x in enumerate(nested))
-    for _ in range(1, depth):
-        depth_n = enumerate_next_depth(depth_n)
-    return (x for x in depth_n)
-
-
-def iter_at_depth(nested: Sequence[Any], depth: int) -> Iterator[Any]:
-    """
-    Iterate over a nested sequence at depth.
-
-    :param nested: a (nested) sequence
-    :param depth: depth of iteration
-
-        * ``1`` => ``nested[i]``
-        * ``2`` => ``nested[:][j]``
-        * ``3`` => ``nested[:][:][k]``
-        * ...
-
-    :return: sub-sequences or items in nested
-
-    >>> sequence = [
-    ...     [[["a", "b"], ["c"]], [["d", "e"]]],
-    ...     [[["f"], ["g", "h"]]]
-    ... ]
-
-    >>> for x in iter_at_depth(sequence, 1): print(x)
-    [[['a', 'b'], ['c']], [['d', 'e']]]
-    [[['f'], ['g', 'h']]]
-
-    >>> for x in iter_at_depth(sequence, 2): print(x)
-    [['a', 'b'], ['c']]
-    [['d', 'e']]
-    [['f'], ['g', 'h']]
-
-    >>> for x in iter_at_depth(sequence, 3): print(x)
-    ['a', 'b']
-    ['c']
-    ['d', 'e']
-    ['f']
-    ['g', 'h']
-
-    >>> list(iter_at_depth(sequence, 4))
-    ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h']
-    """
-    return (value for _, value in enum_at_depth(nested, depth))
-
-
-def iter_tables(tables: TablesList) -> Iterator[list[list[list[Any]]]]:
-    """
-    Iterate over ``tables[i]``
-
-    Analog of iter_at_depth(tables, 1)
-
-    :param tables: ``[[[["string"]]]]``
-    :return: ``tables[0], tables[1], ... tables[i]``
-    """
-    return iter_at_depth(tables, 1)
-
-
-def iter_rows(tables: TablesList) -> Iterator[list[list[Any]]]:
-    """
-    Iterate over ``tables[:][j]``
-
-    Analog of iter_at_depth(tables, 2)
-
-    :param tables: ``[[[["string"]]]]``
-    :return: ``tables[0][0], tables[0][1], ... tables[i][j]``
-    """
-    return iter_at_depth(tables, 2)
-
-
-def iter_cells(tables: TablesList) -> Iterator[list[Any]]:
-    """
-    Iterate over ``tables[:][:][k]``
-
-    Analog of iter_at_depth(tables, 3)
-
-    :param tables: ``[[[["string"]]]]``
-    :return: ``tables[0][0][0], tables[0][0][1], ... tables[i][j][k]``
-    """
-    return iter_at_depth(tables, 3)
-
-
-def iter_paragraphs(tables: TablesList) -> Iterator[str]:
-    """
-    Iterate over ``tables[:][:][:][l]``
-
-    Analog of iter_at_depth(tables, 4)
-
-    :param tables: ``[[[["string"]]]]``
-    :return: ``tables[0][0][0][0], tables[0][0][0][1], ... tables[i][j][k][l]``
-    """
-    return iter_at_depth(tables, 4)
-
-
-def enum_tables(tables: TablesList) -> Iterator[IndexedItem]:
-    """
-    Enumerate over ``tables[i]``
-
-    Analog of enum_at_depth(tables, 1)
-
-    :param tables: ``[[[["string"]]]]``
-    :return:
-        ``((0, ), tables[0]) ... , ((i, ), tables[i])``
-    """
-    return enum_at_depth(tables, 1)
-
-
-def enum_rows(tables: TablesList) -> Iterator[IndexedItem]:
-    """
-    Enumerate over ``tables[:][j]``
-
-    Analog of enum_at_depth(tables, 2)
-
-    :param tables: ``[[[["string"]]]]``
-    :return:
-        ``((0, 0), tables[0][0]) ... , ((i, j), tables[i][j])``
-    """
-    return enum_at_depth(tables, 2)
-
-
-def enum_cells(tables: TablesList) -> Iterator[IndexedItem]:
-    """
-    Enumerate over ``tables[:][:][k]``
-
-    Analog of enum_at_depth(tables, 3)
-
-    :param tables: ``[[[["string"]]]]``
-    :return:
-        ``((0, 0, 0), tables[0][0][0]) ... , ((i, j, k), tables[i][j][k])``
-    """
-    return enum_at_depth(tables, 3)
-
-
-def enum_paragraphs(tables: TablesList) -> Iterator[IndexedItem]:
-    """
-    Enumerate over ``tables[:][:][:][l]``
-
-    Analog of enum_at_depth(tables, 4)
-
-    :param tables: ``[[[["string"]]]]``
-    :return:
-        ``((0, 0, 0, 0), tables[0][0][0][0]) ... , ((i, j, k, l), tables[i][j][k][l])``
-    """
-    return enum_at_depth(tables, 4)
-
-
-def get_text(tables: TablesList) -> str:
-    """
-    Short cut to pull text from any subset of extracted content.
-
-    :param tables: ``[[[["string"]]]]``
-    :return: "string" (all paragraphs in tables joined with '\n\n'
-    """
-    return "\n\n".join(iter_at_depth(tables, 4))
-
-
-def get_html_map(tables: TablesList) -> str:
-    """
-    Create a visual map in html format.
-
-    :param tables: ``[[[["string"]]]]``
-    :return: html to show all strings with index tuples
-
-    Create an html string that can be rendered in a browser to show the relative
-    location and index tuple of every paragraph in the document.
-
-    * Each table will be a grid of cell boxes, outlined in black. * Each paragraph
-    will be prepended with an index tuple. (e.g., ``[[[['text']]]]`` will appear as
-    ``(0, 0, 0, 0) text``.
-    """
-
-    # prepend index tuple to each paragraph
-    tables_4deep = cast(List[List[List[List[str]]]], tables)
-    for (i, j, k, l), paragraph in enum_at_depth(tables, 4):
-        tables_4deep[i][j][k][l] = " ".join([str((i, j, k, l)), paragraph])
-
-    # wrap each paragraph in <pre> tags
-    tables_3deep = cast(List[List[List[str]]], tables_4deep)
-    for (i, j, k), cell in enum_at_depth(tables_4deep, 3):
-        cell = (str(x) for x in cell)
-        tables_3deep[i][j][k] = "".join([f"<pre>{x}</pre>" for x in cell])
-
-    # wrap each cell in <td> tags
-    tables_2deep = cast(List[List[str]], tables_3deep)
-    for (i, j), row in enum_at_depth(tables_3deep, 2):
-        tables_2deep[i][j] = "".join([f"<td>{x}</td>" for x in row])
-
-    # wrap each row in <tr> tags
-    tables_1deep = cast(List[str], tables_2deep)
-    for (i,), table in enum_at_depth(tables_2deep, 1):
-        tables_1deep[i] = "".join(f"<tr>{x}</tr>" for x in table)
-
-    # wrap each table in <table> tags
-    tables_ = "".join([f'<table border="1">{x}</table>' for x in tables_1deep])
-
-    return "<html><body>" + tables_ + "</body></html>"
+"""Iterate over extracted docx content.
+
+:author: Shay Hill
+:created: 6/28/2019
+
+This package extracts docx text as::
+
+    [  # tables
+        [  # table
+            [  # row
+                [  # cell
+                    ""  # paragraph
+                ]
+            ]
+        ]
+    ]
+
+These functions help manipulate that deep nest without deep indentation.
+
+"""
+
+from __future__ import annotations
+
+from typing import Any, Iterable, Iterator, List, NamedTuple, Sequence, cast
+
+TablesList = List[List[List[List[Any]]]]
+
+
+class IndexedItem(NamedTuple):
+    """The address (indices in a nested list) of an item and the item itself."""
+
+    index: tuple[int, ...]
+    value: Any
+
+
+def enum_at_depth(nested: Sequence[Any], depth: int) -> Iterator[IndexedItem]:
+    """Enumerate over a nested sequence at depth.
+
+    :param nested: a (nested) sequence
+    :param depth: depth of iteration
+
+        * ``1`` => ``((i,), nested[i])``
+        * ``2`` => ``((i, j), nested[:][j])``
+        * ``3`` => ``((i, j, k), nested[:][:][k])``
+        * ...
+
+    :return: tuples (tuple "address", item)
+    :raise ValueError: if depth is less than 1
+
+    >>> sequence = [
+    ...     [[["a", "b"], ["c"]], [["d", "e"]]],
+    ...     [[["f"], ["g", "h"]]]
+    ... ]
+
+    >>> for x in enum_at_depth(sequence, 1): print(x)
+    IndexedItem(index=(0,), value=[[['a', 'b'], ['c']], [['d', 'e']]])
+    IndexedItem(index=(1,), value=[[['f'], ['g', 'h']]])
+
+    >>> for x in enum_at_depth(sequence, 2): print(x)
+    IndexedItem(index=(0, 0), value=[['a', 'b'], ['c']])
+    IndexedItem(index=(0, 1), value=[['d', 'e']])
+    IndexedItem(index=(1, 0), value=[['f'], ['g', 'h']])
+
+    >>> for x in enum_at_depth(sequence, 3): print(x)
+    IndexedItem(index=(0, 0, 0), value=['a', 'b'])
+    IndexedItem(index=(0, 0, 1), value=['c'])
+    IndexedItem(index=(0, 1, 0), value=['d', 'e'])
+    IndexedItem(index=(1, 0, 0), value=['f'])
+    IndexedItem(index=(1, 0, 1), value=['g', 'h'])
+
+    >>> for x in enum_at_depth(sequence, 4): print(x)
+    IndexedItem(index=(0, 0, 0, 0), value='a')
+    IndexedItem(index=(0, 0, 0, 1), value='b')
+    IndexedItem(index=(0, 0, 1, 0), value='c')
+    IndexedItem(index=(0, 1, 0, 0), value='d')
+    IndexedItem(index=(0, 1, 0, 1), value='e')
+    IndexedItem(index=(1, 0, 0, 0), value='f')
+    IndexedItem(index=(1, 0, 1, 0), value='g')
+    IndexedItem(index=(1, 0, 1, 1), value='h')
+
+    >>> list(enum_at_depth(sequence, 5))
+    Traceback (most recent call last):
+    ...
+    TypeError: will not iterate over sequence item
+
+    This error is analogous to the ``TypeError: 'int' object is not iterable`` you
+    would see if attempting to enumerate over a non-iterable. In this case,
+    you've attempted to enumerate over an item that *may* be iterable, but is not of
+    the same type as the ``nested`` sequence argument. This type checking is how we
+    can safely descend into a nested list of strings.
+    """
+    if depth < 1:
+        raise ValueError("depth argument must be >= 1")
+    argument_type = type(nested)
+
+    def enumerate_next_depth(enumd: Iterable[IndexedItem]) -> Iterator[IndexedItem]:
+        """
+        Descend into a nested sequence, enumerating along descent
+
+        :param enumd: tuples (tuple of indices, sequences)
+        :return: updated index tuples with items from each sequence.
+        :raises TypeError: if the sequence is not of the same type as the ``nested``.
+            This will happen if you try to iterate into a string in a list of
+            strings.
+        """
+        for index_tuple, sequence in enumd:
+            if not isinstance(sequence, argument_type):
+                raise TypeError("will not iterate over sequence item")
+            for i, item in enumerate(sequence):
+                yield IndexedItem(index_tuple + (i,), item)
+
+    depth_n: Iterator[IndexedItem]
+    depth_n = (IndexedItem((i,), x) for i, x in enumerate(nested))
+    for _ in range(1, depth):
+        depth_n = enumerate_next_depth(depth_n)
+    return (x for x in depth_n)
+
+
+def iter_at_depth(nested: Sequence[Any], depth: int) -> Iterator[Any]:
+    """
+    Iterate over a nested sequence at depth.
+
+    :param nested: a (nested) sequence
+    :param depth: depth of iteration
+
+        * ``1`` => ``nested[i]``
+        * ``2`` => ``nested[:][j]``
+        * ``3`` => ``nested[:][:][k]``
+        * ...
+
+    :return: sub-sequences or items in nested
+
+    >>> sequence = [
+    ...     [[["a", "b"], ["c"]], [["d", "e"]]],
+    ...     [[["f"], ["g", "h"]]]
+    ... ]
+
+    >>> for x in iter_at_depth(sequence, 1): print(x)
+    [[['a', 'b'], ['c']], [['d', 'e']]]
+    [[['f'], ['g', 'h']]]
+
+    >>> for x in iter_at_depth(sequence, 2): print(x)
+    [['a', 'b'], ['c']]
+    [['d', 'e']]
+    [['f'], ['g', 'h']]
+
+    >>> for x in iter_at_depth(sequence, 3): print(x)
+    ['a', 'b']
+    ['c']
+    ['d', 'e']
+    ['f']
+    ['g', 'h']
+
+    >>> list(iter_at_depth(sequence, 4))
+    ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h']
+    """
+    return (value for _, value in enum_at_depth(nested, depth))
+
+
+def iter_tables(tables: TablesList) -> Iterator[list[list[list[Any]]]]:
+    """
+    Iterate over ``tables[i]``
+
+    Analog of iter_at_depth(tables, 1)
+
+    :param tables: ``[[[["string"]]]]``
+    :return: ``tables[0], tables[1], ... tables[i]``
+    """
+    return iter_at_depth(tables, 1)
+
+
+def iter_rows(tables: TablesList) -> Iterator[list[list[Any]]]:
+    """
+    Iterate over ``tables[:][j]``
+
+    Analog of iter_at_depth(tables, 2)
+
+    :param tables: ``[[[["string"]]]]``
+    :return: ``tables[0][0], tables[0][1], ... tables[i][j]``
+    """
+    return iter_at_depth(tables, 2)
+
+
+def iter_cells(tables: TablesList) -> Iterator[list[Any]]:
+    """
+    Iterate over ``tables[:][:][k]``
+
+    Analog of iter_at_depth(tables, 3)
+
+    :param tables: ``[[[["string"]]]]``
+    :return: ``tables[0][0][0], tables[0][0][1], ... tables[i][j][k]``
+    """
+    return iter_at_depth(tables, 3)
+
+
+def iter_paragraphs(tables: TablesList) -> Iterator[str]:
+    """
+    Iterate over ``tables[:][:][:][l]``
+
+    Analog of iter_at_depth(tables, 4)
+
+    :param tables: ``[[[["string"]]]]``
+    :return: ``tables[0][0][0][0], tables[0][0][0][1], ... tables[i][j][k][l]``
+    """
+    return iter_at_depth(tables, 4)
+
+
+def enum_tables(tables: TablesList) -> Iterator[IndexedItem]:
+    """
+    Enumerate over ``tables[i]``
+
+    Analog of enum_at_depth(tables, 1)
+
+    :param tables: ``[[[["string"]]]]``
+    :return:
+        ``((0, ), tables[0]) ... , ((i, ), tables[i])``
+    """
+    return enum_at_depth(tables, 1)
+
+
+def enum_rows(tables: TablesList) -> Iterator[IndexedItem]:
+    """
+    Enumerate over ``tables[:][j]``
+
+    Analog of enum_at_depth(tables, 2)
+
+    :param tables: ``[[[["string"]]]]``
+    :return:
+        ``((0, 0), tables[0][0]) ... , ((i, j), tables[i][j])``
+    """
+    return enum_at_depth(tables, 2)
+
+
+def enum_cells(tables: TablesList) -> Iterator[IndexedItem]:
+    """
+    Enumerate over ``tables[:][:][k]``
+
+    Analog of enum_at_depth(tables, 3)
+
+    :param tables: ``[[[["string"]]]]``
+    :return:
+        ``((0, 0, 0), tables[0][0][0]) ... , ((i, j, k), tables[i][j][k])``
+    """
+    return enum_at_depth(tables, 3)
+
+
+def enum_paragraphs(tables: TablesList) -> Iterator[IndexedItem]:
+    """
+    Enumerate over ``tables[:][:][:][l]``
+
+    Analog of enum_at_depth(tables, 4)
+
+    :param tables: ``[[[["string"]]]]``
+    :return:
+        ``((0, 0, 0, 0), tables[0][0][0][0]) ... , ((i, j, k, l), tables[i][j][k][l])``
+    """
+    return enum_at_depth(tables, 4)
+
+
+def get_text(tables: TablesList) -> str:
+    """
+    Short cut to pull text from any subset of extracted content.
+
+    :param tables: ``[[[["string"]]]]``
+    :return: "string" (all paragraphs in tables joined with '\n\n'
+    """
+    return "\n\n".join(iter_at_depth(tables, 4))
+
+
+def get_html_map(tables: TablesList) -> str:
+    """
+    Create a visual map in html format.
+
+    :param tables: ``[[[["string"]]]]``
+    :return: html to show all strings with index tuples
+
+    Create an html string that can be rendered in a browser to show the relative
+    location and index tuple of every paragraph in the document.
+
+    * Each table will be a grid of cell boxes, outlined in black. * Each paragraph
+    will be prepended with an index tuple. (e.g., ``[[[['text']]]]`` will appear as
+    ``(0, 0, 0, 0) text``.
+    """
+
+    # prepend index tuple to each paragraph
+    tables_4deep = cast(List[List[List[List[str]]]], tables)
+    for (i, j, k, l), paragraph in enum_at_depth(tables, 4):
+        tables_4deep[i][j][k][l] = " ".join([str((i, j, k, l)), paragraph])
+
+    # wrap each paragraph in <pre> tags
+    tables_3deep = cast(List[List[List[str]]], tables_4deep)
+    for (i, j, k), cell in enum_at_depth(tables_4deep, 3):
+        cell = (str(x) for x in cell)
+        tables_3deep[i][j][k] = "".join([f"<pre>{x}</pre>" for x in cell])
+
+    # wrap each cell in <td> tags
+    tables_2deep = cast(List[List[str]], tables_3deep)
+    for (i, j), row in enum_at_depth(tables_3deep, 2):
+        tables_2deep[i][j] = "".join([f"<td>{x}</td>" for x in row])
+
+    # wrap each row in <tr> tags
+    tables_1deep = cast(List[str], tables_2deep)
+    for (i,), table in enum_at_depth(tables_2deep, 1):
+        tables_1deep[i] = "".join(f"<tr>{x}</tr>" for x in table)
+
+    # wrap each table in <table> tags
+    tables_ = "".join([f'<table border="1">{x}</table>' for x in tables_1deep])
+
+    return "<html><body>" + tables_ + "</body></html>"
```

### Comparing `docx2python-2.7.2/docx2python/main.py` & `docx2python-2.7.3/docx2python/main.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-"""Top-level code
-
-:author: Shay Hill
-:created: 7/2/2019
-"""
-from __future__ import annotations
-
-from io import BytesIO
-from pathlib import Path
-from warnings import warn
-
-from .docx_output import DocxContent
-from .docx_reader import DocxReader
-
-
-def docx2python(
-    docx_filename: str | Path | BytesIO,
-    image_folder: str | None = None,
-    html: bool = False,
-    paragraph_styles: bool = False,
-    extract_image: bool | None = None,
-    duplicate_merged_cells: bool = False,
-) -> DocxContent:
-    """
-    Unzip a docx file and extract contents.
-
-    :param docx_filename: path to a docx file
-    :param image_folder: optionally specify an image folder
-        (images in docx will be copied to this folder)
-    :param html: bool, extract some formatting as html
-    :param paragraph_styles: prepend the paragraphs style (if any, else "") to each
-        paragraph. This will only be useful with ``*_runs`` attributes.
-    :param extract_image: bool, extract images from document (default True)
-    :param duplicate_merged_cells: bool, duplicate merged cells to return a mxn
-        nested list for each table (default False)
-    :return: DocxContent object
-    """
-    if extract_image is not None:
-        warn(
-            "'extract_image' is no longer a valid argument for docx2python. If an "
-            + "image_folder is given as an argument to docx2python, images will be "
-            + "written to that folder. A folder can be provided later with "
-            + "``docx2python(filename).write_images(image_folder)``. Images files are "
-            + "available as before with ``docx2text(filename).images`` attribute."
-        )
-    docx_context = DocxReader(
-        docx_filename, html, paragraph_styles, duplicate_merged_cells
-    )
-    docx_content = DocxContent(docx_context, locals())
-    if image_folder:
-        _ = docx_content.images
-    return docx_content
+"""Top-level code
+
+:author: Shay Hill
+:created: 7/2/2019
+"""
+from __future__ import annotations
+
+from io import BytesIO
+from pathlib import Path
+from warnings import warn
+
+from .docx_output import DocxContent
+from .docx_reader import DocxReader
+
+
+def docx2python(
+    docx_filename: str | Path | BytesIO,
+    image_folder: str | None = None,
+    html: bool = False,
+    paragraph_styles: bool = False,
+    extract_image: bool | None = None,
+    duplicate_merged_cells: bool = False,
+) -> DocxContent:
+    """
+    Unzip a docx file and extract contents.
+
+    :param docx_filename: path to a docx file
+    :param image_folder: optionally specify an image folder
+        (images in docx will be copied to this folder)
+    :param html: bool, extract some formatting as html
+    :param paragraph_styles: prepend the paragraphs style (if any, else "") to each
+        paragraph. This will only be useful with ``*_runs`` attributes.
+    :param extract_image: bool, extract images from document (default True)
+    :param duplicate_merged_cells: bool, duplicate merged cells to return a mxn
+        nested list for each table (default False)
+    :return: DocxContent object
+    """
+    if extract_image is not None:
+        warn(
+            "'extract_image' is no longer a valid argument for docx2python. If an "
+            + "image_folder is given as an argument to docx2python, images will be "
+            + "written to that folder. A folder can be provided later with "
+            + "``docx2python(filename).write_images(image_folder)``. Images files are "
+            + "available as before with ``docx2text(filename).images`` attribute."
+        )
+    docx_context = DocxReader(
+        docx_filename, html, paragraph_styles, duplicate_merged_cells
+    )
+    docx_content = DocxContent(docx_context, locals())
+    if image_folder:
+        _ = docx_content.images
+    return docx_content
```

### Comparing `docx2python-2.7.2/docx2python/merge_runs.py` & `docx2python-2.7.3/docx2python/merge_runs.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,154 +1,154 @@
-""" Merge runs with identical formatting.
-
-:author: Shay Hill
-:created: 12/13/2021
-
-Join consecutive xml runs with identical formatting. See docstring for ``merge_elems``.
-"""
-from __future__ import annotations
-
-import functools
-from itertools import groupby
-from typing import TYPE_CHECKING
-
-from lxml.etree import _Element as EtreeElement  # type: ignore
-
-from .attribute_register import RELS_ID, Tags, has_content
-from .text_runs import get_html_formatting
-
-if TYPE_CHECKING:
-    from .docx_reader import File
-
-# identify tags that will be merged together (if formatting is equivalent)
-_MERGEABLE_TAGS = {Tags.RUN, Tags.HYPERLINK, Tags.TEXT, Tags.TEXT_MATH}
-
-
-def _elem_key(file: File, elem: EtreeElement) -> tuple[str, str, list[str]]:
-    """
-    Enough information to tell if two elements are more-or-less identically formatted.
-
-    :param elem: any element in an xml file.
-    :return: A summary of attributes (if two adjacent elements return the same key,
-        they are considered mergeable). Only used to merge elements, so returns None
-        if element tags are not in _MERGEABLE_TAGS.
-
-    Ignore text formatting differences if consecutive link elements point to the same
-    address. Always join these.
-
-    Docx2Text joins consecutive runs and links of the same style. Comparing two
-    elem_key return values will tell you if
-        * elements are the same type
-        * link rels ids reference the same link
-        * run styles are the same (as far as docx2python understands them)
-
-    Elem rId attributes are replaced with rId['Target'] because different rIds can
-    point to identical targets. This is important for hyperlinks, which can look
-    different but point to the same address.
-
-    """
-    tag = elem.tag
-    if tag not in _MERGEABLE_TAGS:
-        return tag, "", []
-
-    # always join links pointing to the same address
-    rels_id = elem.attrib.get(RELS_ID)
-    if rels_id:
-        return tag, str(file.rels[str(rels_id)]), []
-
-    return tag, "", get_html_formatting(elem, file.context.xml2html_format)
-
-
-def merge_elems(file: File, tree: EtreeElement) -> None:
-    """
-    Recursively merge duplicate (as far as docx2python is concerned) elements.
-
-    :param file: File instancce
-    :param tree: root_element from an xml in File instance
-    :effects: Merges consecutive elements if tag, attrib, and style are the same
-
-    There are a few ways consecutive elements can be "identical":
-        * same link
-        * same style
-
-    Often, consecutive, "identical" elements are written as separate elements,
-    because they aren't identical to Word. Word keeps track of revision history,
-    spelling errors, etc., which are meaningless to docx2python.
-
-    <w:p>
-        <w:hyperlink r:id="rId7">  <!-- points to http://www.shayallenhill.com -->
-            <w:r>
-                <w:t>hy</w:t>
-            </w:r>
-        </w:hyperlink>
-        <w:proofErr/>  <!-- docx2python will ignore this proofErr -->
-        <w:hyperlink r:id="rId8">  <!-- points to http://www.shayallenhill.com -->
-            <w:r>
-                <w:t>per</w:t>
-            </w:r>
-        </w:hyperlink>
-        <w:hyperlink r:id="rId9">  <!-- points to http://www.shayallenhill.com -->
-            <w:r w:rsid="asdfas">  <!-- docx2python will ignore this rsid -->
-                <w:t>link</w:t>
-            </w:r>
-        </w:hyperlink>
-    </w:p>
-
-    Docx2python condenses the above to (by merging links)
-
-    <w:p>
-        <w:hyperlink r:id="rId7">  <!-- points to http://www.shayallenhill.com -->
-            <w:r>
-                <w:t>hy</w:t>
-            </w:r>
-            <w:r>
-                <w:t>per</w:t>
-            </w:r>
-            <w:r w:rsid="asdfas">  <!-- docx2python will ignore this rsid -->
-                <w:t>link</w:t>
-            </w:r>
-        </w:hyperlink>
-    </w:p>
-
-    Then to (by merging runs)
-
-    <w:p>
-        <w:hyperlink r:id="rId7">  <!-- points to http://www.shayallenhill.com -->
-            <w:r>
-                <w:t>hy</w:t>
-                <w:t>per</w:t>
-                <w:t>link</w:t>
-            </w:r>
-        </w:hyperlink>
-    </w:p>
-
-    Then finally to (by merging text)
-
-    <w:p>
-        <w:hyperlink r:id="rId7">  <!-- points to http://www.shayallenhill.com -->
-            <w:r>
-                <w:t>hyperlink</w:t>
-            </w:r>
-        </w:hyperlink>
-    </w:p>
-
-    This function only merges runs, text, and hyperlinks, because merging paragraphs
-    or larger elements would ignore information docx2python DOES want to preserve.
-
-    Filter out non-content items so runs can be joined even
-    """
-
-    file_elem_key = functools.partial(_elem_key, file)
-
-    elems = [x for x in tree if has_content(x)]
-    runs = [list(y) for _, y in groupby(elems, key=file_elem_key)]
-
-    for run in (x for x in runs if len(x) > 1 and x[0].tag in _MERGEABLE_TAGS):
-        if run[0].tag in {Tags.TEXT, Tags.TEXT_MATH}:
-            run[0].text = "".join(x.text or "" for x in run)
-        for elem in run[1:]:
-            for e in elem:
-                run[0].append(e)
-            tree.remove(elem)
-
-    for branch in tree:
-        merge_elems(file, branch)
+""" Merge runs with identical formatting.
+
+:author: Shay Hill
+:created: 12/13/2021
+
+Join consecutive xml runs with identical formatting. See docstring for ``merge_elems``.
+"""
+from __future__ import annotations
+
+import functools
+from itertools import groupby
+from typing import TYPE_CHECKING
+
+from lxml.etree import _Element as EtreeElement  # type: ignore
+
+from .attribute_register import RELS_ID, Tags, has_content
+from .text_runs import get_html_formatting
+
+if TYPE_CHECKING:
+    from .docx_reader import File
+
+# identify tags that will be merged together (if formatting is equivalent)
+_MERGEABLE_TAGS = {Tags.RUN, Tags.HYPERLINK, Tags.TEXT, Tags.TEXT_MATH}
+
+
+def _elem_key(file: File, elem: EtreeElement) -> tuple[str, str, list[str]]:
+    """
+    Enough information to tell if two elements are more-or-less identically formatted.
+
+    :param elem: any element in an xml file.
+    :return: A summary of attributes (if two adjacent elements return the same key,
+        they are considered mergeable). Only used to merge elements, so returns None
+        if element tags are not in _MERGEABLE_TAGS.
+
+    Ignore text formatting differences if consecutive link elements point to the same
+    address. Always join these.
+
+    Docx2Text joins consecutive runs and links of the same style. Comparing two
+    elem_key return values will tell you if
+        * elements are the same type
+        * link rels ids reference the same link
+        * run styles are the same (as far as docx2python understands them)
+
+    Elem rId attributes are replaced with rId['Target'] because different rIds can
+    point to identical targets. This is important for hyperlinks, which can look
+    different but point to the same address.
+
+    """
+    tag = elem.tag
+    if tag not in _MERGEABLE_TAGS:
+        return tag, "", []
+
+    # always join links pointing to the same address
+    rels_id = elem.attrib.get(RELS_ID)
+    if rels_id:
+        return tag, str(file.rels[str(rels_id)]), []
+
+    return tag, "", get_html_formatting(elem, file.context.xml2html_format)
+
+
+def merge_elems(file: File, tree: EtreeElement) -> None:
+    """
+    Recursively merge duplicate (as far as docx2python is concerned) elements.
+
+    :param file: File instancce
+    :param tree: root_element from an xml in File instance
+    :effects: Merges consecutive elements if tag, attrib, and style are the same
+
+    There are a few ways consecutive elements can be "identical":
+        * same link
+        * same style
+
+    Often, consecutive, "identical" elements are written as separate elements,
+    because they aren't identical to Word. Word keeps track of revision history,
+    spelling errors, etc., which are meaningless to docx2python.
+
+    <w:p>
+        <w:hyperlink r:id="rId7">  <!-- points to http://www.shayallenhill.com -->
+            <w:r>
+                <w:t>hy</w:t>
+            </w:r>
+        </w:hyperlink>
+        <w:proofErr/>  <!-- docx2python will ignore this proofErr -->
+        <w:hyperlink r:id="rId8">  <!-- points to http://www.shayallenhill.com -->
+            <w:r>
+                <w:t>per</w:t>
+            </w:r>
+        </w:hyperlink>
+        <w:hyperlink r:id="rId9">  <!-- points to http://www.shayallenhill.com -->
+            <w:r w:rsid="asdfas">  <!-- docx2python will ignore this rsid -->
+                <w:t>link</w:t>
+            </w:r>
+        </w:hyperlink>
+    </w:p>
+
+    Docx2python condenses the above to (by merging links)
+
+    <w:p>
+        <w:hyperlink r:id="rId7">  <!-- points to http://www.shayallenhill.com -->
+            <w:r>
+                <w:t>hy</w:t>
+            </w:r>
+            <w:r>
+                <w:t>per</w:t>
+            </w:r>
+            <w:r w:rsid="asdfas">  <!-- docx2python will ignore this rsid -->
+                <w:t>link</w:t>
+            </w:r>
+        </w:hyperlink>
+    </w:p>
+
+    Then to (by merging runs)
+
+    <w:p>
+        <w:hyperlink r:id="rId7">  <!-- points to http://www.shayallenhill.com -->
+            <w:r>
+                <w:t>hy</w:t>
+                <w:t>per</w:t>
+                <w:t>link</w:t>
+            </w:r>
+        </w:hyperlink>
+    </w:p>
+
+    Then finally to (by merging text)
+
+    <w:p>
+        <w:hyperlink r:id="rId7">  <!-- points to http://www.shayallenhill.com -->
+            <w:r>
+                <w:t>hyperlink</w:t>
+            </w:r>
+        </w:hyperlink>
+    </w:p>
+
+    This function only merges runs, text, and hyperlinks, because merging paragraphs
+    or larger elements would ignore information docx2python DOES want to preserve.
+
+    Filter out non-content items so runs can be joined even
+    """
+
+    file_elem_key = functools.partial(_elem_key, file)
+
+    elems = [x for x in tree if has_content(x)]
+    runs = [list(y) for _, y in groupby(elems, key=file_elem_key)]
+
+    for run in (x for x in runs if len(x) > 1 and x[0].tag in _MERGEABLE_TAGS):
+        if run[0].tag in {Tags.TEXT, Tags.TEXT_MATH}:
+            run[0].text = "".join(x.text or "" for x in run)
+        for elem in run[1:]:
+            for e in elem:
+                run[0].append(e)
+            tree.remove(elem)
+
+    for branch in tree:
+        merge_elems(file, branch)
```

### Comparing `docx2python-2.7.2/docx2python/namespace.py` & `docx2python-2.7.3/docx2python/namespace.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-"""Register namespace entries in xml ``document`` elements.
-
-:author: Shay Hill
-:created: 7/5/2019
-
-A ``<w:document>`` element at the top of each xml file defines a namespace::
-
-    <w:document
-        xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships"
-        xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main"
-    />
-
-These entries can be accessed in the file by their abbreviations::
-
-    <w:p>
-        contents of paragraph
-    </w:p>
-
-``lxml.etree`` reads ``"<w:p>"`` as
-
-``"{http://schemas.openxmlformats.org/wordprocessingml/2006/main}p"``
-
-This module defines the necessary namespaces and transforms ``"w:p"`` to
-``{http://...}p``. This allows readable code like::
-
-    if element.tag == qn("w:p"):
-
-instead of::
-
-    if element.tag == "{http://schemas.openxmlformats.org/wordprocessingml/2006/main}p":
-
-If somewhere along the line this package just stops working, it may be that the NSMAP
-entries have been updated for whatever docx you're working with (though that's not
-supposed to ever happen). *If* this happens::
-
-    1) Unzip the docx.
-    2) open ``word/document.xml`` in a text editor.
-    3) Search for xmlns:w=[some string]
-    4) update NSMAP['w'] = some string
-
-Lxml allows (deceptively) easy access to a file's namespaces; however, this is
-problematic because ``root_element.nsmap`` may not retrieve all nsmap entries. Other
-entries may be buried inside sub-environments further down in the tree. It is safer
-to explicate namespace mapping.
-
-If you extend docx2text with other tags, additional NSMAP entries may be necessary.
-"""
-
-
-NSMAP = {
-    "a": "http://schemas.openxmlformats.org/drawingml/2006/main",
-    "cp": "http://schemas.openxmlformats.org/package/2006/metadata/core-properties",
-    "dc": "http://purl.org/dc/elements/1.1/",
-    "dcterms": "http://purl.org/dc/terms/",
-    "m": "http://schemas.openxmlformats.org/officeDocument/2006/math",
-    "r": "http://schemas.openxmlformats.org/officeDocument/2006/relationships",
-    "v": "urn:schemas-microsoft-com:vml",
-    "w": "http://schemas.openxmlformats.org/wordprocessingml/2006/main",
-    "wp": "http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing",
-}
-
-
-def qn(tag: str) -> str:
-    """
-    Turn a namespace-prefixed tag into a Clark-notation qualified tag.
-
-    :param tag: namespace-prefixed tag, e.g. ``w:p``
-    :return: Clark-notation qualified tag,
-        e.g. ``{http://schemas.openxmlformats.org/wordprocessingml/2006/main}p``
-
-    Stands for 'qualified name', a utility function to turn a namespace prefixed tag
-    name into a Clark-notation qualified tag name for lxml.
-
-        >>> qn('w:cSld')
-        '{http://schemas.../main}cSld'
-
-    Source: https://github.com/python-openxml/python-docx/
-    """
-    prefix, tagroot = tag.split(":")
-    uri = NSMAP[prefix]
-    return f"{{{uri}}}{tagroot}"
+"""Register namespace entries in xml ``document`` elements.
+
+:author: Shay Hill
+:created: 7/5/2019
+
+A ``<w:document>`` element at the top of each xml file defines a namespace::
+
+    <w:document
+        xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships"
+        xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main"
+    />
+
+These entries can be accessed in the file by their abbreviations::
+
+    <w:p>
+        contents of paragraph
+    </w:p>
+
+``lxml.etree`` reads ``"<w:p>"`` as
+
+``"{http://schemas.openxmlformats.org/wordprocessingml/2006/main}p"``
+
+This module defines the necessary namespaces and transforms ``"w:p"`` to
+``{http://...}p``. This allows readable code like::
+
+    if element.tag == qn("w:p"):
+
+instead of::
+
+    if element.tag == "{http://schemas.openxmlformats.org/wordprocessingml/2006/main}p":
+
+If somewhere along the line this package just stops working, it may be that the NSMAP
+entries have been updated for whatever docx you're working with (though that's not
+supposed to ever happen). *If* this happens::
+
+    1) Unzip the docx.
+    2) open ``word/document.xml`` in a text editor.
+    3) Search for xmlns:w=[some string]
+    4) update NSMAP['w'] = some string
+
+Lxml allows (deceptively) easy access to a file's namespaces; however, this is
+problematic because ``root_element.nsmap`` may not retrieve all nsmap entries. Other
+entries may be buried inside sub-environments further down in the tree. It is safer
+to explicate namespace mapping.
+
+If you extend docx2text with other tags, additional NSMAP entries may be necessary.
+"""
+
+
+NSMAP = {
+    "a": "http://schemas.openxmlformats.org/drawingml/2006/main",
+    "cp": "http://schemas.openxmlformats.org/package/2006/metadata/core-properties",
+    "dc": "http://purl.org/dc/elements/1.1/",
+    "dcterms": "http://purl.org/dc/terms/",
+    "m": "http://schemas.openxmlformats.org/officeDocument/2006/math",
+    "r": "http://schemas.openxmlformats.org/officeDocument/2006/relationships",
+    "v": "urn:schemas-microsoft-com:vml",
+    "w": "http://schemas.openxmlformats.org/wordprocessingml/2006/main",
+    "wp": "http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing",
+}
+
+
+def qn(tag: str) -> str:
+    """
+    Turn a namespace-prefixed tag into a Clark-notation qualified tag.
+
+    :param tag: namespace-prefixed tag, e.g. ``w:p``
+    :return: Clark-notation qualified tag,
+        e.g. ``{http://schemas.openxmlformats.org/wordprocessingml/2006/main}p``
+
+    Stands for 'qualified name', a utility function to turn a namespace prefixed tag
+    name into a Clark-notation qualified tag name for lxml.
+
+        >>> qn('w:cSld')
+        '{http://schemas.../main}cSld'
+
+    Source: https://github.com/python-openxml/python-docx/
+    """
+    prefix, tagroot = tag.split(":")
+    uri = NSMAP[prefix]
+    return f"{{{uri}}}{tagroot}"
```

### Comparing `docx2python-2.7.2/docx2python/numbering_formats.py` & `docx2python-2.7.3/docx2python/numbering_formats.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-"""Numbering formats for converted XML lists.
-
-:author: Shay Hill
-:created: 6/26/2019
-
-I don't want to add non-ascii text to a potentially ascii-only file, so all bullets
-are '--' and Roman numerals stop at 3999.
-
-Doesn't capture formatting like 1.1.1 or b) or (ii). Only the six basic formats are
-covered::
-
-    -- bullet
-    1  decimal
-    a  lowerLetter
-    A  upperLetter
-    i  lowerRoman
-    I  upperRoman
-"""
-
-from string import ascii_lowercase
-
-# Subs to convert any number of i's to a proper Roman numeral
-# fmt=off
-ROMAN_SUBS = [
-    ("iiiii", "v"),  # 1+1+1+1+1 -> 5
-    ("vv", "x"),  # 5+5 -> 10
-    ("xxxxx", "l"),  # 10+10+10+10 -> 50
-    ("ll", "c"),  # 50+50 -> 100
-    ("ccccc", "d"),  # 100+100+100+100+100 -> 500
-    ("dd", "m"),  # 500+500 -> 1000
-    ("iiii", "iv"),  # 1+1+1+1 -> 4
-    ("viv", "ix"),  # 5+4 -> 9
-    ("xxxx", "xl"),  # 10+10+10+10 -> 40
-    ("lxl", "xc"),  # 50+40 -> 90
-    ("cccc", "cd"),  # 100+100+100+100 -> 40
-    ("dcd", "cm"),  # 500+400 -> 900
-]
-# fmt=on
-
-
-def lower_letter(n: int) -> str:
-    """
-    Convert a positive integer to a string of letters representing base 26.
-
-    :param n: any positive integer
-    :return: the kind of "numbering" used for numbered lists and excel columns.
-        (a, b, c ... aa, ab ...) Zero is undefined.
-    :raise ValueError: if n is not a positive integer
-
-        >>> lower_letter(1)
-        'a'
-        >>> lower_letter(26)
-        'z'
-        >>> lower_letter(27)
-        'aa'
-    """
-    if n < 1:
-        raise ValueError("0 and <1 are not defined for this numbering")
-    result = ""
-    while n:
-        n, remainder = divmod(n - 1, 26)
-        result = ascii_lowercase[remainder] + result
-    return result
-
-
-def upper_letter(n: int) -> str:
-    """Get int as an upprecase letter.
-
-    :param n: any positive integer
-    :return: the kind of "numbering" used for numbered lists and excel columns.
-    """
-    return lower_letter(n).upper()
-
-
-def lower_roman(n: int) -> str:
-    """
-    Convert a positive integer to a lowercase Roman numeral
-
-    :param n: any positive integer
-    :return: Roman number equivalent of n
-    :raise ValueError: if n is not a positive integer
-
-        >>> lower_roman(1)
-        'i'
-        >>> lower_roman(9)
-        'ix'
-        >>> lower_roman(44)
-        'xliv'
-
-    Numbers greater than 3999 can be expressed with a bar over the number. The bar
-    means "times 1000" (e.g., iv with a bar over it would be 4000).
-
-    It'll never happen in this project, and I don't want to add non-ascii to what
-    might be a pure ascii file, so this function will keep adding 'm' to as many
-    thousand as you'd like.
-
-        >>> lower_roman(10000)
-        'mmmmmmmmmm'
-    """
-    if n < 1:
-        raise ValueError(f"the Romans hadn't figured out {n}")
-    result = "i" * n
-    for pattern, replacement in ROMAN_SUBS:
-        result = result.replace(pattern, replacement)
-    return result
-
-
-def upper_roman(n: int) -> str:
-    """Get int as an uppercase Roman numeral.
-
-    :param n: any positive integer
-    :return: Roman number equivalent of n
-    """
-    return lower_roman(n).upper()
-
-
-def decimal(n: int) -> str:
-    """Get int as a decimal number string
-
-    :param n: any integer
-    :return: string such that int(decimal(n)) == n
-    """
-    return str(n)
-
-
-def bullet(_: int = 0) -> str:
-    """Get the string we're using to replace bullets.
-
-    :return: the string we're using to replace bullets.
-    """
-    return "--"
+"""Numbering formats for converted XML lists.
+
+:author: Shay Hill
+:created: 6/26/2019
+
+I don't want to add non-ascii text to a potentially ascii-only file, so all bullets
+are '--' and Roman numerals stop at 3999.
+
+Doesn't capture formatting like 1.1.1 or b) or (ii). Only the six basic formats are
+covered::
+
+    -- bullet
+    1  decimal
+    a  lowerLetter
+    A  upperLetter
+    i  lowerRoman
+    I  upperRoman
+"""
+
+from string import ascii_lowercase
+
+# Subs to convert any number of i's to a proper Roman numeral
+# fmt=off
+ROMAN_SUBS = [
+    ("iiiii", "v"),  # 1+1+1+1+1 -> 5
+    ("vv", "x"),  # 5+5 -> 10
+    ("xxxxx", "l"),  # 10+10+10+10 -> 50
+    ("ll", "c"),  # 50+50 -> 100
+    ("ccccc", "d"),  # 100+100+100+100+100 -> 500
+    ("dd", "m"),  # 500+500 -> 1000
+    ("iiii", "iv"),  # 1+1+1+1 -> 4
+    ("viv", "ix"),  # 5+4 -> 9
+    ("xxxx", "xl"),  # 10+10+10+10 -> 40
+    ("lxl", "xc"),  # 50+40 -> 90
+    ("cccc", "cd"),  # 100+100+100+100 -> 40
+    ("dcd", "cm"),  # 500+400 -> 900
+]
+# fmt=on
+
+
+def lower_letter(n: int) -> str:
+    """
+    Convert a positive integer to a string of letters representing base 26.
+
+    :param n: any positive integer
+    :return: the kind of "numbering" used for numbered lists and excel columns.
+        (a, b, c ... aa, ab ...) Zero is undefined.
+    :raise ValueError: if n is not a positive integer
+
+        >>> lower_letter(1)
+        'a'
+        >>> lower_letter(26)
+        'z'
+        >>> lower_letter(27)
+        'aa'
+    """
+    if n < 1:
+        raise ValueError("0 and <1 are not defined for this numbering")
+    result = ""
+    while n:
+        n, remainder = divmod(n - 1, 26)
+        result = ascii_lowercase[remainder] + result
+    return result
+
+
+def upper_letter(n: int) -> str:
+    """Get int as an upprecase letter.
+
+    :param n: any positive integer
+    :return: the kind of "numbering" used for numbered lists and excel columns.
+    """
+    return lower_letter(n).upper()
+
+
+def lower_roman(n: int) -> str:
+    """
+    Convert a positive integer to a lowercase Roman numeral
+
+    :param n: any positive integer
+    :return: Roman number equivalent of n
+    :raise ValueError: if n is not a positive integer
+
+        >>> lower_roman(1)
+        'i'
+        >>> lower_roman(9)
+        'ix'
+        >>> lower_roman(44)
+        'xliv'
+
+    Numbers greater than 3999 can be expressed with a bar over the number. The bar
+    means "times 1000" (e.g., iv with a bar over it would be 4000).
+
+    It'll never happen in this project, and I don't want to add non-ascii to what
+    might be a pure ascii file, so this function will keep adding 'm' to as many
+    thousand as you'd like.
+
+        >>> lower_roman(10000)
+        'mmmmmmmmmm'
+    """
+    if n < 1:
+        raise ValueError(f"the Romans hadn't figured out {n}")
+    result = "i" * n
+    for pattern, replacement in ROMAN_SUBS:
+        result = result.replace(pattern, replacement)
+    return result
+
+
+def upper_roman(n: int) -> str:
+    """Get int as an uppercase Roman numeral.
+
+    :param n: any positive integer
+    :return: Roman number equivalent of n
+    """
+    return lower_roman(n).upper()
+
+
+def decimal(n: int) -> str:
+    """Get int as a decimal number string
+
+    :param n: any integer
+    :return: string such that int(decimal(n)) == n
+    """
+    return str(n)
+
+
+def bullet(_: int = 0) -> str:
+    """Get the string we're using to replace bullets.
+
+    :return: the string we're using to replace bullets.
+    """
+    return "--"
```

### Comparing `docx2python-2.7.2/docx2python/text_runs.py` & `docx2python-2.7.3/docx2python/text_runs.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,299 +1,299 @@
-"""Get text run formatting.
-
-:author: Shay Hill
-:created: 7/4/2019
-
-Text runs are formatted inline in the ``trash/document.xml`` or header files. Read
-those elements to extract formatting information.
-"""
-from __future__ import annotations
-
-import re
-from collections import defaultdict
-from contextlib import suppress
-from typing import Sequence, Tuple, Union
-
-from lxml.etree import _Element as EtreeElement  # type: ignore
-
-from .attribute_register import HtmlFormatter, Tags
-from .namespace import qn
-
-
-def _elem_tag_str(elem: EtreeElement) -> str:
-    """The text part of an elem.tag (the portion right of the colon)
-
-    :param elem: an xml element
-    :return: the text part of an elem.tag (the portion right of the colon)
-    :raise RuntimeError: if the tag is not qualified
-
-    create with:
-
-        document = etree.fromstring('bytes string')
-        # recursively search document elements.
-
-    **E.g., given**:
-
-        document = etree.fromstring('bytes string')
-        # document.tag = '{http://schemas.openxml.../2006/main}:document'
-        elem_tag_str(document)
-
-    **E.g., returns**:
-
-        'document'
-    """
-    tag_str = re.match(r"{.*}(?P<tag_name>\w+)", elem.tag)
-    if tag_str:
-        return tag_str.group("tag_name")
-    raise RuntimeError("could not get tag from elem")
-
-
-def _gather_sub_vals(element: EtreeElement, qname: str) -> dict[str, str | None]:
-    """Gather formatting elements for a paragraph or text run.
-
-    :param element: a ``<w:r>`` or ``<w:p>`` xml element. Maybe others
-    :param qname: qualified name for child element.
-
-    create with::
-
-        document = etree.fromstring('bytes string')
-        # recursively search document for <w:r> elements.
-
-    :return: Style names ('b/', 'sz', etc.) mapped to values.
-
-    To keep things more homogeneous, I've given tags like ``<w:b/>`` (bold) a value of
-    None, even though they don't take a value in xml.
-
-    Each element of rPr will be either present (returned tag: None) or have a value
-    (returned tag: val).
-
-    **E.g., given**::
-
-         <w:r w:rsidRPr="000E1B98">
-            <w:rPr>
-                <w:rFonts w:ascii="Arial"/>
-                <w:b/>
-                <w:sz w:val="32"/>
-                <w:szCs w:val="32"/>
-                <w:u w:val="single"/>
-            </w:rPr>
-            <w:t>text styled  with rPaa
-            </w:t>
-        </w:r>
-
-    **E.g., returns**::
-
-        {
-            "rFonts": True,
-            "b": None,
-            "u": "single",
-            "i": None,
-            "sz": "32",
-            "color": "red",
-            "szCs": "32",
-        }
-    """
-
-    sub_vals: dict[str, str | None] = {}
-    with suppress(StopIteration):
-        for sub_element in next(element.iterfind(qname)):
-            sub_val = sub_element.attrib.get(qn("w:val"))
-            if sub_val:
-                sub_vals[_elem_tag_str(sub_element)] = str(sub_val)
-            else:
-                sub_vals[_elem_tag_str(sub_element)] = None
-    return sub_vals
-
-
-def gather_Pr(element: EtreeElement) -> dict[str, str | None]:
-    """
-    Gather style values for a <w:r>, <w:tc>, or <w:p> element (maybe others)
-
-    :param element: any xml element. r and p elems typically have Pr values.
-    :return: Style names ('b/', 'sz', etc.) mapped to values.
-
-    These elements often have a subelement ``<w:pPr>`` or ``<w:rPr>`` which contains
-    formatting instructions. This includes colspan, rowspan, and other table-cell
-    properties.
-
-    Will infer a style element qualified name: p -> pPr; r -> rPr
-
-    Call this with any element. Runs and Paragraphs may have a Pr element. Most
-    elements will not, but the function will will quietly return an empty dict.
-    """
-    return _gather_sub_vals(element, element.tag + "Pr")
-
-
-def get_pStyle(paragraph_element: EtreeElement) -> str:
-    """
-    Collect and format paragraph -> pPr -> pStyle value.
-
-    :param paragraph_element: a ``<w:p>`` xml element
-
-    :return: ``[(pStyle value, '')]``
-
-    Also see docstring for ``gather_pPr``
-    """
-    return gather_Pr(paragraph_element).get("pStyle", "") or ""
-
-
-def get_run_formatting(
-    run_element: EtreeElement, xml2html: dict[str, HtmlFormatter]
-) -> list[str]:
-    """
-    Get run-element formatting converted into html.
-
-    :param run_element: a ``<w:r>`` xml element
-        create with::
-
-            document = etree.fromstring('bytes string')
-            # recursively search document for <w:r> elements.
-
-    :param xml2html: mapping to convert xml styles to html styles
-        e.g., {
-            'b': (<function <lambda> at 0x0000026BC7875A60>,),
-            'smallCaps': (<function <lambda> at 0x0000026BC7896DC0>, 'font', 'style')
-        }
-
-    :return: ``['b', 'i', ...]``
-
-    Lists are always returned in order:
-
-    ``"span"`` first then any other styles in alphabetical order.
-
-    Also see docstring for ``gather_rPr``
-    """
-    return _format_Pr_into_html(gather_Pr(run_element), xml2html)
-
-
-def get_paragraph_formatting(
-    paragraph_element: EtreeElement, xml2html: dict[str, HtmlFormatter]
-) -> list[str]:
-    """
-    Get paragraph-element formatting converted into html.
-
-    :param paragraph_element: a ``<w:p>`` xml element
-        create with::
-
-            document = etree.fromstring('bytes string')
-            # recursively search document for <w:r> elements.
-
-    :param xml2html: mapping to convert xml styles to html styles
-        e.g., {
-            'b': (<function <lambda> at 0x0000026BC7875A60>,),
-            'smallCaps': (<function <lambda> at 0x0000026BC7896DC0>, 'font', 'style')
-        }
-
-    :return: ``['b', 'i', ...]``
-
-    Tuples are always returned in order:
-
-    ``"font"`` first then any other styles in alphabetical order.
-
-    Also see docstring for ``gather_rPr``
-    """
-    return _format_Pr_into_html({get_pStyle(paragraph_element): None}, xml2html)
-
-
-def _format_Pr_into_html(
-    Pr2val: dict[str, str | None], xml2html: dict[str, HtmlFormatter]
-) -> list[str]:
-    """
-    Format tags and values into html strings.
-
-    :param Pr2val: tags mapped to values (extracted from xml)
-        e.g., {'b': None, 'bCs': None}
-    :param xml2html: mapping to convert xml styles to html styles
-        e.g., {
-            'b': (<function <lambda> at 0x0000026BC7875A60>,),
-            'smallCaps': (<function <lambda> at 0x0000026BC7896DC0>, 'span', 'style')
-        }
-    :return: the interior part of html opening tags, eg, ['span style="..."', 'b', 'i']
-
-    Types of styles supported:
-    (None, None, formatter -> tag, None)
-        -> outside any containers, no value set, e.g., `<b>`
-    ('span', 'style', formatter -> tag, val)
-        -> inside a span, inside a style property, e.g., `<span style="tag: val">`
-
-    Other formats would probably work, but they aren't necessary to support the tags
-    supported (see README).
-    """
-    style: list[str] = []
-
-    # group together supported formats with the same container and property_
-    # e.g., group together everything that goes into `<span style="$HERE$">`
-    # con_pro2for[(con, pro)] = string created from for
-    cp2f_keytype = Tuple[Union[None, str], Union[None, str]]
-    con_pro2for: defaultdict[cp2f_keytype, list[str]] = defaultdict(list)
-    for tag, val in ((k, v) for k, v in Pr2val.items() if k in xml2html):
-        formatter, container, property_ = xml2html[tag]
-        con_pro2for[(container, property_)].append(formatter(tag, val or ""))
-
-    # group together supported formats with the same container
-    # e.g., group together everything that goes into `<span $HERE$>`
-    # con2pro_for[(con,)] = string created from pro and for
-    con2pro_for: defaultdict[str, list[str]] = defaultdict(list)
-    for k, v in sorted((k, v) for k, v in con_pro2for.items() if k[1] is not None):
-        con2pro_for[k[0] or ""].append(f'{k[1]}="{";".join(sorted(v))}"')
-
-    # incorporate container type into string
-    # style.append(string created from con, pro, and for)
-    for k_, v_ in sorted((k, v) for k, v in con2pro_for.items() if k):
-        style.append(f"{k_} {' '.join(v_)}")
-
-    # add back in formats with no container or property_
-    style += sorted(con_pro2for[(None, None)])
-    return style
-
-
-def get_html_formatting(
-    elem: EtreeElement, xml2html: dict[str, HtmlFormatter]
-) -> list[str]:
-    """
-    Get style for an element (if available)
-
-    :param elem: a run or paragraph element.
-    :param xml2html: mapping to convert xml styles to html styles
-        e.g., {
-            'b': (<function <lambda> at 0x0000026BC7875A60>,),
-            'smallCaps': (<function <lambda> at 0x0000026BC7896DC0>, 'font', 'style')
-        }
-    :return: ``[(rPr, val), (rPr, val) ...]``
-    """
-    if elem.tag == Tags.RUN:
-        return get_run_formatting(elem, xml2html)
-    if elem.tag == Tags.PARAGRAPH:
-        return get_paragraph_formatting(elem, xml2html)
-    return []
-
-
-def html_open(style: Sequence[str]) -> str:
-    """
-    HTML tags to open a style.
-
-    :param style: sequence of html tags without the '<' and '>'
-    :return: opening html tags joined into a single string
-
-    >>> style = ['font color="red" size="32"', 'b', 'i', 'u']
-    >>> html_open(style)
-    '<font color="red" size="32"><b><i><u>'
-    """
-    return "".join(f"<{x}>" for x in style)
-
-
-def html_close(style: list[str]) -> str:
-    """
-    HTML tags to close a style.
-
-    :param style: sequence of html tags without the '<' and '>'
-    :return: closing html tags joined into a single string
-
-    >>> style = ['font color="red" size="32"', 'b', 'i', 'u']
-    >>> html_close(style)
-    '</u></i></b></font>'
-
-    Tags will always be in reverse (of open) order, so open - close will look like::
-
-        <b><i><u>text</u></i></b>
-    """
-    return "".join(f"</{x.split()[0]}>" for x in reversed(style))
+"""Get text run formatting.
+
+:author: Shay Hill
+:created: 7/4/2019
+
+Text runs are formatted inline in the ``trash/document.xml`` or header files. Read
+those elements to extract formatting information.
+"""
+from __future__ import annotations
+
+import re
+from collections import defaultdict
+from contextlib import suppress
+from typing import Sequence, Tuple, Union
+
+from lxml.etree import _Element as EtreeElement  # type: ignore
+
+from .attribute_register import HtmlFormatter, Tags
+from .namespace import qn
+
+
+def _elem_tag_str(elem: EtreeElement) -> str:
+    """The text part of an elem.tag (the portion right of the colon)
+
+    :param elem: an xml element
+    :return: the text part of an elem.tag (the portion right of the colon)
+    :raise RuntimeError: if the tag is not qualified
+
+    create with:
+
+        document = etree.fromstring('bytes string')
+        # recursively search document elements.
+
+    **E.g., given**:
+
+        document = etree.fromstring('bytes string')
+        # document.tag = '{http://schemas.openxml.../2006/main}:document'
+        elem_tag_str(document)
+
+    **E.g., returns**:
+
+        'document'
+    """
+    tag_str = re.match(r"{.*}(?P<tag_name>\w+)", elem.tag)
+    if tag_str:
+        return tag_str.group("tag_name")
+    raise RuntimeError("could not get tag from elem")
+
+
+def _gather_sub_vals(element: EtreeElement, qname: str) -> dict[str, str | None]:
+    """Gather formatting elements for a paragraph or text run.
+
+    :param element: a ``<w:r>`` or ``<w:p>`` xml element. Maybe others
+    :param qname: qualified name for child element.
+
+    create with::
+
+        document = etree.fromstring('bytes string')
+        # recursively search document for <w:r> elements.
+
+    :return: Style names ('b/', 'sz', etc.) mapped to values.
+
+    To keep things more homogeneous, I've given tags like ``<w:b/>`` (bold) a value of
+    None, even though they don't take a value in xml.
+
+    Each element of rPr will be either present (returned tag: None) or have a value
+    (returned tag: val).
+
+    **E.g., given**::
+
+         <w:r w:rsidRPr="000E1B98">
+            <w:rPr>
+                <w:rFonts w:ascii="Arial"/>
+                <w:b/>
+                <w:sz w:val="32"/>
+                <w:szCs w:val="32"/>
+                <w:u w:val="single"/>
+            </w:rPr>
+            <w:t>text styled  with rPaa
+            </w:t>
+        </w:r>
+
+    **E.g., returns**::
+
+        {
+            "rFonts": True,
+            "b": None,
+            "u": "single",
+            "i": None,
+            "sz": "32",
+            "color": "red",
+            "szCs": "32",
+        }
+    """
+
+    sub_vals: dict[str, str | None] = {}
+    with suppress(StopIteration):
+        for sub_element in next(element.iterfind(qname)):
+            sub_val = sub_element.attrib.get(qn("w:val"))
+            if sub_val:
+                sub_vals[_elem_tag_str(sub_element)] = str(sub_val)
+            else:
+                sub_vals[_elem_tag_str(sub_element)] = None
+    return sub_vals
+
+
+def gather_Pr(element: EtreeElement) -> dict[str, str | None]:
+    """
+    Gather style values for a <w:r>, <w:tc>, or <w:p> element (maybe others)
+
+    :param element: any xml element. r and p elems typically have Pr values.
+    :return: Style names ('b/', 'sz', etc.) mapped to values.
+
+    These elements often have a subelement ``<w:pPr>`` or ``<w:rPr>`` which contains
+    formatting instructions. This includes colspan, rowspan, and other table-cell
+    properties.
+
+    Will infer a style element qualified name: p -> pPr; r -> rPr
+
+    Call this with any element. Runs and Paragraphs may have a Pr element. Most
+    elements will not, but the function will will quietly return an empty dict.
+    """
+    return _gather_sub_vals(element, element.tag + "Pr")
+
+
+def get_pStyle(paragraph_element: EtreeElement) -> str:
+    """
+    Collect and format paragraph -> pPr -> pStyle value.
+
+    :param paragraph_element: a ``<w:p>`` xml element
+
+    :return: ``[(pStyle value, '')]``
+
+    Also see docstring for ``gather_pPr``
+    """
+    return gather_Pr(paragraph_element).get("pStyle", "") or ""
+
+
+def get_run_formatting(
+    run_element: EtreeElement, xml2html: dict[str, HtmlFormatter]
+) -> list[str]:
+    """
+    Get run-element formatting converted into html.
+
+    :param run_element: a ``<w:r>`` xml element
+        create with::
+
+            document = etree.fromstring('bytes string')
+            # recursively search document for <w:r> elements.
+
+    :param xml2html: mapping to convert xml styles to html styles
+        e.g., {
+            'b': (<function <lambda> at 0x0000026BC7875A60>,),
+            'smallCaps': (<function <lambda> at 0x0000026BC7896DC0>, 'font', 'style')
+        }
+
+    :return: ``['b', 'i', ...]``
+
+    Lists are always returned in order:
+
+    ``"span"`` first then any other styles in alphabetical order.
+
+    Also see docstring for ``gather_rPr``
+    """
+    return _format_Pr_into_html(gather_Pr(run_element), xml2html)
+
+
+def get_paragraph_formatting(
+    paragraph_element: EtreeElement, xml2html: dict[str, HtmlFormatter]
+) -> list[str]:
+    """
+    Get paragraph-element formatting converted into html.
+
+    :param paragraph_element: a ``<w:p>`` xml element
+        create with::
+
+            document = etree.fromstring('bytes string')
+            # recursively search document for <w:r> elements.
+
+    :param xml2html: mapping to convert xml styles to html styles
+        e.g., {
+            'b': (<function <lambda> at 0x0000026BC7875A60>,),
+            'smallCaps': (<function <lambda> at 0x0000026BC7896DC0>, 'font', 'style')
+        }
+
+    :return: ``['b', 'i', ...]``
+
+    Tuples are always returned in order:
+
+    ``"font"`` first then any other styles in alphabetical order.
+
+    Also see docstring for ``gather_rPr``
+    """
+    return _format_Pr_into_html({get_pStyle(paragraph_element): None}, xml2html)
+
+
+def _format_Pr_into_html(
+    Pr2val: dict[str, str | None], xml2html: dict[str, HtmlFormatter]
+) -> list[str]:
+    """
+    Format tags and values into html strings.
+
+    :param Pr2val: tags mapped to values (extracted from xml)
+        e.g., {'b': None, 'bCs': None}
+    :param xml2html: mapping to convert xml styles to html styles
+        e.g., {
+            'b': (<function <lambda> at 0x0000026BC7875A60>,),
+            'smallCaps': (<function <lambda> at 0x0000026BC7896DC0>, 'span', 'style')
+        }
+    :return: the interior part of html opening tags, eg, ['span style="..."', 'b', 'i']
+
+    Types of styles supported:
+    (None, None, formatter -> tag, None)
+        -> outside any containers, no value set, e.g., `<b>`
+    ('span', 'style', formatter -> tag, val)
+        -> inside a span, inside a style property, e.g., `<span style="tag: val">`
+
+    Other formats would probably work, but they aren't necessary to support the tags
+    supported (see README).
+    """
+    style: list[str] = []
+
+    # group together supported formats with the same container and property_
+    # e.g., group together everything that goes into `<span style="$HERE$">`
+    # con_pro2for[(con, pro)] = string created from for
+    cp2f_keytype = Tuple[Union[None, str], Union[None, str]]
+    con_pro2for: defaultdict[cp2f_keytype, list[str]] = defaultdict(list)
+    for tag, val in ((k, v) for k, v in Pr2val.items() if k in xml2html):
+        formatter, container, property_ = xml2html[tag]
+        con_pro2for[(container, property_)].append(formatter(tag, val or ""))
+
+    # group together supported formats with the same container
+    # e.g., group together everything that goes into `<span $HERE$>`
+    # con2pro_for[(con,)] = string created from pro and for
+    con2pro_for: defaultdict[str, list[str]] = defaultdict(list)
+    for k, v in sorted((k, v) for k, v in con_pro2for.items() if k[1] is not None):
+        con2pro_for[k[0] or ""].append(f'{k[1]}="{";".join(sorted(v))}"')
+
+    # incorporate container type into string
+    # style.append(string created from con, pro, and for)
+    for k_, v_ in sorted((k, v) for k, v in con2pro_for.items() if k):
+        style.append(f"{k_} {' '.join(v_)}")
+
+    # add back in formats with no container or property_
+    style += sorted(con_pro2for[(None, None)])
+    return style
+
+
+def get_html_formatting(
+    elem: EtreeElement, xml2html: dict[str, HtmlFormatter]
+) -> list[str]:
+    """
+    Get style for an element (if available)
+
+    :param elem: a run or paragraph element.
+    :param xml2html: mapping to convert xml styles to html styles
+        e.g., {
+            'b': (<function <lambda> at 0x0000026BC7875A60>,),
+            'smallCaps': (<function <lambda> at 0x0000026BC7896DC0>, 'font', 'style')
+        }
+    :return: ``[(rPr, val), (rPr, val) ...]``
+    """
+    if elem.tag == Tags.RUN:
+        return get_run_formatting(elem, xml2html)
+    if elem.tag == Tags.PARAGRAPH:
+        return get_paragraph_formatting(elem, xml2html)
+    return []
+
+
+def html_open(style: Sequence[str]) -> str:
+    """
+    HTML tags to open a style.
+
+    :param style: sequence of html tags without the '<' and '>'
+    :return: opening html tags joined into a single string
+
+    >>> style = ['font color="red" size="32"', 'b', 'i', 'u']
+    >>> html_open(style)
+    '<font color="red" size="32"><b><i><u>'
+    """
+    return "".join(f"<{x}>" for x in style)
+
+
+def html_close(style: list[str]) -> str:
+    """
+    HTML tags to close a style.
+
+    :param style: sequence of html tags without the '<' and '>'
+    :return: closing html tags joined into a single string
+
+    >>> style = ['font color="red" size="32"', 'b', 'i', 'u']
+    >>> html_close(style)
+    '</u></i></b></font>'
+
+    Tags will always be in reverse (of open) order, so open - close will look like::
+
+        <b><i><u>text</u></i></b>
+    """
+    return "".join(f"</{x.split()[0]}>" for x in reversed(style))
```

### Comparing `docx2python-2.7.2/docx2python/utilities.py` & `docx2python-2.7.3/docx2python/utilities.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-"""Utility / example functions using new (as of 2.0.0 Docx2Python features)
-
-:author: Shay Hill
-:created: 2021-12-21
-
-Docx2Python version two exposes extracted xml in the DocxReader object and has a new
-paragraph_styles argument. These functions use these new features as utilities /
-examples.
-"""
-
-from __future__ import annotations
-
-import copy
-import re
-from pathlib import Path
-from typing import Iterator
-
-from lxml import etree
-from lxml.etree import _Element as EtreeElement  # type: ignore
-
-from docx2python.attribute_register import Tags
-
-from .iterators import iter_at_depth
-from .main import docx2python
-
-
-def _copy_new_text(elem: EtreeElement, new_text: str) -> EtreeElement:
-    """Copy a text element and replace text.
-
-    :param elem: an etree element with tag w:t
-    :param new_text: text to replace elem.text
-    :return: a new etree element with tag w:t and text new_text
-    """
-    new_elem = copy.deepcopy(elem)
-    new_elem.text = new_text
-    return new_elem
-
-
-def replace_root_text(root: EtreeElement, old: str, new: str) -> None:
-    """Replace :old: with :new: in all descendants of :root:
-
-    :param root: an etree element presumably containing descendant text elements
-    :param old: text to be replaced
-    :param new: replacement text
-
-    Will use softbreaks <br> to preserve line breaks in replacement text.
-    """
-
-    def recursive_text_replace(branch: EtreeElement):
-        """Replace any text element contining old with one or more elements.
-
-        :param branch: an etree element
-        """
-        for elem in tuple(branch):
-            if not elem.text or old not in elem.text:
-                recursive_text_replace(elem)
-                continue
-
-            # create a new text element for each line in replacement text
-            text = elem.text.replace(old, new)
-            new_elems = [_copy_new_text(elem, line) for line in text.splitlines()]
-
-            # insert breakpoints where line breaks were
-            breaks = [etree.Element(Tags.BR) for _ in new_elems]
-            new_elems = [x for pair in zip(new_elems, breaks) for x in pair][:-1]
-
-            # replace the original element with the new elements
-            parent = elem.getparent()
-            assert parent is not None
-            index = parent.index(elem)
-            parent[index : index + 1] = new_elems
-
-    recursive_text_replace(root)
-
-
-def replace_docx_text(
-    path_in: Path | str,
-    path_out: Path | str,
-    *replacements: tuple[str, str],
-    html: bool = False,
-) -> None:
-    """Replace text in a docx file.
-
-    :param path_in: path to input docx
-    :param path_out: path to output docx with text replaced
-    :param replacements: tuples of strings (a, b) replace a with b for each in docx.
-    :param html: respect formatting (as far as docx2python can see formatting)
-    """
-    reader = docx2python(path_in, html=html).docx_reader
-    for file in reader.content_files():
-        root = file.root_element
-        for replacement in replacements:
-            replace_root_text(root, *replacement)
-    reader.save(path_out)
-    reader.close()
-
-
-def get_links(path_in: Path | str) -> Iterator[tuple[str, str]]:
-    """Iter links inside a docx file as (href, text)
-
-    :param path_in: path to input docx
-    :yield: every link in the file as a tuple of (href, text)
-    :return: None
-    """
-    link_pattern = re.compile('<a href="(?P<href>[^"]+)">(?P<text>[^<]+)</a>')
-    extraction = docx2python(path_in)
-    for run in iter_at_depth(extraction.document_runs, 5):
-        match = re.match(link_pattern, run)
-        if match:
-            href, text = match.groups()
-            yield href, text
-    extraction.close()
-
-
-def get_headings(path_in: Path | str) -> Iterator[list[str]]:
-    """Iter paragraphs with 'Heading' patagraph_style
-
-    :param path_in: path to input docx
-    :yield: every paragraph with 'Heading' paragraph_style as a list of strings
-    :return: None
-
-    When docx2python paragraph_styles parameter is set to True, the first run in
-    every paragraph will be a paragraph style extracted from the xml, if present.
-    Else, paragraphs style will be "".
-    """
-    heading_pattern = re.compile(r"Heading\d")
-    extraction = docx2python(path_in, paragraph_styles=True)
-    for par in iter_at_depth(extraction.document_runs, 4):
-        if re.match(heading_pattern, par[0]):
-            yield par
-    extraction.close()
+"""Utility / example functions using new (as of 2.0.0 Docx2Python features)
+
+:author: Shay Hill
+:created: 2021-12-21
+
+Docx2Python version two exposes extracted xml in the DocxReader object and has a new
+paragraph_styles argument. These functions use these new features as utilities /
+examples.
+"""
+
+from __future__ import annotations
+
+import copy
+import re
+from pathlib import Path
+from typing import Iterator
+
+from lxml import etree
+from lxml.etree import _Element as EtreeElement  # type: ignore
+
+from docx2python.attribute_register import Tags
+
+from .iterators import iter_at_depth
+from .main import docx2python
+
+
+def _copy_new_text(elem: EtreeElement, new_text: str) -> EtreeElement:
+    """Copy a text element and replace text.
+
+    :param elem: an etree element with tag w:t
+    :param new_text: text to replace elem.text
+    :return: a new etree element with tag w:t and text new_text
+    """
+    new_elem = copy.deepcopy(elem)
+    new_elem.text = new_text
+    return new_elem
+
+
+def replace_root_text(root: EtreeElement, old: str, new: str) -> None:
+    """Replace :old: with :new: in all descendants of :root:
+
+    :param root: an etree element presumably containing descendant text elements
+    :param old: text to be replaced
+    :param new: replacement text
+
+    Will use softbreaks <br> to preserve line breaks in replacement text.
+    """
+
+    def recursive_text_replace(branch: EtreeElement):
+        """Replace any text element contining old with one or more elements.
+
+        :param branch: an etree element
+        """
+        for elem in tuple(branch):
+            if not elem.text or old not in elem.text:
+                recursive_text_replace(elem)
+                continue
+
+            # create a new text element for each line in replacement text
+            text = elem.text.replace(old, new)
+            new_elems = [_copy_new_text(elem, line) for line in text.splitlines()]
+
+            # insert breakpoints where line breaks were
+            breaks = [etree.Element(Tags.BR) for _ in new_elems]
+            new_elems = [x for pair in zip(new_elems, breaks) for x in pair][:-1]
+
+            # replace the original element with the new elements
+            parent = elem.getparent()
+            assert parent is not None
+            index = parent.index(elem)
+            parent[index : index + 1] = new_elems
+
+    recursive_text_replace(root)
+
+
+def replace_docx_text(
+    path_in: Path | str,
+    path_out: Path | str,
+    *replacements: tuple[str, str],
+    html: bool = False,
+) -> None:
+    """Replace text in a docx file.
+
+    :param path_in: path to input docx
+    :param path_out: path to output docx with text replaced
+    :param replacements: tuples of strings (a, b) replace a with b for each in docx.
+    :param html: respect formatting (as far as docx2python can see formatting)
+    """
+    reader = docx2python(path_in, html=html).docx_reader
+    for file in reader.content_files():
+        root = file.root_element
+        for replacement in replacements:
+            replace_root_text(root, *replacement)
+    reader.save(path_out)
+    reader.close()
+
+
+def get_links(path_in: Path | str) -> Iterator[tuple[str, str]]:
+    """Iter links inside a docx file as (href, text)
+
+    :param path_in: path to input docx
+    :yield: every link in the file as a tuple of (href, text)
+    :return: None
+    """
+    link_pattern = re.compile('<a href="(?P<href>[^"]+)">(?P<text>[^<]+)</a>')
+    extraction = docx2python(path_in)
+    for run in iter_at_depth(extraction.document_runs, 5):
+        match = re.match(link_pattern, run)
+        if match:
+            href, text = match.groups()
+            yield href, text
+    extraction.close()
+
+
+def get_headings(path_in: Path | str) -> Iterator[list[str]]:
+    """Iter paragraphs with 'Heading' patagraph_style
+
+    :param path_in: path to input docx
+    :yield: every paragraph with 'Heading' paragraph_style as a list of strings
+    :return: None
+
+    When docx2python paragraph_styles parameter is set to True, the first run in
+    every paragraph will be a paragraph style extracted from the xml, if present.
+    Else, paragraphs style will be "".
+    """
+    heading_pattern = re.compile(r"Heading\d")
+    extraction = docx2python(path_in, paragraph_styles=True)
+    for par in iter_at_depth(extraction.document_runs, 4):
+        if re.match(heading_pattern, par[0]):
+            yield par
+    extraction.close()
```

### Comparing `docx2python-2.7.2/LICENSE.txt` & `docx2python-2.7.3/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2019 Shay Hill
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2019 Shay Hill
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
```

### Comparing `docx2python-2.7.2/pyproject.toml` & `docx2python-2.7.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-[tool.poetry]
-name = "docx2python"
-version = "2.7.2"
-description = "Extract content from docx files"
-authors = ["Shay Hill <shay_public@hotmail.com>"]
-license = "MIT"
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = "^3.8"
-lxml = "^4.9.2"
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
-types-lxml = "^2022.11.8"
-commitizen = "^2.39.1"
-pre-commit = "^3.0.4"
-
-[tool.commitizen]
-name = "cz_conventional_commits"
-version = "2.7.2"
-tag_format = "$version"
-version_files = [
-    "pyproject.toml:^version"
-]
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-# [tox]
-# isolated_build = true
-# envlist = py36
-
-# [testenv]
-# whitelist_externals = poetry
-# commands =
-#     poetry install -v
-#     poetry run pytest tests/
-
-[tool.pyright]
-include = ["src"]
-exclude = ["**/__pycache__.py", "**/tests/**"]
-
-pythonVersion = "3.10"
-pythonPlatform = "Any"
-
-typeCheckingMode = "strict"
-reportShadowedImports = true
-reportCallInDefaultInitializer = true
-reportImplicitStringConcatenation = true
-reportPropertyTypeMismatch = true
-reportUninitializedInstanceVariable = true
-reportUnnecessaryTypeIgnoreComment = true
-reportUnusedCallResult = true
-reportImportCycles = false
-reportIncompatibleMethodOverride = false
-
-venvPath = "C:\\Users\\shaya\\AppData\\Local\\pypoetry\\Cache\\virtualenvs"
-venv = "C:\\Users\\shaya\\AppData\\Local\\pypoetry\\Cache\\virtualenvs\\docx2python-fuFHBYOz-py3.11"
+[tool.poetry]
+name = "docx2python"
+version = "2.7.3"
+description = "Extract content from docx files"
+authors = ["Shay Hill <shay_public@hotmail.com>"]
+license = "MIT"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+lxml = "^4.9.2"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.0"
+types-lxml = "^2022.11.8"
+commitizen = "^2.39.1"
+pre-commit = "^3.0.4"
+
+[tool.commitizen]
+name = "cz_conventional_commits"
+version = "2.7.3"
+tag_format = "$version"
+version_files = [
+    "pyproject.toml:^version"
+]
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+# [tox]
+# isolated_build = true
+# envlist = py36
+
+# [testenv]
+# whitelist_externals = poetry
+# commands =
+#     poetry install -v
+#     poetry run pytest tests/
+
+[tool.pyright]
+include = ["src"]
+exclude = ["**/__pycache__.py", "**/tests/**"]
+
+pythonVersion = "3.10"
+pythonPlatform = "Any"
+
+typeCheckingMode = "strict"
+reportShadowedImports = true
+reportCallInDefaultInitializer = true
+reportImplicitStringConcatenation = true
+reportPropertyTypeMismatch = true
+reportUninitializedInstanceVariable = true
+reportUnnecessaryTypeIgnoreComment = true
+reportUnusedCallResult = true
+reportImportCycles = false
+reportIncompatibleMethodOverride = false
+
+venvPath = "C:\\Users\\shaya\\AppData\\Local\\pypoetry\\Cache\\virtualenvs"
+venv = "C:\\Users\\shaya\\AppData\\Local\\pypoetry\\Cache\\virtualenvs\\docx2python-fuFHBYOz-py3.11"
```

### Comparing `docx2python-2.7.2/README.md` & `docx2python-2.7.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,845 +1,823 @@
-00000000: 2320 646f 6378 3270 7974 686f 6e0d 0a0d  # docx2python...
-00000010: 0a45 7874 7261 6374 2064 6f63 7820 6865  .Extract docx he
-00000020: 6164 6572 732c 2066 6f6f 7465 7273 2c20  aders, footers, 
-00000030: 7465 7874 2c20 666f 6f74 6e6f 7465 732c  text, footnotes,
-00000040: 2065 6e64 6e6f 7465 732c 2070 726f 7065   endnotes, prope
-00000050: 7274 6965 732c 2061 6e64 2069 6d61 6765  rties, and image
-00000060: 7320 746f 2061 2050 7974 686f 6e20 6f62  s to a Python ob
-00000070: 6a65 6374 2e0d 0a0d 0a60 5245 4144 4d45  ject.....`README
-00000080: 5f44 4f43 585f 4649 4c45 5f53 5452 5543  _DOCX_FILE_STRUC
-00000090: 5455 5245 2e6d 6460 206d 6179 2068 656c  TURE.md` may hel
-000000a0: 7020 6966 2079 6f75 2764 206c 696b 6520  p if you'd like 
-000000b0: 746f 2065 7874 656e 6420 646f 6378 3270  to extend docx2p
-000000c0: 7974 686f 6e2e 0d0a 0d0a 466f 7220 6120  ython.....For a 
-000000d0: 7375 6d6d 6172 7920 6f66 2077 6861 7427  summary of what'
-000000e0: 7320 6e65 7720 696e 2064 6f63 7832 7079  s new in docx2py
-000000f0: 7468 6f6e 2032 2c20 7363 726f 6c6c 2064  thon 2, scroll d
-00000100: 6f77 6e20 746f 202a 2a4e 6577 2069 6e20  own to **New in 
-00000110: 646f 6378 3270 7974 686f 6e20 5665 7273  docx2python Vers
-00000120: 696f 6e20 322a 2a0d 0a0d 0a54 6865 2063  ion 2**....The c
-00000130: 6f64 6520 6973 2061 6e20 6578 7061 6e73  ode is an expans
-00000140: 696f 6e2f 636f 6e74 7261 6374 696f 6e20  ion/contraction 
-00000150: 6f66 205b 7079 7468 6f6e 2d64 6f63 7832  of [python-docx2
-00000160: 7478 745d 2868 7474 7073 3a2f 2f67 6974  txt](https://git
-00000170: 6875 622e 636f 6d2f 616e 6b75 7368 7368  hub.com/ankushsh
-00000180: 6168 3839 2f70 7974 686f 6e2d 646f 6378  ah89/python-docx
-00000190: 3274 7874 2920 2843 6f70 7972 6967 6874  2txt) (Copyright
-000001a0: 2028 6329 2032 3031 3520 416e 6b75 7368   (c) 2015 Ankush
-000001b0: 2053 6861 6829 2e20 5468 6520 6f72 6967   Shah). The orig
-000001c0: 696e 616c 2063 6f64 6520 6973 206d 6f73  inal code is mos
-000001d0: 746c 7920 676f 6e65 2c20 6275 7420 736f  tly gone, but so
-000001e0: 6d65 206f 6620 7468 6520 626f 6e65 7320  me of the bones 
-000001f0: 6d61 7920 7374 696c 6c20 6265 2068 6572  may still be her
-00000200: 652e 0d0a 0d0a 5f5f 7368 6172 6564 2066  e.....__shared f
-00000210: 6561 7475 7265 735f 5f3a 0d0a 2a20 6578  eatures__:..* ex
-00000220: 7472 6163 7473 2074 6578 7420 6672 6f6d  tracts text from
-00000230: 2064 6f63 7820 6669 6c65 730d 0a2a 2065   docx files..* e
-00000240: 7874 7261 6374 7320 696d 6167 6573 2066  xtracts images f
-00000250: 726f 6d20 646f 6378 2066 696c 6573 0d0a  rom docx files..
-00000260: 0d0a 5f5f 6164 6469 7469 6f6e 733a 5f5f  ..__additions:__
-00000270: 0d0a 2a20 6578 7472 6163 7473 2066 6f6f  ..* extracts foo
-00000280: 746e 6f74 6573 2061 6e64 2065 6e64 6e6f  tnotes and endno
-00000290: 7465 730d 0a2a 2063 6f6e 7665 7274 7320  tes..* converts 
-000002a0: 6275 6c6c 6574 7320 616e 6420 6e75 6d62  bullets and numb
-000002b0: 6572 6564 206c 6973 7473 2074 6f20 6173  ered lists to as
-000002c0: 6369 6920 7769 7468 2069 6e64 656e 7461  cii with indenta
-000002d0: 7469 6f6e 0d0a 2a20 636f 6e76 6572 7473  tion..* converts
-000002e0: 2068 7970 6572 6c69 6e6b 7320 746f 2060   hyperlinks to `
-000002f0: 603c 6120 6872 6566 3d22 6874 7470 3a2f  `<a href="http:/
-00000300: 2e2e 2e22 3e6c 696e 6b20 7465 7874 3c2f  ...">link text</
-00000310: 613e 6060 0d0a 2a20 7265 7461 696e 7320  a>``..* retains 
-00000320: 736f 6d65 2073 7472 7563 7475 7265 206f  some structure o
-00000330: 6620 7468 6520 6f72 6967 696e 616c 2066  f the original f
-00000340: 696c 6520 286d 6f72 6520 6265 6c6f 7729  ile (more below)
-00000350: 0d0a 2a20 6578 7472 6163 7473 2064 6f63  ..* extracts doc
-00000360: 756d 656e 7420 7072 6f70 6572 7469 6573  ument properties
-00000370: 2028 6372 6561 746f 722c 206c 6173 744d   (creator, lastM
-00000380: 6f64 6966 6965 6442 792c 2065 7463 2e29  odifiedBy, etc.)
-00000390: 0d0a 2a20 696e 7365 7274 7320 696d 6167  ..* inserts imag
-000003a0: 6520 706c 6163 6568 6f6c 6465 7273 2069  e placeholders i
-000003b0: 6e20 7465 7874 2028 6060 272d 2d2d 2d69  n text (``'----i
-000003c0: 6d61 6765 312e 6a70 672d 2d2d 2d27 6060  mage1.jpg----'``
-000003d0: 290d 0a2a 2069 6e73 6572 7473 2070 6c61  )..* inserts pla
-000003e0: 696e 2074 6578 7420 666f 6f74 6e6f 7465  in text footnote
-000003f0: 2061 6e64 2065 6e64 6e6f 7465 2072 6566   and endnote ref
-00000400: 6572 656e 6365 7320 696e 2074 6578 7420  erences in text 
-00000410: 2860 6027 2d2d 2d2d 666f 6f74 6e6f 7465  (``'----footnote
-00000420: 312d 2d2d 2d27 6060 290d 0a2a 2028 6f70  1----'``)..* (op
-00000430: 7469 6f6e 616c 6c79 2920 7265 7461 696e  tionally) retain
-00000440: 7320 666f 6e74 2073 697a 652c 2066 6f6e  s font size, fon
-00000450: 7420 636f 6c6f 722c 2062 6f6c 642c 2069  t color, bold, i
-00000460: 7461 6c69 6373 2c20 616e 6420 756e 6465  talics, and unde
-00000470: 7273 636f 7265 2061 7320 6874 6d6c 0d0a  rscore as html..
-00000480: 2a20 6578 7472 6163 7420 6d61 7468 2065  * extract math e
-00000490: 7175 6174 696f 6e73 0d0a 2a20 6578 7472  quations..* extr
-000004a0: 6163 7420 7573 6572 2073 656c 6563 7469  act user selecti
-000004b0: 6f6e 7320 6672 6f6d 2063 6865 636b 626f  ons from checkbo
-000004c0: 7865 7320 616e 6420 6472 6f70 646f 776e  xes and dropdown
-000004d0: 206d 656e 7573 0d0a 0d0a 5f5f 7375 6274   menus....__subt
-000004e0: 7261 6374 696f 6e73 3a5f 5f0d 0a2a 206e  ractions:__..* n
-000004f0: 6f20 636f 6d6d 616e 642d 6c69 6e65 2069  o command-line i
-00000500: 6e74 6572 6661 6365 0d0a 2a20 7769 6c6c  nterface..* will
-00000510: 206f 6e6c 7920 776f 726b 2077 6974 6820   only work with 
-00000520: 5079 7468 6f6e 2033 2e38 2b0d 0a0d 0a0d  Python 3.8+.....
-00000530: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00000540: 0d0a 6060 6062 6173 680d 0a70 6970 2069  ..```bash..pip i
-00000550: 6e73 7461 6c6c 2064 6f63 7832 7079 7468  nstall docx2pyth
-00000560: 6f6e 0d0a 6060 600d 0a0d 0a23 2320 5573  on..```....## Us
-00000570: 650d 0a0d 0a60 6060 2070 7974 686f 6e0d  e....``` python.
-00000580: 0a66 726f 6d20 646f 6378 3270 7974 686f  .from docx2pytho
-00000590: 6e20 696d 706f 7274 2064 6f63 7832 7079  n import docx2py
-000005a0: 7468 6f6e 0d0a 0d0a 2320 6578 7472 6163  thon....# extrac
-000005b0: 7420 646f 6378 2063 6f6e 7465 6e74 0d0a  t docx content..
-000005c0: 7769 7468 2064 6f63 7832 7079 7468 6f6e  with docx2python
-000005d0: 2827 7061 7468 2f74 6f2f 6669 6c65 2e64  ('path/to/file.d
-000005e0: 6f63 7827 2920 6173 2064 6f63 785f 636f  ocx') as docx_co
-000005f0: 6e74 656e 743a 0d0a 2020 2020 7072 696e  ntent:..    prin
-00000600: 7428 646f 6378 5f63 6f6e 7465 6e74 2e74  t(docx_content.t
-00000610: 6578 7429 0d0a 0d0a 646f 6378 5f63 6f6e  ext)....docx_con
-00000620: 7465 6e74 203d 2064 6f63 7832 7079 7468  tent = docx2pyth
-00000630: 6f6e 2827 7061 7468 2f74 6f2f 6669 6c65  on('path/to/file
-00000640: 2e64 6f63 7827 290d 0a70 7269 6e74 2864  .docx')..print(d
-00000650: 6f63 785f 636f 6e74 656e 742e 7465 7874  ocx_content.text
-00000660: 290d 0a64 6f63 785f 636f 6e74 656e 742e  )..docx_content.
-00000670: 636c 6f73 6528 290d 0a0d 0a23 2065 7874  close()....# ext
-00000680: 7261 6374 2064 6f63 7820 636f 6e74 656e  ract docx conten
-00000690: 742c 2077 7269 7465 2069 6d61 6765 7320  t, write images 
-000006a0: 746f 2069 6d61 6765 5f64 6972 6563 746f  to image_directo
-000006b0: 7279 0d0a 7769 7468 2064 6f63 7832 7079  ry..with docx2py
-000006c0: 7468 6f6e 2827 7061 7468 2f74 6f2f 6669  thon('path/to/fi
-000006d0: 6c65 2e64 6f63 7827 2c20 2770 6174 682f  le.docx', 'path/
-000006e0: 746f 2f69 6d61 6765 5f64 6972 6563 746f  to/image_directo
-000006f0: 7279 2729 2061 7320 646f 6378 5f63 6f6e  ry') as docx_con
-00000700: 7465 6e74 3a0d 0a20 2020 2070 7269 6e74  tent:..    print
-00000710: 2864 6f63 785f 636f 6e74 656e 742e 7465  (docx_content.te
-00000720: 7874 290d 0a0d 0a23 2065 7874 7261 6374  xt)....# extract
-00000730: 2064 6f63 7820 636f 6e74 656e 7420 7769   docx content wi
-00000740: 7468 2062 6173 6963 2066 6f6e 7420 7374  th basic font st
-00000750: 796c 6573 2063 6f6e 7665 7274 6564 2074  yles converted t
-00000760: 6f20 6874 6d6c 0d0a 7769 7468 2064 6f63  o html..with doc
-00000770: 7832 7079 7468 6f6e 2827 7061 7468 2f74  x2python('path/t
-00000780: 6f2f 6669 6c65 2e64 6f63 7827 2c20 6874  o/file.docx', ht
-00000790: 6d6c 3d54 7275 6529 2061 7320 646f 6378  ml=True) as docx
-000007a0: 5f63 6f6e 7465 6e74 3a0d 0a20 2020 2070  _content:..    p
-000007b0: 7269 6e74 2864 6f63 785f 636f 6e74 656e  rint(docx_conten
-000007c0: 742e 7465 7874 290d 0a60 6060 0d0a 0d0a  t.text)..```....
-000007d0: 6064 6f63 7832 7079 7468 6f6e 6020 6f70  `docx2python` op
-000007e0: 656e 7320 6120 7a69 7066 696c 6520 6f62  ens a zipfile ob
-000007f0: 6a65 6374 2061 6e64 2028 6c61 7a69 6c79  ject and (lazily
-00000800: 2920 7265 6164 7320 6974 2e20 5573 6520  ) reads it. Use 
-00000810: 636f 6e74 6578 7420 6d61 6e61 6765 6d65  context manageme
-00000820: 6e74 2028 6077 6974 6820 2e2e 2e20 6173  nt (`with ... as
-00000830: 6029 2074 6f20 636c 6f73 6520 7468 6973  `) to close this
-00000840: 207a 6970 6669 6c65 206f 626a 6563 7420   zipfile object 
-00000850: 6f72 2065 7870 6c69 6369 746c 7920 636c  or explicitly cl
-00000860: 6f73 6520 7769 7468 2060 646f 6378 5f63  ose with `docx_c
-00000870: 6f6e 7465 6e74 2e63 6c6f 7365 2829 602e  ontent.close()`.
-00000880: 0d0a 0d0a 4e6f 7465 206f 6e20 6874 6d6c  ....Note on html
-00000890: 2066 6561 7475 7265 3a0d 0a2a 2073 7570   feature:..* sup
-000008a0: 706f 7274 7320 6060 3c69 3e60 6069 7461  ports ``<i>``ita
-000008b0: 6c69 632c 2060 603c 623e 6060 626f 6c64  lic, ``<b>``bold
-000008c0: 2c20 6060 3c75 3e60 6075 6e64 6572 6c69  , ``<u>``underli
-000008d0: 6e65 2c20 6060 3c73 3e60 6073 7472 696b  ne, ``<s>``strik
-000008e0: 652c 2060 603c 7375 703e 6060 7375 7065  e, ``<sup>``supe
-000008f0: 7273 6372 6970 742c 2060 603c 7375 623e  rscript, ``<sub>
-00000900: 6060 7375 6273 6372 6970 742c 2060 603c  ``subscript, ``<
-00000910: 7370 616e 2073 7479 6c65 3d22 666f 6e74  span style="font
-00000920: 2d76 6172 6961 6e74 3a20 736d 616c 6c2d  -variant: small-
-00000930: 6361 7073 223e 6060 736d 616c 6c20 6361  caps">``small ca
-00000940: 7073 2c20 6060 3c73 7061 6e20 7374 796c  ps, ``<span styl
-00000950: 653d 2274 6578 742d 7472 616e 7366 6f72  e="text-transfor
-00000960: 6d3a 7570 7065 7263 6173 6522 3e60 6061  m:uppercase">``a
-00000970: 6c6c 2063 6170 732c 2060 603c 7370 616e  ll caps, ``<span
-00000980: 2073 7479 6c65 3d22 6261 636b 6772 6f75   style="backgrou
-00000990: 6e64 2d63 6f6c 6f72 3a20 7965 6c6c 6f77  nd-color: yellow
-000009a0: 223e 6060 6869 6768 6c69 6768 7465 642c  ">``highlighted,
-000009b0: 2060 603c 7370 616e 2073 7479 6c65 3d22   ``<span style="
-000009c0: 666f 6e74 2d73 697a 653a 3332 223e 6060  font-size:32">``
-000009d0: 666f 6e74 2073 697a 652c 2060 603c 7370  font size, ``<sp
-000009e0: 616e 2073 7479 6c65 3d22 636f 6c6f 723a  an style="color:
-000009f0: 2366 6630 3030 3022 3e60 6063 6f6c 6f72  #ff0000">``color
-00000a00: 6564 2074 6578 742e 0d0a 2a20 6879 7065  ed text...* hype
-00000a10: 726c 696e 6b73 2077 696c 6c20 616c 7761  rlinks will alwa
-00000a20: 7973 2062 6520 6578 706f 7274 6564 2061  ys be exported a
-00000a30: 7320 6874 6d6c 2028 6060 3c61 2068 7265  s html (``<a hre
-00000a40: 663d 2268 7474 703a 2f2e 2e2e 223e 6c69  f="http:/...">li
-00000a50: 6e6b 2074 6578 743c 2f61 3e60 6029 2c20  nk text</a>``), 
-00000a60: 6576 656e 2069 6620 6060 6874 6d6c 3d46  even if ``html=F
-00000a70: 616c 7365 6060 2c20 6265 6361 7573 6520  alse``, because 
-00000a80: 4920 636f 756c 646e 2774 2074 6869 6e6b  I couldn't think
-00000a90: 206f 6620 6120 6d6f 7265 2063 616e 6f6e   of a more canon
-00000aa0: 6963 616c 2072 6570 7265 7365 6e74 6174  ical representat
-00000ab0: 696f 6e2e 0d0a 2a20 6576 6572 7920 7461  ion...* every ta
-00000ac0: 6720 6f70 656e 2069 6e20 6120 7061 7261  g open in a para
-00000ad0: 6772 6170 6820 7769 6c6c 2062 6520 636c  graph will be cl
-00000ae0: 6f73 6564 2069 6e20 7468 6174 2070 6172  osed in that par
-00000af0: 6167 7261 7068 2028 616e 642c 2077 6865  agraph (and, whe
-00000b00: 7265 2061 7070 726f 7072 6961 7465 2c20  re appropriate, 
-00000b10: 7265 6f70 656e 6564 2069 6e20 7468 6520  reopened in the 
-00000b20: 6e65 7874 2070 6172 6167 7261 7068 292e  next paragraph).
-00000b30: 2049 6620 7477 6f20 7375 6273 6571 7565   If two subseque
-00000b40: 6e63 7420 7061 7261 6772 6170 6873 2061  nct paragraphs a
-00000b50: 7265 2062 6f6c 642c 2074 6865 7920 7769  re bold, they wi
-00000b60: 6c6c 2062 6520 7265 7475 726e 6564 2061  ll be returned a
-00000b70: 7320 603c 623e 7061 7261 6772 6170 6820  s `<b>paragraph 
-00000b80: 613c 2f62 3e60 2c20 603c 623e 7061 7261  a</b>`, `<b>para
-00000b90: 6772 6170 6820 623c 2f62 3e60 2e20 5468  graph b</b>`. Th
-00000ba0: 6973 2069 7320 696e 7465 6e74 696f 6e61  is is intentiona
-00000bb0: 6c20 746f 206d 616b 6520 2065 6163 6820  l to make  each 
-00000bc0: 7061 7261 6772 6170 6820 6974 7320 6f77  paragraph its ow
-00000bd0: 6e20 656e 7469 7479 2e0d 0a2a 2069 6620  n entity...* if 
-00000be0: 796f 7520 7370 6563 6966 7920 6068 746d  you specify `htm
-00000bf0: 6c3d 5472 7565 602c 2060 2660 2c20 603e  l=True`, `&`, `>
-00000c00: 6020 616e 6420 603c 6020 696e 2079 6f75  ` and `<` in you
-00000c10: 7220 646f 6378 2074 6578 7420 7769 6c6c  r docx text will
-00000c20: 2062 6520 656e 636f 6465 6420 6173 2060   be encoded as `
-00000c30: 2661 6d70 602c 2060 2667 743b 6020 616e  &amp`, `&gt;` an
-00000c40: 6420 6026 6c74 3b60 0d0a 0d0a 2323 2052  d `&lt;`....## R
-00000c50: 6574 7572 6e20 5661 6c75 650d 0a0d 0a46  eturn Value....F
-00000c60: 756e 6374 696f 6e20 6064 6f63 7832 7079  unction `docx2py
-00000c70: 7468 6f6e 6020 7265 7475 726e 7320 6120  thon` returns a 
-00000c80: 446f 6378 436f 6e74 656e 7420 696e 7374  DocxContent inst
-00000c90: 616e 6365 2077 6974 6820 7365 7665 7261  ance with severa
-00000ca0: 6c20 6174 7472 6962 7574 6573 2e0d 0a0d  l attributes....
-00000cb0: 0a5f 5f68 6561 6465 725f 5f20 2d20 636f  .__header__ - co
-00000cc0: 6e74 656e 7473 206f 6620 7468 6520 646f  ntents of the do
-00000cd0: 6378 2068 6561 6465 7273 2069 6e20 7468  cx headers in th
-00000ce0: 6520 7265 7475 726e 2066 6f72 6d61 7420  e return format 
-00000cf0: 6465 7363 7269 6265 6420 6865 7265 696e  described herein
-00000d00: 0d0a 0d0a 5f5f 666f 6f74 6572 5f5f 202d  ....__footer__ -
-00000d10: 2063 6f6e 7465 6e74 7320 6f66 2074 6865   contents of the
-00000d20: 2064 6f63 7820 666f 6f74 6572 7320 696e   docx footers in
-00000d30: 2074 6865 2072 6574 7572 6e20 666f 726d   the return form
-00000d40: 6174 2064 6573 6372 6962 6564 2068 6572  at described her
-00000d50: 6569 6e0d 0a0d 0a5f 5f62 6f64 795f 5f20  ein....__body__ 
-00000d60: 2d20 636f 6e74 656e 7473 206f 6620 7468  - contents of th
-00000d70: 6520 646f 6378 2069 6e20 7468 6520 7265  e docx in the re
-00000d80: 7475 726e 2066 6f72 6d61 7420 6465 7363  turn format desc
-00000d90: 7269 6265 6420 6865 7265 696e 0d0a 0d0a  ribed herein....
-00000da0: 5f5f 666f 6f74 6e6f 7465 735f 5f20 2d20  __footnotes__ - 
-00000db0: 636f 6e74 656e 7473 206f 6620 7468 6520  contents of the 
-00000dc0: 646f 6378 2069 6e20 7468 6520 7265 7475  docx in the retu
-00000dd0: 726e 2066 6f72 6d61 7420 6465 7363 7269  rn format descri
-00000de0: 6265 6420 6865 7265 696e 0d0a 0d0a 5f5f  bed herein....__
-00000df0: 656e 646e 6f74 6573 5f5f 202d 2063 6f6e  endnotes__ - con
-00000e00: 7465 6e74 7320 6f66 2074 6865 2064 6f63  tents of the doc
-00000e10: 7820 696e 2074 6865 2072 6574 7572 6e20  x in the return 
-00000e20: 666f 726d 6174 2064 6573 6372 6962 6564  format described
-00000e30: 2068 6572 6569 6e0d 0a0d 0a5f 5f64 6f63   herein....__doc
-00000e40: 756d 656e 745f 5f20 2d20 6865 6164 6572  ument__ - header
-00000e50: 2020 2b20 626f 6479 202b 2066 6f6f 7465    + body + foote
-00000e60: 7220 2872 6561 6420 6f6e 6c79 290d 0a0d  r (read only)...
-00000e70: 0a5f 5f74 6578 745f 5f20 2d20 616c 6c20  .__text__ - all 
-00000e80: 646f 6378 2074 6578 7420 6173 206f 6e65  docx text as one
-00000e90: 2073 7472 696e 672c 2073 696d 696c 6172   string, similar
-00000ea0: 2074 6f20 7768 6174 2079 6f75 2764 2067   to what you'd g
-00000eb0: 6574 2066 726f 6d20 6070 7974 686f 6e2d  et from `python-
-00000ec0: 646f 6378 3274 7874 600d 0a0d 0a5f 5f70  docx2txt`....__p
-00000ed0: 726f 7065 7274 6965 735f 5f20 2d20 646f  roperties__ - do
-00000ee0: 6378 2070 726f 7065 7274 7920 6e61 6d65  cx property name
-00000ef0: 7320 6d61 7070 6564 2074 6f20 7661 6c75  s mapped to valu
-00000f00: 6573 2028 652e 672e 2c20 607b 226c 6173  es (e.g., `{"las
-00000f10: 744d 6f64 6966 6965 6442 7922 3a20 2253  tModifiedBy": "S
-00000f20: 6861 7920 4869 6c6c 227d 6029 0d0a 0d0a  hay Hill"}`)....
-00000f30: 5f5f 696d 6167 6573 5f5f 202d 2069 6d61  __images__ - ima
-00000f40: 6765 206e 616d 6573 206d 6170 7065 6420  ge names mapped 
-00000f50: 746f 2069 6d61 6765 7320 696e 2062 696e  to images in bin
-00000f60: 6172 7920 666f 726d 6174 2e20 5772 6974  ary format. Writ
-00000f70: 6520 746f 2066 696c 6573 7973 7465 6d20  e to filesystem 
-00000f80: 7769 7468 0d0a 0d0a 6060 600d 0a66 6f72  with....```..for
-00000f90: 206e 616d 652c 2069 6d61 6765 2069 6e20   name, image in 
-00000fa0: 7265 7375 6c74 2e69 6d61 6765 732e 6974  result.images.it
-00000fb0: 656d 7328 293a 0d0a 2020 2020 7769 7468  ems():..    with
-00000fc0: 206f 7065 6e28 6e61 6d65 2c20 2777 6227   open(name, 'wb'
-00000fd0: 2920 6173 2069 6d61 6765 5f64 6573 7469  ) as image_desti
-00000fe0: 6e61 7469 6f6e 3a0d 0a20 2020 2020 2020  nation:..       
-00000ff0: 2077 7269 7465 2869 6d61 6765 5f64 6573   write(image_des
-00001000: 7469 6e61 7469 6f6e 2c20 696d 6167 6529  tination, image)
-00001010: 0d0a 0d0a 2320 6f72 0d0a 0d0a 7769 7468  ....# or....with
-00001020: 2064 6f63 7832 7079 7468 6f6e 2827 7061   docx2python('pa
-00001030: 7468 2f74 6f2f 6669 6c65 2e64 6f63 7827  th/to/file.docx'
-00001040: 2c20 2770 6174 682f 746f 2f69 6d61 6765  , 'path/to/image
-00001050: 2f64 6972 6563 746f 7279 2729 2061 7320  /directory') as 
-00001060: 646f 6378 5f63 6f6e 7465 6e74 3a0d 0a20  docx_content:.. 
-00001070: 2020 202e 2e2e 0d0a 0d0a 2320 6f72 0d0a     .......# or..
-00001080: 0d0a 7769 7468 2064 6f63 7832 7079 7468  ..with docx2pyth
-00001090: 6f6e 2827 7061 7468 2f74 6f2f 6669 6c65  on('path/to/file
-000010a0: 2e64 6f63 7827 2920 6173 2064 6f63 785f  .docx') as docx_
-000010b0: 636f 6e74 656e 743a 0d0a 2020 2020 646f  content:..    do
-000010c0: 6378 5f63 6f6e 7465 6e74 2e73 6176 655f  cx_content.save_
-000010d0: 696d 6167 6573 2827 7061 7468 2f74 6f2f  images('path/to/
-000010e0: 696d 6167 652f 6469 7265 6374 6f72 7927  image/directory'
-000010f0: 290d 0a0d 0a60 6060 0d0a 0d0a 5f5f 646f  )....```....__do
-00001100: 6378 5f72 6561 6465 725f 5f20 2d20 6120  cx_reader__ - a 
-00001110: 446f 6378 5265 6164 6572 2028 7365 6520  DocxReader (see 
-00001120: 6064 6f63 785f 7265 6164 6572 2e70 7960  `docx_reader.py`
-00001130: 2920 696e 7374 616e 6365 2077 6974 6820  ) instance with 
-00001140: 7365 7665 7261 6c20 6d65 7468 6f64 7320  several methods 
-00001150: 666f 7220 6578 7472 6163 7469 6e67 2078  for extracting x
-00001160: 6d6c 2070 6f72 7469 6f6e 732e 0d0a 0d0a  ml portions.....
-00001170: 0d0a 2323 2041 7267 756d 656e 7473 0d0a  ..## Arguments..
-00001180: 0d0a 2020 2020 6465 6620 646f 6378 3270  ..    def docx2p
-00001190: 7974 686f 6e28 0d0a 2020 2020 2020 2020  ython(..        
-000011a0: 646f 6378 5f66 696c 656e 616d 653a 2073  docx_filename: s
-000011b0: 7472 207c 2050 6174 6820 7c20 4279 7465  tr | Path | Byte
-000011c0: 7349 4f2c 0d0a 2020 2020 2020 2020 696d  sIO,..        im
-000011d0: 6167 655f 666f 6c64 6572 3a20 7374 7220  age_folder: str 
-000011e0: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0d0a  | None = None,..
-000011f0: 2020 2020 2020 2020 6874 6d6c 3a20 626f          html: bo
-00001200: 6f6c 203d 2046 616c 7365 2c0d 0a20 2020  ol = False,..   
-00001210: 2020 2020 2070 6172 6167 7261 7068 5f73       paragraph_s
-00001220: 7479 6c65 733a 2062 6f6f 6c20 3d20 4661  tyles: bool = Fa
-00001230: 6c73 652c 0d0a 2020 2020 2020 2020 6578  lse,..        ex
-00001240: 7472 6163 745f 696d 6167 653a 2062 6f6f  tract_image: boo
-00001250: 6c20 7c20 4e6f 6e65 203d 204e 6f6e 652c  l | None = None,
-00001260: 0d0a 2020 2020 2020 2020 6475 706c 6963  ..        duplic
-00001270: 6174 655f 6d65 7267 6564 5f63 656c 6c73  ate_merged_cells
-00001280: 3a20 626f 6f6c 203d 2046 616c 7365 0d0a  : bool = False..
-00001290: 2020 2020 2920 2d3e 2044 6f63 7843 6f6e      ) -> DocxCon
-000012a0: 7465 6e74 3a0d 0a20 2020 2020 2020 2022  tent:..        "
-000012b0: 2222 0d0a 2020 2020 2020 2020 556e 7a69  ""..        Unzi
-000012c0: 7020 6120 646f 6378 2066 696c 6520 616e  p a docx file an
-000012d0: 6420 6578 7472 6163 7420 636f 6e74 656e  d extract conten
-000012e0: 7473 2e0d 0a0d 0a20 2020 2020 2020 203a  ts.....        :
-000012f0: 7061 7261 6d20 646f 6378 5f66 696c 656e  param docx_filen
-00001300: 616d 653a 2070 6174 6820 746f 2061 2064  ame: path to a d
-00001310: 6f63 7820 6669 6c65 0d0a 2020 2020 2020  ocx file..      
-00001320: 2020 3a70 6172 616d 2069 6d61 6765 5f66    :param image_f
-00001330: 6f6c 6465 723a 206f 7074 696f 6e61 6c6c  older: optionall
-00001340: 7920 7370 6563 6966 7920 616e 2069 6d61  y specify an ima
-00001350: 6765 2066 6f6c 6465 720d 0a20 2020 2020  ge folder..     
-00001360: 2020 2020 2020 2028 696d 6167 6573 2069         (images i
-00001370: 6e20 646f 6378 2077 696c 6c20 6265 2063  n docx will be c
-00001380: 6f70 6965 6420 746f 2074 6869 7320 666f  opied to this fo
-00001390: 6c64 6572 290d 0a20 2020 2020 2020 203a  lder)..        :
-000013a0: 7061 7261 6d20 6874 6d6c 3a20 626f 6f6c  param html: bool
-000013b0: 2c20 6578 7472 6163 7420 736f 6d65 2066  , extract some f
-000013c0: 6f72 6d61 7474 696e 6720 6173 2068 746d  ormatting as htm
-000013d0: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
-000013e0: 6d20 7061 7261 6772 6170 685f 7374 796c  m paragraph_styl
-000013f0: 6573 3a20 7072 6570 656e 6420 7468 6520  es: prepend the 
-00001400: 7061 7261 6772 6170 6873 2073 7479 6c65  paragraphs style
-00001410: 2028 6966 2061 6e79 2c20 656c 7365 2022   (if any, else "
-00001420: 2229 2074 6f20 6561 6368 0d0a 2020 2020  ") to each..    
-00001430: 2020 2020 2020 2020 7061 7261 6772 6170          paragrap
-00001440: 682e 2054 6869 7320 7769 6c6c 206f 6e6c  h. This will onl
-00001450: 7920 6265 2075 7365 6675 6c20 7769 7468  y be useful with
-00001460: 2060 602a 5f72 756e 7360 6020 6174 7472   ``*_runs`` attr
-00001470: 6962 7574 6573 2e0d 0a20 2020 2020 2020  ibutes...       
-00001480: 203a 7061 7261 6d20 6475 706c 6963 6174   :param duplicat
-00001490: 655f 6d65 7267 6564 5f63 656c 6c73 3a20  e_merged_cells: 
-000014a0: 626f 6f6c 2c20 6475 706c 6963 6174 6520  bool, duplicate 
-000014b0: 6d65 7267 6564 2063 656c 6c73 2074 6f20  merged cells to 
-000014c0: 7265 7475 726e 2061 206d 786e 0d0a 2020  return a mxn..  
-000014d0: 2020 2020 2020 2020 2020 6e65 7374 6564            nested
-000014e0: 206c 6973 7420 666f 7220 6561 6368 2074   list for each t
-000014f0: 6162 6c65 2028 6465 6661 756c 7420 4661  able (default Fa
-00001500: 6c73 6529 0d0a 2020 2020 2020 2020 3a72  lse)..        :r
-00001510: 6574 7572 6e3a 2044 6f63 7843 6f6e 7465  eturn: DocxConte
-00001520: 6e74 206f 626a 6563 740d 0a20 2020 2020  nt object..     
-00001530: 2020 2022 2222 0d0a 0d0a 0d0a 2323 2052     """......## R
-00001540: 6574 7572 6e20 466f 726d 6174 0d0a 0d0a  eturn Format....
-00001550: 536f 6d65 2073 7472 7563 7475 7265 2077  Some structure w
-00001560: 696c 6c20 6265 206d 6169 6e74 6169 6e65  ill be maintaine
-00001570: 642e 2054 6578 7420 7769 6c6c 2062 6520  d. Text will be 
-00001580: 7265 7475 726e 6564 2069 6e20 6120 6e65  returned in a ne
-00001590: 7374 6564 206c 6973 742c 2077 6974 6820  sted list, with 
-000015a0: 7061 7261 6772 6170 6873 2061 6c77 6179  paragraphs alway
-000015b0: 7320 6174 2064 6570 7468 2034 2028 692e  s at depth 4 (i.
-000015c0: 652e 2c20 606f 7574 7075 742e 626f 6479  e., `output.body
-000015d0: 5b69 5d5b 6a5d 5b6b 5d5b 6c5d 6020 7769  [i][j][k][l]` wi
-000015e0: 6c6c 2062 6520 6120 7061 7261 6772 6170  ll be a paragrap
-000015f0: 6829 2e0d 0a0d 0a49 6620 796f 7572 2064  h).....If your d
-00001600: 6f63 7820 6861 7320 6e6f 2074 6162 6c65  ocx has no table
-00001610: 732c 206f 7574 7075 742e 626f 6479 2077  s, output.body w
-00001620: 696c 6c20 6170 7065 6172 2061 7320 6f6e  ill appear as on
-00001630: 6520 6120 7461 626c 6520 7769 7468 2061  e a table with a
-00001640: 6c6c 2063 6f6e 7465 6e74 2069 6e20 6f6e  ll content in on
-00001650: 6520 6365 6c6c 3a0d 0a0d 0a60 6060 7079  e cell:....```py
-00001660: 7468 6f6e 0d0a 5b20 2023 2064 6f63 756d  thon..[  # docum
-00001670: 656e 740d 0a20 2020 205b 2020 2320 7461  ent..    [  # ta
-00001680: 626c 650d 0a20 2020 2020 2020 205b 2020  ble..        [  
-00001690: 2320 726f 770d 0a20 2020 2020 2020 2020  # row..         
-000016a0: 2020 205b 2020 2320 6365 6c6c 0d0a 2020     [  # cell..  
-000016b0: 2020 2020 2020 2020 2020 2020 2020 2250                "P
-000016c0: 6172 6167 7261 7068 2031 222c 0d0a 2020  aragraph 1",..  
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2250                "P
-000016e0: 6172 6167 7261 7068 2032 222c 0d0a 2020  aragraph 2",..  
-000016f0: 2020 2020 2020 2020 2020 2020 2020 222d                "-
-00001700: 2d20 6275 6c6c 6574 6564 206c 6973 7422  - bulleted list"
-00001710: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001720: 2020 2022 2d2d 2063 6f6e 7469 6e75 696e     "-- continuin
-00001730: 6720 6275 6c6c 6574 6564 206c 6973 7422  g bulleted list"
-00001740: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00001750: 2020 2022 3129 2020 6e75 6d62 6572 6564     "1)  numbered
-00001760: 206c 6973 7422 2c0d 0a20 2020 2020 2020   list",..       
-00001770: 2020 2020 2020 2020 2022 3229 2020 636f           "2)  co
-00001780: 6e74 696e 7569 6e67 206e 756d 6265 7265  ntinuing numbere
-00001790: 6420 6c69 7374 220d 0a20 2020 2020 2020  d list"..       
-000017a0: 2020 2020 2020 2020 2022 2020 2020 6129           "    a)
-000017b0: 2020 7375 626c 6973 7422 2c0d 0a20 2020    sublist",..   
-000017c0: 2020 2020 2020 2020 2020 2020 2022 2020               "  
-000017d0: 2020 2020 2020 6929 2020 7375 626c 6973        i)  sublis
-000017e0: 7420 6f66 2073 7562 6c69 7374 222c 0d0a  t of sublist",..
-000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001800: 2233 2920 206b 6565 7073 2074 7261 636b  "3)  keeps track
-00001810: 206f 6620 696e 6465 6e74 696f 6e20 6c65   of indention le
-00001820: 7665 6c73 222c 0d0a 2020 2020 2020 2020  vels",..        
-00001830: 2020 2020 2020 2020 2220 2020 2061 2920          "    a) 
-00001840: 2072 6573 6574 7320 7375 626c 6973 7420   resets sublist 
-00001850: 636f 756e 7465 7273 220d 0a20 2020 2020  counters"..     
-00001860: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
-00001870: 2020 5d0d 0a20 2020 2020 5d0d 0a20 5d0d    ]..     ].. ].
-00001880: 0a60 6060 0d0a 0d0a 5461 626c 6520 6365  .```....Table ce
-00001890: 6c6c 7320 7769 6c6c 2061 7070 6561 7220  lls will appear 
-000018a0: 6173 2074 6162 6c65 2063 656c 6c73 2e20  as table cells. 
-000018b0: 5465 7874 206f 7574 7369 6465 2074 6162  Text outside tab
-000018c0: 6c65 7320 7769 6c6c 2061 7070 6561 7220  les will appear 
-000018d0: 6173 2074 6162 6c65 2063 656c 6c73 2e0d  as table cells..
-000018e0: 0a0d 0a0d 0a41 2064 6f63 7820 646f 6375  .....A docx docu
-000018f0: 6d65 6e74 2063 616e 2062 6520 7461 626c  ment can be tabl
-00001900: 6573 2077 6974 6869 6e20 7461 626c 6573  es within tables
-00001910: 2077 6974 6869 6e20 7461 626c 6573 2e20   within tables. 
-00001920: 446f 6378 3250 7974 686f 6e20 666c 6174  Docx2Python flat
-00001930: 7465 6e73 206d 6f73 7420 6f66 2074 6869  tens most of thi
-00001940: 7320 746f 206d 6f72 6520 6561 7369 6c79  s to more easily
-00001950: 206e 6176 6967 6174 650d 0a77 6974 6869   navigate..withi
-00001960: 6e20 7468 6520 636f 6e74 656e 742e 0d0a  n the content...
-00001970: 0d0a 2323 2057 6f72 6b69 6e67 2077 6974  ..## Working wit
-00001980: 6820 6f75 7470 7574 0d0a 0d0a 5468 6973  h output....This
-00001990: 2070 6163 6b61 6765 2070 726f 7669 6465   package provide
-000019a0: 7320 7365 7665 7261 6c20 646f 6375 6d65  s several docume
-000019b0: 6e74 6564 2068 656c 7065 7220 6675 6e63  nted helper func
-000019c0: 7469 6f6e 7320 696e 205b 7468 6520 6060  tions in [the ``
-000019d0: 646f 6378 3270 7974 686f 6e2e 6974 6572  docx2python.iter
-000019e0: 6174 6f72 7360 6020 6d6f 6475 6c65 5d28  ators`` module](
-000019f0: 6874 7470 733a 2f2f 646f 6378 3270 7974  https://docx2pyt
-00001a00: 686f 6e2e 7265 6164 7468 6564 6f63 732e  hon.readthedocs.
-00001a10: 696f 2f65 6e2f 6c61 7465 7374 2f64 6f63  io/en/latest/doc
-00001a20: 7832 7079 7468 6f6e 2e68 746d 6c23 6d6f  x2python.html#mo
-00001a30: 6475 6c65 2d69 7465 7261 746f 7273 292e  dule-iterators).
-00001a40: 2048 6572 6520 6172 6520 6120 6665 7720   Here are a few 
-00001a50: 7265 6369 7065 7320 706f 7373 6962 6c65  recipes possible
-00001a60: 2077 6974 6820 7468 6573 6520 6675 6e63   with these func
-00001a70: 7469 6f6e 733a 0d0a 0d0a 6060 6070 7974  tions:....```pyt
-00001a80: 686f 6e0d 0a66 726f 6d20 646f 6378 3270  hon..from docx2p
-00001a90: 7974 686f 6e2e 6974 6572 6174 6f72 7320  ython.iterators 
-00001aa0: 696d 706f 7274 2065 6e75 6d5f 6365 6c6c  import enum_cell
-00001ab0: 730d 0a0d 0a64 6566 2072 656d 6f76 655f  s....def remove_
-00001ac0: 656d 7074 795f 7061 7261 6772 6170 6873  empty_paragraphs
-00001ad0: 2874 6162 6c65 7329 3a0d 0a20 2020 2066  (tables):..    f
-00001ae0: 6f72 2028 692c 206a 2c20 6b29 2c20 6365  or (i, j, k), ce
-00001af0: 6c6c 2069 6e20 656e 756d 5f63 656c 6c73  ll in enum_cells
-00001b00: 2874 6162 6c65 7329 3a0d 0a20 2020 2020  (tables):..     
-00001b10: 2020 2074 6162 6c65 735b 695d 5b6a 5d5b     tables[i][j][
-00001b20: 6b5d 203d 205b 7820 666f 7220 7820 696e  k] = [x for x in
-00001b30: 2063 656c 6c20 6966 2078 5d0d 0a60 6060   cell if x]..```
-00001b40: 0d0a 0d0a 6060 600d 0a3e 3e3e 2074 6162  ....```..>>> tab
-00001b50: 6c65 7320 3d20 5b5b 5b5b 2761 272c 2027  les = [[[['a', '
-00001b60: 6227 5d2c 205b 2761 272c 2027 272c 2027  b'], ['a', '', '
-00001b70: 6427 2c20 2727 5d5d 5d5d 0d0a 3e3e 3e20  d', '']]]]..>>> 
-00001b80: 7265 6d6f 7665 5f65 6d70 7479 5f70 6172  remove_empty_par
-00001b90: 6167 7261 7068 7328 7461 626c 6573 290d  agraphs(tables).
-00001ba0: 0a20 2020 205b 5b5b 5b27 6127 2c20 2762  .    [[[['a', 'b
-00001bb0: 275d 2c20 5b27 6127 2c20 2764 275d 5d5d  '], ['a', 'd']]]
-00001bc0: 5d0d 0a60 6060 0d0a 0d0a 6060 6070 7974  ]..```....```pyt
-00001bd0: 686f 6e0d 0a66 726f 6d20 646f 6378 3270  hon..from docx2p
-00001be0: 7974 686f 6e2e 6974 6572 6174 6f72 7320  ython.iterators 
-00001bf0: 696d 706f 7274 2065 6e75 6d5f 6174 5f64  import enum_at_d
-00001c00: 6570 7468 0d0a 0d0a 6465 6620 6874 6d6c  epth....def html
-00001c10: 5f6d 6170 2874 6162 6c65 7329 202d 3e20  _map(tables) -> 
-00001c20: 7374 723a 0d0a 2020 2020 2222 2243 7265  str:..    """Cre
-00001c30: 6174 6520 616e 2048 544d 4c20 6d61 7020  ate an HTML map 
-00001c40: 6f66 2064 6f63 756d 656e 7420 636f 6e74  of document cont
-00001c50: 656e 7473 2e0d 0a0d 0a20 2020 2052 656e  ents.....    Ren
-00001c60: 6465 7220 7468 6973 2069 6e20 6120 6272  der this in a br
-00001c70: 6f77 7365 7220 746f 2076 6973 7561 6c6c  owser to visuall
-00001c80: 7920 7365 6172 6368 2066 6f72 2064 6174  y search for dat
-00001c90: 612e 0d0a 0d0a 2020 2020 3a74 6162 6c65  a.....    :table
-00001ca0: 733a 2076 616c 7565 2063 6f75 6c64 2063  s: value could c
-00001cb0: 6f6d 6520 6672 6f6d 2c20 652e 672e 2c0d  ome from, e.g.,.
-00001cc0: 0a20 2020 2020 2020 202a 2064 6f63 785f  .        * docx_
-00001cd0: 746f 5f74 6578 745f 6f75 7470 7574 2e64  to_text_output.d
-00001ce0: 6f63 756d 656e 740d 0a20 2020 2020 2020  ocument..       
-00001cf0: 202a 2064 6f63 785f 746f 5f74 6578 745f   * docx_to_text_
-00001d00: 6f75 7470 7574 2e62 6f64 790d 0a20 2020  output.body..   
-00001d10: 2022 2222 0d0a 0d0a 2020 2020 2320 7072   """....    # pr
-00001d20: 6570 656e 6420 696e 6465 7820 7475 706c  epend index tupl
-00001d30: 6520 746f 2065 6163 6820 7061 7261 6772  e to each paragr
-00001d40: 6170 680d 0a20 2020 2066 6f72 2028 692c  aph..    for (i,
-00001d50: 206a 2c20 6b2c 206c 292c 2070 6172 6167   j, k, l), parag
-00001d60: 7261 7068 2069 6e20 656e 756d 5f61 745f  raph in enum_at_
-00001d70: 6465 7074 6828 7461 626c 6573 2c20 3429  depth(tables, 4)
-00001d80: 3a0d 0a20 2020 2020 2020 2074 6162 6c65  :..        table
-00001d90: 735b 695d 5b6a 5d5b 6b5d 5b6c 5d20 3d20  s[i][j][k][l] = 
-00001da0: 2220 222e 6a6f 696e 285b 7374 7228 2869  " ".join([str((i
-00001db0: 2c20 6a2c 206b 2c20 6c29 292c 2070 6172  , j, k, l)), par
-00001dc0: 6167 7261 7068 5d29 0d0a 0d0a 2020 2020  agraph])....    
-00001dd0: 2320 7772 6170 2065 6163 6820 7061 7261  # wrap each para
-00001de0: 6772 6170 6820 696e 203c 7072 653e 2074  graph in <pre> t
-00001df0: 6167 730d 0a20 2020 2066 6f72 2028 692c  ags..    for (i,
-00001e00: 206a 2c20 6b29 2c20 6365 6c6c 2069 6e20   j, k), cell in 
-00001e10: 656e 756d 5f61 745f 6465 7074 6828 7461  enum_at_depth(ta
-00001e20: 626c 6573 2c20 3329 3a0d 0a20 2020 2020  bles, 3):..     
-00001e30: 2020 2074 6162 6c65 735b 695d 5b6a 5d5b     tables[i][j][
-00001e40: 6b5d 203d 2022 222e 6a6f 696e 285b 223c  k] = "".join(["<
-00001e50: 7072 653e 7b78 7d3c 2f70 7265 3e22 2e66  pre>{x}</pre>".f
-00001e60: 6f72 6d61 7428 7829 2066 6f72 2078 2069  ormat(x) for x i
-00001e70: 6e20 6365 6c6c 5d29 0d0a 0d0a 2020 2020  n cell])....    
-00001e80: 2320 7772 6170 2065 6163 6820 6365 6c6c  # wrap each cell
-00001e90: 2069 6e20 3c74 643e 2074 6167 730d 0a20   in <td> tags.. 
-00001ea0: 2020 2066 6f72 2028 692c 206a 292c 2072     for (i, j), r
-00001eb0: 6f77 2069 6e20 656e 756d 5f61 745f 6465  ow in enum_at_de
-00001ec0: 7074 6828 7461 626c 6573 2c20 3229 3a0d  pth(tables, 2):.
-00001ed0: 0a20 2020 2020 2020 2074 6162 6c65 735b  .        tables[
-00001ee0: 695d 5b6a 5d20 3d20 2222 2e6a 6f69 6e28  i][j] = "".join(
-00001ef0: 5b22 3c74 643e 7b78 7d3c 2f74 643e 222e  ["<td>{x}</td>".
-00001f00: 666f 726d 6174 2878 2920 666f 7220 7820  format(x) for x 
-00001f10: 696e 2072 6f77 5d29 0d0a 0d0a 2020 2020  in row])....    
-00001f20: 2320 7772 6170 2065 6163 6820 726f 7720  # wrap each row 
-00001f30: 696e 203c 7472 3e20 7461 6773 0d0a 2020  in <tr> tags..  
-00001f40: 2020 666f 7220 2869 2c29 2c20 7461 626c    for (i,), tabl
-00001f50: 6520 696e 2065 6e75 6d5f 6174 5f64 6570  e in enum_at_dep
-00001f60: 7468 2874 6162 6c65 732c 2031 293a 0d0a  th(tables, 1):..
-00001f70: 2020 2020 2020 2020 7461 626c 6573 5b69          tables[i
-00001f80: 5d20 3d20 2222 2e6a 6f69 6e28 223c 7472  ] = "".join("<tr
-00001f90: 3e7b 787d 3c2f 7472 3e22 2e66 6f72 6d61  >{x}</tr>".forma
-00001fa0: 7428 7829 2066 6f72 2078 2069 6e20 7461  t(x) for x in ta
-00001fb0: 626c 6529 0d0a 0d0a 2020 2020 2320 7772  ble)....    # wr
-00001fc0: 6170 2065 6163 6820 7461 626c 6520 696e  ap each table in
-00001fd0: 203c 7461 626c 653e 2074 6167 730d 0a20   <table> tags.. 
-00001fe0: 2020 2074 6162 6c65 7320 3d20 2222 2e6a     tables = "".j
-00001ff0: 6f69 6e28 5b27 3c74 6162 6c65 2062 6f72  oin(['<table bor
-00002000: 6465 723d 2231 223e 7b78 7d3c 2f74 6162  der="1">{x}</tab
-00002010: 6c65 3e27 2e66 6f72 6d61 7428 7829 2066  le>'.format(x) f
-00002020: 6f72 2078 2069 6e20 7461 626c 6573 5d29  or x in tables])
-00002030: 0d0a 0d0a 2020 2020 7265 7475 726e 205b  ....    return [
-00002040: 223c 6874 6d6c 3e3c 626f 6479 3e22 5d20  "<html><body>"] 
-00002050: 2b20 7461 626c 6573 202b 205b 223c 2f62  + tables + ["</b
-00002060: 6f64 793e 3c2f 6874 6d6c 3e22 5d0d 0a60  ody></html>"]..`
-00002070: 6060 0d0a 0d0a 6060 600d 0a3e 3e3e 2074  ``....```..>>> t
-00002080: 6162 6c65 7320 3d20 5b5b 5b5b 2761 272c  ables = [[[['a',
-00002090: 2027 6227 5d2c 205b 2761 272c 2027 6427   'b'], ['a', 'd'
-000020a0: 5d5d 5d5d 0d0a 3e3e 3e20 6874 6d6c 5f6d  ]]]]..>>> html_m
-000020b0: 6170 2874 6162 6c65 7329 0d0a 3c68 746d  ap(tables)..<htm
-000020c0: 6c3e 0d0a 2020 2020 3c62 6f64 793e 0d0a  l>..    <body>..
-000020d0: 2020 2020 2020 2020 3c74 6162 6c65 2062          <table b
-000020e0: 6f72 6465 723d 2231 223e 0d0a 2020 2020  order="1">..    
-000020f0: 2020 2020 2020 2020 3c74 723e 0d0a 2020          <tr>..  
-00002100: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-00002110: 643e 0d0a 2020 2020 2020 2020 2020 2020  d>..            
-00002120: 2020 2020 2020 2020 2728 302c 2030 2c20          '(0, 0, 
-00002130: 302c 2030 2920 6127 0d0a 2020 2020 2020  0, 0) a'..      
-00002140: 2020 2020 2020 2020 2020 2020 2020 2728                '(
-00002150: 302c 2030 2c20 302c 2031 2920 6227 0d0a  0, 0, 0, 1) b'..
-00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002170: 3c2f 7464 3e0d 0a20 2020 2020 2020 2020  </td>..         
-00002180: 2020 2020 2020 203c 7464 3e0d 0a20 2020         <td>..   
-00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021a0: 2027 2830 2c20 302c 2031 2c20 3029 2061   '(0, 0, 1, 0) a
-000021b0: 270d 0a20 2020 2020 2020 2020 2020 2020  '..             
-000021c0: 2020 2020 2020 2027 2830 2c20 302c 2031         '(0, 0, 1
-000021d0: 2c20 3129 2064 270d 0a20 2020 2020 2020  , 1) d'..       
-000021e0: 2020 2020 2020 2020 203c 2f74 643e 0d0a           </td>..
-000021f0: 2020 2020 2020 2020 2020 2020 3c2f 7472              </tr
-00002200: 3e0d 0a20 2020 2020 2020 203c 2f74 6162  >..        </tab
-00002210: 6c65 3e0d 0a20 2020 203c 2f62 6f64 793e  le>..    </body>
-00002220: 0d0a 3c2f 6874 6d6c 3e0d 0a60 6060 0d0a  ..</html>..```..
-00002230: 0d0a 5b53 6565 2068 656c 7065 7220 6675  ..[See helper fu
-00002240: 6e63 7469 6f6e 732e 5d28 6874 7470 733a  nctions.](https:
-00002250: 2f2f 646f 6378 3270 7974 686f 6e2e 7265  //docx2python.re
-00002260: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00002270: 6c61 7465 7374 2f69 6e64 6578 2e68 746d  latest/index.htm
-00002280: 6c29 0d0a 0d0a 536f 6d65 2066 696e 6520  l)....Some fine 
-00002290: 7072 696e 7420 6162 6f75 7420 6368 6563  print about chec
-000022a0: 6b62 6f78 6573 3a0d 0a0d 0a4d 5320 576f  kboxes:....MS Wo
-000022b0: 7264 2068 6173 2063 6865 636b 626f 7865  rd has checkboxe
-000022c0: 7320 7468 6174 2063 616e 2062 6520 6368  s that can be ch
-000022d0: 6563 6b65 6420 616e 7920 7469 6d65 2c20  ecked any time, 
-000022e0: 616e 6420 6f74 6865 7273 2074 6861 7420  and others that 
-000022f0: 6361 6e20 6f6e 6c79 2062 6520 6368 6563  can only be chec
-00002300: 6b65 6420 7768 656e 2074 6865 2066 6f72  ked when the for
-00002310: 6d20 6973 206c 6f63 6b65 642e 0d0a 5468  m is locked...Th
-00002320: 6520 7072 6576 696f 7573 2070 7269 6e74  e previous print
-00002330: 2061 732e 2060 605c 7532 3631 3060 6020   as. ``\u2610`` 
-00002340: 286f 7065 6e20 6368 6563 6b62 6f78 2920  (open checkbox) 
-00002350: 6f72 2060 605c 7532 3631 3260 6020 2863  or ``\u2612`` (c
-00002360: 726f 7373 6564 2063 6865 636b 626f 7829  rossed checkbox)
-00002370: 2e20 5768 6963 6820 7468 6973 206d 6f64  . Which this mod
-00002380: 756c 652c 2074 6865 206c 6174 7465 7220  ule, the latter 
-00002390: 7769 6c6c 0d0a 746f 6f2e 2049 2067 6176  will..too. I gav
-000023a0: 6520 6368 6563 6b62 6f78 6573 2061 2062  e checkboxes a b
-000023b0: 6169 6c6f 7574 2076 616c 7565 206f 6620  ailout value of 
-000023c0: 6060 2d2d 2d2d 6368 6563 6b62 6f78 2066  ``----checkbox f
-000023d0: 6169 6c65 642d 2d2d 2d60 6020 6966 2074  ailed----`` if t
-000023e0: 6865 2078 6d6c 2064 6f65 736e 2774 206c  he xml doesn't l
-000023f0: 6f6f 6b20 6c69 6b65 2049 2065 7870 6563  ook like I expec
-00002400: 7420 6974 2074 6f2c 0d0a 6265 6361 7573  t it to,..becaus
-00002410: 6520 4920 646f 6e27 7420 6861 7665 2073  e I don't have s
-00002420: 6576 6572 616c 2d74 686f 7573 616e 6420  everal-thousand 
-00002430: 7465 7374 2066 696c 6573 2077 6974 6820  test files with 
-00002440: 6368 6563 6b62 6f78 6573 2028 6173 2049  checkboxes (as I
-00002450: 2064 6964 2077 6974 6820 6d6f 7374 206f   did with most o
-00002460: 6620 7468 6520 6f74 6865 7220 666f 726d  f the other form
-00002470: 2065 6c65 6d65 6e74 7329 2e0d 0a43 6865   elements)...Che
-00002480: 636b 626f 7865 7320 2a73 686f 756c 642a  ckboxes *should*
-00002490: 2077 6f72 6b2c 2062 7574 2070 6c65 6173   work, but pleas
-000024a0: 6520 6c65 7420 6d65 206b 6e6f 7720 6966  e let me know if
-000024b0: 2079 6f75 2065 6e63 6f75 6e74 6572 2061   you encounter a
-000024c0: 6e79 2074 6861 7420 646f 206e 6f74 2e0d  ny that do not..
-000024d0: 0a0d 0a23 204e 6577 2069 6e20 646f 6378  ...# New in docx
-000024e0: 3270 7974 686f 6e20 5665 7273 696f 6e20  2python Version 
-000024f0: 320d 0a0d 0a23 2320 6d65 7267 6520 636f  2....## merge co
-00002500: 6e73 6563 7574 6976 6520 7275 6e73 2077  nsecutive runs w
-00002510: 6974 6820 6964 656e 7469 6361 6c20 666f  ith identical fo
-00002520: 726d 6174 7469 6e67 0d0a 0d0a 4d53 2057  rmatting....MS W
-00002530: 6f72 6420 7769 6c6c 2062 7265 616b 2075  ord will break u
-00002540: 7020 7465 7874 2072 756e 7320 6172 6269  p text runs arbi
-00002550: 7472 6172 696c 792c 206f 6674 656e 2069  trarily, often i
-00002560: 6e20 7468 6520 6d69 6464 6c65 206f 6620  n the middle of 
-00002570: 6120 776f 7264 2e0d 0a0d 0a0d 0a20 2020  a word.......   
-00002580: 203c 773a 723e 0d0a 2020 2020 2020 2020   <w:r>..        
-00002590: 3c77 3a74 3e77 6f72 6b20 746f 2069 6d3c  <w:t>work to im<
-000025a0: 2f77 3a74 3e0d 0a20 2020 203c 2f77 3a72  /w:t>..    </w:r
-000025b0: 3e0d 0a20 2020 203c 773a 723e 0d0a 2020  >..    <w:r>..  
-000025c0: 2020 2020 2020 3c77 3a74 3e70 726f 7665        <w:t>prove
-000025d0: 2064 6f63 7832 7079 7468 6f6e 3c2f 773a   docx2python</w:
-000025e0: 743e 0d0a 2020 2020 3c2f 773a 723e 0d0a  t>..    </w:r>..
-000025f0: 0d0a 5468 6973 206d 616b 6573 2074 6869  ..This makes thi
-00002600: 6e67 7320 6c69 6b65 2061 6c67 6f72 6974  ngs like algorit
-00002610: 686d 6963 2073 6561 7263 682d 616e 642d  hmic search-and-
-00002620: 7265 706c 6163 6520 7072 6f62 6c65 6d61  replace problema
-00002630: 7469 632e 2044 6f63 7832 7079 7468 6f6e  tic. Docx2python
-00002640: 2064 6f65 7320 6e6f 7420 6375 7272 656e   does not curren
-00002650: 746c 7920 7772 6974 6520 646f 6378 2066  tly write docx f
-00002660: 696c 6573 2c0d 0a62 7574 2049 206f 6674  iles,..but I oft
-00002670: 656e 2075 7365 2064 6f63 7820 7465 6d70  en use docx temp
-00002680: 6c61 7465 7320 7769 7468 2070 6c61 6365  lates with place
-00002690: 686f 6c64 6572 7320 2865 2e67 2e2c 2060  holders (e.g., `
-000026a0: 2343 4154 4547 4f52 595f 4e41 4d45 2360  #CATEGORY_NAME#`
-000026b0: 2920 7468 656e 2072 6570 6c61 6365 2074  ) then replace t
-000026c0: 686f 7365 2070 6c61 6365 686f 6c64 6572  hose placeholder
-000026d0: 7320 7769 7468 2064 6174 612e 0d0a 5468  s with data...Th
-000026e0: 6973 2077 6f6e 2774 2077 6f72 6b20 6966  is won't work if
-000026f0: 2079 6f75 7220 706c 6163 6568 6f6c 6465   your placeholde
-00002700: 7273 2061 7265 2062 726f 6b65 6e20 7570  rs are broken up
-00002710: 2028 652e 672c 2060 2343 4154 602c 2060   (e.g, `#CAT`, `
-00002720: 4560 2c20 6047 4f52 595f 4e41 4d45 2360  E`, `GORY_NAME#`
-00002730: 292e 0d0a 0d0a 446f 6378 3270 7974 686f  ).....Docx2pytho
-00002740: 6e20 7631 206d 6572 6765 7320 7375 6368  n v1 merges such
-00002750: 2072 756e 7320 746f 6765 7468 6572 2077   runs together w
-00002760: 6865 6e20 6578 706f 7274 696e 6720 7465  hen exporting te
-00002770: 7874 2e20 446f 6378 3270 7974 686f 6e20  xt. Docx2python 
-00002780: 7632 2077 696c 6c20 6d65 7267 6520 7375  v2 will merge su
-00002790: 6368 2072 756e 7320 696e 2074 6865 2058  ch runs in the X
-000027a0: 4d4c 2061 7320 610d 0a70 7265 2d70 726f  ML as a..pre-pro
-000027b0: 6365 7373 696e 6720 7374 6570 2e20 5468  cessing step. Th
-000027c0: 6973 2077 696c 6c20 616c 6c6f 7720 7361  is will allow sa
-000027d0: 7669 6e67 2073 7563 6820 2272 6570 6169  ving such "repai
-000027e0: 7265 6422 2058 4d4c 206c 6174 6572 206f  red" XML later o
-000027f0: 6e2e 0d0a 0d0a 2323 206d 6572 6765 2063  n.....## merge c
-00002800: 6f6e 7365 6375 7469 7665 206c 696e 6b73  onsecutive links
-00002810: 2077 6974 6820 6964 656e 7469 6361 6c20   with identical 
-00002820: 6872 6566 730d 0a0d 0a4d 5320 576f 7264  hrefs....MS Word
-00002830: 2077 696c 6c20 6272 6561 6b20 7570 206c   will break up l
-00002840: 696e 6b73 2c20 6769 7669 6e67 2065 6163  inks, giving eac
-00002850: 6820 6c69 6e6b 2061 2064 6966 6665 7265  h link a differe
-00002860: 6e74 2060 7249 6460 2c20 6576 656e 2077  nt `rId`, even w
-00002870: 6865 6e20 7468 6573 6520 6072 4964 7360  hen these `rIds`
-00002880: 2070 6f69 6e74 2074 6f20 7468 6520 7361   point to the sa
-00002890: 6d65 2061 6464 7265 7373 2e0d 0a0d 0a20  me address..... 
-000028a0: 2020 203c 773a 6879 7065 726c 696e 6b20     <w:hyperlink 
-000028b0: 723a 6964 3d22 7249 6431 3322 3e20 2023  r:id="rId13">  #
-000028c0: 2072 4944 3133 2070 6f69 6e74 7320 746f   rID13 points to
-000028d0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000028e0: 636f 6d2f 5368 6179 4869 6c6c 2f64 6f63  com/ShayHill/doc
-000028f0: 7832 7079 7468 6f6e 0d0a 2020 2020 2020  x2python..      
-00002900: 2020 3c77 3a72 3e0d 0a20 2020 2020 2020    <w:r>..       
-00002910: 2020 2020 203c 773a 743e 646f 6378 3270       <w:t>docx2p
-00002920: 793c 2f77 3a74 3e0d 0a20 2020 2020 2020  y</w:t>..       
-00002930: 203c 2f77 3a72 3e0d 0a20 2020 203c 2f77   </w:r>..    </w
-00002940: 3a68 7970 6572 6c69 6e6b 3e0d 0a20 2020  :hyperlink>..   
-00002950: 203c 773a 6879 7065 726c 696e 6b20 723a   <w:hyperlink r:
-00002960: 6964 3d22 7249 6431 3422 3e20 2023 2072  id="rId14">  # r
-00002970: 4944 3134 2041 4c53 4f20 706f 696e 7473  ID14 ALSO points
-00002980: 2074 6f20 6874 7470 733a 2f2f 6769 7468   to https://gith
-00002990: 7562 2e63 6f6d 2f53 6861 7948 696c 6c2f  ub.com/ShayHill/
-000029a0: 646f 6378 3270 7974 686f 6e0d 0a20 2020  docx2python..   
-000029b0: 2020 2020 203c 773a 723e 0d0a 2020 2020       <w:r>..    
-000029c0: 2020 2020 2020 2020 3c77 3a74 3e74 686f          <w:t>tho
-000029d0: 6e3c 2f77 3a74 3e0d 0a20 2020 2020 2020  n</w:t>..       
-000029e0: 203c 2f77 3a72 3e0d 0a20 2020 203c 2f77   </w:r>..    </w
-000029f0: 3a68 7970 6572 6c69 6e6b 3e0d 0a0d 0a54  :hyperlink>....T
-00002a00: 6869 7320 6973 2073 696d 696c 6172 2074  his is similar t
-00002a10: 6f20 7468 6520 6272 6f6b 656e 2d75 7020  o the broken-up 
-00002a20: 7275 6e73 2c20 6275 7420 7468 6520 6361  runs, but the ca
-00002a30: 7573 6520 6973 2061 206c 6974 746c 6520  use is a little 
-00002a40: 6465 6570 6572 2069 6e2e 2044 6f63 7832  deeper in. Docx2
-00002a50: 7079 7468 6f6e 2076 3120 6d61 6b65 7320  python v1 makes 
-00002a60: 6120 6d65 7373 206f 6620 7468 6573 652e  a mess of these.
-00002a70: 0d0a 0d0a 2020 2020 3c61 2068 7265 663d  ....    <a href=
-00002a80: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00002a90: 636f 6d2f 5368 6179 4869 6c6c 2f64 6f63  com/ShayHill/doc
-00002aa0: 7832 7079 7468 6f6e 223e 646f 6378 3270  x2python">docx2p
-00002ab0: 793c 2f61 3e0d 0a20 2020 203c 6120 6872  y</a>..    <a hr
-00002ac0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00002ad0: 7562 2e63 6f6d 2f53 6861 7948 696c 6c2f  ub.com/ShayHill/
-00002ae0: 646f 6378 3270 7974 686f 6e22 3e74 686f  docx2python">tho
-00002af0: 6e3c 2f61 3e0d 0a0d 0a44 6f63 7832 7079  n</a>....Docx2py
-00002b00: 7468 6f6e 2076 3220 7769 6c6c 206d 6572  thon v2 will mer
-00002b10: 6765 2073 7563 6820 6c69 6e6b 7320 746f  ge such links to
-00002b20: 6765 7468 6572 2069 6e20 7468 6520 584d  gether in the XM
-00002b30: 4c20 6173 2061 2070 7265 2d70 726f 6365  L as a pre-proce
-00002b40: 7373 696e 6720 7374 6570 2e20 4173 2061  ssing step. As a
-00002b50: 626f 7665 2c20 7468 6973 2077 696c 6c20  bove, this will 
-00002b60: 616c 6c6f 7720 7361 7669 6e67 0d0a 7375  allow saving..su
-00002b70: 6368 2022 7265 7061 6972 6564 2220 584d  ch "repaired" XM
-00002b80: 4c20 6c61 7465 7220 6f6e 2e0d 0a0d 0a23  L later on.....#
-00002b90: 2320 636f 7272 6563 746c 7920 6861 6e64  # correctly hand
-00002ba0: 6c65 206e 6573 7465 6420 7061 7261 6772  le nested paragr
-00002bb0: 6170 6873 0d0a 0d0a 4d53 2057 6f72 6420  aphs....MS Word 
-00002bc0: 7769 6c6c 206e 6573 7420 7061 7261 6772  will nest paragr
-00002bd0: 6170 6873 0d0a 0d0a 2020 2020 3c77 3a70  aphs....    <w:p
-00002be0: 3e0d 0a20 2020 2020 2020 203c 773a 723e  >..        <w:r>
-00002bf0: 0d0a 2020 2020 2020 2020 2020 2020 3c77  ..            <w
-00002c00: 3a74 3e74 6578 743c 2f77 3a74 3e0d 0a20  :t>text</w:t>.. 
-00002c10: 2020 2020 2020 203c 2f77 3a72 3e0d 0a20         </w:r>.. 
-00002c20: 2020 2020 2020 203c 773a 703e 2020 2320         <w:p>  # 
-00002c30: 7061 7261 6772 6170 6820 696e 7369 6465  paragraph inside
-00002c40: 2061 2070 6172 6167 7261 7068 0d0a 2020   a paragraph..  
-00002c50: 2020 2020 2020 2020 2020 3c77 3a72 3e0d            <w:r>.
-00002c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002c70: 203c 773a 743e 7465 7874 3c2f 773a 743e   <w:t>text</w:t>
-00002c80: 0d0a 2020 2020 2020 2020 2020 2020 3c2f  ..            </
-00002c90: 773a 723e 0d0a 2020 2020 2020 2020 3c2f  w:r>..        </
-00002ca0: 773a 703e 0d0a 2020 2020 2020 2020 3c77  w:p>..        <w
-00002cb0: 3a72 3e0d 0a20 2020 2020 2020 2020 2020  :r>..           
-00002cc0: 203c 773a 743e 7465 7874 3c2f 773a 743e   <w:t>text</w:t>
-00002cd0: 0d0a 2020 2020 2020 2020 3c2f 773a 723e  ..        </w:r>
-00002ce0: 0d0a 2020 2020 3c2f 773a 703e 0d0a 0d0a  ..    </w:p>....
-00002cf0: 4920 6861 7665 6e27 7420 6265 656e 2061  I haven't been a
-00002d00: 626c 6520 746f 2063 7265 6174 6520 7375  ble to create su
-00002d10: 6368 2061 2070 6172 6167 7261 7068 2c20  ch a paragraph, 
-00002d20: 6275 7420 4927 7665 2066 6f75 6e64 2061  but I've found a
-00002d30: 2066 6577 2066 696c 6573 2074 6861 7420   few files that 
-00002d40: 6861 7665 2074 6865 6d2e 2044 6f63 7832  have them. Docx2
-00002d50: 7079 686f 6e20 7631 2077 696c 6c20 6f6d  pyhon v1 will om
-00002d60: 6974 0d0a 636c 6f73 696e 6720 6874 6d6c  it..closing html
-00002d70: 2074 6167 7320 7768 656e 2061 206e 6577   tags when a new
-00002d80: 2070 6172 6167 7261 7068 2069 7320 6f70   paragraph is op
-00002d90: 656e 6564 2062 6566 6f72 6520 7468 6520  ened before the 
-00002da0: 6f6c 6420 7061 7261 6772 6170 6820 6973  old paragraph is
-00002db0: 2063 6c6f 7365 642e 0d0a 0d0a 2020 2020   closed.....    
-00002dc0: 3c62 3e6f 7574 6572 2070 6172 2062 6f6c  <b>outer par bol
-00002dd0: 6420 7465 7874 0d0a 0d0a 2020 2020 3c69  d text....    <i
-00002de0: 3e54 6869 7320 7465 7874 2069 7320 696e  >This text is in
-00002df0: 206e 6573 7465 6420 7061 7220 286e 6f74   nested par (not
-00002e00: 2062 6f6c 6429 3c2f 693e 0d0a 0d0a 2020   bold)</i>....  
-00002e10: 2020 6f75 7465 7220 7061 7220 626f 6c64    outer par bold
-00002e20: 2074 6578 743c 2f62 3e0d 0a0d 0a44 6f63   text</b>....Doc
-00002e30: 7832 7079 7468 6f6e 2076 3220 7769 6c6c  x2python v2 will
-00002e40: 2063 6f72 7265 6374 6c79 2068 616e 646c   correctly handl
-00002e50: 6520 7375 6368 2063 6173 6573 2c20 6275  e such cases, bu
-00002e60: 7420 7468 6973 2077 696c 6c20 7265 7175  t this will requ
-00002e70: 6972 6520 7375 6273 7461 6e74 6961 6c20  ire substantial 
-00002e80: 696e 7465 726e 616c 2063 6861 6e67 6573  internal changes
-00002e90: 2074 6f20 7468 6520 7761 790d 0a64 6f63   to the way..doc
-00002ea0: 7832 7079 7468 6f6e 206f 7065 6e73 2061  x2python opens a
-00002eb0: 6e64 2063 6c6f 7365 7320 7061 7261 6772  nd closes paragr
-00002ec0: 6170 6873 2e0d 0a0d 0a20 2020 203c 623e  aphs.....    <b>
-00002ed0: 6f75 7465 7220 7061 7220 626f 6c64 2074  outer par bold t
-00002ee0: 6578 743c 2f62 3e0d 0a0d 0a20 2020 203c  ext</b>....    <
-00002ef0: 693e 5468 6973 2074 6578 7420 6973 2069  i>This text is i
-00002f00: 6e20 6e65 7374 6564 2070 6172 2028 6e6f  n nested par (no
-00002f10: 7420 626f 6c64 293c 2f69 3e0d 0a0d 0a20  t bold)</i>.... 
-00002f20: 2020 203c 2f62 3e6f 7574 6572 2070 6172     </b>outer par
-00002f30: 2062 6f6c 6420 7465 7874 3c2f 623e 0d0a   bold text</b>..
-00002f40: 0d0a 2323 2070 6172 6167 7261 7068 2073  ..## paragraph s
-00002f50: 7479 6c65 730d 0a0d 0a54 6865 2069 6e74  tyles....The int
-00002f60: 6572 6e61 6c20 6368 616e 6765 7320 616c  ernal changes al
-00002f70: 6c6f 7720 666f 7220 6561 7379 2061 6363  low for easy acc
-00002f80: 6573 7320 746f 2070 6172 6167 7261 7068  ess to paragraph
-00002f90: 2073 7479 6c65 7320 2865 2e67 2e2c 2060   styles (e.g., `
-00002fa0: 4865 6164 696e 6720 3160 292e 2044 6f63  Heading 1`). Doc
-00002fb0: 7832 7079 7468 6f6e 2076 3120 6967 6e6f  x2python v1 igno
-00002fc0: 7265 7320 7468 6573 652c 2065 7665 6e0d  res these, even.
-00002fd0: 0a77 6974 6820 6068 746d 6c3d 5472 7565  .with `html=True
-00002fe0: 602e 2044 6f63 7832 7079 7468 6f6e 2076  `. Docx2python v
-00002ff0: 3220 7769 6c6c 2063 6170 7475 7265 2070  2 will capture p
-00003000: 6172 6167 7261 7068 2073 7479 6c65 732e  aragraph styles.
-00003010: 0d0a 0d0a 2020 2020 3c68 313e 6831 2069  ....    <h1>h1 i
-00003020: 7320 6120 7061 7261 6772 6170 6820 7374  s a paragraph st
-00003030: 796c 653c 623e 626f 6c64 2069 7320 6120  yle<b>bold is a 
-00003040: 7275 6e20 7374 796c 653c 2f62 3e3c 2f68  run style</b></h
-00003050: 313e 0d0a 0d0a 2323 2065 7870 6f72 7420  1>....## export 
-00003060: 786d 6c0d 0a0d 0a54 6f20 616c 6c6f 7720  xml....To allow 
-00003070: 6162 6f76 652d 6465 7363 7269 6265 6420  above-described 
-00003080: 6c69 6768 7420 6564 6974 696e 6720 2865  light editing (e
-00003090: 2e67 2e2c 2073 6561 7263 6820 616e 6420  .g., search and 
-000030a0: 7265 706c 6163 6529 2c20 646f 6378 3270  replace), docx2p
-000030b0: 7974 686f 6e20 7632 2077 696c 6c20 6769  ython v2 will gi
-000030c0: 7665 2074 6865 2075 7365 7220 6163 6365  ve the user acce
-000030d0: 7373 2074 6f0d 0a0d 0a20 2020 2031 2e20  ss to....    1. 
-000030e0: 6578 7472 6163 7465 6420 786d 6c20 6669  extracted xml fi
-000030f0: 6c65 730d 0a20 2020 2032 2e20 7468 6520  les..    2. the 
-00003100: 6675 6e63 7469 6f6e 7320 7573 6564 2074  functions used t
-00003110: 6f20 7772 6974 6520 7468 6573 6520 6669  o write these fi
-00003120: 6c65 7320 746f 2061 2064 6f63 780d 0a0d  les to a docx...
-00003130: 0a54 6865 2075 7365 7220 6361 6e20 6f6e  .The user can on
-00003140: 6c79 2067 6f20 736f 2066 6172 2077 6974  ly go so far wit
-00003150: 6820 7468 6973 2e20 4120 646f 6378 2066  h this. A docx f
-00003160: 696c 6520 6973 2062 7569 6c74 2066 726f  ile is built fro
-00003170: 6d20 666f 6c64 6572 7320 6675 6c6c 206f  m folders full o
-00003180: 6620 786d 6c20 6669 6c65 732e 204e 6f6e  f xml files. Non
-00003190: 6520 6f66 2074 6865 7365 2078 6d6c 0d0a  e of these xml..
-000031a0: 6669 6c65 7320 6172 6520 7365 6c66 2063  files are self c
-000031b0: 6f6e 7461 696e 6564 2e20 4275 7420 7365  ontained. But se
-000031c0: 6172 6368 2061 6e64 2072 6570 6c61 6365  arch and replace
-000031d0: 2069 7320 656e 6f75 6768 2074 6f20 6d61   is enough to ma
-000031e0: 6b65 2064 6f63 756d 656e 7420 7465 6d70  ke document temp
-000031f0: 6c61 7465 7320 2864 6f63 756d 656e 7473  lates (documents
-00003200: 2077 6974 6820 706c 6163 6568 6f6c 6465   with placeholde
-00003210: 7273 2066 6f72 0d0a 6461 7461 292c 2061  rs for..data), a
-00003220: 6e64 2074 6861 7427 7320 7072 6574 7479  nd that's pretty
-00003230: 2075 7365 6675 6c20 696e 2069 7473 656c   useful in itsel
-00003240: 662e 0d0a 0d0a 2323 2065 7870 6f73 6520  f.....## expose 
-00003250: 736f 6d65 2069 6e74 6572 6d65 6469 6174  some intermediat
-00003260: 6520 6675 6e63 7469 6f6e 616c 6974 790d  e functionality.
-00003270: 0a0d 0a4e 6176 6967 6174 696e 6720 7468  ...Navigating th
-00003280: 726f 7567 6820 584d 4c20 6973 2073 7472  rough XML is str
-00003290: 6169 6768 7466 6f72 7761 7264 2077 6974  aightforward wit
-000032a0: 6820 606c 786d 6c60 2e20 4974 2069 7320  h `lxml`. It is 
-000032b0: 6120 7365 7061 7261 7465 2073 7465 7020  a separate step 
-000032c0: 746f 2074 616b 6520 7768 6174 6576 6572  to take whatever
-000032d0: 2079 6f75 2066 696e 6420 616e 6420 6272   you find and br
-000032e0: 696e 6720 6974 0d0a 2a6f 7574 2a20 6f66  ing it..*out* of
-000032f0: 2074 6865 2058 4d4c 2e20 466f 7220 696e   the XML. For in
-00003300: 7374 616e 6365 2c20 796f 7520 6d61 7920  stance, you may 
-00003310: 7761 6e74 2074 6f20 6974 6572 6174 6520  want to iterate 
-00003320: 6f76 6572 2061 2064 6f63 756d 656e 742c  over a document,
-00003330: 206c 6f6f 6b69 6e67 2066 6f72 2070 6172   looking for par
-00003340: 6167 7261 7068 7320 7769 7468 2061 2070  agraphs with a p
-00003350: 6172 7469 6375 6c61 720d 0a66 6f72 6d61  articular..forma
-00003360: 742c 2074 6865 6e20 7075 6c6c 2074 6865  t, then pull the
-00003370: 2074 6578 7420 6f75 7420 6f66 2074 686f   text out of tho
-00003380: 7365 2070 6172 6167 7261 7068 732e 2044  se paragraphs. D
-00003390: 6f63 7832 7079 7468 6f6e 2076 3120 6469  ocx2python v1 di
-000033a0: 6420 6e6f 7420 7365 7061 7261 7465 206f  d not separate o
-000033b0: 7220 6578 706f 7365 2022 6974 6572 2074  r expose "iter t
-000033c0: 6865 2064 6f63 756d 656e 7422 2061 6e64  he document" and
-000033d0: 0d0a 2270 756c 6c20 7468 6520 636f 6e74  .."pull the cont
-000033e0: 656e 7422 2e20 446f 6378 3270 7974 686f  ent". Docx2pytho
-000033f0: 6e20 7632 2073 6570 6172 6174 6573 2061  n v2 separates a
-00003400: 6e64 2065 7870 6f73 6573 2074 6865 7365  nd exposes these
-00003410: 2073 7465 7073 2e20 5468 6973 2077 696c   steps. This wil
-00003420: 6c20 616c 6c6f 7720 6561 7369 6572 2065  l allow easier e
-00003430: 7874 656e 7369 6f6e 2e0d 0a0d 0a53 6565  xtension.....See
-00003440: 2074 6865 2060 646f 6378 5f72 6561 6465   the `docx_reade
-00003450: 722e 7079 6020 6d6f 6475 6c65 2061 6e64  r.py` module and
-00003460: 2073 696d 706c 6520 6578 616d 706c 6573   simple examples
-00003470: 2069 6e20 7468 6520 6075 7469 6c69 7469   in the `utiliti
-00003480: 6573 2e70 7960 206d 6f64 756c 652e 0d0a  es.py` module...
-00003490: 0d0a 2323 2073 6565 2075 7469 6c69 7469  ..## see utiliti
-000034a0: 6573 2e70 7920 666f 7220 6578 616d 706c  es.py for exampl
-000034b0: 6573 206f 6620 6d61 6a6f 7220 6e65 7720  es of major new 
-000034c0: 6665 6174 7572 6573 2e0d 0a              features...
+00000000: 2320 646f 6378 3270 7974 686f 6e0a 0a45  # docx2python..E
+00000010: 7874 7261 6374 2064 6f63 7820 6865 6164  xtract docx head
+00000020: 6572 732c 2066 6f6f 7465 7273 2c20 7465  ers, footers, te
+00000030: 7874 2c20 666f 6f74 6e6f 7465 732c 2065  xt, footnotes, e
+00000040: 6e64 6e6f 7465 732c 2070 726f 7065 7274  ndnotes, propert
+00000050: 6965 732c 2061 6e64 2069 6d61 6765 7320  ies, and images 
+00000060: 746f 2061 2050 7974 686f 6e20 6f62 6a65  to a Python obje
+00000070: 6374 2e0a 0a60 5245 4144 4d45 5f44 4f43  ct...`README_DOC
+00000080: 585f 4649 4c45 5f53 5452 5543 5455 5245  X_FILE_STRUCTURE
+00000090: 2e6d 6460 206d 6179 2068 656c 7020 6966  .md` may help if
+000000a0: 2079 6f75 2764 206c 696b 6520 746f 2065   you'd like to e
+000000b0: 7874 656e 6420 646f 6378 3270 7974 686f  xtend docx2pytho
+000000c0: 6e2e 0a0a 466f 7220 6120 7375 6d6d 6172  n...For a summar
+000000d0: 7920 6f66 2077 6861 7427 7320 6e65 7720  y of what's new 
+000000e0: 696e 2064 6f63 7832 7079 7468 6f6e 2032  in docx2python 2
+000000f0: 2c20 7363 726f 6c6c 2064 6f77 6e20 746f  , scroll down to
+00000100: 202a 2a4e 6577 2069 6e20 646f 6378 3270   **New in docx2p
+00000110: 7974 686f 6e20 5665 7273 696f 6e20 322a  ython Version 2*
+00000120: 2a0a 0a54 6865 2063 6f64 6520 6973 2061  *..The code is a
+00000130: 6e20 6578 7061 6e73 696f 6e2f 636f 6e74  n expansion/cont
+00000140: 7261 6374 696f 6e20 6f66 205b 7079 7468  raction of [pyth
+00000150: 6f6e 2d64 6f63 7832 7478 745d 2868 7474  on-docx2txt](htt
+00000160: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000170: 616e 6b75 7368 7368 6168 3839 2f70 7974  ankushshah89/pyt
+00000180: 686f 6e2d 646f 6378 3274 7874 2920 2843  hon-docx2txt) (C
+00000190: 6f70 7972 6967 6874 2028 6329 2032 3031  opyright (c) 201
+000001a0: 3520 416e 6b75 7368 2053 6861 6829 2e20  5 Ankush Shah). 
+000001b0: 5468 6520 6f72 6967 696e 616c 2063 6f64  The original cod
+000001c0: 6520 6973 206d 6f73 746c 7920 676f 6e65  e is mostly gone
+000001d0: 2c20 6275 7420 736f 6d65 206f 6620 7468  , but some of th
+000001e0: 6520 626f 6e65 7320 6d61 7920 7374 696c  e bones may stil
+000001f0: 6c20 6265 2068 6572 652e 0a0a 5f5f 7368  l be here...__sh
+00000200: 6172 6564 2066 6561 7475 7265 735f 5f3a  ared features__:
+00000210: 0a2a 2065 7874 7261 6374 7320 7465 7874  .* extracts text
+00000220: 2066 726f 6d20 646f 6378 2066 696c 6573   from docx files
+00000230: 0a2a 2065 7874 7261 6374 7320 696d 6167  .* extracts imag
+00000240: 6573 2066 726f 6d20 646f 6378 2066 696c  es from docx fil
+00000250: 6573 0a0a 5f5f 6164 6469 7469 6f6e 733a  es..__additions:
+00000260: 5f5f 0a2a 2065 7874 7261 6374 7320 666f  __.* extracts fo
+00000270: 6f74 6e6f 7465 7320 616e 6420 656e 646e  otnotes and endn
+00000280: 6f74 6573 0a2a 2063 6f6e 7665 7274 7320  otes.* converts 
+00000290: 6275 6c6c 6574 7320 616e 6420 6e75 6d62  bullets and numb
+000002a0: 6572 6564 206c 6973 7473 2074 6f20 6173  ered lists to as
+000002b0: 6369 6920 7769 7468 2069 6e64 656e 7461  cii with indenta
+000002c0: 7469 6f6e 0a2a 2063 6f6e 7665 7274 7320  tion.* converts 
+000002d0: 6879 7065 726c 696e 6b73 2074 6f20 6060  hyperlinks to ``
+000002e0: 3c61 2068 7265 663d 2268 7474 703a 2f2e  <a href="http:/.
+000002f0: 2e2e 223e 6c69 6e6b 2074 6578 743c 2f61  ..">link text</a
+00000300: 3e60 600a 2a20 7265 7461 696e 7320 736f  >``.* retains so
+00000310: 6d65 2073 7472 7563 7475 7265 206f 6620  me structure of 
+00000320: 7468 6520 6f72 6967 696e 616c 2066 696c  the original fil
+00000330: 6520 286d 6f72 6520 6265 6c6f 7729 0a2a  e (more below).*
+00000340: 2065 7874 7261 6374 7320 646f 6375 6d65   extracts docume
+00000350: 6e74 2070 726f 7065 7274 6965 7320 2863  nt properties (c
+00000360: 7265 6174 6f72 2c20 6c61 7374 4d6f 6469  reator, lastModi
+00000370: 6669 6564 4279 2c20 6574 632e 290a 2a20  fiedBy, etc.).* 
+00000380: 696e 7365 7274 7320 696d 6167 6520 706c  inserts image pl
+00000390: 6163 6568 6f6c 6465 7273 2069 6e20 7465  aceholders in te
+000003a0: 7874 2028 6060 272d 2d2d 2d69 6d61 6765  xt (``'----image
+000003b0: 312e 6a70 672d 2d2d 2d27 6060 290a 2a20  1.jpg----'``).* 
+000003c0: 696e 7365 7274 7320 706c 6169 6e20 7465  inserts plain te
+000003d0: 7874 2066 6f6f 746e 6f74 6520 616e 6420  xt footnote and 
+000003e0: 656e 646e 6f74 6520 7265 6665 7265 6e63  endnote referenc
+000003f0: 6573 2069 6e20 7465 7874 2028 6060 272d  es in text (``'-
+00000400: 2d2d 2d66 6f6f 746e 6f74 6531 2d2d 2d2d  ---footnote1----
+00000410: 2760 6029 0a2a 2028 6f70 7469 6f6e 616c  '``).* (optional
+00000420: 6c79 2920 7265 7461 696e 7320 666f 6e74  ly) retains font
+00000430: 2073 697a 652c 2066 6f6e 7420 636f 6c6f   size, font colo
+00000440: 722c 2062 6f6c 642c 2069 7461 6c69 6373  r, bold, italics
+00000450: 2c20 616e 6420 756e 6465 7273 636f 7265  , and underscore
+00000460: 2061 7320 6874 6d6c 0a2a 2065 7874 7261   as html.* extra
+00000470: 6374 206d 6174 6820 6571 7561 7469 6f6e  ct math equation
+00000480: 730a 2a20 6578 7472 6163 7420 7573 6572  s.* extract user
+00000490: 2073 656c 6563 7469 6f6e 7320 6672 6f6d   selections from
+000004a0: 2063 6865 636b 626f 7865 7320 616e 6420   checkboxes and 
+000004b0: 6472 6f70 646f 776e 206d 656e 7573 0a0a  dropdown menus..
+000004c0: 5f5f 7375 6274 7261 6374 696f 6e73 3a5f  __subtractions:_
+000004d0: 5f0a 2a20 6e6f 2063 6f6d 6d61 6e64 2d6c  _.* no command-l
+000004e0: 696e 6520 696e 7465 7266 6163 650a 2a20  ine interface.* 
+000004f0: 7769 6c6c 206f 6e6c 7920 776f 726b 2077  will only work w
+00000500: 6974 6820 5079 7468 6f6e 2033 2e38 2b0a  ith Python 3.8+.
+00000510: 0a0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000520: 6e0a 6060 6062 6173 680a 7069 7020 696e  n.```bash.pip in
+00000530: 7374 616c 6c20 646f 6378 3270 7974 686f  stall docx2pytho
+00000540: 6e0a 6060 600a 0a23 2320 5573 650a 0a60  n.```..## Use..`
+00000550: 6060 2070 7974 686f 6e0a 6672 6f6d 2064  `` python.from d
+00000560: 6f63 7832 7079 7468 6f6e 2069 6d70 6f72  ocx2python impor
+00000570: 7420 646f 6378 3270 7974 686f 6e0a 0a23  t docx2python..#
+00000580: 2065 7874 7261 6374 2064 6f63 7820 636f   extract docx co
+00000590: 6e74 656e 740a 7769 7468 2064 6f63 7832  ntent.with docx2
+000005a0: 7079 7468 6f6e 2827 7061 7468 2f74 6f2f  python('path/to/
+000005b0: 6669 6c65 2e64 6f63 7827 2920 6173 2064  file.docx') as d
+000005c0: 6f63 785f 636f 6e74 656e 743a 0a20 2020  ocx_content:.   
+000005d0: 2070 7269 6e74 2864 6f63 785f 636f 6e74   print(docx_cont
+000005e0: 656e 742e 7465 7874 290a 0a64 6f63 785f  ent.text)..docx_
+000005f0: 636f 6e74 656e 7420 3d20 646f 6378 3270  content = docx2p
+00000600: 7974 686f 6e28 2770 6174 682f 746f 2f66  ython('path/to/f
+00000610: 696c 652e 646f 6378 2729 0a70 7269 6e74  ile.docx').print
+00000620: 2864 6f63 785f 636f 6e74 656e 742e 7465  (docx_content.te
+00000630: 7874 290a 646f 6378 5f63 6f6e 7465 6e74  xt).docx_content
+00000640: 2e63 6c6f 7365 2829 0a0a 2320 6578 7472  .close()..# extr
+00000650: 6163 7420 646f 6378 2063 6f6e 7465 6e74  act docx content
+00000660: 2c20 7772 6974 6520 696d 6167 6573 2074  , write images t
+00000670: 6f20 696d 6167 655f 6469 7265 6374 6f72  o image_director
+00000680: 790a 7769 7468 2064 6f63 7832 7079 7468  y.with docx2pyth
+00000690: 6f6e 2827 7061 7468 2f74 6f2f 6669 6c65  on('path/to/file
+000006a0: 2e64 6f63 7827 2c20 2770 6174 682f 746f  .docx', 'path/to
+000006b0: 2f69 6d61 6765 5f64 6972 6563 746f 7279  /image_directory
+000006c0: 2729 2061 7320 646f 6378 5f63 6f6e 7465  ') as docx_conte
+000006d0: 6e74 3a0a 2020 2020 7072 696e 7428 646f  nt:.    print(do
+000006e0: 6378 5f63 6f6e 7465 6e74 2e74 6578 7429  cx_content.text)
+000006f0: 0a0a 2320 6578 7472 6163 7420 646f 6378  ..# extract docx
+00000700: 2063 6f6e 7465 6e74 2077 6974 6820 6261   content with ba
+00000710: 7369 6320 666f 6e74 2073 7479 6c65 7320  sic font styles 
+00000720: 636f 6e76 6572 7465 6420 746f 2068 746d  converted to htm
+00000730: 6c0a 7769 7468 2064 6f63 7832 7079 7468  l.with docx2pyth
+00000740: 6f6e 2827 7061 7468 2f74 6f2f 6669 6c65  on('path/to/file
+00000750: 2e64 6f63 7827 2c20 6874 6d6c 3d54 7275  .docx', html=Tru
+00000760: 6529 2061 7320 646f 6378 5f63 6f6e 7465  e) as docx_conte
+00000770: 6e74 3a0a 2020 2020 7072 696e 7428 646f  nt:.    print(do
+00000780: 6378 5f63 6f6e 7465 6e74 2e74 6578 7429  cx_content.text)
+00000790: 0a60 6060 0a0a 6064 6f63 7832 7079 7468  .```..`docx2pyth
+000007a0: 6f6e 6020 6f70 656e 7320 6120 7a69 7066  on` opens a zipf
+000007b0: 696c 6520 6f62 6a65 6374 2061 6e64 2028  ile object and (
+000007c0: 6c61 7a69 6c79 2920 7265 6164 7320 6974  lazily) reads it
+000007d0: 2e20 5573 6520 636f 6e74 6578 7420 6d61  . Use context ma
+000007e0: 6e61 6765 6d65 6e74 2028 6077 6974 6820  nagement (`with 
+000007f0: 2e2e 2e20 6173 6029 2074 6f20 636c 6f73  ... as`) to clos
+00000800: 6520 7468 6973 207a 6970 6669 6c65 206f  e this zipfile o
+00000810: 626a 6563 7420 6f72 2065 7870 6c69 6369  bject or explici
+00000820: 746c 7920 636c 6f73 6520 7769 7468 2060  tly close with `
+00000830: 646f 6378 5f63 6f6e 7465 6e74 2e63 6c6f  docx_content.clo
+00000840: 7365 2829 602e 0a0a 4e6f 7465 206f 6e20  se()`...Note on 
+00000850: 6874 6d6c 2066 6561 7475 7265 3a0a 2a20  html feature:.* 
+00000860: 7375 7070 6f72 7473 2060 603c 693e 6060  supports ``<i>``
+00000870: 6974 616c 6963 2c20 6060 3c62 3e60 6062  italic, ``<b>``b
+00000880: 6f6c 642c 2060 603c 753e 6060 756e 6465  old, ``<u>``unde
+00000890: 726c 696e 652c 2060 603c 733e 6060 7374  rline, ``<s>``st
+000008a0: 7269 6b65 2c20 6060 3c73 7570 3e60 6073  rike, ``<sup>``s
+000008b0: 7570 6572 7363 7269 7074 2c20 6060 3c73  uperscript, ``<s
+000008c0: 7562 3e60 6073 7562 7363 7269 7074 2c20  ub>``subscript, 
+000008d0: 6060 3c73 7061 6e20 7374 796c 653d 2266  ``<span style="f
+000008e0: 6f6e 742d 7661 7269 616e 743a 2073 6d61  ont-variant: sma
+000008f0: 6c6c 2d63 6170 7322 3e60 6073 6d61 6c6c  ll-caps">``small
+00000900: 2063 6170 732c 2060 603c 7370 616e 2073   caps, ``<span s
+00000910: 7479 6c65 3d22 7465 7874 2d74 7261 6e73  tyle="text-trans
+00000920: 666f 726d 3a75 7070 6572 6361 7365 223e  form:uppercase">
+00000930: 6060 616c 6c20 6361 7073 2c20 6060 3c73  ``all caps, ``<s
+00000940: 7061 6e20 7374 796c 653d 2262 6163 6b67  pan style="backg
+00000950: 726f 756e 642d 636f 6c6f 723a 2079 656c  round-color: yel
+00000960: 6c6f 7722 3e60 6068 6967 686c 6967 6874  low">``highlight
+00000970: 6564 2c20 6060 3c73 7061 6e20 7374 796c  ed, ``<span styl
+00000980: 653d 2266 6f6e 742d 7369 7a65 3a33 3222  e="font-size:32"
+00000990: 3e60 6066 6f6e 7420 7369 7a65 2c20 6060  >``font size, ``
+000009a0: 3c73 7061 6e20 7374 796c 653d 2263 6f6c  <span style="col
+000009b0: 6f72 3a23 6666 3030 3030 223e 6060 636f  or:#ff0000">``co
+000009c0: 6c6f 7265 6420 7465 7874 2e0a 2a20 6879  lored text..* hy
+000009d0: 7065 726c 696e 6b73 2077 696c 6c20 616c  perlinks will al
+000009e0: 7761 7973 2062 6520 6578 706f 7274 6564  ways be exported
+000009f0: 2061 7320 6874 6d6c 2028 6060 3c61 2068   as html (``<a h
+00000a00: 7265 663d 2268 7474 703a 2f2e 2e2e 223e  ref="http:/...">
+00000a10: 6c69 6e6b 2074 6578 743c 2f61 3e60 6029  link text</a>``)
+00000a20: 2c20 6576 656e 2069 6620 6060 6874 6d6c  , even if ``html
+00000a30: 3d46 616c 7365 6060 2c20 6265 6361 7573  =False``, becaus
+00000a40: 6520 4920 636f 756c 646e 2774 2074 6869  e I couldn't thi
+00000a50: 6e6b 206f 6620 6120 6d6f 7265 2063 616e  nk of a more can
+00000a60: 6f6e 6963 616c 2072 6570 7265 7365 6e74  onical represent
+00000a70: 6174 696f 6e2e 0a2a 2065 7665 7279 2074  ation..* every t
+00000a80: 6167 206f 7065 6e20 696e 2061 2070 6172  ag open in a par
+00000a90: 6167 7261 7068 2077 696c 6c20 6265 2063  agraph will be c
+00000aa0: 6c6f 7365 6420 696e 2074 6861 7420 7061  losed in that pa
+00000ab0: 7261 6772 6170 6820 2861 6e64 2c20 7768  ragraph (and, wh
+00000ac0: 6572 6520 6170 7072 6f70 7269 6174 652c  ere appropriate,
+00000ad0: 2072 656f 7065 6e65 6420 696e 2074 6865   reopened in the
+00000ae0: 206e 6578 7420 7061 7261 6772 6170 6829   next paragraph)
+00000af0: 2e20 4966 2074 776f 2073 7562 7365 7175  . If two subsequ
+00000b00: 656e 6374 2070 6172 6167 7261 7068 7320  enct paragraphs 
+00000b10: 6172 6520 626f 6c64 2c20 7468 6579 2077  are bold, they w
+00000b20: 696c 6c20 6265 2072 6574 7572 6e65 6420  ill be returned 
+00000b30: 6173 2060 3c62 3e70 6172 6167 7261 7068  as `<b>paragraph
+00000b40: 2061 3c2f 623e 602c 2060 3c62 3e70 6172   a</b>`, `<b>par
+00000b50: 6167 7261 7068 2062 3c2f 623e 602e 2054  agraph b</b>`. T
+00000b60: 6869 7320 6973 2069 6e74 656e 7469 6f6e  his is intention
+00000b70: 616c 2074 6f20 6d61 6b65 2020 6561 6368  al to make  each
+00000b80: 2070 6172 6167 7261 7068 2069 7473 206f   paragraph its o
+00000b90: 776e 2065 6e74 6974 792e 0a2a 2069 6620  wn entity..* if 
+00000ba0: 796f 7520 7370 6563 6966 7920 6068 746d  you specify `htm
+00000bb0: 6c3d 5472 7565 602c 2060 2660 2c20 603e  l=True`, `&`, `>
+00000bc0: 6020 616e 6420 603c 6020 696e 2079 6f75  ` and `<` in you
+00000bd0: 7220 646f 6378 2074 6578 7420 7769 6c6c  r docx text will
+00000be0: 2062 6520 656e 636f 6465 6420 6173 2060   be encoded as `
+00000bf0: 2661 6d70 602c 2060 2667 743b 6020 616e  &amp`, `&gt;` an
+00000c00: 6420 6026 6c74 3b60 0a0a 2323 2052 6574  d `&lt;`..## Ret
+00000c10: 7572 6e20 5661 6c75 650a 0a46 756e 6374  urn Value..Funct
+00000c20: 696f 6e20 6064 6f63 7832 7079 7468 6f6e  ion `docx2python
+00000c30: 6020 7265 7475 726e 7320 6120 446f 6378  ` returns a Docx
+00000c40: 436f 6e74 656e 7420 696e 7374 616e 6365  Content instance
+00000c50: 2077 6974 6820 7365 7665 7261 6c20 6174   with several at
+00000c60: 7472 6962 7574 6573 2e0a 0a5f 5f68 6561  tributes...__hea
+00000c70: 6465 725f 5f20 2d20 636f 6e74 656e 7473  der__ - contents
+00000c80: 206f 6620 7468 6520 646f 6378 2068 6561   of the docx hea
+00000c90: 6465 7273 2069 6e20 7468 6520 7265 7475  ders in the retu
+00000ca0: 726e 2066 6f72 6d61 7420 6465 7363 7269  rn format descri
+00000cb0: 6265 6420 6865 7265 696e 0a0a 5f5f 666f  bed herein..__fo
+00000cc0: 6f74 6572 5f5f 202d 2063 6f6e 7465 6e74  oter__ - content
+00000cd0: 7320 6f66 2074 6865 2064 6f63 7820 666f  s of the docx fo
+00000ce0: 6f74 6572 7320 696e 2074 6865 2072 6574  oters in the ret
+00000cf0: 7572 6e20 666f 726d 6174 2064 6573 6372  urn format descr
+00000d00: 6962 6564 2068 6572 6569 6e0a 0a5f 5f62  ibed herein..__b
+00000d10: 6f64 795f 5f20 2d20 636f 6e74 656e 7473  ody__ - contents
+00000d20: 206f 6620 7468 6520 646f 6378 2069 6e20   of the docx in 
+00000d30: 7468 6520 7265 7475 726e 2066 6f72 6d61  the return forma
+00000d40: 7420 6465 7363 7269 6265 6420 6865 7265  t described here
+00000d50: 696e 0a0a 5f5f 666f 6f74 6e6f 7465 735f  in..__footnotes_
+00000d60: 5f20 2d20 636f 6e74 656e 7473 206f 6620  _ - contents of 
+00000d70: 7468 6520 646f 6378 2069 6e20 7468 6520  the docx in the 
+00000d80: 7265 7475 726e 2066 6f72 6d61 7420 6465  return format de
+00000d90: 7363 7269 6265 6420 6865 7265 696e 0a0a  scribed herein..
+00000da0: 5f5f 656e 646e 6f74 6573 5f5f 202d 2063  __endnotes__ - c
+00000db0: 6f6e 7465 6e74 7320 6f66 2074 6865 2064  ontents of the d
+00000dc0: 6f63 7820 696e 2074 6865 2072 6574 7572  ocx in the retur
+00000dd0: 6e20 666f 726d 6174 2064 6573 6372 6962  n format describ
+00000de0: 6564 2068 6572 6569 6e0a 0a5f 5f64 6f63  ed herein..__doc
+00000df0: 756d 656e 745f 5f20 2d20 6865 6164 6572  ument__ - header
+00000e00: 2020 2b20 626f 6479 202b 2066 6f6f 7465    + body + foote
+00000e10: 7220 2872 6561 6420 6f6e 6c79 290a 0a5f  r (read only).._
+00000e20: 5f74 6578 745f 5f20 2d20 616c 6c20 646f  _text__ - all do
+00000e30: 6378 2074 6578 7420 6173 206f 6e65 2073  cx text as one s
+00000e40: 7472 696e 672c 2073 696d 696c 6172 2074  tring, similar t
+00000e50: 6f20 7768 6174 2079 6f75 2764 2067 6574  o what you'd get
+00000e60: 2066 726f 6d20 6070 7974 686f 6e2d 646f   from `python-do
+00000e70: 6378 3274 7874 600a 0a5f 5f70 726f 7065  cx2txt`..__prope
+00000e80: 7274 6965 735f 5f20 2d20 646f 6378 2070  rties__ - docx p
+00000e90: 726f 7065 7274 7920 6e61 6d65 7320 6d61  roperty names ma
+00000ea0: 7070 6564 2074 6f20 7661 6c75 6573 2028  pped to values (
+00000eb0: 652e 672e 2c20 607b 226c 6173 744d 6f64  e.g., `{"lastMod
+00000ec0: 6966 6965 6442 7922 3a20 2253 6861 7920  ifiedBy": "Shay 
+00000ed0: 4869 6c6c 227d 6029 0a0a 5f5f 696d 6167  Hill"}`)..__imag
+00000ee0: 6573 5f5f 202d 2069 6d61 6765 206e 616d  es__ - image nam
+00000ef0: 6573 206d 6170 7065 6420 746f 2069 6d61  es mapped to ima
+00000f00: 6765 7320 696e 2062 696e 6172 7920 666f  ges in binary fo
+00000f10: 726d 6174 2e20 5772 6974 6520 746f 2066  rmat. Write to f
+00000f20: 696c 6573 7973 7465 6d20 7769 7468 0a0a  ilesystem with..
+00000f30: 6060 600a 666f 7220 6e61 6d65 2c20 696d  ```.for name, im
+00000f40: 6167 6520 696e 2072 6573 756c 742e 696d  age in result.im
+00000f50: 6167 6573 2e69 7465 6d73 2829 3a0a 2020  ages.items():.  
+00000f60: 2020 7769 7468 206f 7065 6e28 6e61 6d65    with open(name
+00000f70: 2c20 2777 6227 2920 6173 2069 6d61 6765  , 'wb') as image
+00000f80: 5f64 6573 7469 6e61 7469 6f6e 3a0a 2020  _destination:.  
+00000f90: 2020 2020 2020 7772 6974 6528 696d 6167        write(imag
+00000fa0: 655f 6465 7374 696e 6174 696f 6e2c 2069  e_destination, i
+00000fb0: 6d61 6765 290a 0a23 206f 720a 0a77 6974  mage)..# or..wit
+00000fc0: 6820 646f 6378 3270 7974 686f 6e28 2770  h docx2python('p
+00000fd0: 6174 682f 746f 2f66 696c 652e 646f 6378  ath/to/file.docx
+00000fe0: 272c 2027 7061 7468 2f74 6f2f 696d 6167  ', 'path/to/imag
+00000ff0: 652f 6469 7265 6374 6f72 7927 2920 6173  e/directory') as
+00001000: 2064 6f63 785f 636f 6e74 656e 743a 0a20   docx_content:. 
+00001010: 2020 202e 2e2e 0a0a 2320 6f72 0a0a 7769     .....# or..wi
+00001020: 7468 2064 6f63 7832 7079 7468 6f6e 2827  th docx2python('
+00001030: 7061 7468 2f74 6f2f 6669 6c65 2e64 6f63  path/to/file.doc
+00001040: 7827 2920 6173 2064 6f63 785f 636f 6e74  x') as docx_cont
+00001050: 656e 743a 0a20 2020 2064 6f63 785f 636f  ent:.    docx_co
+00001060: 6e74 656e 742e 7361 7665 5f69 6d61 6765  ntent.save_image
+00001070: 7328 2770 6174 682f 746f 2f69 6d61 6765  s('path/to/image
+00001080: 2f64 6972 6563 746f 7279 2729 0a0a 6060  /directory')..``
+00001090: 600a 0a5f 5f64 6f63 785f 7265 6164 6572  `..__docx_reader
+000010a0: 5f5f 202d 2061 2044 6f63 7852 6561 6465  __ - a DocxReade
+000010b0: 7220 2873 6565 2060 646f 6378 5f72 6561  r (see `docx_rea
+000010c0: 6465 722e 7079 6029 2069 6e73 7461 6e63  der.py`) instanc
+000010d0: 6520 7769 7468 2073 6576 6572 616c 206d  e with several m
+000010e0: 6574 686f 6473 2066 6f72 2065 7874 7261  ethods for extra
+000010f0: 6374 696e 6720 786d 6c20 706f 7274 696f  cting xml portio
+00001100: 6e73 2e0a 0a0a 2323 2041 7267 756d 656e  ns....## Argumen
+00001110: 7473 0a0a 2020 2020 6465 6620 646f 6378  ts..    def docx
+00001120: 3270 7974 686f 6e28 0a20 2020 2020 2020  2python(.       
+00001130: 2064 6f63 785f 6669 6c65 6e61 6d65 3a20   docx_filename: 
+00001140: 7374 7220 7c20 5061 7468 207c 2042 7974  str | Path | Byt
+00001150: 6573 494f 2c0a 2020 2020 2020 2020 696d  esIO,.        im
+00001160: 6167 655f 666f 6c64 6572 3a20 7374 7220  age_folder: str 
+00001170: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
+00001180: 2020 2020 2020 2068 746d 6c3a 2062 6f6f         html: boo
+00001190: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+000011a0: 2020 2070 6172 6167 7261 7068 5f73 7479     paragraph_sty
+000011b0: 6c65 733a 2062 6f6f 6c20 3d20 4661 6c73  les: bool = Fals
+000011c0: 652c 0a20 2020 2020 2020 2065 7874 7261  e,.        extra
+000011d0: 6374 5f69 6d61 6765 3a20 626f 6f6c 207c  ct_image: bool |
+000011e0: 204e 6f6e 6520 3d20 4e6f 6e65 2c0a 2020   None = None,.  
+000011f0: 2020 2020 2020 6475 706c 6963 6174 655f        duplicate_
+00001200: 6d65 7267 6564 5f63 656c 6c73 3a20 626f  merged_cells: bo
+00001210: 6f6c 203d 2046 616c 7365 0a20 2020 2029  ol = False.    )
+00001220: 202d 3e20 446f 6378 436f 6e74 656e 743a   -> DocxContent:
+00001230: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00001240: 2020 2020 2055 6e7a 6970 2061 2064 6f63       Unzip a doc
+00001250: 7820 6669 6c65 2061 6e64 2065 7874 7261  x file and extra
+00001260: 6374 2063 6f6e 7465 6e74 732e 0a0a 2020  ct contents...  
+00001270: 2020 2020 2020 3a70 6172 616d 2064 6f63        :param doc
+00001280: 785f 6669 6c65 6e61 6d65 3a20 7061 7468  x_filename: path
+00001290: 2074 6f20 6120 646f 6378 2066 696c 650a   to a docx file.
+000012a0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+000012b0: 6d61 6765 5f66 6f6c 6465 723a 206f 7074  mage_folder: opt
+000012c0: 696f 6e61 6c6c 7920 7370 6563 6966 7920  ionally specify 
+000012d0: 616e 2069 6d61 6765 2066 6f6c 6465 720a  an image folder.
+000012e0: 2020 2020 2020 2020 2020 2020 2869 6d61              (ima
+000012f0: 6765 7320 696e 2064 6f63 7820 7769 6c6c  ges in docx will
+00001300: 2062 6520 636f 7069 6564 2074 6f20 7468   be copied to th
+00001310: 6973 2066 6f6c 6465 7229 0a20 2020 2020  is folder).     
+00001320: 2020 203a 7061 7261 6d20 6874 6d6c 3a20     :param html: 
+00001330: 626f 6f6c 2c20 6578 7472 6163 7420 736f  bool, extract so
+00001340: 6d65 2066 6f72 6d61 7474 696e 6720 6173  me formatting as
+00001350: 2068 746d 6c0a 2020 2020 2020 2020 3a70   html.        :p
+00001360: 6172 616d 2070 6172 6167 7261 7068 5f73  aram paragraph_s
+00001370: 7479 6c65 733a 2070 7265 7065 6e64 2074  tyles: prepend t
+00001380: 6865 2070 6172 6167 7261 7068 7320 7374  he paragraphs st
+00001390: 796c 6520 2869 6620 616e 792c 2065 6c73  yle (if any, els
+000013a0: 6520 2222 2920 746f 2065 6163 680a 2020  e "") to each.  
+000013b0: 2020 2020 2020 2020 2020 7061 7261 6772            paragr
+000013c0: 6170 682e 2054 6869 7320 7769 6c6c 206f  aph. This will o
+000013d0: 6e6c 7920 6265 2075 7365 6675 6c20 7769  nly be useful wi
+000013e0: 7468 2060 602a 5f72 756e 7360 6020 6174  th ``*_runs`` at
+000013f0: 7472 6962 7574 6573 2e0a 2020 2020 2020  tributes..      
+00001400: 2020 3a70 6172 616d 2064 7570 6c69 6361    :param duplica
+00001410: 7465 5f6d 6572 6765 645f 6365 6c6c 733a  te_merged_cells:
+00001420: 2062 6f6f 6c2c 2064 7570 6c69 6361 7465   bool, duplicate
+00001430: 206d 6572 6765 6420 6365 6c6c 7320 746f   merged cells to
+00001440: 2072 6574 7572 6e20 6120 6d78 6e0a 2020   return a mxn.  
+00001450: 2020 2020 2020 2020 2020 6e65 7374 6564            nested
+00001460: 206c 6973 7420 666f 7220 6561 6368 2074   list for each t
+00001470: 6162 6c65 2028 6465 6661 756c 7420 4661  able (default Fa
+00001480: 6c73 6529 0a20 2020 2020 2020 203a 7265  lse).        :re
+00001490: 7475 726e 3a20 446f 6378 436f 6e74 656e  turn: DocxConten
+000014a0: 7420 6f62 6a65 6374 0a20 2020 2020 2020  t object.       
+000014b0: 2022 2222 0a0a 0a23 2320 5265 7475 726e   """...## Return
+000014c0: 2046 6f72 6d61 740a 0a53 6f6d 6520 7374   Format..Some st
+000014d0: 7275 6374 7572 6520 7769 6c6c 2062 6520  ructure will be 
+000014e0: 6d61 696e 7461 696e 6564 2e20 5465 7874  maintained. Text
+000014f0: 2077 696c 6c20 6265 2072 6574 7572 6e65   will be returne
+00001500: 6420 696e 2061 206e 6573 7465 6420 6c69  d in a nested li
+00001510: 7374 2c20 7769 7468 2070 6172 6167 7261  st, with paragra
+00001520: 7068 7320 616c 7761 7973 2061 7420 6465  phs always at de
+00001530: 7074 6820 3420 2869 2e65 2e2c 2060 6f75  pth 4 (i.e., `ou
+00001540: 7470 7574 2e62 6f64 795b 695d 5b6a 5d5b  tput.body[i][j][
+00001550: 6b5d 5b6c 5d60 2077 696c 6c20 6265 2061  k][l]` will be a
+00001560: 2070 6172 6167 7261 7068 292e 0a0a 4966   paragraph)...If
+00001570: 2079 6f75 7220 646f 6378 2068 6173 206e   your docx has n
+00001580: 6f20 7461 626c 6573 2c20 6f75 7470 7574  o tables, output
+00001590: 2e62 6f64 7920 7769 6c6c 2061 7070 6561  .body will appea
+000015a0: 7220 6173 206f 6e65 2061 2074 6162 6c65  r as one a table
+000015b0: 2077 6974 6820 616c 6c20 636f 6e74 656e   with all conten
+000015c0: 7420 696e 206f 6e65 2063 656c 6c3a 0a0a  t in one cell:..
+000015d0: 6060 6070 7974 686f 6e0a 5b20 2023 2064  ```python.[  # d
+000015e0: 6f63 756d 656e 740a 2020 2020 5b20 2023  ocument.    [  #
+000015f0: 2074 6162 6c65 0a20 2020 2020 2020 205b   table.        [
+00001600: 2020 2320 726f 770a 2020 2020 2020 2020    # row.        
+00001610: 2020 2020 5b20 2023 2063 656c 6c0a 2020      [  # cell.  
+00001620: 2020 2020 2020 2020 2020 2020 2020 2250                "P
+00001630: 6172 6167 7261 7068 2031 222c 0a20 2020  aragraph 1",.   
+00001640: 2020 2020 2020 2020 2020 2020 2022 5061               "Pa
+00001650: 7261 6772 6170 6820 3222 2c0a 2020 2020  ragraph 2",.    
+00001660: 2020 2020 2020 2020 2020 2020 222d 2d20              "-- 
+00001670: 6275 6c6c 6574 6564 206c 6973 7422 2c0a  bulleted list",.
+00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001690: 222d 2d20 636f 6e74 696e 7569 6e67 2062  "-- continuing b
+000016a0: 756c 6c65 7465 6420 6c69 7374 222c 0a20  ulleted list",. 
+000016b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000016c0: 3129 2020 6e75 6d62 6572 6564 206c 6973  1)  numbered lis
+000016d0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+000016e0: 2020 2020 2232 2920 2063 6f6e 7469 6e75      "2)  continu
+000016f0: 696e 6720 6e75 6d62 6572 6564 206c 6973  ing numbered lis
+00001700: 7422 0a20 2020 2020 2020 2020 2020 2020  t".             
+00001710: 2020 2022 2020 2020 6129 2020 7375 626c     "    a)  subl
+00001720: 6973 7422 2c0a 2020 2020 2020 2020 2020  ist",.          
+00001730: 2020 2020 2020 2220 2020 2020 2020 2069        "        i
+00001740: 2920 2073 7562 6c69 7374 206f 6620 7375  )  sublist of su
+00001750: 626c 6973 7422 2c0a 2020 2020 2020 2020  blist",.        
+00001760: 2020 2020 2020 2020 2233 2920 206b 6565          "3)  kee
+00001770: 7073 2074 7261 636b 206f 6620 696e 6465  ps track of inde
+00001780: 6e74 696f 6e20 6c65 7665 6c73 222c 0a20  ntion levels",. 
+00001790: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000017a0: 2020 2020 6129 2020 7265 7365 7473 2073      a)  resets s
+000017b0: 7562 6c69 7374 2063 6f75 6e74 6572 7322  ublist counters"
+000017c0: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+000017d0: 2020 2020 2020 205d 0a20 2020 2020 5d0a         ].     ].
+000017e0: 205d 0a60 6060 0a0a 5461 626c 6520 6365   ].```..Table ce
+000017f0: 6c6c 7320 7769 6c6c 2061 7070 6561 7220  lls will appear 
+00001800: 6173 2074 6162 6c65 2063 656c 6c73 2e20  as table cells. 
+00001810: 5465 7874 206f 7574 7369 6465 2074 6162  Text outside tab
+00001820: 6c65 7320 7769 6c6c 2061 7070 6561 7220  les will appear 
+00001830: 6173 2074 6162 6c65 2063 656c 6c73 2e0a  as table cells..
+00001840: 0a0a 4120 646f 6378 2064 6f63 756d 656e  ..A docx documen
+00001850: 7420 6361 6e20 6265 2074 6162 6c65 7320  t can be tables 
+00001860: 7769 7468 696e 2074 6162 6c65 7320 7769  within tables wi
+00001870: 7468 696e 2074 6162 6c65 732e 2044 6f63  thin tables. Doc
+00001880: 7832 5079 7468 6f6e 2066 6c61 7474 656e  x2Python flatten
+00001890: 7320 6d6f 7374 206f 6620 7468 6973 2074  s most of this t
+000018a0: 6f20 6d6f 7265 2065 6173 696c 7920 6e61  o more easily na
+000018b0: 7669 6761 7465 0a77 6974 6869 6e20 7468  vigate.within th
+000018c0: 6520 636f 6e74 656e 742e 0a0a 2323 2057  e content...## W
+000018d0: 6f72 6b69 6e67 2077 6974 6820 6f75 7470  orking with outp
+000018e0: 7574 0a0a 5468 6973 2070 6163 6b61 6765  ut..This package
+000018f0: 2070 726f 7669 6465 7320 7365 7665 7261   provides severa
+00001900: 6c20 646f 6375 6d65 6e74 6564 2068 656c  l documented hel
+00001910: 7065 7220 6675 6e63 7469 6f6e 7320 696e  per functions in
+00001920: 205b 7468 6520 6060 646f 6378 3270 7974   [the ``docx2pyt
+00001930: 686f 6e2e 6974 6572 6174 6f72 7360 6020  hon.iterators`` 
+00001940: 6d6f 6475 6c65 5d28 6874 7470 733a 2f2f  module](https://
+00001950: 646f 6378 3270 7974 686f 6e2e 7265 6164  docx2python.read
+00001960: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00001970: 7465 7374 2f64 6f63 7832 7079 7468 6f6e  test/docx2python
+00001980: 2e68 746d 6c23 6d6f 6475 6c65 2d69 7465  .html#module-ite
+00001990: 7261 746f 7273 292e 2048 6572 6520 6172  rators). Here ar
+000019a0: 6520 6120 6665 7720 7265 6369 7065 7320  e a few recipes 
+000019b0: 706f 7373 6962 6c65 2077 6974 6820 7468  possible with th
+000019c0: 6573 6520 6675 6e63 7469 6f6e 733a 0a0a  ese functions:..
+000019d0: 6060 6070 7974 686f 6e0a 6672 6f6d 2064  ```python.from d
+000019e0: 6f63 7832 7079 7468 6f6e 2e69 7465 7261  ocx2python.itera
+000019f0: 746f 7273 2069 6d70 6f72 7420 656e 756d  tors import enum
+00001a00: 5f63 656c 6c73 0a0a 6465 6620 7265 6d6f  _cells..def remo
+00001a10: 7665 5f65 6d70 7479 5f70 6172 6167 7261  ve_empty_paragra
+00001a20: 7068 7328 7461 626c 6573 293a 0a20 2020  phs(tables):.   
+00001a30: 2066 6f72 2028 692c 206a 2c20 6b29 2c20   for (i, j, k), 
+00001a40: 6365 6c6c 2069 6e20 656e 756d 5f63 656c  cell in enum_cel
+00001a50: 6c73 2874 6162 6c65 7329 3a0a 2020 2020  ls(tables):.    
+00001a60: 2020 2020 7461 626c 6573 5b69 5d5b 6a5d      tables[i][j]
+00001a70: 5b6b 5d20 3d20 5b78 2066 6f72 2078 2069  [k] = [x for x i
+00001a80: 6e20 6365 6c6c 2069 6620 785d 0a60 6060  n cell if x].```
+00001a90: 0a0a 6060 600a 3e3e 3e20 7461 626c 6573  ..```.>>> tables
+00001aa0: 203d 205b 5b5b 5b27 6127 2c20 2762 275d   = [[[['a', 'b']
+00001ab0: 2c20 5b27 6127 2c20 2727 2c20 2764 272c  , ['a', '', 'd',
+00001ac0: 2027 275d 5d5d 5d0a 3e3e 3e20 7265 6d6f   '']]]].>>> remo
+00001ad0: 7665 5f65 6d70 7479 5f70 6172 6167 7261  ve_empty_paragra
+00001ae0: 7068 7328 7461 626c 6573 290a 2020 2020  phs(tables).    
+00001af0: 5b5b 5b5b 2761 272c 2027 6227 5d2c 205b  [[[['a', 'b'], [
+00001b00: 2761 272c 2027 6427 5d5d 5d5d 0a60 6060  'a', 'd']]]].```
+00001b10: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
+00001b20: 2064 6f63 7832 7079 7468 6f6e 2e69 7465   docx2python.ite
+00001b30: 7261 746f 7273 2069 6d70 6f72 7420 656e  rators import en
+00001b40: 756d 5f61 745f 6465 7074 680a 0a64 6566  um_at_depth..def
+00001b50: 2068 746d 6c5f 6d61 7028 7461 626c 6573   html_map(tables
+00001b60: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
+00001b70: 2243 7265 6174 6520 616e 2048 544d 4c20  "Create an HTML 
+00001b80: 6d61 7020 6f66 2064 6f63 756d 656e 7420  map of document 
+00001b90: 636f 6e74 656e 7473 2e0a 0a20 2020 2052  contents...    R
+00001ba0: 656e 6465 7220 7468 6973 2069 6e20 6120  ender this in a 
+00001bb0: 6272 6f77 7365 7220 746f 2076 6973 7561  browser to visua
+00001bc0: 6c6c 7920 7365 6172 6368 2066 6f72 2064  lly search for d
+00001bd0: 6174 612e 0a0a 2020 2020 3a74 6162 6c65  ata...    :table
+00001be0: 733a 2076 616c 7565 2063 6f75 6c64 2063  s: value could c
+00001bf0: 6f6d 6520 6672 6f6d 2c20 652e 672e 2c0a  ome from, e.g.,.
+00001c00: 2020 2020 2020 2020 2a20 646f 6378 5f74          * docx_t
+00001c10: 6f5f 7465 7874 5f6f 7574 7075 742e 646f  o_text_output.do
+00001c20: 6375 6d65 6e74 0a20 2020 2020 2020 202a  cument.        *
+00001c30: 2064 6f63 785f 746f 5f74 6578 745f 6f75   docx_to_text_ou
+00001c40: 7470 7574 2e62 6f64 790a 2020 2020 2222  tput.body.    ""
+00001c50: 220a 0a20 2020 2023 2070 7265 7065 6e64  "..    # prepend
+00001c60: 2069 6e64 6578 2074 7570 6c65 2074 6f20   index tuple to 
+00001c70: 6561 6368 2070 6172 6167 7261 7068 0a20  each paragraph. 
+00001c80: 2020 2066 6f72 2028 692c 206a 2c20 6b2c     for (i, j, k,
+00001c90: 206c 292c 2070 6172 6167 7261 7068 2069   l), paragraph i
+00001ca0: 6e20 656e 756d 5f61 745f 6465 7074 6828  n enum_at_depth(
+00001cb0: 7461 626c 6573 2c20 3429 3a0a 2020 2020  tables, 4):.    
+00001cc0: 2020 2020 7461 626c 6573 5b69 5d5b 6a5d      tables[i][j]
+00001cd0: 5b6b 5d5b 6c5d 203d 2022 2022 2e6a 6f69  [k][l] = " ".joi
+00001ce0: 6e28 5b73 7472 2828 692c 206a 2c20 6b2c  n([str((i, j, k,
+00001cf0: 206c 2929 2c20 7061 7261 6772 6170 685d   l)), paragraph]
+00001d00: 290a 0a20 2020 2023 2077 7261 7020 6561  )..    # wrap ea
+00001d10: 6368 2070 6172 6167 7261 7068 2069 6e20  ch paragraph in 
+00001d20: 3c70 7265 3e20 7461 6773 0a20 2020 2066  <pre> tags.    f
+00001d30: 6f72 2028 692c 206a 2c20 6b29 2c20 6365  or (i, j, k), ce
+00001d40: 6c6c 2069 6e20 656e 756d 5f61 745f 6465  ll in enum_at_de
+00001d50: 7074 6828 7461 626c 6573 2c20 3329 3a0a  pth(tables, 3):.
+00001d60: 2020 2020 2020 2020 7461 626c 6573 5b69          tables[i
+00001d70: 5d5b 6a5d 5b6b 5d20 3d20 2222 2e6a 6f69  ][j][k] = "".joi
+00001d80: 6e28 5b22 3c70 7265 3e7b 787d 3c2f 7072  n(["<pre>{x}</pr
+00001d90: 653e 222e 666f 726d 6174 2878 2920 666f  e>".format(x) fo
+00001da0: 7220 7820 696e 2063 656c 6c5d 290a 0a20  r x in cell]).. 
+00001db0: 2020 2023 2077 7261 7020 6561 6368 2063     # wrap each c
+00001dc0: 656c 6c20 696e 203c 7464 3e20 7461 6773  ell in <td> tags
+00001dd0: 0a20 2020 2066 6f72 2028 692c 206a 292c  .    for (i, j),
+00001de0: 2072 6f77 2069 6e20 656e 756d 5f61 745f   row in enum_at_
+00001df0: 6465 7074 6828 7461 626c 6573 2c20 3229  depth(tables, 2)
+00001e00: 3a0a 2020 2020 2020 2020 7461 626c 6573  :.        tables
+00001e10: 5b69 5d5b 6a5d 203d 2022 222e 6a6f 696e  [i][j] = "".join
+00001e20: 285b 223c 7464 3e7b 787d 3c2f 7464 3e22  (["<td>{x}</td>"
+00001e30: 2e66 6f72 6d61 7428 7829 2066 6f72 2078  .format(x) for x
+00001e40: 2069 6e20 726f 775d 290a 0a20 2020 2023   in row])..    #
+00001e50: 2077 7261 7020 6561 6368 2072 6f77 2069   wrap each row i
+00001e60: 6e20 3c74 723e 2074 6167 730a 2020 2020  n <tr> tags.    
+00001e70: 666f 7220 2869 2c29 2c20 7461 626c 6520  for (i,), table 
+00001e80: 696e 2065 6e75 6d5f 6174 5f64 6570 7468  in enum_at_depth
+00001e90: 2874 6162 6c65 732c 2031 293a 0a20 2020  (tables, 1):.   
+00001ea0: 2020 2020 2074 6162 6c65 735b 695d 203d       tables[i] =
+00001eb0: 2022 222e 6a6f 696e 2822 3c74 723e 7b78   "".join("<tr>{x
+00001ec0: 7d3c 2f74 723e 222e 666f 726d 6174 2878  }</tr>".format(x
+00001ed0: 2920 666f 7220 7820 696e 2074 6162 6c65  ) for x in table
+00001ee0: 290a 0a20 2020 2023 2077 7261 7020 6561  )..    # wrap ea
+00001ef0: 6368 2074 6162 6c65 2069 6e20 3c74 6162  ch table in <tab
+00001f00: 6c65 3e20 7461 6773 0a20 2020 2074 6162  le> tags.    tab
+00001f10: 6c65 7320 3d20 2222 2e6a 6f69 6e28 5b27  les = "".join(['
+00001f20: 3c74 6162 6c65 2062 6f72 6465 723d 2231  <table border="1
+00001f30: 223e 7b78 7d3c 2f74 6162 6c65 3e27 2e66  ">{x}</table>'.f
+00001f40: 6f72 6d61 7428 7829 2066 6f72 2078 2069  ormat(x) for x i
+00001f50: 6e20 7461 626c 6573 5d29 0a0a 2020 2020  n tables])..    
+00001f60: 7265 7475 726e 205b 223c 6874 6d6c 3e3c  return ["<html><
+00001f70: 626f 6479 3e22 5d20 2b20 7461 626c 6573  body>"] + tables
+00001f80: 202b 205b 223c 2f62 6f64 793e 3c2f 6874   + ["</body></ht
+00001f90: 6d6c 3e22 5d0a 6060 600a 0a60 6060 0a3e  ml>"].```..```.>
+00001fa0: 3e3e 2074 6162 6c65 7320 3d20 5b5b 5b5b  >> tables = [[[[
+00001fb0: 2761 272c 2027 6227 5d2c 205b 2761 272c  'a', 'b'], ['a',
+00001fc0: 2027 6427 5d5d 5d5d 0a3e 3e3e 2068 746d   'd']]]].>>> htm
+00001fd0: 6c5f 6d61 7028 7461 626c 6573 290a 3c68  l_map(tables).<h
+00001fe0: 746d 6c3e 0a20 2020 203c 626f 6479 3e0a  tml>.    <body>.
+00001ff0: 2020 2020 2020 2020 3c74 6162 6c65 2062          <table b
+00002000: 6f72 6465 723d 2231 223e 0a20 2020 2020  order="1">.     
+00002010: 2020 2020 2020 203c 7472 3e0a 2020 2020         <tr>.    
+00002020: 2020 2020 2020 2020 2020 2020 3c74 643e              <td>
+00002030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002040: 2020 2020 2027 2830 2c20 302c 2030 2c20       '(0, 0, 0, 
+00002050: 3029 2061 270a 2020 2020 2020 2020 2020  0) a'.          
+00002060: 2020 2020 2020 2020 2020 2728 302c 2030            '(0, 0
+00002070: 2c20 302c 2031 2920 6227 0a20 2020 2020  , 0, 1) b'.     
+00002080: 2020 2020 2020 2020 2020 203c 2f74 643e             </td>
+00002090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000020a0: 203c 7464 3e0a 2020 2020 2020 2020 2020   <td>.          
+000020b0: 2020 2020 2020 2020 2020 2728 302c 2030            '(0, 0
+000020c0: 2c20 312c 2030 2920 6127 0a20 2020 2020  , 1, 0) a'.     
+000020d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000020e0: 2830 2c20 302c 2031 2c20 3129 2064 270a  (0, 0, 1, 1) d'.
+000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002100: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+00002110: 2020 3c2f 7472 3e0a 2020 2020 2020 2020    </tr>.        
+00002120: 3c2f 7461 626c 653e 0a20 2020 203c 2f62  </table>.    </b
+00002130: 6f64 793e 0a3c 2f68 746d 6c3e 0a60 6060  ody>.</html>.```
+00002140: 0a0a 5b53 6565 2068 656c 7065 7220 6675  ..[See helper fu
+00002150: 6e63 7469 6f6e 732e 5d28 6874 7470 733a  nctions.](https:
+00002160: 2f2f 646f 6378 3270 7974 686f 6e2e 7265  //docx2python.re
+00002170: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00002180: 6c61 7465 7374 2f69 6e64 6578 2e68 746d  latest/index.htm
+00002190: 6c29 0a0a 536f 6d65 2066 696e 6520 7072  l)..Some fine pr
+000021a0: 696e 7420 6162 6f75 7420 6368 6563 6b62  int about checkb
+000021b0: 6f78 6573 3a0a 0a4d 5320 576f 7264 2068  oxes:..MS Word h
+000021c0: 6173 2063 6865 636b 626f 7865 7320 7468  as checkboxes th
+000021d0: 6174 2063 616e 2062 6520 6368 6563 6b65  at can be checke
+000021e0: 6420 616e 7920 7469 6d65 2c20 616e 6420  d any time, and 
+000021f0: 6f74 6865 7273 2074 6861 7420 6361 6e20  others that can 
+00002200: 6f6e 6c79 2062 6520 6368 6563 6b65 6420  only be checked 
+00002210: 7768 656e 2074 6865 2066 6f72 6d20 6973  when the form is
+00002220: 206c 6f63 6b65 642e 0a54 6865 2070 7265   locked..The pre
+00002230: 7669 6f75 7320 7072 696e 7420 6173 2e20  vious print as. 
+00002240: 6060 5c75 3236 3130 6060 2028 6f70 656e  ``\u2610`` (open
+00002250: 2063 6865 636b 626f 7829 206f 7220 6060   checkbox) or ``
+00002260: 5c75 3236 3132 6060 2028 6372 6f73 7365  \u2612`` (crosse
+00002270: 6420 6368 6563 6b62 6f78 292e 2057 6869  d checkbox). Whi
+00002280: 6368 2074 6869 7320 6d6f 6475 6c65 2c20  ch this module, 
+00002290: 7468 6520 6c61 7474 6572 2077 696c 6c0a  the latter will.
+000022a0: 746f 6f2e 2049 2067 6176 6520 6368 6563  too. I gave chec
+000022b0: 6b62 6f78 6573 2061 2062 6169 6c6f 7574  kboxes a bailout
+000022c0: 2076 616c 7565 206f 6620 6060 2d2d 2d2d   value of ``----
+000022d0: 6368 6563 6b62 6f78 2066 6169 6c65 642d  checkbox failed-
+000022e0: 2d2d 2d60 6020 6966 2074 6865 2078 6d6c  ---`` if the xml
+000022f0: 2064 6f65 736e 2774 206c 6f6f 6b20 6c69   doesn't look li
+00002300: 6b65 2049 2065 7870 6563 7420 6974 2074  ke I expect it t
+00002310: 6f2c 0a62 6563 6175 7365 2049 2064 6f6e  o,.because I don
+00002320: 2774 2068 6176 6520 7365 7665 7261 6c2d  't have several-
+00002330: 7468 6f75 7361 6e64 2074 6573 7420 6669  thousand test fi
+00002340: 6c65 7320 7769 7468 2063 6865 636b 626f  les with checkbo
+00002350: 7865 7320 2861 7320 4920 6469 6420 7769  xes (as I did wi
+00002360: 7468 206d 6f73 7420 6f66 2074 6865 206f  th most of the o
+00002370: 7468 6572 2066 6f72 6d20 656c 656d 656e  ther form elemen
+00002380: 7473 292e 0a43 6865 636b 626f 7865 7320  ts)..Checkboxes 
+00002390: 2a73 686f 756c 642a 2077 6f72 6b2c 2062  *should* work, b
+000023a0: 7574 2070 6c65 6173 6520 6c65 7420 6d65  ut please let me
+000023b0: 206b 6e6f 7720 6966 2079 6f75 2065 6e63   know if you enc
+000023c0: 6f75 6e74 6572 2061 6e79 2074 6861 7420  ounter any that 
+000023d0: 646f 206e 6f74 2e0a 0a23 204e 6577 2069  do not...# New i
+000023e0: 6e20 646f 6378 3270 7974 686f 6e20 5665  n docx2python Ve
+000023f0: 7273 696f 6e20 320a 0a23 2320 6d65 7267  rsion 2..## merg
+00002400: 6520 636f 6e73 6563 7574 6976 6520 7275  e consecutive ru
+00002410: 6e73 2077 6974 6820 6964 656e 7469 6361  ns with identica
+00002420: 6c20 666f 726d 6174 7469 6e67 0a0a 4d53  l formatting..MS
+00002430: 2057 6f72 6420 7769 6c6c 2062 7265 616b   Word will break
+00002440: 2075 7020 7465 7874 2072 756e 7320 6172   up text runs ar
+00002450: 6269 7472 6172 696c 792c 206f 6674 656e  bitrarily, often
+00002460: 2069 6e20 7468 6520 6d69 6464 6c65 206f   in the middle o
+00002470: 6620 6120 776f 7264 2e0a 0a0a 2020 2020  f a word....    
+00002480: 3c77 3a72 3e0a 2020 2020 2020 2020 3c77  <w:r>.        <w
+00002490: 3a74 3e77 6f72 6b20 746f 2069 6d3c 2f77  :t>work to im</w
+000024a0: 3a74 3e0a 2020 2020 3c2f 773a 723e 0a20  :t>.    </w:r>. 
+000024b0: 2020 203c 773a 723e 0a20 2020 2020 2020     <w:r>.       
+000024c0: 203c 773a 743e 7072 6f76 6520 646f 6378   <w:t>prove docx
+000024d0: 3270 7974 686f 6e3c 2f77 3a74 3e0a 2020  2python</w:t>.  
+000024e0: 2020 3c2f 773a 723e 0a0a 5468 6973 206d    </w:r>..This m
+000024f0: 616b 6573 2074 6869 6e67 7320 6c69 6b65  akes things like
+00002500: 2061 6c67 6f72 6974 686d 6963 2073 6561   algorithmic sea
+00002510: 7263 682d 616e 642d 7265 706c 6163 6520  rch-and-replace 
+00002520: 7072 6f62 6c65 6d61 7469 632e 2044 6f63  problematic. Doc
+00002530: 7832 7079 7468 6f6e 2064 6f65 7320 6e6f  x2python does no
+00002540: 7420 6375 7272 656e 746c 7920 7772 6974  t currently writ
+00002550: 6520 646f 6378 2066 696c 6573 2c0a 6275  e docx files,.bu
+00002560: 7420 4920 6f66 7465 6e20 7573 6520 646f  t I often use do
+00002570: 6378 2074 656d 706c 6174 6573 2077 6974  cx templates wit
+00002580: 6820 706c 6163 6568 6f6c 6465 7273 2028  h placeholders (
+00002590: 652e 672e 2c20 6023 4341 5445 474f 5259  e.g., `#CATEGORY
+000025a0: 5f4e 414d 4523 6029 2074 6865 6e20 7265  _NAME#`) then re
+000025b0: 706c 6163 6520 7468 6f73 6520 706c 6163  place those plac
+000025c0: 6568 6f6c 6465 7273 2077 6974 6820 6461  eholders with da
+000025d0: 7461 2e0a 5468 6973 2077 6f6e 2774 2077  ta..This won't w
+000025e0: 6f72 6b20 6966 2079 6f75 7220 706c 6163  ork if your plac
+000025f0: 6568 6f6c 6465 7273 2061 7265 2062 726f  eholders are bro
+00002600: 6b65 6e20 7570 2028 652e 672c 2060 2343  ken up (e.g, `#C
+00002610: 4154 602c 2060 4560 2c20 6047 4f52 595f  AT`, `E`, `GORY_
+00002620: 4e41 4d45 2360 292e 0a0a 446f 6378 3270  NAME#`)...Docx2p
+00002630: 7974 686f 6e20 7631 206d 6572 6765 7320  ython v1 merges 
+00002640: 7375 6368 2072 756e 7320 746f 6765 7468  such runs togeth
+00002650: 6572 2077 6865 6e20 6578 706f 7274 696e  er when exportin
+00002660: 6720 7465 7874 2e20 446f 6378 3270 7974  g text. Docx2pyt
+00002670: 686f 6e20 7632 2077 696c 6c20 6d65 7267  hon v2 will merg
+00002680: 6520 7375 6368 2072 756e 7320 696e 2074  e such runs in t
+00002690: 6865 2058 4d4c 2061 7320 610a 7072 652d  he XML as a.pre-
+000026a0: 7072 6f63 6573 7369 6e67 2073 7465 702e  processing step.
+000026b0: 2054 6869 7320 7769 6c6c 2061 6c6c 6f77   This will allow
+000026c0: 2073 6176 696e 6720 7375 6368 2022 7265   saving such "re
+000026d0: 7061 6972 6564 2220 584d 4c20 6c61 7465  paired" XML late
+000026e0: 7220 6f6e 2e0a 0a23 2320 6d65 7267 6520  r on...## merge 
+000026f0: 636f 6e73 6563 7574 6976 6520 6c69 6e6b  consecutive link
+00002700: 7320 7769 7468 2069 6465 6e74 6963 616c  s with identical
+00002710: 2068 7265 6673 0a0a 4d53 2057 6f72 6420   hrefs..MS Word 
+00002720: 7769 6c6c 2062 7265 616b 2075 7020 6c69  will break up li
+00002730: 6e6b 732c 2067 6976 696e 6720 6561 6368  nks, giving each
+00002740: 206c 696e 6b20 6120 6469 6666 6572 656e   link a differen
+00002750: 7420 6072 4964 602c 2065 7665 6e20 7768  t `rId`, even wh
+00002760: 656e 2074 6865 7365 2060 7249 6473 6020  en these `rIds` 
+00002770: 706f 696e 7420 746f 2074 6865 2073 616d  point to the sam
+00002780: 6520 6164 6472 6573 732e 0a0a 2020 2020  e address...    
+00002790: 3c77 3a68 7970 6572 6c69 6e6b 2072 3a69  <w:hyperlink r:i
+000027a0: 643d 2272 4964 3133 223e 2020 2320 7249  d="rId13">  # rI
+000027b0: 4431 3320 706f 696e 7473 2074 6f20 6874  D13 points to ht
+000027c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000027d0: 2f53 6861 7948 696c 6c2f 646f 6378 3270  /ShayHill/docx2p
+000027e0: 7974 686f 6e0a 2020 2020 2020 2020 3c77  ython.        <w
+000027f0: 3a72 3e0a 2020 2020 2020 2020 2020 2020  :r>.            
+00002800: 3c77 3a74 3e64 6f63 7832 7079 3c2f 773a  <w:t>docx2py</w:
+00002810: 743e 0a20 2020 2020 2020 203c 2f77 3a72  t>.        </w:r
+00002820: 3e0a 2020 2020 3c2f 773a 6879 7065 726c  >.    </w:hyperl
+00002830: 696e 6b3e 0a20 2020 203c 773a 6879 7065  ink>.    <w:hype
+00002840: 726c 696e 6b20 723a 6964 3d22 7249 6431  rlink r:id="rId1
+00002850: 3422 3e20 2023 2072 4944 3134 2041 4c53  4">  # rID14 ALS
+00002860: 4f20 706f 696e 7473 2074 6f20 6874 7470  O points to http
+00002870: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f53  s://github.com/S
+00002880: 6861 7948 696c 6c2f 646f 6378 3270 7974  hayHill/docx2pyt
+00002890: 686f 6e0a 2020 2020 2020 2020 3c77 3a72  hon.        <w:r
+000028a0: 3e0a 2020 2020 2020 2020 2020 2020 3c77  >.            <w
+000028b0: 3a74 3e74 686f 6e3c 2f77 3a74 3e0a 2020  :t>thon</w:t>.  
+000028c0: 2020 2020 2020 3c2f 773a 723e 0a20 2020        </w:r>.   
+000028d0: 203c 2f77 3a68 7970 6572 6c69 6e6b 3e0a   </w:hyperlink>.
+000028e0: 0a54 6869 7320 6973 2073 696d 696c 6172  .This is similar
+000028f0: 2074 6f20 7468 6520 6272 6f6b 656e 2d75   to the broken-u
+00002900: 7020 7275 6e73 2c20 6275 7420 7468 6520  p runs, but the 
+00002910: 6361 7573 6520 6973 2061 206c 6974 746c  cause is a littl
+00002920: 6520 6465 6570 6572 2069 6e2e 2044 6f63  e deeper in. Doc
+00002930: 7832 7079 7468 6f6e 2076 3120 6d61 6b65  x2python v1 make
+00002940: 7320 6120 6d65 7373 206f 6620 7468 6573  s a mess of thes
+00002950: 652e 0a0a 2020 2020 3c61 2068 7265 663d  e...    <a href=
+00002960: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00002970: 636f 6d2f 5368 6179 4869 6c6c 2f64 6f63  com/ShayHill/doc
+00002980: 7832 7079 7468 6f6e 223e 646f 6378 3270  x2python">docx2p
+00002990: 793c 2f61 3e0a 2020 2020 3c61 2068 7265  y</a>.    <a hre
+000029a0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
+000029b0: 622e 636f 6d2f 5368 6179 4869 6c6c 2f64  b.com/ShayHill/d
+000029c0: 6f63 7832 7079 7468 6f6e 223e 7468 6f6e  ocx2python">thon
+000029d0: 3c2f 613e 0a0a 446f 6378 3270 7974 686f  </a>..Docx2pytho
+000029e0: 6e20 7632 2077 696c 6c20 6d65 7267 6520  n v2 will merge 
+000029f0: 7375 6368 206c 696e 6b73 2074 6f67 6574  such links toget
+00002a00: 6865 7220 696e 2074 6865 2058 4d4c 2061  her in the XML a
+00002a10: 7320 6120 7072 652d 7072 6f63 6573 7369  s a pre-processi
+00002a20: 6e67 2073 7465 702e 2041 7320 6162 6f76  ng step. As abov
+00002a30: 652c 2074 6869 7320 7769 6c6c 2061 6c6c  e, this will all
+00002a40: 6f77 2073 6176 696e 670a 7375 6368 2022  ow saving.such "
+00002a50: 7265 7061 6972 6564 2220 584d 4c20 6c61  repaired" XML la
+00002a60: 7465 7220 6f6e 2e0a 0a23 2320 636f 7272  ter on...## corr
+00002a70: 6563 746c 7920 6861 6e64 6c65 206e 6573  ectly handle nes
+00002a80: 7465 6420 7061 7261 6772 6170 6873 0a0a  ted paragraphs..
+00002a90: 4d53 2057 6f72 6420 7769 6c6c 206e 6573  MS Word will nes
+00002aa0: 7420 7061 7261 6772 6170 6873 0a0a 2020  t paragraphs..  
+00002ab0: 2020 3c77 3a70 3e0a 2020 2020 2020 2020    <w:p>.        
+00002ac0: 3c77 3a72 3e0a 2020 2020 2020 2020 2020  <w:r>.          
+00002ad0: 2020 3c77 3a74 3e74 6578 743c 2f77 3a74    <w:t>text</w:t
+00002ae0: 3e0a 2020 2020 2020 2020 3c2f 773a 723e  >.        </w:r>
+00002af0: 0a20 2020 2020 2020 203c 773a 703e 2020  .        <w:p>  
+00002b00: 2320 7061 7261 6772 6170 6820 696e 7369  # paragraph insi
+00002b10: 6465 2061 2070 6172 6167 7261 7068 0a20  de a paragraph. 
+00002b20: 2020 2020 2020 2020 2020 203c 773a 723e             <w:r>
+00002b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b40: 203c 773a 743e 7465 7874 3c2f 773a 743e   <w:t>text</w:t>
+00002b50: 0a20 2020 2020 2020 2020 2020 203c 2f77  .            </w
+00002b60: 3a72 3e0a 2020 2020 2020 2020 3c2f 773a  :r>.        </w:
+00002b70: 703e 0a20 2020 2020 2020 203c 773a 723e  p>.        <w:r>
+00002b80: 0a20 2020 2020 2020 2020 2020 203c 773a  .            <w:
+00002b90: 743e 7465 7874 3c2f 773a 743e 0a20 2020  t>text</w:t>.   
+00002ba0: 2020 2020 203c 2f77 3a72 3e0a 2020 2020       </w:r>.    
+00002bb0: 3c2f 773a 703e 0a0a 4920 6861 7665 6e27  </w:p>..I haven'
+00002bc0: 7420 6265 656e 2061 626c 6520 746f 2063  t been able to c
+00002bd0: 7265 6174 6520 7375 6368 2061 2070 6172  reate such a par
+00002be0: 6167 7261 7068 2c20 6275 7420 4927 7665  agraph, but I've
+00002bf0: 2066 6f75 6e64 2061 2066 6577 2066 696c   found a few fil
+00002c00: 6573 2074 6861 7420 6861 7665 2074 6865  es that have the
+00002c10: 6d2e 2044 6f63 7832 7079 686f 6e20 7631  m. Docx2pyhon v1
+00002c20: 2077 696c 6c20 6f6d 6974 0a63 6c6f 7369   will omit.closi
+00002c30: 6e67 2068 746d 6c20 7461 6773 2077 6865  ng html tags whe
+00002c40: 6e20 6120 6e65 7720 7061 7261 6772 6170  n a new paragrap
+00002c50: 6820 6973 206f 7065 6e65 6420 6265 666f  h is opened befo
+00002c60: 7265 2074 6865 206f 6c64 2070 6172 6167  re the old parag
+00002c70: 7261 7068 2069 7320 636c 6f73 6564 2e0a  raph is closed..
+00002c80: 0a20 2020 203c 623e 6f75 7465 7220 7061  .    <b>outer pa
+00002c90: 7220 626f 6c64 2074 6578 740a 0a20 2020  r bold text..   
+00002ca0: 203c 693e 5468 6973 2074 6578 7420 6973   <i>This text is
+00002cb0: 2069 6e20 6e65 7374 6564 2070 6172 2028   in nested par (
+00002cc0: 6e6f 7420 626f 6c64 293c 2f69 3e0a 0a20  not bold)</i>.. 
+00002cd0: 2020 206f 7574 6572 2070 6172 2062 6f6c     outer par bol
+00002ce0: 6420 7465 7874 3c2f 623e 0a0a 446f 6378  d text</b>..Docx
+00002cf0: 3270 7974 686f 6e20 7632 2077 696c 6c20  2python v2 will 
+00002d00: 636f 7272 6563 746c 7920 6861 6e64 6c65  correctly handle
+00002d10: 2073 7563 6820 6361 7365 732c 2062 7574   such cases, but
+00002d20: 2074 6869 7320 7769 6c6c 2072 6571 7569   this will requi
+00002d30: 7265 2073 7562 7374 616e 7469 616c 2069  re substantial i
+00002d40: 6e74 6572 6e61 6c20 6368 616e 6765 7320  nternal changes 
+00002d50: 746f 2074 6865 2077 6179 0a64 6f63 7832  to the way.docx2
+00002d60: 7079 7468 6f6e 206f 7065 6e73 2061 6e64  python opens and
+00002d70: 2063 6c6f 7365 7320 7061 7261 6772 6170   closes paragrap
+00002d80: 6873 2e0a 0a20 2020 203c 623e 6f75 7465  hs...    <b>oute
+00002d90: 7220 7061 7220 626f 6c64 2074 6578 743c  r par bold text<
+00002da0: 2f62 3e0a 0a20 2020 203c 693e 5468 6973  /b>..    <i>This
+00002db0: 2074 6578 7420 6973 2069 6e20 6e65 7374   text is in nest
+00002dc0: 6564 2070 6172 2028 6e6f 7420 626f 6c64  ed par (not bold
+00002dd0: 293c 2f69 3e0a 0a20 2020 203c 2f62 3e6f  )</i>..    </b>o
+00002de0: 7574 6572 2070 6172 2062 6f6c 6420 7465  uter par bold te
+00002df0: 7874 3c2f 623e 0a0a 2323 2070 6172 6167  xt</b>..## parag
+00002e00: 7261 7068 2073 7479 6c65 730a 0a54 6865  raph styles..The
+00002e10: 2069 6e74 6572 6e61 6c20 6368 616e 6765   internal change
+00002e20: 7320 616c 6c6f 7720 666f 7220 6561 7379  s allow for easy
+00002e30: 2061 6363 6573 7320 746f 2070 6172 6167   access to parag
+00002e40: 7261 7068 2073 7479 6c65 7320 2865 2e67  raph styles (e.g
+00002e50: 2e2c 2060 4865 6164 696e 6720 3160 292e  ., `Heading 1`).
+00002e60: 2044 6f63 7832 7079 7468 6f6e 2076 3120   Docx2python v1 
+00002e70: 6967 6e6f 7265 7320 7468 6573 652c 2065  ignores these, e
+00002e80: 7665 6e0a 7769 7468 2060 6874 6d6c 3d54  ven.with `html=T
+00002e90: 7275 6560 2e20 446f 6378 3270 7974 686f  rue`. Docx2pytho
+00002ea0: 6e20 7632 2077 696c 6c20 6361 7074 7572  n v2 will captur
+00002eb0: 6520 7061 7261 6772 6170 6820 7374 796c  e paragraph styl
+00002ec0: 6573 2e0a 0a20 2020 203c 6831 3e68 3120  es...    <h1>h1 
+00002ed0: 6973 2061 2070 6172 6167 7261 7068 2073  is a paragraph s
+00002ee0: 7479 6c65 3c62 3e62 6f6c 6420 6973 2061  tyle<b>bold is a
+00002ef0: 2072 756e 2073 7479 6c65 3c2f 623e 3c2f   run style</b></
+00002f00: 6831 3e0a 0a23 2320 6578 706f 7274 2078  h1>..## export x
+00002f10: 6d6c 0a0a 546f 2061 6c6c 6f77 2061 626f  ml..To allow abo
+00002f20: 7665 2d64 6573 6372 6962 6564 206c 6967  ve-described lig
+00002f30: 6874 2065 6469 7469 6e67 2028 652e 672e  ht editing (e.g.
+00002f40: 2c20 7365 6172 6368 2061 6e64 2072 6570  , search and rep
+00002f50: 6c61 6365 292c 2064 6f63 7832 7079 7468  lace), docx2pyth
+00002f60: 6f6e 2076 3220 7769 6c6c 2067 6976 6520  on v2 will give 
+00002f70: 7468 6520 7573 6572 2061 6363 6573 7320  the user access 
+00002f80: 746f 0a0a 2020 2020 312e 2065 7874 7261  to..    1. extra
+00002f90: 6374 6564 2078 6d6c 2066 696c 6573 0a20  cted xml files. 
+00002fa0: 2020 2032 2e20 7468 6520 6675 6e63 7469     2. the functi
+00002fb0: 6f6e 7320 7573 6564 2074 6f20 7772 6974  ons used to writ
+00002fc0: 6520 7468 6573 6520 6669 6c65 7320 746f  e these files to
+00002fd0: 2061 2064 6f63 780a 0a54 6865 2075 7365   a docx..The use
+00002fe0: 7220 6361 6e20 6f6e 6c79 2067 6f20 736f  r can only go so
+00002ff0: 2066 6172 2077 6974 6820 7468 6973 2e20   far with this. 
+00003000: 4120 646f 6378 2066 696c 6520 6973 2062  A docx file is b
+00003010: 7569 6c74 2066 726f 6d20 666f 6c64 6572  uilt from folder
+00003020: 7320 6675 6c6c 206f 6620 786d 6c20 6669  s full of xml fi
+00003030: 6c65 732e 204e 6f6e 6520 6f66 2074 6865  les. None of the
+00003040: 7365 2078 6d6c 0a66 696c 6573 2061 7265  se xml.files are
+00003050: 2073 656c 6620 636f 6e74 6169 6e65 642e   self contained.
+00003060: 2042 7574 2073 6561 7263 6820 616e 6420   But search and 
+00003070: 7265 706c 6163 6520 6973 2065 6e6f 7567  replace is enoug
+00003080: 6820 746f 206d 616b 6520 646f 6375 6d65  h to make docume
+00003090: 6e74 2074 656d 706c 6174 6573 2028 646f  nt templates (do
+000030a0: 6375 6d65 6e74 7320 7769 7468 2070 6c61  cuments with pla
+000030b0: 6365 686f 6c64 6572 7320 666f 720a 6461  ceholders for.da
+000030c0: 7461 292c 2061 6e64 2074 6861 7427 7320  ta), and that's 
+000030d0: 7072 6574 7479 2075 7365 6675 6c20 696e  pretty useful in
+000030e0: 2069 7473 656c 662e 0a0a 2323 2065 7870   itself...## exp
+000030f0: 6f73 6520 736f 6d65 2069 6e74 6572 6d65  ose some interme
+00003100: 6469 6174 6520 6675 6e63 7469 6f6e 616c  diate functional
+00003110: 6974 790a 0a4e 6176 6967 6174 696e 6720  ity..Navigating 
+00003120: 7468 726f 7567 6820 584d 4c20 6973 2073  through XML is s
+00003130: 7472 6169 6768 7466 6f72 7761 7264 2077  traightforward w
+00003140: 6974 6820 606c 786d 6c60 2e20 4974 2069  ith `lxml`. It i
+00003150: 7320 6120 7365 7061 7261 7465 2073 7465  s a separate ste
+00003160: 7020 746f 2074 616b 6520 7768 6174 6576  p to take whatev
+00003170: 6572 2079 6f75 2066 696e 6420 616e 6420  er you find and 
+00003180: 6272 696e 6720 6974 0a2a 6f75 742a 206f  bring it.*out* o
+00003190: 6620 7468 6520 584d 4c2e 2046 6f72 2069  f the XML. For i
+000031a0: 6e73 7461 6e63 652c 2079 6f75 206d 6179  nstance, you may
+000031b0: 2077 616e 7420 746f 2069 7465 7261 7465   want to iterate
+000031c0: 206f 7665 7220 6120 646f 6375 6d65 6e74   over a document
+000031d0: 2c20 6c6f 6f6b 696e 6720 666f 7220 7061  , looking for pa
+000031e0: 7261 6772 6170 6873 2077 6974 6820 6120  ragraphs with a 
+000031f0: 7061 7274 6963 756c 6172 0a66 6f72 6d61  particular.forma
+00003200: 742c 2074 6865 6e20 7075 6c6c 2074 6865  t, then pull the
+00003210: 2074 6578 7420 6f75 7420 6f66 2074 686f   text out of tho
+00003220: 7365 2070 6172 6167 7261 7068 732e 2044  se paragraphs. D
+00003230: 6f63 7832 7079 7468 6f6e 2076 3120 6469  ocx2python v1 di
+00003240: 6420 6e6f 7420 7365 7061 7261 7465 206f  d not separate o
+00003250: 7220 6578 706f 7365 2022 6974 6572 2074  r expose "iter t
+00003260: 6865 2064 6f63 756d 656e 7422 2061 6e64  he document" and
+00003270: 0a22 7075 6c6c 2074 6865 2063 6f6e 7465  ."pull the conte
+00003280: 6e74 222e 2044 6f63 7832 7079 7468 6f6e  nt". Docx2python
+00003290: 2076 3220 7365 7061 7261 7465 7320 616e   v2 separates an
+000032a0: 6420 6578 706f 7365 7320 7468 6573 6520  d exposes these 
+000032b0: 7374 6570 732e 2054 6869 7320 7769 6c6c  steps. This will
+000032c0: 2061 6c6c 6f77 2065 6173 6965 7220 6578   allow easier ex
+000032d0: 7465 6e73 696f 6e2e 0a0a 5365 6520 7468  tension...See th
+000032e0: 6520 6064 6f63 785f 7265 6164 6572 2e70  e `docx_reader.p
+000032f0: 7960 206d 6f64 756c 6520 616e 6420 7369  y` module and si
+00003300: 6d70 6c65 2065 7861 6d70 6c65 7320 696e  mple examples in
+00003310: 2074 6865 2060 7574 696c 6974 6965 732e   the `utilities.
+00003320: 7079 6020 6d6f 6475 6c65 2e0a 0a23 2320  py` module...## 
+00003330: 7365 6520 7574 696c 6974 6965 732e 7079  see utilities.py
+00003340: 2066 6f72 2065 7861 6d70 6c65 7320 6f66   for examples of
+00003350: 206d 616a 6f72 206e 6577 2066 6561 7475   major new featu
+00003360: 7265 732e 0a                             res..
```

### Comparing `docx2python-2.7.2/PKG-INFO` & `docx2python-2.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx2python
-Version: 2.7.2
+Version: 2.7.3
 Summary: Extract content from docx files
 License: MIT
 Author: Shay Hill
 Author-email: shay_public@hotmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

