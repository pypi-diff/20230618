# Comparing `tmp/tamp-1.1.2.tar.gz` & `tmp/tamp-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamp-1.1.2.tar", max compression
+gzip compressed data, was "tamp-1.1.3.tar", max compression
```

## Comparing `tamp-1.1.2.tar` & `tamp-1.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-06-15 21:03:04.536048 tamp-1.1.2/LICENSE
--rw-r--r--   0        0        0    17339 2023-06-15 21:03:04.536048 tamp-1.1.2/README.rst
--rw-r--r--   0        0        0     2851 2023-06-15 21:03:04.540048 tamp-1.1.2/build.py
--rw-r--r--   0        0        0     5577 2023-06-15 21:03:33.391772 tamp-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2806 2023-06-15 21:03:33.395772 tamp-1.1.2/tamp/__init__.py
--rw-r--r--   0        0        0     1619 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/__init__.pyi
--rw-r--r--   0        0        0       57 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/__main__.py
--rw-r--r--   0        0        0       65 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_common.pxd
--rw-r--r--   0        0        0      343 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_common.pyx
--rw-r--r--   0        0        0     4498 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_compressor.pyx
--rw-r--r--   0        0        0     4168 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_decompressor.pyx
--rw-r--r--   0        0        0      834 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/common.c
--rw-r--r--   0        0        0     1791 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/common.h
--rw-r--r--   0        0        0    11680 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/compressor.c
--rw-r--r--   0        0        0     5468 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/compressor.h
--rw-r--r--   0        0        0     8976 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/decompressor.c
--rw-r--r--   0        0        0     2524 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/decompressor.h
--rw-r--r--   0        0        0        0 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/cli/__init__.py
--rw-r--r--   0        0        0     2715 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/cli/main.py
--rw-r--r--   0        0        0     8656 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/compressor.py
--rw-r--r--   0        0        0     7257 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/compressor_viper.py
--rw-r--r--   0        0        0     2802 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/ctamp.pxd
--rw-r--r--   0        0        0     7882 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/decompressor.py
--rw-r--r--   0        0        0     9681 2023-06-15 21:03:04.548048 tamp-1.1.2/tamp/decompressor_viper.py
--rw-r--r--   0        0        0        0 2023-06-15 21:03:04.548048 tamp-1.1.2/tamp/py.typed
--rw-r--r--   0        0        0    17951 1970-01-01 00:00:00.000000 tamp-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-18 01:50:59.167596 tamp-1.1.3/LICENSE
+-rw-r--r--   0        0        0    17337 2023-06-18 01:50:59.167596 tamp-1.1.3/README.rst
+-rw-r--r--   0        0        0     2851 2023-06-18 01:50:59.167596 tamp-1.1.3/build.py
+-rw-r--r--   0        0        0     5577 2023-06-18 01:51:23.343887 tamp-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2806 2023-06-18 01:51:23.343887 tamp-1.1.3/tamp/__init__.py
+-rw-r--r--   0        0        0     1619 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/__init__.pyi
+-rw-r--r--   0        0        0       57 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/__main__.py
+-rw-r--r--   0        0        0       65 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/_c_common.pxd
+-rw-r--r--   0        0        0      343 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/_c_common.pyx
+-rw-r--r--   0        0        0     4498 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/_c_compressor.pyx
+-rw-r--r--   0        0        0     4168 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/_c_decompressor.pyx
+-rw-r--r--   0        0        0      850 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/_c_src/tamp/common.c
+-rw-r--r--   0        0        0     1791 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/_c_src/tamp/common.h
+-rw-r--r--   0        0        0    12242 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/_c_src/tamp/compressor.c
+-rw-r--r--   0        0        0     5805 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/_c_src/tamp/compressor.h
+-rw-r--r--   0        0        0     9591 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/_c_src/tamp/decompressor.c
+-rw-r--r--   0        0        0     2787 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/_c_src/tamp/decompressor.h
+-rw-r--r--   0        0        0        0 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/cli/__init__.py
+-rw-r--r--   0        0        0     2715 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/cli/main.py
+-rw-r--r--   0        0        0     8656 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/compressor.py
+-rw-r--r--   0        0        0     7257 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/compressor_viper.py
+-rw-r--r--   0        0        0     2802 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/ctamp.pxd
+-rw-r--r--   0        0        0     7882 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/decompressor.py
+-rw-r--r--   0        0        0     9681 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/decompressor_viper.py
+-rw-r--r--   0        0        0        0 2023-06-18 01:50:59.171596 tamp-1.1.3/tamp/py.typed
+-rw-r--r--   0        0        0    17949 1970-01-01 00:00:00.000000 tamp-1.1.3/PKG-INFO
```

### Comparing `tamp-1.1.2/LICENSE` & `tamp-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/README.rst` & `tamp-1.1.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     * ``tamp/_c_src/``
 
 * High compression ratios and low memory use.
 
 * Compact compression and decompression implementations.
 
