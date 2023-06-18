# Comparing `tmp/css_inline-0.8.7.tar.gz` & `tmp/css_inline-0.9.0.tar.gz`

## Comparing `css_inline-0.8.7.tar` & `css_inline-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,39 @@
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 css_inline-0.8.7/local_dependencies/css-inline/Cargo.toml
--rw-r--r--   0     1001      123     5371 2023-01-30 21:02:06.000000 css_inline-0.8.7/local_dependencies/css-inline/README.md
--rw-r--r--   0     1001      123    12376 2023-01-30 21:02:06.000000 css_inline-0.8.7/local_dependencies/css-inline/benches/inliner.rs
--rw-r--r--   0     1001      123     1122 2023-01-30 21:02:06.000000 css_inline-0.8.7/local_dependencies/css-inline/benches/styles.css
--rw-r--r--   0     1001      123     2535 2023-01-30 21:02:06.000000 css_inline-0.8.7/local_dependencies/css-inline/src/error.rs
--rw-r--r--   0     1001      123    19671 2023-01-30 21:02:06.000000 css_inline-0.8.7/local_dependencies/css-inline/src/lib.rs
--rw-r--r--   0     1001      123     5517 2023-01-30 21:02:06.000000 css_inline-0.8.7/local_dependencies/css-inline/src/main.rs
--rw-r--r--   0     1001      123     2370 2023-01-30 21:02:06.000000 css_inline-0.8.7/local_dependencies/css-inline/src/parser.rs
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 css_inline-0.8.7/Cargo.toml
--rw-r--r--   0     1001      123      235 2023-01-30 21:02:06.000000 css_inline-0.8.7/.gitignore
--rw-r--r--   0     1001      123     7655 2023-01-30 21:02:06.000000 css_inline-0.8.7/CHANGELOG.md
--rw-r--r--   0     1001      123     6162 2023-01-30 21:02:06.000000 css_inline-0.8.7/README.md
--rw-r--r--   0     1001      123    17848 2023-01-30 21:02:06.000000 css_inline-0.8.7/benches/bench.py
--rw-r--r--   0     1001      123      415 2023-01-30 21:02:06.000000 css_inline-0.8.7/build.rs
--rw-r--r--   0     1001      123      876 2023-01-30 21:02:06.000000 css_inline-0.8.7/css_inline.pyi
--rw-r--r--   0     1001      123     1449 2023-01-30 21:02:06.000000 css_inline-0.8.7/pyproject.toml
--rw-r--r--   0     1001      123        7 2023-01-30 21:02:06.000000 css_inline-0.8.7/rust-toolchain
--rw-r--r--   0     1001      123     6791 2023-01-30 21:02:06.000000 css_inline-0.8.7/src/lib.rs
--rw-r--r--   0     1001      123       20 2023-01-30 21:02:06.000000 css_inline-0.8.7/tests-py/external.css
--rw-r--r--   0     1001      123     3234 2023-01-30 21:02:06.000000 css_inline-0.8.7/tests-py/test_inlining.py
--rw-r--r--   0     1001      123      160 2023-01-30 21:02:06.000000 css_inline-0.8.7/tox.ini
--rw-r--r--   0     1001      123    37613 2023-01-30 21:02:57.000000 css_inline-0.8.7/Cargo.lock
--rw-r--r--   0        0        0     7379 1970-01-01 00:00:00.000000 css_inline-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 css_inline-0.9.0/local_dependencies/css-inline/Cargo.toml
+-rw-r--r--   0     1001      123     5296 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/README.md
+-rw-r--r--   0     1001      123    12376 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/benches/inliner.rs
+-rw-r--r--   0     1001      123     1122 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/benches/styles.css
+-rw-r--r--   0     1001      123       47 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/rustfmt.toml
+-rw-r--r--   0     1001      123     2535 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/error.rs
+-rw-r--r--   0     1001      123     1784 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/attributes.rs
+-rw-r--r--   0     1001      123    12645 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/document.rs
+-rw-r--r--   0     1001      123     7735 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/element.rs
+-rw-r--r--   0     1001      123     2346 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/iter.rs
+-rw-r--r--   0     1001      123      262 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/mod.rs
+-rw-r--r--   0     1001      123     2932 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/node.rs
+-rw-r--r--   0     1001      123     8331 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/parser.rs
+-rw-r--r--   0     1001      123      666 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/selectors/attr_value.rs
+-rw-r--r--   0     1001      123     1195 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/selectors/local_name.rs
+-rw-r--r--   0     1001      123     1950 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/selectors/mod.rs
+-rw-r--r--   0     1001      123     1574 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/selectors/parser.rs
+-rw-r--r--   0     1001      123     1351 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/selectors/pseudo_classes.rs
+-rw-r--r--   0     1001      123      410 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/selectors/pseudo_elements.rs
+-rw-r--r--   0     1001      123      808 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/selectors/selector_impl.rs
+-rw-r--r--   0     1001      123     7242 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/html/serializer.rs
+-rw-r--r--   0     1001      123    17609 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/lib.rs
+-rw-r--r--   0     1001      123     5550 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/main.rs
+-rw-r--r--   0     1001      123     2370 2023-06-10 17:00:06.000000 css_inline-0.9.0/local_dependencies/css-inline/src/parser.rs
+-rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 css_inline-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      123      235 2023-06-10 17:00:06.000000 css_inline-0.9.0/.gitignore
+-rw-r--r--   0     1001      123     8066 2023-06-10 17:00:06.000000 css_inline-0.9.0/CHANGELOG.md
+-rw-r--r--   0     1001      123     6091 2023-06-10 17:00:06.000000 css_inline-0.9.0/README.md
+-rw-r--r--   0     1001      123    17848 2023-06-10 17:00:06.000000 css_inline-0.9.0/benches/bench.py
+-rw-r--r--   0     1001      123      415 2023-06-10 17:00:06.000000 css_inline-0.9.0/build.rs
+-rw-r--r--   0     1001      123     1031 2023-06-10 17:00:06.000000 css_inline-0.9.0/css_inline.pyi
+-rw-r--r--   0     1001      123     1442 2023-06-10 17:00:06.000000 css_inline-0.9.0/pyproject.toml
+-rw-r--r--   0     1001      123        7 2023-06-10 17:00:06.000000 css_inline-0.9.0/rust-toolchain
+-rw-r--r--   0     1001      123     7377 2023-06-10 17:00:06.000000 css_inline-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      123       20 2023-06-10 17:00:06.000000 css_inline-0.9.0/tests-py/external.css
+-rw-r--r--   0     1001      123     3234 2023-06-10 17:00:06.000000 css_inline-0.9.0/tests-py/test_inlining.py
+-rw-r--r--   0     1001      123      160 2023-06-10 17:00:06.000000 css_inline-0.9.0/tox.ini
+-rw-r--r--   0     1001      123    34891 2023-06-10 17:00:32.000000 css_inline-0.9.0/Cargo.lock
+-rw-r--r--   0        0        0     7308 1970-01-01 00:00:00.000000 css_inline-0.9.0/PKG-INFO
```

### Comparing `css_inline-0.8.7/local_dependencies/css-inline/Cargo.toml` & `css_inline-0.9.0/local_dependencies/css-inline/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "css-inline"
-version = "0.8.5"
+version = "0.9.0"
 authors = ["Dmitry Dygalo <dadygalo@gmail.com>"]
 edition = "2021"
 license = "MIT"
 readme = "../README.md"
 description = "A crate for inlining CSS into 'style' HTML attributes."
 repository = "https://github.com/Stranger6667/css-inline"
 keywords = ["html", "css", "css-inline", "email"]
