# Comparing `tmp/rebookmaker-0.8.8.tar.gz` & `tmp/rebookmaker-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rebookmaker-0.8.8.tar", last modified: Mon Apr 25 06:21:51 2022, max compression
+gzip compressed data, was "rebookmaker-0.8.9.tar", last modified: Sun Jun 18 16:15:57 2023, max compression
```

## Comparing `rebookmaker-0.8.8.tar` & `rebookmaker-0.8.9.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2022-04-25 06:21:51.011460 rebookmaker-0.8.8/
--rw-r--r--   0 shlomif    (500) shlomif    (500)       31 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/AUTHORS
--rw-r--r--   0 shlomif    (500) shlomif    (500)     1609 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/CHANGELOG.rst
--rw-r--r--   0 shlomif    (500) shlomif    (500)     1519 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/LICENSE
--rw-r--r--   0 shlomif    (500) shlomif    (500)      191 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/MANIFEST.in
--rw-r--r--   0 shlomif    (500) shlomif    (500)     4812 2022-04-25 06:21:51.011460 rebookmaker-0.8.8/PKG-INFO
--rw-r--r--   0 shlomif    (500) shlomif    (500)     4138 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/README
--rw-r--r--   0 shlomif    (500) shlomif    (500)     4138 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/README.rst
-drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2022-04-25 06:21:51.007460 rebookmaker-0.8.8/docs/
--rw-r--r--   0 shlomif    (500) shlomif    (500)      538 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/docs/CHANGELOG.rst
--rw-r--r--   0 shlomif    (500) shlomif    (500)     2206 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/docs/CONTRIBUTING.rst
--rw-r--r--   0 shlomif    (500) shlomif    (500)     1901 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/docs/LICENSE.rst
--rw-r--r--   0 shlomif    (500) shlomif    (500)     4138 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/docs/README.rst
--rw-r--r--   0 shlomif    (500) shlomif    (500)     7437 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/docs/conf.py
-drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2022-04-25 06:21:51.007460 rebookmaker-0.8.8/docs/html/
--rw-r--r--   0 shlomif    (500) shlomif    (500)      333 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/docs/html/index.html
--rw-r--r--   0 shlomif    (500) shlomif    (500)      274 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/docs/index.rst
-drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2022-04-25 06:21:51.008460 rebookmaker-0.8.8/rebookmaker/
--rwxr-xr-x   0 shlomif    (500) shlomif    (500)    14623 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/__init__.py
--rwxr-xr-x   0 shlomif    (500) shlomif    (500)      495 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/__main__.py
-drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2022-04-25 06:21:50.943461 rebookmaker-0.8.8/rebookmaker/data/
-drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2022-04-25 06:21:51.010460 rebookmaker-0.8.8/rebookmaker/data/templates/
--rw-r--r--   0 shlomif    (500) shlomif    (500)      242 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/data/templates/container.xml.jinja
--rw-r--r--   0 shlomif    (500) shlomif    (500)     1950 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/data/templates/content.opf.jinja
--rw-r--r--   0 shlomif    (500) shlomif    (500)      638 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/data/templates/cover.html.jinja
--rw-r--r--   0 shlomif    (500) shlomif    (500)      462 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/data/templates/nav.html.jinja
--rw-r--r--   0 shlomif    (500) shlomif    (500)       68 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/data/templates/onepixel.png
--rw-r--r--   0 shlomif    (500) shlomif    (500)    16254 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/data/templates/onepixel.xcf
--rw-r--r--   0 shlomif    (500) shlomif    (500)      425 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/data/templates/toc.html.jinja
--rw-r--r--   0 shlomif    (500) shlomif    (500)      508 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/data/templates/toc.ncx.jinja
--rwxr-xr-x   0 shlomif    (500) shlomif    (500)      794 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/rebookmaker
--rwxr-xr-x   0 shlomif    (500) shlomif    (500)      260 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/rebookmaker/template.py
-drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2022-04-25 06:21:51.009460 rebookmaker-0.8.8/rebookmaker.egg-info/
--rw-r--r--   0 shlomif    (500) shlomif    (500)     4812 2022-04-25 06:21:50.000000 rebookmaker-0.8.8/rebookmaker.egg-info/PKG-INFO
--rw-r--r--   0 shlomif    (500) shlomif    (500)      923 2022-04-25 06:21:50.000000 rebookmaker-0.8.8/rebookmaker.egg-info/SOURCES.txt
--rw-r--r--   0 shlomif    (500) shlomif    (500)        1 2022-04-25 06:21:50.000000 rebookmaker-0.8.8/rebookmaker.egg-info/dependency_links.txt
--rw-r--r--   0 shlomif    (500) shlomif    (500)        1 2022-04-25 06:18:54.000000 rebookmaker-0.8.8/rebookmaker.egg-info/not-zip-safe
--rw-r--r--   0 shlomif    (500) shlomif    (500)       76 2022-04-25 06:21:50.000000 rebookmaker-0.8.8/rebookmaker.egg-info/requires.txt
--rw-r--r--   0 shlomif    (500) shlomif    (500)       12 2022-04-25 06:21:50.000000 rebookmaker-0.8.8/rebookmaker.egg-info/top_level.txt
--rw-r--r--   0 shlomif    (500) shlomif    (500)       76 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/requirements.txt
--rw-r--r--   0 shlomif    (500) shlomif    (500)      259 2022-04-25 06:21:51.011460 rebookmaker-0.8.8/setup.cfg
--rwxr-xr-x   0 shlomif    (500) shlomif    (500)     1421 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/setup.py
-drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2022-04-25 06:21:51.011460 rebookmaker-0.8.8/tests/
--rwxr-xr-x   0 shlomif    (500) shlomif    (500)     1625 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/tests/__init__.py
--rwxr-xr-x   0 shlomif    (500) shlomif    (500)      324 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/tests/test_rebook.py
--rwxr-xr-x   0 shlomif    (500) shlomif    (500)      993 2022-04-25 06:18:53.000000 rebookmaker-0.8.8/tests/test_sanity.py
+drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2023-06-18 16:15:57.270017 rebookmaker-0.8.9/
+-rw-r--r--   0 shlomif    (500) shlomif    (500)       31 2023-06-18 16:15:21.000000 rebookmaker-0.8.9/AUTHORS
+-rw-r--r--   0 shlomif    (500) shlomif    (500)     1643 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/CHANGELOG.rst
+-rw-r--r--   0 shlomif    (500) shlomif    (500)     1519 2023-06-18 16:15:21.000000 rebookmaker-0.8.9/LICENSE
+-rw-r--r--   0 shlomif    (500) shlomif    (500)      191 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/MANIFEST.in
+-rw-r--r--   0 shlomif    (500) shlomif    (500)     4861 2023-06-18 16:15:57.270017 rebookmaker-0.8.9/PKG-INFO
+-rw-r--r--   0 shlomif    (500) shlomif    (500)     4138 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/README
+-rw-r--r--   0 shlomif    (500) shlomif    (500)     4138 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/README.rst
+drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2023-06-18 16:15:57.265017 rebookmaker-0.8.9/docs/
+-rw-r--r--   0 shlomif    (500) shlomif    (500)      538 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/docs/CHANGELOG.rst
+-rw-r--r--   0 shlomif    (500) shlomif    (500)     2206 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/docs/CONTRIBUTING.rst
+-rw-r--r--   0 shlomif    (500) shlomif    (500)     1901 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/docs/LICENSE.rst
+-rw-r--r--   0 shlomif    (500) shlomif    (500)     4138 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/docs/README.rst
+-rw-r--r--   0 shlomif    (500) shlomif    (500)     7437 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/docs/conf.py
+drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2023-06-18 16:15:57.266017 rebookmaker-0.8.9/docs/html/
+-rw-r--r--   0 shlomif    (500) shlomif    (500)      333 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/docs/html/index.html
+-rw-r--r--   0 shlomif    (500) shlomif    (500)      274 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/docs/index.rst
+drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2023-06-18 16:15:57.266017 rebookmaker-0.8.9/rebookmaker/
+-rwxr-xr-x   0 shlomif    (500) shlomif    (500)    14623 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/__init__.py
+-rwxr-xr-x   0 shlomif    (500) shlomif    (500)      495 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/__main__.py
+drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2023-06-18 16:15:57.262017 rebookmaker-0.8.9/rebookmaker/data/
+drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2023-06-18 16:15:57.269017 rebookmaker-0.8.9/rebookmaker/data/templates/
+-rw-r--r--   0 shlomif    (500) shlomif    (500)      242 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/data/templates/container.xml.jinja
+-rw-r--r--   0 shlomif    (500) shlomif    (500)     1950 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/data/templates/content.opf.jinja
+-rw-r--r--   0 shlomif    (500) shlomif    (500)      638 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/data/templates/cover.html.jinja
+-rw-r--r--   0 shlomif    (500) shlomif    (500)      462 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/data/templates/nav.html.jinja
+-rw-r--r--   0 shlomif    (500) shlomif    (500)       68 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/data/templates/onepixel.png
+-rw-r--r--   0 shlomif    (500) shlomif    (500)    16254 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/data/templates/onepixel.xcf
+-rw-r--r--   0 shlomif    (500) shlomif    (500)      425 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/data/templates/toc.html.jinja
+-rw-r--r--   0 shlomif    (500) shlomif    (500)      508 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/data/templates/toc.ncx.jinja
+-rwxr-xr-x   0 shlomif    (500) shlomif    (500)      794 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/rebookmaker
+-rwxr-xr-x   0 shlomif    (500) shlomif    (500)      260 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/rebookmaker/template.py
+drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2023-06-18 16:15:57.268017 rebookmaker-0.8.9/rebookmaker.egg-info/
+-rw-r--r--   0 shlomif    (500) shlomif    (500)     4861 2023-06-18 16:15:55.000000 rebookmaker-0.8.9/rebookmaker.egg-info/PKG-INFO
+-rw-r--r--   0 shlomif    (500) shlomif    (500)      961 2023-06-18 16:15:57.000000 rebookmaker-0.8.9/rebookmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 shlomif    (500) shlomif    (500)        1 2023-06-18 16:15:55.000000 rebookmaker-0.8.9/rebookmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 shlomif    (500) shlomif    (500)       58 2023-06-18 16:15:56.000000 rebookmaker-0.8.9/rebookmaker.egg-info/entry_points.txt
+-rw-r--r--   0 shlomif    (500) shlomif    (500)        1 2023-06-18 16:15:34.000000 rebookmaker-0.8.9/rebookmaker.egg-info/not-zip-safe
+-rw-r--r--   0 shlomif    (500) shlomif    (500)       87 2023-06-18 16:15:56.000000 rebookmaker-0.8.9/rebookmaker.egg-info/requires.txt
+-rw-r--r--   0 shlomif    (500) shlomif    (500)       12 2023-06-18 16:15:56.000000 rebookmaker-0.8.9/rebookmaker.egg-info/top_level.txt
+-rw-r--r--   0 shlomif    (500) shlomif    (500)       87 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/requirements.txt
+-rw-r--r--   0 shlomif    (500) shlomif    (500)      259 2023-06-18 16:15:57.271017 rebookmaker-0.8.9/setup.cfg
+-rwxr-xr-x   0 shlomif    (500) shlomif    (500)     1623 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/setup.py
+drwxr-xr-x   0 shlomif    (500) shlomif    (500)        0 2023-06-18 16:15:57.270017 rebookmaker-0.8.9/tests/
+-rwxr-xr-x   0 shlomif    (500) shlomif    (500)     1625 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/tests/__init__.py
+-rwxr-xr-x   0 shlomif    (500) shlomif    (500)      324 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/tests/test_rebook.py
+-rwxr-xr-x   0 shlomif    (500) shlomif    (500)      993 2023-06-18 16:15:22.000000 rebookmaker-0.8.9/tests/test_sanity.py
```

### Comparing `rebookmaker-0.8.8/CHANGELOG.rst` & `rebookmaker-0.8.9/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 =====================
 Appendix C. Changelog
 =====================
 :Info: This is the changelog for rebookmaker.
 :Author: Shlomi Fish <shlomif@cpan.org>
 :Copyright: © 2020, Shlomi Fish.
 :License: BSD (see /LICENSE or :doc:`Appendix B <LICENSE>`.)
