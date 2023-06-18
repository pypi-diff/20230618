# Comparing `tmp/pandoc-beamer-block-0.2.0.tar.gz` & `tmp/pandoc_beamer_block-1.0.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc-beamer-block-0.2.0.tar", last modified: Thu Jul  7 18:39:49 2022, max compression
+gzip compressed data, was "pandoc_beamer_block-1.0.0.0.tar", max compression
```

## Comparing `pandoc-beamer-block-0.2.0.tar` & `pandoc_beamer_block-1.0.0.0.tar`

### file list

```diff
@@ -1,15 +1,5 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 18:39:49.400306 pandoc-beamer-block-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-07-07 18:39:38.000000 pandoc-beamer-block-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-07-07 18:39:38.000000 pandoc-beamer-block-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10027 2022-07-07 18:39:49.400306 pandoc-beamer-block-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8824 2022-07-07 18:39:38.000000 pandoc-beamer-block-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-07 18:39:49.400306 pandoc-beamer-block-0.2.0/pandoc_beamer_block.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10027 2022-07-07 18:39:49.000000 pandoc-beamer-block-0.2.0/pandoc_beamer_block.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-07-07 18:39:49.000000 pandoc-beamer-block-0.2.0/pandoc_beamer_block.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-07 18:39:49.000000 pandoc-beamer-block-0.2.0/pandoc_beamer_block.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-07 18:39:49.000000 pandoc-beamer-block-0.2.0/pandoc_beamer_block.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-07-07 18:39:49.000000 pandoc-beamer-block-0.2.0/pandoc_beamer_block.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-07-07 18:39:49.000000 pandoc-beamer-block-0.2.0/pandoc_beamer_block.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-07-07 18:39:38.000000 pandoc-beamer-block-0.2.0/pandoc_beamer_block.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-07-07 18:39:49.400306 pandoc-beamer-block-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3783 2022-07-07 18:39:38.000000 pandoc-beamer-block-0.2.0/setup.py
+-rw-r--r--   0        0        0     1521 2023-06-18 13:41:49.899906 pandoc_beamer_block-1.0.0.0/LICENSE
+-rw-r--r--   0        0        0     8926 2023-06-18 13:41:49.899906 pandoc_beamer_block-1.0.0.0/README.md
+-rw-r--r--   0        0        0     2792 2023-06-18 13:41:49.903906 pandoc_beamer_block-1.0.0.0/pandoc_beamer_block.py
+-rw-r--r--   0        0        0     2935 2023-06-18 13:41:49.903906 pandoc_beamer_block-1.0.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10044 1970-01-01 00:00:00.000000 pandoc_beamer_block-1.0.0.0/PKG-INFO
```

### Comparing `pandoc-beamer-block-0.2.0/LICENSE` & `pandoc_beamer_block-1.0.0.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2019-2021, Christophe Demko
+Copyright (c) 2019-2023, Christophe Demko
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `pandoc-beamer-block-0.2.0/PKG-INFO` & `pandoc_beamer_block-1.0.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,92 @@
 Metadata-Version: 2.1
 Name: pandoc-beamer-block
-Version: 0.2.0
+Version: 1.0.0.0
 Summary: A pandoc filter for adding beamer block on specific div
-Home-page: https://github.com/chdemko/pandoc-beamer-block
+Home-page: https://github.com/chdemko/pandoc-latex-french-spaces
+License: BSD-3-Clause
+Keywords: pandoc,filters,latex,french,spaces
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
-Maintainer: Christophe Demko
-Maintainer-email: chdemko@gmail.com
-License: BSD-3-Clause
-Download-URL: https://github.com/chdemko/pandoc-beamer-block/archive/develop.zip
-Keywords: pandoc,filters,block,latex,beamer
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Filters
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Natural Language :: English
+Requires-Dist: panflute (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
-# pandoc-beamer-block
-[![Build Status](https://img.shields.io/travis/chdemko/pandoc-beamer-block/0.2.0.svg?logo=travis)](https://travis-ci.org/chdemko/pandoc-beamer-block/branches)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-block/0.2.0.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-block?branch=0.2.0)
+
+# Installation
+![Python package](https://github.com/chdemko/pandoc-beamer-block/workflows/Python%20package/badge.svg?branch=develop)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-block/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-block?branch=develop)
 [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-beamer-block/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-beamer-block/)
 [![Code Beat](https://codebeat.co/badges/cb5538dc-f30b-4ac4-abf6-3c213682c54d)](https://codebeat.co/projects/github-com-chdemko-pandoc-beamer-block-develop/)
 [![Codacy](https://img.shields.io/codacy/grade/af5a670790264990811713280a8f8dcf.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-beamer-block)
 [![CodeFactor](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-block/badge)](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-block)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-beamer-block.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-block/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-beamer-block.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-block/)
-[![License](https://img.shields.io/pypi/l/pandoc-beamer-block.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-beamer-block/0.2.0/LICENSE)
+[![License](https://img.shields.io/pypi/l/pandoc-beamer-block.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-beamer-block/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-beamer-block.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-block/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Downloads](https://pepy.tech/badge/pandoc-beamer-block)](https://pepy.tech/project/pandoc-beamer-block)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-beamer-block.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-block/)
 [![Docs](https://img.shields.io/readthedocs/pandoc-beamer-block.svg?logo=read-the-docs&logoColor=white)](http://pandoc-beamer-block.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
 
 *pandoc-beamer-block* is a [pandoc] filter for adding beamer block to `div`s.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [Read the docs pages](http://pandoc-beamer-block.readthedocs.io/en/0.2.0/).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-beamer-block
-
-Installation
+Instructions
 ------------
 
-*pandoc-beamer-block* requires [python 3.6], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
+*pandoc-beamer-block* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
 
-Install *pandoc-beamer-block* as root using the bash command
+Install *pandoc-beamer-block* using the bash command
 
-    pip install pandoc-beamer-block
+~~~shell
+$ pip install pandoc-beamer-block
+~~~
 
 To upgrade to the most recent release, use
 
-    pip install --upgrade pandoc-beamer-block
+~~~shell
+$ pip install --upgrade pandoc-beamer-block
+~~~
 
 To upgrade to the current code, use
 
-    pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-block
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-block
+~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
-    apt-get update
-    apt-get install python-pip
+~~~shell
+$ sudo apt-get update
+$ sudo apt-get install python3-pip
+~~~
 
-[python 3.6]: https://www.python.org
+[python]: https://www.python.org
 [on Windows]: https://www.python.org/downloads/windows
 [PyPI]: https://pypi.org
 
 
 Getting Help
 ------------
 
 If you have any difficulties with pandoc-beamer-block, please feel welcome to [file an issue] on github so that we can help.
 
 [file an issue]: https://github.com/chdemko/pandoc-beamer-block/issues
 
 
-
```