@@ -19,26 +19,23 @@
 default = ["cli", "http", "file"]
 cli = ["pico-args", "rayon"]
 http = ["attohttpc"]
 file = []
 
 [dependencies]
 cssparser = "0.29"
-kuchiki = "0.8"
+html5ever = "0.26.0"
 memchr = "2.4"
 attohttpc = { version = "0", default-features = false, features = ["compress", "tls-rustls"], optional = true }
 url = "2"
 smallvec = "1"
 indexmap = "1.8.1"
 pico-args = { version = "0.3", optional = true }
 rayon = { version = "1.5", optional = true }
-
-[dev-dependencies]
-assert_cmd = "2.0.6"
-criterion = ">= 0.1"
+selectors = "0.24.0"
 
 [[bench]]
 name = "inliner"
 harness = false
 
 [profile.release]
 lto = "fat"
```

### Comparing `css_inline-0.8.7/local_dependencies/css-inline/README.md` & `css_inline-0.9.0/local_dependencies/css-inline/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     </body>
 </html>
 ```
 
 To use it in your project add the following line to your `dependencies` section in the project's `Cargo.toml` file:
 
 ```toml
-css-inline = "0.8"
+css-inline = "0.9"
 ```
 
 Minimum Supported Rust Version is 1.60.
 
 ## Usage
 
 ```rust
@@ -112,15 +112,15 @@
     <h1>Big Text</h1>
 </body>
 </html>
 ```
 
 ## Standards support & restrictions
 
-`css-inline` is built on top of [kuchiki](https://crates.io/crates/kuchiki) and [cssparser](https://crates.io/crates/cssparser) and relies on their behavior for HTML / CSS parsing and serialization.
+`css-inline` is built on top of [cssparser](https://crates.io/crates/cssparser) and relies on its behavior for CSS parsing.
 Notably:
 
 - Only HTML 5, XHTML is not supported;
 - Only CSS 3;
 - Only UTF-8 for string representation. Other document encodings are not yet supported.
 
 ## Bindings
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 documents. It is built with Mozilla's Servo project components. When you send
 HTML emails, you need to use "style" attributes instead of "style" tags. For
 example, this HTML: ```html
 ****** Big Text ******
 ``` Will be turned into this: ```html
 ****** Big Text ******
 ``` To use it in your project add the following line to your `dependencies`
-section in the project's `Cargo.toml` file: ```toml css-inline = "0.8" ```
+section in the project's `Cargo.toml` file: ```toml css-inline = "0.9" ```
 Minimum Supported Rust Version is 1.60. ## Usage ```rust const HTML: &str = r#"
 ****** Big Text ******
 "#; fn main() -> Result<(), css_inline::InlineError> { let inlined =
 css_inline::inline(HTML)?; // Do something with inlined HTML, e.g. send an
 email Ok(()) } ``` ### Features & Configuration `css-inline` can be configured
 by using `CSSInliner::options()` that implements the Builder pattern: ```rust
 const HTML: &str = "..."; fn main() -> Result<(), css_inline::InlineError>
@@ -31,17 +31,16 @@
 stylesheets should be loaded or not. Default: `true` - `extra_css`. Additional
 CSS to inline. Default: `None` If you'd like to skip CSS inlining for an HTML
 tag, add `data-css-inline="ignore"` attribute to it: ```html
 ****** Big Text ******
 ``` This attribute also allows you to skip `link` and `style` tags: ```html
 ****** Big Text ******
 ``` ## Standards support & restrictions `css-inline` is built on top of
-[kuchiki](https://crates.io/crates/kuchiki) and [cssparser](https://crates.io/
-crates/cssparser) and relies on their behavior for HTML / CSS parsing and
-serialization. Notably: - Only HTML 5, XHTML is not supported; - Only CSS 3; -
+[cssparser](https://crates.io/crates/cssparser) and relies on its behavior for
+CSS parsing. Notably: - Only HTML 5, XHTML is not supported; - Only CSS 3; -
 Only UTF-8 for string representation. Other document encodings are not yet
 supported. ## Bindings There are bindings for Python and WebAssembly in the
 `bindings` directory. ## Command Line Interface `css-inline` provides a
 command-line interface: ```text css-inline --help css-inline inlines CSS into
 HTML documents. USAGE: css-inline [OPTIONS] [PATH ...] command | css-inline
 [OPTIONS] ARGS: ... An HTML document to process. In each specified document
 "css-inline" will look for all relevant "style" and "link" tags, will load CSS
```

### Comparing `css_inline-0.8.7/local_dependencies/css-inline/benches/inliner.rs` & `css_inline-0.9.0/local_dependencies/css-inline/benches/inliner.rs`

 * *Files identical despite different names*

### Comparing `css_inline-0.8.7/local_dependencies/css-inline/benches/styles.css` & `css_inline-0.9.0/local_dependencies/css-inline/benches/styles.css`

 * *Files identical despite different names*

### Comparing `css_inline-0.8.7/local_dependencies/css-inline/src/error.rs` & `css_inline-0.9.0/local_dependencies/css-inline/src/error.rs`

 * *Files identical despite different names*

### Comparing `css_inline-0.8.7/local_dependencies/css-inline/src/lib.rs` & `css_inline-0.9.0/local_dependencies/css-inline/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -21,29 +21,28 @@
     unused_import_braces,
     unused_qualifications,
     variant_size_differences,
     rust_2018_idioms,
     rust_2018_compatibility
 )]
 
-use kuchiki::{
-    parse_html, traits::TendrilSink, ElementData, Node, NodeDataRef, NodeRef, Specificity,
-};
-
 pub mod error;
+mod html;
 mod parser;
 
 pub use error::InlineError;
 use indexmap::IndexMap;
 use smallvec::{smallvec, SmallVec};
 use std::{
     borrow::Cow,
     io::{ErrorKind, Write},
 };
 
+use crate::html::{Document, NodeId, Specificity};
+pub use html::DEFAULT_HTML_TREE_CAPACITY;
 pub use url::{ParseError, Url};
 
 /// Replace double quotes in property values.
 ///
 /// This implementation is deliberately simplistic and covers only `font-family`, but escaping
 /// might be needed in other properties that accept strings.
 macro_rules! replace_double_quotes {
@@ -69,27 +68,31 @@
     /// Whether remote stylesheets should be loaded or not.
     pub load_remote_stylesheets: bool,
     // The point of using `Cow` here is Python bindings, where it is problematic to pass a reference
     // without dealing with memory leaks & unsafe. With `Cow` we can use moved values as `String` in
     // Python wrapper for `CSSInliner` and `&str` in Rust & simple functions on the Python side
     /// Additional CSS to inline.
     pub extra_css: Option<Cow<'a, str>>,
+    /// Pre-allocate capacity for HTML nodes during parsing.
+    /// It can improve performance when you have an estimate of the number of nodes in your HTML document.
+    pub preallocate_node_capacity: usize,
 }
 
 impl<'a> InlineOptions<'a> {
     /// Options for "compact" HTML output.
     #[must_use]
     #[inline]
     pub const fn compact() -> Self {
         InlineOptions {
             inline_style_tags: true,
             remove_style_tags: true,
             base_url: None,
             load_remote_stylesheets: true,
             extra_css: None,
+            preallocate_node_capacity: DEFAULT_HTML_TREE_CAPACITY,
         }
     }
 
     /// Override whether "style" tags should be inlined.
     #[must_use]
     pub fn inline_style_tags(mut self, inline_style_tags: bool) -> Self {
         self.inline_style_tags = inline_style_tags;
@@ -120,14 +123,21 @@
     /// Set additional CSS to inline.
     #[must_use]
     pub fn extra_css(mut self, extra_css: Option<Cow<'a, str>>) -> Self {
         self.extra_css = extra_css;
         self
     }
 
+    /// Set the initial node capacity for HTML tree.
+    #[must_use]
+    pub fn preallocate_node_capacity(mut self, preallocate_node_capacity: usize) -> Self {
+        self.preallocate_node_capacity = preallocate_node_capacity;
+        self
+    }
+
     /// Create a new `CSSInliner` instance from this options.
     #[must_use]
     pub const fn build(self) -> CSSInliner<'a> {
         CSSInliner::new(self)
     }
 }
 