-:Date: 2022-04-25
-:Version: 0.8.8
+:Date: 2023-06-18
+:Version: 0.8.9
 
 .. index:: CHANGELOG
 
 GitHub holds releases, too
 ==========================
 
 More information can be found on GitHub in the `releases section
 <https://github.com/shlomif/rebookmaker/releases>`_.
 
 Version History
 ===============
 
+0.8.9
+    bs4 → beautifulsoup4
+
 0.8.8
     Update code for version 3.x.y of jinja2.
 
     Silence bs4 warning.
 
 0.8.7
     Get XHTML ( *.xhtml ) pages to validate by stripping the <!DOCTYPE>
```

### Comparing `rebookmaker-0.8.8/LICENSE` & `rebookmaker-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rebookmaker-0.8.8/PKG-INFO` & `rebookmaker-0.8.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rebookmaker
-Version: 0.8.8
+Version: 0.8.9
 Summary: EPUB generator
 Home-page: https://github.com/shlomif/rebookmaker
 Author: Shlomi Fish
 Author-email: shlomif@cpan.org
 License: 3-clause BSD
 Keywords: rebookmaker
 Platform: any
@@ -12,25 +12,26 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: AUTHORS
 
 ==============================================================================
 rebookmaker.  EPUB generator
 ==============================================================================
 :Info: This is the README file for rebookmaker.
 :Author: Shlomi Fish <shlomif@cpan.org>
 :Copyright: © 2020, Shlomi Fish.