-  * Compiled C library is <7.5KB (compressor + decompressor).
+  * Compiled C library is <4KB (compressor + decompressor).
 
 * Mid-stream flushing.
 
   * Allows for submission of messages while continuing to compress subsequent data.
 
 * Customizable dictionary for greater compression of small messages.
 
@@ -285,15 +285,15 @@
 
 +---------------+--------------------+-------+------+--------------+-----------------+
 | Action        | tamp               | tamp  | zlib | heatshrink   | heatshrink      |
 |               | (Python Reference) | (C)   |      | (with index) | (without index) |
 +===============+====================+=======+======+==============+=================+
 | Compression   | 109.5              | 16.45 | 4.84 | 6.22         | 41.729          |
 +---------------+--------------------+-------+------+--------------+-----------------+
-| Decompression | 54.0               | 0.98  | 0.08 | 0.82         | 0.82            |
+| Decompression | 54.0               | 0.70  | 0.98 | 0.82         | 0.82            |
 +---------------+--------------------+-------+------+--------------+-----------------+
 
 Heatshrink v0.4.1 was used in these benchmarks.
 When heathshrink uses an index, an additional ``(1 << (windowBits + 1))`` bytes of memory are used, tripling the memory requirement.
 Tamp could use a similar indexing to increase compression speed, but has chosen not to to focus on the primary goal of a low-memory compressor.
 
 Binary Size
@@ -303,15 +303,15 @@
 Numbers reported in bytes.
 
 +--------------------+------------+--------------+---------------------------+
 | Library            | Compressor | Decompressor | Compressor + Decompressor |
 +====================+============+==============+===========================+
 | Tamp (micropython) | 4779       | 4717         | 8262                      |
 +--------------------+------------+--------------+---------------------------+
-| Tamp (C)           | 2996       | 2192         | 5064                      |
+| Tamp (C)           | 2008       | 1976         | 3848                      |
 +--------------------+------------+--------------+---------------------------+
 | Heatshrink         | 2956       | 3876         | 6832                      |
 +--------------------+------------+--------------+---------------------------+
 | uzlib              | 2355       | 3963         | 6318                      |
 +--------------------+------------+--------------+---------------------------+
 
 Heatshrink doesn't include a high level API; in an apples-to-apples comparison the Tamp library would be even smaller.
```

### Comparing `tamp-1.1.2/build.py` & `tamp-1.1.3/build.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/pyproject.toml` & `tamp-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "tamp"
-version = "1.1.2"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "1.1.3"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/tamp"
 repository = "https://github.com/BrianPugh/tamp"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.rst"
 packages = [{include = "tamp"}]
```

### Comparing `tamp-1.1.2/tamp/__init__.py` & `tamp-1.1.3/tamp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Don't manually change, let poetry-dynamic-versioning-plugin handle it.
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 
 class ExcessBitsError(Exception):
     """Provided data has more bits than expected ``literal`` bits."""
 
 
 def bit_size(value):
```

### Comparing `tamp-1.1.2/tamp/__init__.pyi` & `tamp-1.1.3/tamp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/tamp/_c_compressor.pyx` & `tamp-1.1.3/tamp/_c_compressor.pyx`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/tamp/_c_decompressor.pyx` & `tamp-1.1.3/tamp/_c_decompressor.pyx`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/tamp/_c_src/tamp/common.c` & `tamp-1.1.3/tamp/_c_src/tamp/common.c`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 }
 
 
 void tamp_initialize_dictionary(unsigned char *buffer, size_t size){
     uint32_t seed = 3758097560;
     uint32_t randbuf = 0;
     for(size_t i=0; i < size; i++){
-        if( (i & 0x7) == 0)
+        if( TAMP_UNLIKELY((i & 0x7) == 0) )
             randbuf = xorshift32(&seed);
         buffer[i] = common_characters[randbuf & 0x0F];
         randbuf >>= 4;
     }
 }
```

### Comparing `tamp-1.1.2/tamp/_c_src/tamp/common.h` & `tamp-1.1.3/tamp/_c_src/tamp/common.h`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/tamp/_c_src/tamp/compressor.c` & `tamp-1.1.3/tamp/_c_src/tamp/compressor.c`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 #include <stdbool.h>
 
 #define MAX(x, y) (((x) > (y)) ? (x) : (y))
 #define MIN(x, y) (((x) < (y)) ? (x) : (y))
 #define BUILD_BUG_ON(condition) ((void)sizeof(char[1 - 2*!!(condition)]))
 
 #define MAX_PATTERN_SIZE (compressor->min_pattern_size + 13)