@@ -136,20 +146,20 @@
     fn default() -> Self {
         InlineOptions {
             inline_style_tags: true,
             remove_style_tags: false,
             base_url: None,
             load_remote_stylesheets: true,
             extra_css: None,
+            preallocate_node_capacity: 0,
         }
     }
 }
 
 type Result<T> = std::result::Result<T, InlineError>;
-const CSS_INLINE_ATTRIBUTE: &str = "data-css-inline";
 
 /// Customizable CSS inliner.
 #[derive(Debug)]
 pub struct CSSInliner<'a> {
     options: InlineOptions<'a>,
 }
 
@@ -222,118 +232,66 @@
     /// Inlining might fail for the following reasons:
     ///   - Missing stylesheet file;
     ///   - Remote stylesheet is not available;
     ///   - IO errors;
     ///   - Internal CSS selector parsing error;
     #[inline]
     pub fn inline_to<W: Write>(&self, html: &str, target: &mut W) -> Result<()> {
-        let document = parse_html().one(html);
+        let mut document =
+            Document::parse_with_options(html.as_bytes(), self.options.preallocate_node_capacity);
         // CSS rules may overlap, and the final set of rules applied to an element depend on
         // selectors' specificity - selectors with higher specificity have more priority.
         // Inlining happens in two major steps:
         //   1. All available styles are mapped to respective elements together with their
         //      selector's specificity. When two rules overlap on the same declaration, then
         //      the one with higher specificity replaces another.
         //   2. Resulting styles are merged into existing "style" tags.
-        #[allow(clippy::mutable_key_type)]
-        // Each matched element is identified by their raw pointers - they are evaluated once
-        // and then reused, which allows O(1) access to find them.
-        // Internally, their raw pointers are used to implement `Eq`, which seems like the only
-        // reasonable approach to compare them (performance-wise).
         let mut styles = IndexMap::with_capacity(128);
-        let mut style_tags: SmallVec<[NodeDataRef<ElementData>; 4]> = smallvec![];
         if self.options.inline_style_tags {
-            for style_tag in document
-                .select("style")
-                .map_err(|_| InlineError::ParseError(Cow::from("Unknown error")))?
-            {
-                if style_tag.attributes.borrow().get(CSS_INLINE_ATTRIBUTE) == Some("ignore") {
-                    continue;
-                }
-                if let Some(first_child) = style_tag.as_node().first_child() {
-                    if let Some(css_cell) = first_child.as_text() {
-                        process_css(&document, css_cell.borrow().as_str(), &mut styles);
-                    }
-                }
-                if self.options.remove_style_tags {
-                    style_tags.push(style_tag);
-                }
-            }
-        }
-        if self.options.remove_style_tags {
-            if !self.options.inline_style_tags {
-                style_tags.extend(
-                    document
-                        .select("style")
-                        .map_err(|_| error::InlineError::ParseError(Cow::from("Unknown error")))?,
-                );
-            }
-            for style_tag in &style_tags {
-                style_tag.as_node().detach();
+            for style in document.styles() {
+                process_css(&document, style, &mut styles);
             }
         }
-
         if self.options.load_remote_stylesheets {
-            let mut links = document
-                .select("link[rel~=stylesheet]")
-                .map_err(|_| error::InlineError::ParseError(Cow::from("Unknown error")))?
-                .filter_map(|link_tag| {
-                    if link_tag.attributes.borrow().get(CSS_INLINE_ATTRIBUTE) == Some("ignore") {
-                        None
-                    } else {
-                        link_tag.attributes.borrow().get("href").map(str::to_string)
-                    }
-                })
-                .filter(|link| !link.is_empty())
-                .collect::<Vec<String>>();
+            let mut links = document.stylesheets().collect::<Vec<&str>>();
             links.sort_unstable();
             links.dedup();
             for href in &links {
                 let url = self.get_full_url(href);
                 let css = load_external(url.as_ref())?;
                 process_css(&document, css.as_str(), &mut styles);
             }
         }
         if let Some(extra_css) = &self.options.extra_css {
             process_css(&document, extra_css, &mut styles);
         }
         for (node_id, styles) in styles {
-            // SAFETY: All nodes are alive as long as `document` is in scope.
-            // Therefore, any `document` children should be alive and it is safe to dereference
-            // pointers to them
-            let node = unsafe { &*node_id };
-            // It can be borrowed if the current selector matches <link> tag, that is
-            // already borrowed in `inline_to`. We can ignore such matches
-            if let Ok(mut attributes) = node
-                .as_element()
-                .expect("Element is expected")
-                .attributes
-                .try_borrow_mut()
-            {
-                // Skip inlining for tags that have `data-css-inline="ignore"` attribute
-                if attributes.get(CSS_INLINE_ATTRIBUTE) == Some("ignore") {
-                    continue;
+            let node = &mut document[node_id];
+            let element = if let Some(element) = node.as_not_ignored_element_mut() {
+                element
+            } else {
+                continue;
+            };
+            let attributes = &mut element.attributes;
+            if let Some(existing_style) = attributes.get_style_mut() {
+                *existing_style = merge_styles(existing_style, &styles)?.into();
+            } else {
+                let mut final_styles = String::with_capacity(128);
+                let mut styles = styles.iter().collect::<Vec<_>>();
+                styles.sort_unstable_by(|(_, (a, _)), (_, (b, _))| a.cmp(b));
+                for (name, (_, value)) in styles {
+                    final_styles.push_str(name.as_str());
+                    final_styles.push(':');
+                    replace_double_quotes!(final_styles, name, value);
+                    final_styles.push(';');
                 }
-                if let Some(existing_style) = attributes.get_mut("style") {
-                    *existing_style = merge_styles(existing_style, &styles)?;
-                } else {
-                    let mut final_styles = String::with_capacity(128);
-                    let mut styles = styles.iter().collect::<Vec<_>>();
-                    styles.sort_unstable_by(|(_, (a, _)), (_, (b, _))| a.cmp(b));
-                    for (name, (_, value)) in styles {
-                        final_styles.push_str(name.as_str());
-                        final_styles.push(':');
-                        replace_double_quotes!(final_styles, name, value);
-                        final_styles.push(';');
-                    }
-                    attributes.insert("style", final_styles);
-                };
-            }
+                attributes.set_style(final_styles);
+            };
         }
-        document.serialize(target)?;
+        document.serialize(target, self.options.remove_style_tags)?;
         Ok(())
     }
 
     fn get_full_url<'u>(&self, href: &'u str) -> Cow<'u, str> {
         // Valid absolute URL
         if Url::parse(href).is_ok() {
             return Cow::Borrowed(href);
@@ -386,36 +344,34 @@
                 ErrorKind::Unsupported,
                 "Loading local files requires the `file` feature",
             )))
         }
     }
 }
 