-:Date: 2022-04-25
-:Version: 0.8.8
+:Date: 2023-06-18
+:Version: 0.8.9
 
 .. index: README
 .. image:: https://travis-ci.org/shlomif/rebookmaker.svg?branch=master
    :target: https://travis-ci.org/shlomif/rebookmaker
 
 PURPOSE
 -------
@@ -120,9 +121,7 @@
 OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
```

### Comparing `rebookmaker-0.8.8/README` & `rebookmaker-0.8.9/README`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ==============================================================================
 rebookmaker.  EPUB generator
 ==============================================================================
 :Info: This is the README file for rebookmaker.
 :Author: Shlomi Fish <shlomif@cpan.org>
 :Copyright: © 2020, Shlomi Fish.
-:Date: 2022-04-25
-:Version: 0.8.8
+:Date: 2023-06-18
+:Version: 0.8.9
 
 .. index: README
 .. image:: https://travis-ci.org/shlomif/rebookmaker.svg?branch=master
    :target: https://travis-ci.org/shlomif/rebookmaker
 
 PURPOSE
 -------
```

### Comparing `rebookmaker-0.8.8/README.rst` & `rebookmaker-0.8.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ==============================================================================
 rebookmaker.  EPUB generator
 ==============================================================================
 :Info: This is the README file for rebookmaker.
 :Author: Shlomi Fish <shlomif@cpan.org>
 :Copyright: © 2020, Shlomi Fish.