### Comparing `pandoc-beamer-block-0.2.0/README.md` & `pandoc_beamer_block-1.0.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,60 @@
-# pandoc-beamer-block
-[![Build Status](https://img.shields.io/travis/chdemko/pandoc-beamer-block/0.2.0.svg?logo=travis)](https://travis-ci.org/chdemko/pandoc-beamer-block/branches)
-[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-block/0.2.0.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-block?branch=0.2.0)
+# Installation
+![Python package](https://github.com/chdemko/pandoc-beamer-block/workflows/Python%20package/badge.svg?branch=develop)
+[![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-beamer-block/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-beamer-block?branch=develop)
 [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-beamer-block/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-beamer-block/)
 [![Code Beat](https://codebeat.co/badges/cb5538dc-f30b-4ac4-abf6-3c213682c54d)](https://codebeat.co/projects/github-com-chdemko-pandoc-beamer-block-develop/)
 [![Codacy](https://img.shields.io/codacy/grade/af5a670790264990811713280a8f8dcf.svg?logo=codacy&logoColor=white)](https://www.codacy.com/app/chdemko/pandoc-beamer-block)
 [![CodeFactor](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-block/badge)](https://www.codefactor.io/repository/github/chdemko/pandoc-beamer-block)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-beamer-block.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-block/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-beamer-block.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-block/)
-[![License](https://img.shields.io/pypi/l/pandoc-beamer-block.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-beamer-block/0.2.0/LICENSE)
+[![License](https://img.shields.io/pypi/l/pandoc-beamer-block.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-beamer-block/develop/LICENSE)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-beamer-block.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-beamer-block/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Downloads](https://pepy.tech/badge/pandoc-beamer-block)](https://pepy.tech/project/pandoc-beamer-block)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-beamer-block.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-beamer-block/)
 [![Docs](https://img.shields.io/readthedocs/pandoc-beamer-block.svg?logo=read-the-docs&logoColor=white)](http://pandoc-beamer-block.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
 
 *pandoc-beamer-block* is a [pandoc] filter for adding beamer block to `div`s.
 
 [pandoc]: http://pandoc.org/
 
-Documentation
--------------
-
-See the [Read the docs pages](http://pandoc-beamer-block.readthedocs.io/en/0.2.0/).
-
-Usage
------
-
-To apply the filter, use the following option with pandoc:
-
-    --filter pandoc-beamer-block
-
-Installation
+Instructions
 ------------
 
-*pandoc-beamer-block* requires [python 3.6], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
+*pandoc-beamer-block* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
 
-Install *pandoc-beamer-block* as root using the bash command
+Install *pandoc-beamer-block* using the bash command
 
-    pip install pandoc-beamer-block
+~~~shell
+$ pip install pandoc-beamer-block
+~~~
 
 To upgrade to the most recent release, use
 
-    pip install --upgrade pandoc-beamer-block
+~~~shell
+$ pip install --upgrade pandoc-beamer-block
+~~~
 
 To upgrade to the current code, use
 
-    pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-block
+~~~shell
+$ pip install --upgrade --force git+https://github.com/chdemko/pandoc-beamer-block
+~~~
 
 `pip` is a script that downloads and installs modules from the Python Package Index, [PyPI].  It should come installed with your python distribution. If you are running linux, `pip` may be bundled separately. On a Debian-based system (including Ubuntu), you can install it as root using
 
-    apt-get update
-    apt-get install python-pip
+~~~shell
+$ sudo apt-get update
+$ sudo apt-get install python3-pip
+~~~
 
-[python 3.6]: https://www.python.org
+[python]: https://www.python.org
 [on Windows]: https://www.python.org/downloads/windows
 [PyPI]: https://pypi.org
 
 
 Getting Help
 ------------
```

### Comparing `pandoc-beamer-block-0.2.0/pandoc_beamer_block.py` & `pandoc_beamer_block-1.0.0.0/pandoc_beamer_block.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 #!/usr/bin/env python
 
 """
-Pandoc filter for adding beamer block on specific div
+Pandoc filter for adding beamer block on specific div.
 """
 
-from panflute import convert_text, run_filter, Div, RawBlock
+from panflute import Div, RawBlock, convert_text, run_filter  # type: ignore
 
 
 def prepare(doc):
     """
-    Prepare the document
+    Prepare the document.
 
     Arguments
     ---------
-        doc:
-            The pandoc document
+    doc
+        The pandoc document
     """
-
     # Prepare the definitions
     doc.defined = []
 
     # Get the meta data
     meta = doc.get_metadata("pandoc-beamer-block")
 
     if isinstance(meta, list):
-
         # Loop on all definitions
         for definition in meta:
-
             # Verify the definition
             if (
                 isinstance(definition, dict)
                 and "classes" in definition
                 and isinstance(definition["classes"], list)
             ):
                 definition["classes"] = frozenset(definition["classes"])
                 definition["type"] = definition.get("type", "info")
                 doc.defined.append(definition)
 
 
 def latex(elem, environment, title):
     """
-    Generate the LaTeX code
+    Generate the LaTeX code.
 
     Arguments
     ---------
-        elem:
-            The current element
+    elem
+        The current element
 
-        environment:
-            The environment to add
+    environment
+        The environment to add
 
-        title:
-            The environment title
+    title
+        The environment title
 
     Returns
     -------
         A list of pandoc elements.
     """
     return [
         RawBlock(f"\\begin{{{environment}}}{title}", "tex"),
@@ -67,25 +64,28 @@
 
 def block(elem, doc):
     """
     Transform div element.
 
     Arguments
     ---------
-        elem:
-            current element
-        doc:
-            pandoc document
+    elem
+        current element
+    doc
+        pandoc document
+
+    Returns
+    -------
+        A list of pandoc elements or None.
     """
     if doc.format == "beamer" and isinstance(elem, Div):
         classes = frozenset(elem.classes)
 
         # Loop on all fontsize definition
         for definition in doc.defined:
-
             # Are the classes correct?
             if classes >= definition["classes"]:
                 if "title" in elem.attributes:
                     escaped = elem.attributes["title"].translate(
                         str.maketrans({"{": r"\{", "}": r"\}", "%": r"\%"})
                     )
                     title = f"{{{convert_text(escaped, output_format='latex')}}}"
@@ -98,19 +98,23 @@
                     return latex(elem, "exampleblock", title)
                 return latex(elem, "block", title)
     return None
 
 
 def main(doc=None):
     """
-    main function.
+    Convert the pandoc document.
 
     Arguments
     ---------
-        doc:
-            pandoc document
+    doc
+        pandoc document
+
+    Returns
+    -------
+        The modified pandoc document.
     """
     return run_filter(block, doc=doc, prepare=prepare)
 
 
 if __name__ == "__main__":
     main()
```