-type NodeId = *const Node;
-
 #[allow(clippy::mutable_key_type)]
 fn process_css(
-    document: &NodeRef,
+    document: &Document,
     css: &str,
     styles: &mut IndexMap<NodeId, IndexMap<String, (Specificity, String)>>,
 ) {
     let mut parse_input = cssparser::ParserInput::new(css);
     let mut parser = cssparser::Parser::new(&mut parse_input);
     let rule_list =
         cssparser::RuleListParser::new_for_stylesheet(&mut parser, parser::CSSRuleListParser);
     for (selectors, declarations) in rule_list.flatten() {
         // Only CSS Syntax Level 3 is supported, therefore it is OK to split by `,`
         // With `is` or `where` selectors (Level 4) this split should be done on the parser level
         for selector in selectors.split(',') {
             if let Ok(matching_elements) = document.select(selector) {
                 // There is always only one selector applied
-                let specificity = matching_elements.selectors.0[0].specificity();
+                let specificity = matching_elements.specificity();
                 for matching_element in matching_elements {
                     let element_styles = styles
-                        .entry(&**matching_element.as_node())
+                        .entry(matching_element.node_id)
                         .or_insert_with(|| IndexMap::with_capacity(8));
                     // Iterate over pairs of property name & value
                     // Example: `padding`, `0`
                     for (name, value) in &declarations {
                         match element_styles.entry(name.to_string()) {
                             indexmap::map::Entry::Occupied(mut entry) => {
                                 if entry.get().0 <= specificity {
```

### Comparing `css_inline-0.8.7/local_dependencies/css-inline/src/main.rs` & `css_inline-0.9.0/local_dependencies/css-inline/src/main.rs`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         };
         let options = InlineOptions {
             inline_style_tags: args.inline_style_tags,
             remove_style_tags: args.remove_style_tags,
             base_url: parse_url(args.base_url)?,
             load_remote_stylesheets: args.load_remote_stylesheets,
             extra_css: args.extra_css.as_deref().map(Cow::Borrowed),
+            ..Default::default()
         };
         let inliner = CSSInliner::new(options);
         if args.files.is_empty() {
             let mut buffer = String::new();
             io::stdin().read_to_string(&mut buffer)?;
             inliner.inline_to(buffer.as_str().trim(), &mut io::stdout())?;
         } else {
```

### Comparing `css_inline-0.8.7/local_dependencies/css-inline/src/parser.rs` & `css_inline-0.9.0/local_dependencies/css-inline/src/parser.rs`

 * *Files identical despite different names*

### Comparing `css_inline-0.8.7/Cargo.toml` & `css_inline-0.9.0/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [package]
 name = "css-inline-python"
-version = "0.8.7"
+version = "0.9.0"
 authors = ["Dmitry Dygalo <dadygalo@gmail.com>"]
 edition = "2021"
 rust-version = "1.60"
 
 [lib]
 name = "css_inline"
 crate-type = ["cdylib"]
 
 [build-dependencies]
-built = { version = "0.5", features = ["chrono"] }
+built = { version = "0.6", features = ["chrono"] }
 
 [dependencies.css-inline]
 path = "local_dependencies/css-inline"
 version = "*"
 default-features = false
 features = ["http", "file"]
 
 [dependencies]
 url = "2"
 rayon = "1"
-pyo3 = { version = "0.18.0", features = ["extension-module", "abi3-py37"] }
+pyo3 = { version = "0.19.0", features = ["extension-module", "abi3-py37"] }
 pyo3-built = "0.4"
 
 [profile.release]
 codegen-units = 1
 lto = "fat"
```

### Comparing `css_inline-0.8.7/CHANGELOG.md` & `css_inline-0.9.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.9.0] - 2023-06-10
+
+### Fixed
+
+- Serialize all HTML attributes without escaping. [#184](https://github.com/Stranger6667/css-inline/issues/184)
+
+### Changed
+
+- Update `PyO3` to `0.19.0`.
+
+### Performance
+
+- 30-50% average performance improvement due switch to a custom-built HTML tree representation and serializer.
+
 ## [0.8.7] - 2023-01-30
 
 ### Added
 
 - Distribute typing information. [#167](https://github.com/Stranger6667/css-inline/issues/167)
 
 ### Changed
@@ -232,15 +246,16 @@
 
 - Panic in cases when styles are applied to the currently processed "link" tags.
 
 ## 0.1.0 - 2020-06-24
 
 - Initial public release
 
-[Unreleased]: https://github.com/Stranger6667/css-inline/compare/python-v0.8.7...HEAD
+[Unreleased]: https://github.com/Stranger6667/css-inline/compare/python-v0.9.0...HEAD
+[0.9.0]: https://github.com/Stranger6667/css-inline/compare/python-v0.8.7...python-v0.9.0
 [0.8.7]: https://github.com/Stranger6667/css-inline/compare/python-v0.8.6...python-v0.8.7
 [0.8.6]: https://github.com/Stranger6667/css-inline/compare/python-v0.8.5...python-v0.8.6
 [0.8.5]: https://github.com/Stranger6667/css-inline/compare/python-v0.8.4...python-v0.8.5
 [0.8.4]: https://github.com/Stranger6667/css-inline/compare/python-v0.8.3...python-v0.8.4
 [0.8.3]: https://github.com/Stranger6667/css-inline/compare/python-v0.8.2...python-v0.8.3
 [0.8.2]: https://github.com/Stranger6667/css-inline/compare/python-v0.8.1...python-v0.8.2
 [0.8.1]: https://github.com/Stranger6667/css-inline/compare/python-v0.8.0...python-v0.8.1
```

### Comparing `css_inline-0.8.7/README.md` & `css_inline-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```
 
 Pre-compiled wheels for most popular platforms are provided. If your platform is not in the support table below, you will need
 a Rust compiler to build this package from source. The minimum supported Rust version is 1.60.
 
 ## Usage
 
-To inline CSS in a HTML document:
+To inline CSS in an HTML document:
 
 ```python
 import css_inline
 
 HTML = """<html>
 <head>
     <title>Test</title>
@@ -114,15 +114,15 @@
 # styles/email is relative to the current directory
 inliner = css_inline.CSSInliner(base_url="file://styles/email/")
 inliner.inline("...")
 ```
 
 ## Standards support & restrictions
 
-`css-inline` is built on top of [kuchiki](https://crates.io/crates/kuchiki) and [cssparser](https://crates.io/crates/cssparser) and relies on their behavior for HTML / CSS parsing and serialization.
+`css-inline` is built on top of [cssparser](https://crates.io/crates/cssparser) and relies on its behavior for CSS parsing.
 Notably:
 
 - Only HTML 5, XHTML is not supported;
 - Only CSS 3;
 - Only UTF-8 for string representation. Other document encodings are not yet supported.
 
 If you'd like to work around some XHTML compatibility issues like closing empty tags (`<hr>` vs. `<hr/>`), you can use the following snippet that involves `lxml`:
@@ -140,38 +140,38 @@
 ## Performance
 
 Due to the usage of efficient tooling from Mozilla's Servo project (`html5ever`, `rust-cssparser` and others) this
 library has excellent performance characteristics. In comparison with other Python projects, it is usually >10x faster than the nearest alternative.
 
 For inlining CSS in the html document from the `Usage` section above there is the following breakdown in the benchmarks:
 
-- `css_inline 0.8.2` - 22.42 us
-- `premailer 3.10.0` - 332.02 us (**x14.81**)
-- `toronado 0.1.0` - 1.59 ms (**x71.17**)
-- `inlinestyler 0.2.5` - 2.35 ms (**x105.07**)
-- `pynliner 0.8.0` - 2.79 ms (**x124.80**)
+- `css_inline 0.9.0` - 13.58 us
+- `premailer 3.10.0` - 310.06 us (**x22.83**)
+- `toronado 0.1.0` - 1.43 ms (**x105.32**)
+- `inlinestyler 0.2.5` - 2.11 ms (**x155.46**)
+- `pynliner 0.8.0` - 2.51 ms (**x184.97**)
 
 Realistic email 1:
 
-- `css_inline 0.8.2` - 487.75 us
-- `premailer 3.10.0` - 3.92 ms (**x8.05**)
-- `toronado 0.1.0` - 52.09 ms (**x106.81**)
-- `inlinestyler 0.2.5` - 81.17 ms (**x166.43**)
-- `pynliner 0.8.0` - 128.81 ms (**x264.1**)
+- `css_inline 0.9.0` - 266.53 us
+- `premailer 3.10.0` - 2.78 ms (**x10.47**)
+- `toronado 0.1.0` - 31.20 ms (**x117.09**)
+- `inlinestyler 0.2.5` - 52.64 ms (**x197.52**)
+- `pynliner 0.8.0` - 101.14 ms (**x379.47**)
 
 Realistic email 2:
 
-- `css_inline 0.8.2` - 386.64 us
-- `premailer 3.10.0` - 4.82 ms (**x12.47**)
+- `css_inline 0.9.0` - 237.23 us
+- `premailer 3.10.0` - 4.07 ms (**x17.24**)
 - `toronado 0.1.0` - `Error: Pseudo-elements are not supported`
-- `inlinestyler 0.2.5` - 40.80 ms (**x105.54**)
+- `inlinestyler 0.2.5` - 33.87 ms (**x142.81**)
 - `pynliner 0.8.0` - `Error: No match was found`
 
 You can take a look at the benchmarks' code at `benches/bench.py` file.
-The results above were measured with stable `rustc 1.64.0`, `Python 3.10.4`, `Linux x86_64` on i8700K, and 32GB RAM.
+The results above were measured with stable `rustc 1.69.0`, `Python 3.11.0`, `Linux x86_64` on i8700K, and 32GB RAM.
 
 ## Comparison with other libraries
 
 Besides performance, `css-inline` differs from other Python libraries for CSS inlining.
 
 - Generally supports more CSS features than other libraries (for example, `toronado` and `pynliner` do not support pseudo-elements);
 - It has fewer configuration options and not as flexible as `premailer`;
```

### Comparing `css_inline-0.8.7/benches/bench.py` & `css_inline-0.9.0/benches/bench.py`

 * *Files identical despite different names*

### Comparing `css_inline-0.8.7/pyproject.toml` & `css_inline-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -39,12 +39,12 @@
 requires-python = ">=3.7"
 
 [project.urls]
 homepage = "https://github.com/Stranger6667/css-inline/tree/master/bindings/python"
 repository = "https://github.com/Stranger6667/css-inline"
 
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.1"]
 build-backend = "maturin"
 
 [tool.maturin]
 strip = true
```

### Comparing `css_inline-0.8.7/src/lib.rs` & `css_inline-0.9.0/src/lib.rs`

 * *Files 18% similar despite different names*

```diff
@@ -63,41 +63,43 @@
     Ok(if let Some(url) = url {
         Some(url::Url::parse(url.as_str()).map_err(UrlError)?)
     } else {
         None
     })
 }
 
-/// CSSInliner(inline_style_tags=True, remove_style_tags=False, base_url=None, load_remote_stylesheets=True, extra_css=None)
+/// CSSInliner(inline_style_tags=True, remove_style_tags=False, base_url=None, load_remote_stylesheets=True, extra_css=None, preallocate_node_capacity=0)
 ///
 /// Customizable CSS inliner.
 #[pyclass]
-#[pyo3(
-    text_signature = "(inline_style_tags=True, remove_style_tags=False, base_url=None, load_remote_stylesheets=True, extra_css=None)"
-)]
 struct CSSInliner {
     inner: rust_inline::CSSInliner<'static>,
 }
 
 #[pymethods]
 impl CSSInliner {
-    #[new]
+    #[new(
+        text_signature = "(inline_style_tags=True, remove_style_tags=False, base_url=None, load_remote_stylesheets=True, extra_css=None, preallocate_node_capacity=0)"
+    )]
     fn new(
         inline_style_tags: Option<bool>,
         remove_style_tags: Option<bool>,
         base_url: Option<String>,
         load_remote_stylesheets: Option<bool>,
         extra_css: Option<String>,
+        preallocate_node_capacity: Option<usize>,
     ) -> PyResult<Self> {
         let options = rust_inline::InlineOptions {
             inline_style_tags: inline_style_tags.unwrap_or(true),
             remove_style_tags: remove_style_tags.unwrap_or(false),
             base_url: parse_url(base_url)?,
             load_remote_stylesheets: load_remote_stylesheets.unwrap_or(true),
             extra_css: extra_css.map(Cow::Owned),
+            preallocate_node_capacity: preallocate_node_capacity
+                .unwrap_or(rust_inline::DEFAULT_HTML_TREE_CAPACITY),
         };
         Ok(CSSInliner {
             inner: rust_inline::CSSInliner::new(options),
         })
     }
 
     /// inline(html)
@@ -127,21 +129,24 @@
 fn inline(
     html: &str,
     inline_style_tags: Option<bool>,
     remove_style_tags: Option<bool>,
     base_url: Option<String>,
     load_remote_stylesheets: Option<bool>,
     extra_css: Option<&str>,
+    preallocate_node_capacity: Option<usize>,
 ) -> PyResult<String> {
     let options = rust_inline::InlineOptions {
         inline_style_tags: inline_style_tags.unwrap_or(true),
         remove_style_tags: remove_style_tags.unwrap_or(false),
         base_url: parse_url(base_url)?,
         load_remote_stylesheets: load_remote_stylesheets.unwrap_or(true),
         extra_css: extra_css.map(Cow::Borrowed),
+        preallocate_node_capacity: preallocate_node_capacity
+            .unwrap_or(rust_inline::DEFAULT_HTML_TREE_CAPACITY),
     };
     let inliner = rust_inline::CSSInliner::new(options);
     Ok(inliner.inline(html).map_err(InlineErrorWrapper)?)
 }
 
 /// inline_many(htmls, inline_style_tags=True, remove_style_tags=False, base_url=None, load_remote_stylesheets=True, extra_css=None)
 ///
@@ -153,21 +158,24 @@
 fn inline_many(
     htmls: &PyList,
     inline_style_tags: Option<bool>,
     remove_style_tags: Option<bool>,
     base_url: Option<String>,
     load_remote_stylesheets: Option<bool>,
     extra_css: Option<&str>,
+    preallocate_node_capacity: Option<usize>,
 ) -> PyResult<Vec<String>> {
     let options = rust_inline::InlineOptions {
         inline_style_tags: inline_style_tags.unwrap_or(true),
         remove_style_tags: remove_style_tags.unwrap_or(false),
         base_url: parse_url(base_url)?,
         load_remote_stylesheets: load_remote_stylesheets.unwrap_or(true),
         extra_css: extra_css.map(Cow::Borrowed),
+        preallocate_node_capacity: preallocate_node_capacity
+            .unwrap_or(rust_inline::DEFAULT_HTML_TREE_CAPACITY),
     };
     let inliner = rust_inline::CSSInliner::new(options);
     inline_many_impl(&inliner, htmls)
 }
 
 fn inline_many_impl(
     inliner: &rust_inline::CSSInliner<'_>,
```

### Comparing `css_inline-0.8.7/tests-py/test_inlining.py` & `css_inline-0.9.0/tests-py/test_inlining.py`

 * *Files identical despite different names*

### Comparing `css_inline-0.8.7/Cargo.lock` & `css_inline-0.9.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,33 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "attohttpc"
-version = "0.24.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b85f766c20e6ae766956f7a2fcc4e0931e79a7e1f48b29132b5d647021114914"
+checksum = "7e57d6e7a84f33ff3316e97af3180fe7f86597a6a60161c0be70c0e45f382620"
 dependencies = [
  "flate2",
  "http",
  "log",
  "rustls",
  "url",
  "webpki",
@@ -42,39 +48,39 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "built"
-version = "0.5.2"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9c056b9ed43aee5e064b683aa1ec783e19c6acec7559e3ae931b7490472fbe"
+checksum = "96f9cdd34d6eb553f9ea20e5bf84abb7b13c729f113fc1d8e49dc00ad9fa8738"
 dependencies = [
  "cargo-lock",
  "chrono",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
 name = "bytes"
-version = "1.3.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfb24e866b15a1af2a1b663f10c6b6b8f397a84aadb828f12e5b289ec23a3a3c"
+checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
 [[package]]
 name = "cargo-lock"
 version = "8.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "031718ddb8f78aa5def78a09e90defe30151d1f6c672f937af4dd916429ed996"
 dependencies = [
@@ -94,266 +100,196 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.23"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b0a3d9ed01224b22057780a37bb8c5dbfe1be8ba48678e7bf57ec4b385411f"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
- "num-integer",
  "num-traits",
  "winapi",
 ]
 
 [[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
-
-[[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.6"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "715e8152b692bba2d374b53d4875445368fdf21a94751410af607a5ac677d1fc"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
 dependencies = [
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.13"
+version = "0.9.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01a9af1f4c2ef74bb8aa1f7e19706bc72d03598c8a570bb5de72243c7a9d9d5a"
+checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.7.1",
+ "memoffset 0.8.0",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.14"
+version = "0.8.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
+checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "css-inline"
-version = "0.8.5"
+version = "0.9.0"
 dependencies = [
  "attohttpc",
- "cssparser 0.29.6",
+ "cssparser",
+ "html5ever",
  "indexmap",
- "kuchiki",
  "memchr",
+ "selectors",
  "smallvec",
  "url",
 ]
 
 [[package]]
 name = "css-inline-python"
-version = "0.8.7"
+version = "0.9.0"
 dependencies = [
  "built",
  "css-inline",
  "pyo3",
  "pyo3-built",
  "rayon",
  "url",
 ]
 
 [[package]]
 name = "cssparser"
-version = "0.27.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "754b69d351cdc2d8ee09ae203db831e005560fc6030da058f86ad60c92a9cb0a"
-dependencies = [
- "cssparser-macros",
- "dtoa-short",
- "itoa 0.4.8",
- "matches",
- "phf 0.8.0",
- "proc-macro2",
- "quote",
- "smallvec",
- "syn",
-]
-
-[[package]]
-name = "cssparser"
 version = "0.29.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f93d03419cb5950ccfd3daf3ff1c7a36ace64609a1a8746d493df1ca0afde0fa"
 dependencies = [
  "cssparser-macros",
  "dtoa-short",
- "itoa 1.0.5",
+ "itoa",
  "matches",
  "phf 0.10.1",
  "proc-macro2",
  "quote",
  "smallvec",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "cssparser-macros"
-version = "0.6.0"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfae75de57f2b2e85e8768c3ea840fd159c8f33e2b6522c7835b7abac81be16e"
+checksum = "13b588ba4ac1a99f7f2964d24b3d896ddc6bf847ee3855dbd4366f058cfcd331"
 dependencies = [
  "quote",
- "syn",
-]
-
-[[package]]
-name = "cxx"
-version = "1.0.88"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "322296e2f2e5af4270b54df9e85a02ff037e271af20ba3e7fe1575515dc840b8"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.88"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "017a1385b05d631e7875b1f151c9f012d37b53491e2a87f65bff5c262b2111d8"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.88"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c26bbb078acf09bc1ecda02d4223f03bdd28bd4874edcb0379138efc499ce971"
-
-[[package]]
-name = "cxxbridge-macro"
-version = "1.0.88"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "357f40d1f06a24b60ae1fe122542c1fb05d28d32acb2aed064e84bc2ad1e252e"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
 dependencies = [
  "convert_case",
  "proc-macro2",
  "quote",
  "rustc_version",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "dtoa"
-version = "0.4.8"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56899898ce76aaf4a0f24d914c97ea6ed976d42fec6ad33fcbb0a1103e07b2b0"
+checksum = "65d09067bfacaa79114679b279d7f5885b53295b1e2cfb4e79c8e4bd3d633169"
 
 [[package]]
 name = "dtoa-short"
-version = "0.3.3"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bde03329ae10e79ede66c9ce4dc930aa8599043b0743008548680f25b91502d6"
+checksum = "dbaceec3c6e4211c79e7b1800fb9680527106beb2f9c51904a3210c03a448c74"
 dependencies = [
  "dtoa",
 ]
 
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "futf"
 version = "0.1.5"
@@ -382,17 +318,17 @@
  "cfg-if",
  "libc",
  "wasi 0.9.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
@@ -408,169 +344,138 @@
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "html5ever"
-version = "0.25.2"
+version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5c13fb08e5d4dfc151ee5e88bae63f7773d61852f3bdc73c9f4b9e1bde03148"
+checksum = "bea68cab48b8459f17cf1c944c67ddc572d272d9f2b274140f223ecb1da4a3b7"
 dependencies = [
  "log",
  "mac",
  "markup5ever",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75f43d41e26995c17e71ee126451dd3941010b0514a81a9d11f3b341debc2399"
+checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
 dependencies = [
  "bytes",
  "fnv",
- "itoa 1.0.5",
+ "itoa",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.53"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64c122667b287044802d6ce17ee2ddf13207ed924c712de9a66a5814d5b64765"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "winapi",
+ "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itoa"
-version = "0.4.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b71991ff56294aa922b450139ee08b3bfc70982c6b2c7562771375cf73542dd4"
-
-[[package]]
-name = "itoa"
-version = "1.0.5"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.60"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "kuchiki"
-version = "0.8.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ea8e9c6e031377cff82ee3001dc8026cdf431ed4e2e6b51f98ab8c73484a358"
-dependencies = [
- "cssparser 0.27.2",
- "html5ever",
- "matches",
- "selectors",
-]
-
-[[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
-
-[[package]]
-name = "link-cplusplus"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "mac"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c41e0c4fef86961ac6d6f8a82609f55f31b05e4fce149ac5710e439df7619ba4"
 
 [[package]]
 name = "markup5ever"
-version = "0.10.1"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a24f40fb03852d1cdd84330cddcaf98e9ec08a7b7768e952fad3b4cf048ec8fd"
+checksum = "7a2629bb1404f3d34c2e921f21fd34ba00b206124c81f65c50b43b6aaefeb016"
 dependencies = [
  "log",
- "phf 0.8.0",
- "phf_codegen",
+ "phf 0.10.1",
+ "phf_codegen 0.10.0",
  "string_cache",
  "string_cache_codegen",
  "tendril",
 ]
 
 [[package]]
 name = "matches"
@@ -582,35 +487,35 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.7.1"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "new_debug_unreachable"
 version = "1.0.4"
@@ -620,24 +525,14 @@
 [[package]]
 name = "nodrop"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72ef4a56884ca558e5ddb05a1d1e7e1bfd9a68d9ed024c21704cc98872dae1bb"
 
 [[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
@@ -650,65 +545,63 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.6"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba1ef8814b5c993410bb3adfad7a5ed269563e4a2f90c41f5d85be7fb47133bf"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "phf"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3dfb61232e34fcb633f43d12c58f83c1df82962dcdfa565a4e866ffc17dafe12"
 dependencies = [
- "phf_macros 0.8.0",
  "phf_shared 0.8.0",
- "proc-macro-hack",
 ]
 
 [[package]]
 name = "phf"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fabbf1ead8a5bcbc20f5f8b939ee3f5b0f6f281b6ad3468b84656b658b455259"
 dependencies = [
- "phf_macros 0.10.0",
+ "phf_macros",
  "phf_shared 0.10.0",
  "proc-macro-hack",
 ]
 
 [[package]]
 name = "phf_codegen"
 version = "0.8.0"
@@ -716,14 +609,24 @@
 checksum = "cbffee61585b0411840d3ece935cce9cb6321f01c45477d30066498cd5e1a815"
 dependencies = [
  "phf_generator 0.8.0",
  "phf_shared 0.8.0",
 ]
 
 [[package]]
+name = "phf_codegen"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4fb1c3a8bc4dd4e5cfce29b44ffc14bedd2ee294559a294e2a4d4c9e9a6a13cd"
+dependencies = [
+ "phf_generator 0.10.0",
+ "phf_shared 0.10.0",
+]
+
+[[package]]
 name = "phf_generator"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17367f0cc86f2d25802b2c26ee58a7b23faeccf78a396094c13dced0d0182526"
 dependencies = [
  "phf_shared 0.8.0",
  "rand 0.7.3",
@@ -737,38 +640,24 @@
 dependencies = [
  "phf_shared 0.10.0",
  "rand 0.8.5",
 ]
 
 [[package]]
 name = "phf_macros"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f6fde18ff429ffc8fe78e2bf7f8b7a5a5a6e2a8b58bc5a9ac69198bbda9189c"
-dependencies = [
- "phf_generator 0.8.0",
- "phf_shared 0.8.0",
- "proc-macro-hack",
- "proc-macro2",
- "quote",
- "syn",
-]
-
-[[package]]
-name = "phf_macros"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "58fdf3184dd560f160dd73922bea2d5cd6e8f064bf4b13110abd81b03697b4e0"
 dependencies = [
  "phf_generator 0.10.0",
  "phf_shared 0.10.0",
  "proc-macro-hack",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "phf_shared"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c00cf8b9eafe68dde5e9eaa2cef8ee84a9336a47d566ec55ca16589633b65af7"
@@ -801,92 +690,92 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.50"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ef7d57beacfaf2d8aee5937dab7b7f28de3cb8b1828479bb5de2a7106f2bae2"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccd4149c8c3975099622b4e1962dac27565cf5663b76452c3e2b66e0b6824277"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.8.0",
+ "memoffset 0.9.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cd09fe469834db21ee60e0051030339e5d361293d8cb5ec02facf7fdcf52dbf"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-built"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be6d574e0f8cab2cdd1eeeb640cbf845c974519fa9e9b62fa9c08ecece0ca5de"
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c427c9a96b9c5b12156dbc11f76b14f49e9aae8905ca783ea87c249044ef137"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b822bbba9d60630a44d2109bc410489bb2f439b33e3a14ddeb8a40b378a7c4"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84ae898104f7c99db06231160770f3e40dad6eb9021daddc0fedfa3e41dff10a"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.7.3"
@@ -943,15 +832,15 @@
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.10",
 ]
 
 [[package]]
 name = "rand_hc"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
@@ -966,39 +855,39 @@
 checksum = "16abd0c1b639e9eb4d7c50c0b8100b0d0f849be2349829c740fe8e6eb4816429"
 dependencies = [
  "rand_core 0.5.1",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db3a213adf02b3bcfd2d3846bb41cb22857d131789e01df434fb7e7bc0759b7"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.10.2"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "356a0625f1954f730c0201cdab48611198dc6ce21f4acff55089b5a78e6e835b"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "ring"
 version = "0.16.20"
@@ -1021,100 +910,102 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.20.8"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fff78fc74d175294f4e83b28343315ffcfb114b156f0185e9741cb5570f50e2f"
+checksum = "c911ba11bc8433e811ce56fde130ccf32f5127cab0e0194e9c68c5a5b671791e"
 dependencies = [
  "log",
  "ring",
+ "rustls-webpki",
  "sct",
- "webpki",
 ]
 
 [[package]]
-name = "scopeguard"
-version = "1.1.0"
+name = "rustls-webpki"
+version = "0.100.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "d6207cd5ed3d8dca7816f8f3725513a34609c0c765bf652b8c3cb4cfd87db46b"
+dependencies = [
+ "ring",
+ "untrusted",
+]
 
 [[package]]
-name = "scratch"
-version = "1.0.3"
+name = "scopeguard"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddccb15bcce173023b3fedd9436f882a0739b8dfb45e4f6b6002bee5929f61b2"
+checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "sct"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "selectors"
-version = "0.22.0"
+version = "0.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df320f1889ac4ba6bc0cdc9c9af7af4bd64bb927bccdf32d81140dc1f9be12fe"
+checksum = "0c37578180969d00692904465fb7f6b3d50b9a2b952b87c23d0e2e5cb5013416"
 dependencies = [
  "bitflags",
- "cssparser 0.27.2",
+ "cssparser",
  "derive_more",
  "fxhash",
  "log",
- "matches",
  "phf 0.8.0",
- "phf_codegen",
+ "phf_codegen 0.8.0",
  "precomputed-hash",
  "servo_arc",
  "smallvec",
- "thin-slice",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58bc9567378fc7690d6b2addae4e60ac2eeea07becb2c64b9f218b53865cba2a"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "servo_arc"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d98238b800e0d1576d8b6e3de32827c2d74bee68bb97748dcf5071fb53965432"
+checksum = "d52aa42f8fdf0fed91e5ce7f23d8138441002fa31dca008acf47e6fd4721f741"
 dependencies = [
  "nodrop",
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "siphasher"
@@ -1138,17 +1029,17 @@
 name = "stable_deref_trait"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
 
 [[package]]
 name = "string_cache"
-version = "0.8.4"
+version = "0.8.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213494b7a2b503146286049378ce02b482200519accc31872ee8be91fa820a08"
+checksum = "f91138e76242f575eb1d3b38b4f1362f10d3a43f47d182a5b359af488a02293b"
 dependencies = [
  "new_debug_unreachable",
  "once_cell",
  "parking_lot",
  "phf_shared 0.10.0",
  "precomputed-hash",
  "serde",
@@ -1164,123 +1055,113 @@
  "phf_shared 0.10.0",
  "proc-macro2",
  "quote",
 ]
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tendril"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d24a120c5fc464a3458240ee02c299ebcb9d67b5249c8848b09d639dca8d7bb0"
 dependencies = [
  "futf",
  "mac",
  "utf-8",
 ]
 
 [[package]]
-name = "termcolor"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
-dependencies = [
- "winapi-util",
-]
-
-[[package]]
-name = "thin-slice"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8eaa81235c7058867fa8c0e7314f33dcce9c215f535d1913822a2b3f5e289f3c"
-
-[[package]]
 name = "tinyvec"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
 dependencies = [
  "tinyvec_macros",
 ]
 
 [[package]]
 name = "tinyvec_macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cda74da7e1a664f795bb1f8a87ec406fb89a02522cf6e50620d016add6dbbf5c"
+checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "toml"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.10"
+version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d54675592c1dbefd78cbd98db9bacd89886e1ca50692a0692baefffdeb92dd58"
+checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
-name = "unicode-width"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
-
-[[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
@@ -1299,71 +1180,71 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.83"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
 name = "web-sys"
-version = "0.3.60"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcda906d8be16e728fd5adc5b729afad4e444e106ab28cd1c7256e54fa61510f"
+checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki"
@@ -1373,19 +1254,19 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "webpki-roots"
-version = "0.22.6"
+version = "0.23.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6c71e40d7d2c34a5106301fb632274ca37242cd0c9d3e64dbece371a40a2d87"
+checksum = "b03058f88386e5ff5310d9111d53f48b17d732b401aeb83a8d5190f2ac459338"
 dependencies = [
- "webpki",
+ "rustls-webpki",
 ]
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
@@ -1397,77 +1278,77 @@
 [[package]]
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
-name = "winapi-util"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
-dependencies = [
- "winapi",
-]
-
-[[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `css_inline-0.8.7/PKG-INFO` & `css_inline-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: css-inline
-Version: 0.8.7
+Version: 0.9.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Rust
 Summary: Fast CSS inlining written in Rust
 Author: Dmitry Dygalo <dadygalo@gmail.com>
 Author-email: Dmitry Dygalo <dadygalo@gmail.com>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/Stranger6667/css-inline
 Project-URL: homepage, https://github.com/Stranger6667/css-inline/tree/master/bindings/python
+Project-URL: repository, https://github.com/Stranger6667/css-inline
 
 # css_inline
 
 [![Build](https://github.com/Stranger6667/css-inline/workflows/ci/badge.svg)](https://github.com/Stranger6667/css-inline/actions)
 [![PyPI](https://img.shields.io/pypi/v/css_inline.svg)](https://pypi.org/project/css_inline/)
 [![Python versions](https://img.shields.io/pypi/pyversions/css_inline.svg)](https://pypi.org/project/css_inline/)
 [![License](https://img.shields.io/pypi/l/css_inline.svg)](https://opensource.org/licenses/MIT)
@@ -53,15 +53,15 @@
 ```
 
 Pre-compiled wheels for most popular platforms are provided. If your platform is not in the support table below, you will need
 a Rust compiler to build this package from source. The minimum supported Rust version is 1.60.
 
 ## Usage
 
-To inline CSS in a HTML document:
+To inline CSS in an HTML document:
 
 ```python
 import css_inline
 
 HTML = """<html>
 <head>
     <title>Test</title>
@@ -141,15 +141,15 @@
 # styles/email is relative to the current directory
 inliner = css_inline.CSSInliner(base_url="file://styles/email/")
 inliner.inline("...")
 ```
 
 ## Standards support & restrictions
 
-`css-inline` is built on top of [kuchiki](https://crates.io/crates/kuchiki) and [cssparser](https://crates.io/crates/cssparser) and relies on their behavior for HTML / CSS parsing and serialization.
+`css-inline` is built on top of [cssparser](https://crates.io/crates/cssparser) and relies on its behavior for CSS parsing.
 Notably:
 
 - Only HTML 5, XHTML is not supported;
 - Only CSS 3;
 - Only UTF-8 for string representation. Other document encodings are not yet supported.
 
 If you'd like to work around some XHTML compatibility issues like closing empty tags (`<hr>` vs. `<hr/>`), you can use the following snippet that involves `lxml`:
@@ -167,38 +167,38 @@
 ## Performance
 
 Due to the usage of efficient tooling from Mozilla's Servo project (`html5ever`, `rust-cssparser` and others) this
 library has excellent performance characteristics. In comparison with other Python projects, it is usually >10x faster than the nearest alternative.
 
 For inlining CSS in the html document from the `Usage` section above there is the following breakdown in the benchmarks:
 
-- `css_inline 0.8.2` - 22.42 us
-- `premailer 3.10.0` - 332.02 us (**x14.81**)
-- `toronado 0.1.0` - 1.59 ms (**x71.17**)
-- `inlinestyler 0.2.5` - 2.35 ms (**x105.07**)
-- `pynliner 0.8.0` - 2.79 ms (**x124.80**)
+- `css_inline 0.9.0` - 13.58 us
+- `premailer 3.10.0` - 310.06 us (**x22.83**)
+- `toronado 0.1.0` - 1.43 ms (**x105.32**)
+- `inlinestyler 0.2.5` - 2.11 ms (**x155.46**)
+- `pynliner 0.8.0` - 2.51 ms (**x184.97**)
 
 Realistic email 1:
 
-- `css_inline 0.8.2` - 487.75 us
-- `premailer 3.10.0` - 3.92 ms (**x8.05**)
-- `toronado 0.1.0` - 52.09 ms (**x106.81**)
-- `inlinestyler 0.2.5` - 81.17 ms (**x166.43**)
-- `pynliner 0.8.0` - 128.81 ms (**x264.1**)
+- `css_inline 0.9.0` - 266.53 us
+- `premailer 3.10.0` - 2.78 ms (**x10.47**)
+- `toronado 0.1.0` - 31.20 ms (**x117.09**)
+- `inlinestyler 0.2.5` - 52.64 ms (**x197.52**)
+- `pynliner 0.8.0` - 101.14 ms (**x379.47**)
 
 Realistic email 2:
 
-- `css_inline 0.8.2` - 386.64 us
-- `premailer 3.10.0` - 4.82 ms (**x12.47**)
+- `css_inline 0.9.0` - 237.23 us
+- `premailer 3.10.0` - 4.07 ms (**x17.24**)
 - `toronado 0.1.0` - `Error: Pseudo-elements are not supported`
-- `inlinestyler 0.2.5` - 40.80 ms (**x105.54**)
+- `inlinestyler 0.2.5` - 33.87 ms (**x142.81**)
 - `pynliner 0.8.0` - `Error: No match was found`
 
 You can take a look at the benchmarks' code at `benches/bench.py` file.
-The results above were measured with stable `rustc 1.64.0`, `Python 3.10.4`, `Linux x86_64` on i8700K, and 32GB RAM.
+The results above were measured with stable `rustc 1.69.0`, `Python 3.11.0`, `Linux x86_64` on i8700K, and 32GB RAM.
 
 ## Comparison with other libraries
 
 Besides performance, `css-inline` differs from other Python libraries for CSS inlining.
 
 - Generally supports more CSS features than other libraries (for example, `toronado` and `pynliner` do not support pseudo-elements);
 - It has fewer configuration options and not as flexible as `premailer`;
```