-:Date: 2022-04-25
-:Version: 0.8.8
+:Date: 2023-06-18
+:Version: 0.8.9
 
 .. index: README
 .. image:: https://travis-ci.org/shlomif/rebookmaker.svg?branch=master
    :target: https://travis-ci.org/shlomif/rebookmaker
 
 PURPOSE
 -------
```

### Comparing `rebookmaker-0.8.8/docs/CHANGELOG.rst` & `rebookmaker-0.8.9/docs/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 =====================
 Appendix C. Changelog
 =====================
 :Info: This is the changelog for rebookmaker.
 :Author: Shlomi Fish <shlomif@cpan.org>
 :Copyright: © 2020, Shlomi Fish.
 :License: BSD (see /LICENSE or :doc:`Appendix B <LICENSE>`.)
-:Date: 2022-04-25
-:Version: 0.8.8
+:Date: 2023-06-18
+:Version: 0.8.9
 
 .. index:: CHANGELOG
 
 GitHub holds releases, too
 ==========================
 
 More information can be found on GitHub in the `releases section
```

### Comparing `rebookmaker-0.8.8/docs/CONTRIBUTING.rst` & `rebookmaker-0.8.9/docs/CONTRIBUTING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ==============================
 Appendix A. Contribution rules
 ==============================
 :Info: Those are the contribution rules for rebookmaker.