-#define WINDOW_SIZE (1 << compressor->conf.window)
+#define WINDOW_SIZE (1 << compressor->conf_window)
 // 0xF because sizeof(TampCompressor.input) == 16;
 #define input_add(offset) (\
             (compressor->input_pos + offset) & 0xF \
         )
 #define read_input(offset) ( \
         compressor->input[input_add(offset)] \
         )
-#define IS_LITERAL_FLAG (1 << compressor->conf.literal)
+#define IS_LITERAL_FLAG (1 << compressor->conf_literal)
 
 #define FLUSH_CODE (0xAB)
 
 // encodes [min_pattern_bytes, min_pattern_bytes + 13] pattern lengths
 static const unsigned char huffman_codes[] = {
     0x0, 0x3, 0x8, 0xb, 0x14, 0x24, 0x26, 0x2b, 0x4b, 0x54, 0x94, 0x95, 0xaa, 0x27
 };
@@ -35,31 +35,25 @@
 }
 
 /**
  * @brief Partially flush the internal bit buffer.
  *
  * Up to 7 bits may remain in the internal bit buffer.
  */
-static inline tamp_res partial_flush(TampCompressor *compressor, unsigned char *output, size_t output_size, size_t *output_written_size){
-    *output_written_size = output_size;
-
-    while(compressor->bit_buffer_pos >= 8 && output_size){
-        *output = compressor->bit_buffer >> 24;
-        output++;
-        output_size--;
-        compressor->bit_buffer <<= 8;
-        compressor->bit_buffer_pos -= 8;
-    }
-    (*output_written_size) -= output_size;
-    if(compressor->bit_buffer_pos >= 8)
-        return TAMP_OUTPUT_FULL;
-    return TAMP_OK;
+static inline tamp_res partial_flush(TampCompressor *compressor, unsigned char *output, size_t output_size, size_t *output_written_size) {
+    for (
+        *output_written_size = output_size;
+        compressor->bit_buffer_pos >= 8 && output_size;
+        output_size--, compressor->bit_buffer_pos -= 8, compressor->bit_buffer <<= 8
+        )
+        *output++ = compressor->bit_buffer >> 24;
+    *output_written_size -= output_size;
+    return (compressor->bit_buffer_pos >= 8) ? TAMP_OUTPUT_FULL : TAMP_OK;
 }
 
-
 /**
  * @brief Find the best match for the current input buffer.
  *
  * WARNING: this optimized implementation expects a little endian system.
  *
  * @param[in,out] compressor TampCompressor object to perform search on.
  * @param[out] match_index  If match_size is 0, this value is undefined.
@@ -74,22 +68,23 @@
 
     if(TAMP_UNLIKELY(compressor->input_size < compressor->min_pattern_size))
         return;
 
     const uint16_t first_second = (read_input(0) << 8) | read_input(1);
     const uint16_t window_size_minus_1 = WINDOW_SIZE - 1;
     const uint8_t max_pattern_size = MIN(compressor->input_size, MAX_PATTERN_SIZE);
-    uint16_t meow = compressor->window[0];
+    uint16_t window_rolling_2_byte = compressor->window[0];
     unsigned char c;
 
     for(uint16_t window_index=0; window_index < window_size_minus_1; window_index++){
-        meow <<= 8;
-        meow |= compressor->window[window_index + 1];
-        if(TAMP_LIKELY(meow != first_second))
+        window_rolling_2_byte <<= 8;
+        window_rolling_2_byte |= compressor->window[window_index + 1];
+        if(TAMP_LIKELY(window_rolling_2_byte != first_second)){
             continue;
+        }
 
         for(uint8_t input_offset=2; ; input_offset++){
             if(TAMP_UNLIKELY(input_offset > *match_size)){
                 *match_size = input_offset;
                 *match_index = window_index;
                 if(TAMP_UNLIKELY(*match_size == max_pattern_size))
                     return;
@@ -113,19 +108,22 @@
         return TAMP_INVALID_CONF;
     if( conf->literal < 5 || conf->literal > 8)
         return TAMP_INVALID_CONF;
 
     for(uint8_t i=0; i < sizeof(TampCompressor); i++)  // Zero-out the struct
         ((unsigned char *)compressor)[i] = 0;
 
-    compressor->conf = *conf;
+    compressor->conf_literal = conf->literal;
+    compressor->conf_window = conf->window;
+    compressor->conf_use_custom_dictionary = conf->use_custom_dictionary;
+
     compressor->window = window;
     compressor->min_pattern_size = tamp_compute_min_pattern_size(conf->window, conf->literal);
 
-    if(!compressor->conf.use_custom_dictionary)
+    if(!compressor->conf_use_custom_dictionary)
         tamp_initialize_dictionary(window, (1 << conf->window));
 
     // Write header to bit buffer
     write_to_bit_buffer(compressor, conf->window - 8, 3);
     write_to_bit_buffer(compressor, conf->literal - 5, 2);
     write_to_bit_buffer(compressor, conf->use_custom_dictionary, 1);
     write_to_bit_buffer(compressor, 0, 1);  // Reserved
@@ -133,123 +131,129 @@
 
     return TAMP_OK;
 }
 
 
 tamp_res tamp_compressor_compress_poll(TampCompressor *compressor, unsigned char *output, size_t output_size, size_t *output_written_size){
     tamp_res res;
-    const uint16_t window_mask = (1 << compressor->conf.window) - 1;
+    const uint16_t window_mask = (1 << compressor->conf_window) - 1;
     size_t output_written_size_proxy;
 
     if(!output_written_size)
         output_written_size = &output_written_size_proxy;
     *output_written_size = 0;
 
-    if(compressor->input_size == 0)
+    if(TAMP_UNLIKELY(compressor->input_size == 0))
         return TAMP_OK;
 
     {
         // Make sure there's enough room in the bit buffer.
         size_t flush_bytes_written;
         res = partial_flush(compressor, output, output_size, &flush_bytes_written);
         (*output_written_size) += flush_bytes_written;
-        if(res != TAMP_OK)
+        if(TAMP_UNLIKELY(res != TAMP_OK))
             return res;
         output_size -= flush_bytes_written;
         output += flush_bytes_written;
     }
 
-    if(output_size == 0)
+    if(TAMP_UNLIKELY(output_size == 0))
         return TAMP_OUTPUT_FULL;
 
     uint8_t match_size = 0;
     uint16_t match_index = 0;
     find_best_match(compressor, &match_index, &match_size);
 
-    if(match_size < compressor->min_pattern_size){
+    if(TAMP_UNLIKELY(match_size < compressor->min_pattern_size)){
         // Write LITERAL
         match_size = 1;
         unsigned char c = read_input(0);
-        if(c >> compressor->conf.literal){
+        if(TAMP_UNLIKELY(c >> compressor->conf_literal)){
             return TAMP_EXCESS_BITS;
         }
-        write_to_bit_buffer(compressor, IS_LITERAL_FLAG | c, compressor->conf.literal + 1);
+        write_to_bit_buffer(compressor, IS_LITERAL_FLAG | c, compressor->conf_literal + 1);
     }
     else{
         // Write TOKEN
         uint8_t huffman_index = match_size - compressor->min_pattern_size;
         write_to_bit_buffer(compressor, huffman_codes[huffman_index], huffman_bits[huffman_index]);
-        write_to_bit_buffer(compressor, match_index, compressor->conf.window);
+        write_to_bit_buffer(compressor, match_index, compressor->conf_window);
     }
     // Populate Window
     for(uint8_t i=0; i < match_size; i++){
         compressor->window[compressor->window_pos] = read_input(0);
         compressor->window_pos = (compressor->window_pos + 1) & window_mask;
         compressor->input_pos = input_add(1);
-        compressor->input_size--;
     }
+    compressor->input_size -= match_size;
 
     return TAMP_OK;
 }
 
 
 void tamp_compressor_sink(
         TampCompressor *compressor,
         const unsigned char *input,
         size_t input_size,
         size_t *consumed_size
         ){
-    if(consumed_size)
+    size_t consumed_size_proxy;
+    if(TAMP_LIKELY(consumed_size))
         *consumed_size = 0;
+    else
+        consumed_size = &consumed_size_proxy;
 
     for(size_t i=0; i < input_size; i++){
         if(TAMP_UNLIKELY(compressor->input_size == sizeof(compressor->input)))
             break;
         compressor->input[input_add(compressor->input_size)] = input[i];
         compressor->input_size += 1;
-        if(consumed_size)
-            (*consumed_size)++;
+        (*consumed_size)++;
     }
 }
 
 tamp_res tamp_compressor_compress(
         TampCompressor *compressor,
         unsigned char *output,
         size_t output_size,
         size_t *output_written_size,
         const unsigned char *input,
         size_t input_size,
         size_t *input_consumed_size
         ){
     tamp_res res;
+    size_t input_consumed_size_proxy, output_written_size_proxy;
 
-    if(output_written_size)
+    if(TAMP_LIKELY(output_written_size))
         *output_written_size = 0;
-    if(input_consumed_size)
+    else
+        output_written_size = &output_written_size_proxy;
+
+    if(TAMP_LIKELY(input_consumed_size))
         *input_consumed_size = 0;
+    else
+        input_consumed_size = &input_consumed_size_proxy;
 
     while(input_size > 0 && output_size > 0){
         {
             // Sink Data into input buffer.
             size_t consumed;
             tamp_compressor_sink(compressor, input, input_size, &consumed);
             input += consumed;
             input_size -= consumed;
-            if(input_consumed_size)
-                (*input_consumed_size) += consumed;
+            (*input_consumed_size) += consumed;
         }
-        if(compressor->input_size == sizeof(compressor->input)){
+        if(TAMP_LIKELY(compressor->input_size == sizeof(compressor->input))){
             // Input buffer is full and ready to start compressing.
             size_t chunk_output_written_size;
             res = tamp_compressor_compress_poll(compressor, output, output_size, &chunk_output_written_size);
             output += chunk_output_written_size;
             output_size -= chunk_output_written_size;
-            if(output_written_size)
-                (*output_written_size) += chunk_output_written_size;
-            if(res != TAMP_OK)
+            (*output_written_size) += chunk_output_written_size;
+            if(TAMP_UNLIKELY(res != TAMP_OK))
                 return res;
         }
     }
     return TAMP_OK;
 }
 
 tamp_res tamp_compressor_flush(
@@ -267,27 +271,27 @@
         output_written_size = &output_written_size_proxy;
     *output_written_size = 0;
 
     while(compressor->input_size){
         // Compress the remainder of the input buffer.
         res = tamp_compressor_compress_poll(compressor, output, output_size, &chunk_output_written_size);
         (*output_written_size) += chunk_output_written_size;
-        if(res != TAMP_OK)
+        if(TAMP_UNLIKELY(res != TAMP_OK))
             return res;
         output_size -= chunk_output_written_size;
         output += chunk_output_written_size;
     }
 
     // Perform partial flush to see if we need a FLUSH token, and to subsequently
     // make room for the FLUSH token.
     res = partial_flush(compressor, output, output_size, &chunk_output_written_size);
     output_size -= chunk_output_written_size;
     (*output_written_size) += chunk_output_written_size;
     output += chunk_output_written_size;
-    if(res != TAMP_OK)
+    if(TAMP_UNLIKELY(res != TAMP_OK))
         return res;
 
     // Check if there's enough output buffer space
     if (compressor->bit_buffer_pos){
         if (output_size == 0){
             return TAMP_OUTPUT_FULL;
         }
@@ -333,25 +337,25 @@
             output,
             output_size,
             output_written_size,
             input,
             input_size,
             input_consumed_size
             );
-    if(res != TAMP_OK)
+    if(TAMP_UNLIKELY(res != TAMP_OK))
         return res;
 
     res = tamp_compressor_flush(
             compressor,
             output + *output_written_size,
             output_size - *output_written_size,
             &flush_size,
             write_token
             );
 
     (*output_written_size) += flush_size;
 
-    if(res != TAMP_OK)
+    if(TAMP_UNLIKELY(res != TAMP_OK))
         return res;
 
     return TAMP_OK;
 }
```

### Comparing `tamp-1.1.2/tamp/_c_src/tamp/compressor.h` & `tamp-1.1.3/tamp/_c_src/tamp/compressor.h`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,31 @@
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 #include "common.h"
 
+/* Externally, do not directly edit ANY of these attributes */
 typedef struct TampCompressor{
+    /* nicely aligned attributes */
     unsigned char *window;
-    TampConf conf;
     unsigned char input[16];
     uint32_t bit_buffer;
+
+    /* Conf attributes */
+    uint32_t conf_window:4;   // number of window bits
+    uint32_t conf_literal:4;  // number of literal bits
+    uint32_t conf_use_custom_dictionary:1;  // Use a custom initialized dictionary.
+
+    /* Other small attributes */
+    uint32_t window_pos:15;
     uint32_t bit_buffer_pos:6;
     uint32_t min_pattern_size:2;
-    uint32_t window_pos:15;
+
     uint32_t input_size:5;
     uint32_t input_pos:4;
 } TampCompressor;
 
 
 /**
  * @brief Initialize Tamp Compressor object.
```

### Comparing `tamp-1.1.2/tamp/_c_src/tamp/decompressor.c` & `tamp-1.1.3/tamp/_c_src/tamp/decompressor.c`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 #include "decompressor.h"
 #include "common.h"
 #include "assert.h"
 
 #define MAX(x, y) (((x) > (y)) ? (x) : (y))
 #define MIN(x, y) (((x) < (y)) ? (x) : (y))
 
-#define FLUSH 127
+#define FLUSH 15
+
+const uint8_t HUFFMAN_TABLE[128] = {50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 50, 85, 85, 85, 85, 122, 123, 104, 104, 86, 86, 86, 86, 93, 93, 93, 93, 68, 68, 68, 68, 68, 68, 68, 68, 105, 105, 124, 127, 87, 87, 87, 87, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 51, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17, 17};
+
 
 /**
  * @brief Decode a huffman match-size symbol from the decompressor's bit_buffer.
  *
  * Internally updates bit_buffer and bit_buffer_pos.
- * Returns -1 if input has been exhausted; buffer will NOT be restored.
+ *
+ * bit_buffer is GUARANTEED to have enough bits to decode something.
  *
  * @return Tamp Status Code.
  *     TAMP_INVALID_SYMBOL if no valid symbol decoded. Buffer is NOT restored.
  */
 static int8_t huffman_decode(uint32_t *bit_buffer, uint8_t *bit_buffer_pos){
-    uint8_t code = 0;
+    uint8_t code;
+    uint8_t bit_len;
 
-    while(TAMP_LIKELY(*bit_buffer_pos != 0)){
-        code = (code << 1) | (*bit_buffer >> 31);
-        *bit_buffer <<= 1;
-        *bit_buffer_pos -= 1;
-        switch(code){
-            case 0:   return 0;
-            case 3:   return 1;
-            case 8:   return 2;
-            case 11:  return 3;
-            case 20:  return 4;
-            case 36:  return 5;
-            case 38:  return 6;
-            case 43:  return 7;
-            case 75:  return 8;
-            case 84:  return 9;
-            case 148: return 10;
-            case 149: return 11;
-            case 170: return 12;
-            case 39:  return 13;
-            case 171: return FLUSH;
-        }
-    }
-    return -1;
+    (*bit_buffer_pos)--;
+    code = *bit_buffer >> 31;
+    *bit_buffer <<= 1;
+    if(TAMP_LIKELY(code == 0))
+        return 0;
+
+    code = *bit_buffer >> (32 - 7);
+    code = HUFFMAN_TABLE[code];
+    bit_len = code >> 4;
+    *bit_buffer <<= bit_len;
+    (*bit_buffer_pos) -= bit_len;
+
+    return code & 0xF;
 }
 
 tamp_res tamp_decompressor_read_header(TampConf *conf, const unsigned char *input, size_t input_size, size_t *input_consumed_size) {
     if(input_consumed_size)
         (*input_consumed_size) = 0;
     if(input_size == 0)
         return TAMP_INPUT_EXHAUSTED;
@@ -64,39 +59,38 @@
 }
 
 /**
  * Populate the rest of the decompressor structure after the following fields have been populated:
  *   * conf
  *   * window
  */
-static tamp_res tamp_decompressor_populate_from_conf(TampDecompressor *decompressor){
-    const TampConf *conf = &(decompressor->conf);
-    if(conf->window < 8 || conf->window > 15)
+static tamp_res tamp_decompressor_populate_from_conf(TampDecompressor *decompressor, uint8_t conf_window, uint8_t conf_literal, uint8_t conf_use_custom_dictionary){
+    if(conf_window < 8 || conf_window > 15)
         return TAMP_INVALID_CONF;
-    if(conf->literal < 5 || conf->literal > 8)
+    if(conf_literal < 5 || conf_literal > 8)
         return TAMP_INVALID_CONF;
-    if(!conf->use_custom_dictionary)
-        tamp_initialize_dictionary(decompressor->window, (1 << conf->window));
+    if(!conf_use_custom_dictionary)
+        tamp_initialize_dictionary(decompressor->window, (1 << conf_window));
+
+    decompressor->conf_window = conf_window;
+    decompressor->conf_literal = conf_literal;
 
-    decompressor->min_pattern_size = tamp_compute_min_pattern_size(
-            conf->window, conf->literal
-    );
+    decompressor->min_pattern_size = tamp_compute_min_pattern_size(conf_window, conf_literal);
     decompressor->configured = true;
 
     return TAMP_OK;
 }
 
 tamp_res tamp_decompressor_init(TampDecompressor *decompressor, const TampConf *conf, unsigned char *window){
     tamp_res res = TAMP_OK;
     for(uint8_t i=0; i < sizeof(TampDecompressor); i++)  // Zero-out the struct
         ((unsigned char *)decompressor)[i] = 0;
     decompressor->window = window;
     if(conf){
-        decompressor->conf = *conf;
-        res = tamp_decompressor_populate_from_conf(decompressor);
+        res = tamp_decompressor_populate_from_conf(decompressor, conf->window, conf->literal, conf->use_custom_dictionary);
     }
 
     return res;
 }
 
 tamp_res tamp_decompressor_decompress(
         TampDecompressor *decompressor,
@@ -105,15 +99,15 @@
         size_t *output_written_size,
         const unsigned char *input,
         size_t input_size,
         size_t *input_consumed_size
         ){
     size_t input_consumed_size_proxy;
     size_t output_written_size_proxy;
-    const uint16_t window_mask = (1 << decompressor->conf.window) - 1;
+    const uint16_t window_mask = (1 << decompressor->conf_window) - 1;
     tamp_res res;
     const unsigned char *input_end = input + input_size;
     const unsigned char *output_end = output + output_size;
 
     if(!output_written_size)
         output_written_size = &output_written_size_proxy;
     if(!input_consumed_size)
@@ -121,21 +115,22 @@
 
     *input_consumed_size = 0;
     *output_written_size = 0;
 
     if(!decompressor->configured){
         //Read in header
         size_t header_consumed_size;
-        res = tamp_decompressor_read_header(&decompressor->conf, input, input_end - input, &header_consumed_size);
+        TampConf conf;
+        res = tamp_decompressor_read_header(&conf, input, input_end - input, &header_consumed_size);
         if(res != TAMP_OK)
             return res;
         input += header_consumed_size;
         (*input_consumed_size) += header_consumed_size;
 
-        res = tamp_decompressor_populate_from_conf(decompressor);
+        res = tamp_decompressor_populate_from_conf(decompressor, conf.window, conf.literal, conf.use_custom_dictionary);
         if(res != TAMP_OK)
             return res;
     }
     while(input != input_end || decompressor->bit_buffer_pos){
         // Populate the bit buffer
         while(input != input_end && decompressor->bit_buffer_pos <= 24){
             decompressor->bit_buffer_pos += 8;
@@ -149,75 +144,80 @@
 
         if(TAMP_UNLIKELY(output == output_end))
             return TAMP_OUTPUT_FULL;
 
         // Hint that patterns are more likely than literals
         if(TAMP_UNLIKELY(decompressor->bit_buffer >> 31)){
             // is literal
-            if(TAMP_UNLIKELY(decompressor->bit_buffer_pos < (1 + decompressor->conf.literal)))
+            if(TAMP_UNLIKELY(decompressor->bit_buffer_pos < (1 + decompressor->conf_literal)))
                 return TAMP_INPUT_EXHAUSTED;
             decompressor->bit_buffer <<= 1;  // shift out the is_literal flag
 
             // Copy literal to output
-            *output = decompressor->bit_buffer >> (32 - decompressor->conf.literal);
-            decompressor->bit_buffer <<= decompressor->conf.literal;
-            decompressor->bit_buffer_pos -= (1 + decompressor->conf.literal);
+            *output = decompressor->bit_buffer >> (32 - decompressor->conf_literal);
+            decompressor->bit_buffer <<= decompressor->conf_literal;
+            decompressor->bit_buffer_pos -= (1 + decompressor->conf_literal);
 
             // Update window
             decompressor->window[decompressor->window_pos] = *output;
             decompressor->window_pos = (decompressor->window_pos + 1) & window_mask;
 
             output++;
             (*output_written_size)++;
         }
         else{
             // is token; attempt a decode
+            /* copy the bit buffers so that we can abort at any time */
             uint32_t bit_buffer = decompressor->bit_buffer;
             uint16_t window_offset;
             uint16_t window_offset_skip;
             uint8_t bit_buffer_pos = decompressor->bit_buffer_pos;
             int8_t match_size;
             int8_t match_size_skip;
 
             // shift out the is_literal flag
             bit_buffer <<= 1;
             bit_buffer_pos--;
 
-            if((TAMP_UNLIKELY(match_size = huffman_decode(&bit_buffer, &bit_buffer_pos)) < 0)){
+            // There must be at least 8 bits, otherwise no possible decoding.
+            if(TAMP_UNLIKELY(bit_buffer_pos < 8))
+                return TAMP_INPUT_EXHAUSTED;
+
+            if(TAMP_UNLIKELY(match_size = huffman_decode(&bit_buffer, &bit_buffer_pos)) < 0){
                 // Insufficient input
                 return TAMP_INPUT_EXHAUSTED;
             }
             if(TAMP_UNLIKELY(match_size == FLUSH)){
                 // flush bit_buffer to the nearest byte and skip the remainder of decoding
                 decompressor->bit_buffer = bit_buffer << (bit_buffer_pos & 7);
                 decompressor->bit_buffer_pos = bit_buffer_pos & ~7;  // Round bit_buffer_pos down to nearest multiple of 8.
                 continue;
             }
-            if(TAMP_UNLIKELY(bit_buffer_pos < decompressor->conf.window)){
+            if(TAMP_UNLIKELY(bit_buffer_pos < decompressor->conf_window)){
                 // There are not enough bits to decode window offset
                 return TAMP_INPUT_EXHAUSTED;
             }
             match_size += decompressor->min_pattern_size;
-            window_offset = bit_buffer >> (32 - decompressor->conf.window);
+            window_offset = bit_buffer >> (32 - decompressor->conf_window);
 
             // Apply skip_bytes
             match_size_skip = match_size - decompressor->skip_bytes;
             window_offset_skip = window_offset + decompressor->skip_bytes;
 
             // Check if we are output-buffer-limited, and if so to set skip_bytes
             // Otherwise, update the decompressor buffers
             size_t remaining = output_end - output;
             if(TAMP_UNLIKELY((uint8_t)match_size_skip > remaining)){
                 decompressor->skip_bytes += remaining;
                 match_size_skip = remaining;
             }
             else {
                 decompressor->skip_bytes = 0;
-                decompressor->bit_buffer = bit_buffer << decompressor->conf.window;
-                decompressor->bit_buffer_pos = bit_buffer_pos - decompressor->conf.window;
+                decompressor->bit_buffer = bit_buffer << decompressor->conf_window;
+                decompressor->bit_buffer_pos = bit_buffer_pos - decompressor->conf_window;
             }
 
             // Copy pattern to output
             for(uint8_t i=0; i < match_size_skip; i++){
                 *output++ = decompressor->window[window_offset_skip + i];
             }
             (*output_written_size) += match_size_skip;
```

### Comparing `tamp-1.1.2/tamp/_c_src/tamp/decompressor.h` & `tamp-1.1.3/tamp/_c_src/tamp/decompressor.h`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,29 @@
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 #include "common.h"
 
+/* Externally, do not directly edit ANY of these attributes */
 typedef struct {
     unsigned char *window;
-    TampConf conf;
     uint32_t bit_buffer;
+
+    /* Conf attributes */
+    uint32_t conf_window:4;   // number of window bits
+    uint32_t conf_literal:4;  // number of literal bits
+    //uint32_t conf_use_custom_dictionary:1;  // Not used past initialization.
+
     uint32_t bit_buffer_pos:6;
     uint32_t min_pattern_size:2;
     uint32_t window_pos:15;
     uint32_t configured:1;  // Whether or not conf has been properly set
+
     uint32_t skip_bytes:4;  // Skip this many decompressed bytes (from previous output-buffer-limited decompression).
 } TampDecompressor;
 
 /**
  * @brief Read tamp header and populate configuration.
  *
  * Don't invoke if setting conf to NULL in tamp_decompressor_init.
```

### Comparing `tamp-1.1.2/tamp/cli/main.py` & `tamp-1.1.3/tamp/cli/main.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/tamp/compressor.py` & `tamp-1.1.3/tamp/compressor.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/tamp/compressor_viper.py` & `tamp-1.1.3/tamp/compressor_viper.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/tamp/ctamp.pxd` & `tamp-1.1.3/tamp/ctamp.pxd`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/tamp/decompressor.py` & `tamp-1.1.3/tamp/decompressor.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/tamp/decompressor_viper.py` & `tamp-1.1.3/tamp/decompressor_viper.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.2/PKG-INFO` & `tamp-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tamp
-Version: 1.1.2
+Version: 1.1.3
 Summary: 
 Home-page: https://github.com/BrianPugh/tamp
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -47,15 +47,15 @@
 
     * ``tamp/_c_src/``
 
 * High compression ratios and low memory use.
 
 * Compact compression and decompression implementations.
 
-  * Compiled C library is <7.5KB (compressor + decompressor).
+  * Compiled C library is <4KB (compressor + decompressor).
 
 * Mid-stream flushing.
 
   * Allows for submission of messages while continuing to compress subsequent data.
 
 * Customizable dictionary for greater compression of small messages.
 
@@ -303,15 +303,15 @@
 
 +---------------+--------------------+-------+------+--------------+-----------------+
 | Action        | tamp               | tamp  | zlib | heatshrink   | heatshrink      |
 |               | (Python Reference) | (C)   |      | (with index) | (without index) |
 +===============+====================+=======+======+==============+=================+
 | Compression   | 109.5              | 16.45 | 4.84 | 6.22         | 41.729          |
 +---------------+--------------------+-------+------+--------------+-----------------+
-| Decompression | 54.0               | 0.98  | 0.08 | 0.82         | 0.82            |
+| Decompression | 54.0               | 0.70  | 0.98 | 0.82         | 0.82            |
 +---------------+--------------------+-------+------+--------------+-----------------+
 
 Heatshrink v0.4.1 was used in these benchmarks.
 When heathshrink uses an index, an additional ``(1 << (windowBits + 1))`` bytes of memory are used, tripling the memory requirement.
 Tamp could use a similar indexing to increase compression speed, but has chosen not to to focus on the primary goal of a low-memory compressor.
 
 Binary Size
@@ -321,15 +321,15 @@
 Numbers reported in bytes.
 
 +--------------------+------------+--------------+---------------------------+
 | Library            | Compressor | Decompressor | Compressor + Decompressor |
 +====================+============+==============+===========================+
 | Tamp (micropython) | 4779       | 4717         | 8262                      |
 +--------------------+------------+--------------+---------------------------+
-| Tamp (C)           | 2996       | 2192         | 5064                      |
+| Tamp (C)           | 2008       | 1976         | 3848                      |
 +--------------------+------------+--------------+---------------------------+
 | Heatshrink         | 2956       | 3876         | 6832                      |
 +--------------------+------------+--------------+---------------------------+
 | uzlib              | 2355       | 3963         | 6318                      |
 +--------------------+------------+--------------+---------------------------+
 
 Heatshrink doesn't include a high level API; in an apples-to-apples comparison the Tamp library would be even smaller.
```