-:Copyright: © 2012-2022, Chris Warrick.
+:Copyright: © 2012-2023, Chris Warrick.
 :License: 3-clause BSD
 
 .. index:: contributing
 
 Do you want to contribute to this project?  Great!  I’d love to see some help,
 but you must comply with some rules.
```

### Comparing `rebookmaker-0.8.8/docs/LICENSE.rst` & `rebookmaker-0.8.9/docs/LICENSE.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 =======================================================
 Appendix B. License for rebookmaker
 =======================================================
 :Info: This is the license for rebookmaker.
 :Author: Shlomi Fish <shlomif@cpan.org>
 :Copyright: © 2020, Shlomi Fish.
 :License: BSD (see /LICENSE or :doc:`Appendix B <LICENSE>`.)
-:Date: 2022-04-25
-:Version: 0.8.8
+:Date: 2023-06-18
+:Version: 0.8.9
 
 .. index:: LICENSE
 
 Copyright © 2020, Shlomi Fish.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
```

### Comparing `rebookmaker-0.8.8/docs/README.rst` & `rebookmaker-0.8.9/docs/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ==============================================================================
 rebookmaker.  EPUB generator
 ==============================================================================
 :Info: This is the README file for rebookmaker.
 :Author: Shlomi Fish <shlomif@cpan.org>
 :Copyright: © 2020, Shlomi Fish.
-:Date: 2022-04-25
-:Version: 0.8.8
+:Date: 2023-06-18
+:Version: 0.8.9
 
 .. index: README
 .. image:: https://travis-ci.org/shlomif/rebookmaker.svg?branch=master
    :target: https://travis-ci.org/shlomif/rebookmaker
 
 PURPOSE
 -------
```

### Comparing `rebookmaker-0.8.8/docs/conf.py` & `rebookmaker-0.8.9/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 copyright = u'2020, Shlomi Fish'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.8.8'
+version = '0.8.9'
 # The full version, including alpha/beta/rc tags.
-release = '0.8.8'
+release = '0.8.9'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `rebookmaker-0.8.8/rebookmaker/__init__.py` & `rebookmaker-0.8.9/rebookmaker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- encoding: utf-8 -*-
-# rebookmaker v0.8.8
+# rebookmaker v0.8.9
 # EPUB generator
 # Copyright © 2020, Shlomi Fish.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
@@ -36,15 +36,15 @@
 EPUB generator
 
 :Copyright: © 2020, Shlomi Fish.
 :License: BSD (see /LICENSE).
 """
 
 __title__ = 'rebookmaker'
-__version__ = '0.8.8'
+__version__ = '0.8.9'
 __author__ = 'Shlomi Fish'
 __license__ = '3-clause BSD'
 __docformat__ = 'restructuredtext en'
 
 __all__ = ()
 
 # import gettext
```

### Comparing `rebookmaker-0.8.8/rebookmaker/data/templates/content.opf.jinja` & `rebookmaker-0.8.9/rebookmaker/data/templates/content.opf.jinja`

 * *Files identical despite different names*

### Comparing `rebookmaker-0.8.8/rebookmaker/data/templates/cover.html.jinja` & `rebookmaker-0.8.9/rebookmaker/data/templates/cover.html.jinja`

 * *Files identical despite different names*

### Comparing `rebookmaker-0.8.8/rebookmaker/data/templates/onepixel.xcf` & `rebookmaker-0.8.9/rebookmaker/data/templates/onepixel.xcf`

 * *Files identical despite different names*

### Comparing `rebookmaker-0.8.8/rebookmaker/rebookmaker` & `rebookmaker-0.8.9/rebookmaker/rebookmaker`

 * *Files identical despite different names*

### Comparing `rebookmaker-0.8.8/rebookmaker.egg-info/PKG-INFO` & `rebookmaker-0.8.9/rebookmaker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rebookmaker
-Version: 0.8.8
+Version: 0.8.9
 Summary: EPUB generator
 Home-page: https://github.com/shlomif/rebookmaker
 Author: Shlomi Fish
 Author-email: shlomif@cpan.org
 License: 3-clause BSD
 Keywords: rebookmaker
 Platform: any
@@ -12,25 +12,26 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: AUTHORS
 
 ==============================================================================
 rebookmaker.  EPUB generator
 ==============================================================================
 :Info: This is the README file for rebookmaker.
 :Author: Shlomi Fish <shlomif@cpan.org>
 :Copyright: © 2020, Shlomi Fish.
-:Date: 2022-04-25
-:Version: 0.8.8
+:Date: 2023-06-18
+:Version: 0.8.9
 
 .. index: README
 .. image:: https://travis-ci.org/shlomif/rebookmaker.svg?branch=master
    :target: https://travis-ci.org/shlomif/rebookmaker
 
 PURPOSE
 -------
@@ -120,9 +121,7 @@
 OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
```

### Comparing `rebookmaker-0.8.8/rebookmaker.egg-info/SOURCES.txt` & `rebookmaker-0.8.9/rebookmaker.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 rebookmaker/__init__.py
 rebookmaker/__main__.py
 rebookmaker/rebookmaker
 rebookmaker/template.py
 rebookmaker.egg-info/PKG-INFO
 rebookmaker.egg-info/SOURCES.txt
 rebookmaker.egg-info/dependency_links.txt
+rebookmaker.egg-info/entry_points.txt
 rebookmaker.egg-info/not-zip-safe
 rebookmaker.egg-info/requires.txt
 rebookmaker.egg-info/top_level.txt
 rebookmaker/data/templates/container.xml.jinja
 rebookmaker/data/templates/content.opf.jinja
 rebookmaker/data/templates/cover.html.jinja
 rebookmaker/data/templates/nav.html.jinja
```

### Comparing `rebookmaker-0.8.8/setup.py` & `rebookmaker-0.8.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 import io
 from setuptools import setup, find_packages
 
 
 setup(name='rebookmaker',
-      version='0.8.8',
+      version='0.8.9',
       description='EPUB generator',
       keywords='rebookmaker',
       author='Shlomi Fish',
       author_email='shlomif@cpan.org',
       url='https://github.com/shlomif/rebookmaker',
       license='3-clause BSD',
       long_description=io.open(
@@ -21,14 +21,20 @@
                    'Programming Language :: Python',
                    'Programming Language :: Python :: 3',
                    'Programming Language :: Python :: 3.6',
                    'Programming Language :: Python :: 3.7',
                    'Programming Language :: Python :: 3.8',
                    'Programming Language :: Python :: 3.9',
                    'Programming Language :: Python :: 3.10',
+                   'Programming Language :: Python :: 3.11',
                    ],
       packages=find_packages(exclude=('tests', 'tests.*')),
       include_package_data=True,
     package_data={'': ['data/templates/*.jinja','data/templates/*.png','data/templates/*.xcf'],},
     scripts=['rebookmaker/rebookmaker'],
-      install_requires=['bs4','coverage','jinja2>=3.0.1','lxml','markupsafe','pytest','pytest-cov','requests','twine'],
+      install_requires=['beautifulsoup4','coverage','jinja2>=3.0.1','lxml','markupsafe','pytest','pytest-cov','requests','twine'],
+      entry_points={
+          'console_scripts': [
+              'rebookmaker = rebookmaker.__main__:main',
+          ]
+      },
       )
```

### Comparing `rebookmaker-0.8.8/tests/__init__.py` & `rebookmaker-0.8.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rebookmaker-0.8.8/tests/test_sanity.py` & `rebookmaker-0.8.9/tests/test_sanity.py`

 * *Files identical despite different names*

