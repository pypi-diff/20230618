# Comparing `tmp/pandoc_latex_french_spaces-1.0.0.tar.gz` & `tmp/pandoc_latex_french_spaces-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc_latex_french_spaces-1.0.0.tar", max compression
+gzip compressed data, was "pandoc_latex_french_spaces-1.0.0.1.tar", max compression
```

## Comparing `pandoc_latex_french_spaces-1.0.0.tar` & `pandoc_latex_french_spaces-1.0.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1521 2023-06-17 15:21:00.730985 pandoc_latex_french_spaces-1.0.0/LICENSE
--rw-r--r--   0        0        0     9097 2023-06-17 15:21:00.730985 pandoc_latex_french_spaces-1.0.0/README.md
--rw-r--r--   0        0        0     1168 2023-06-17 15:21:00.730985 pandoc_latex_french_spaces-1.0.0/pandoc_latex_french_spaces.py
--rw-r--r--   0        0        0     2954 2023-06-17 15:21:00.730985 pandoc_latex_french_spaces-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    10218 1970-01-01 00:00:00.000000 pandoc_latex_french_spaces-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-06-18 12:48:35.376884 pandoc_latex_french_spaces-1.0.0.1/LICENSE
+-rw-r--r--   0        0        0     9405 2023-06-18 12:48:35.376884 pandoc_latex_french_spaces-1.0.0.1/README.md
+-rw-r--r--   0        0        0     1168 2023-06-18 12:48:35.376884 pandoc_latex_french_spaces-1.0.0.1/pandoc_latex_french_spaces.py
+-rw-r--r--   0        0        0     2961 2023-06-18 12:48:35.376884 pandoc_latex_french_spaces-1.0.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10528 1970-01-01 00:00:00.000000 pandoc_latex_french_spaces-1.0.0.1/PKG-INFO
```

### Comparing `pandoc_latex_french_spaces-1.0.0/LICENSE` & `pandoc_latex_french_spaces-1.0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc_latex_french_spaces-1.0.0/README.md` & `pandoc_latex_french_spaces-1.0.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-french-spaces/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-latex-french-spaces?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-french-spaces.svg?logo=scrutinizer)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-french-spaces/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-french-spaces.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-latex-french-spaces/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-french-spaces.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-latex-french-spaces/)
 [![License](https://img.shields.io/pypi/l/pandoc-latex-french-spaces.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-latex-french-spaces/develop/LICENSE)
 [![Repo Size](https://img.shields.io/github/repo-size/chdemko/pandoc-latex-french-spaces.svg)](http://pandoc-latex-french-spaces.readthedocs.io/en/latest/)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-french-spaces.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-latex-french-spaces/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Downloads](https://pepy.tech/badge/pandoc-latex-french-spaces)](https://pepy.tech/project/pandoc-latex-french-spaces)
 [![Source Rank](https://img.shields.io/librariesio/sourcerank/pypi/pandoc-latex-french-spaces.svg?logo=koding&logoColor=white)](https://libraries.io/pypi/pandoc-latex-french-spaces)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-french-spaces.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-latex-french-spaces/)
 [![Docs](https://img.shields.io/readthedocs/pandoc-latex-french-spaces.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-french-spaces.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
 
 license icon by [Daniel Bruce](https://www.iconfinder.com/icons/216659/license_icon),
@@ -23,15 +25,15 @@
 *pandoc-latex-french-spaces* is a [pandoc] filter for dealing with french spacing rules for ponctuations in *LaTeX*.
 
 [pandoc]: http://pandoc.org/
 
 Instructions
 ------------
 
-*pandoc-latex-french-spaces* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. python 3.x will do.
+*pandoc-latex-french-spaces* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
 
 Install *pandoc-latex-french-spaces* as using the bash command
 
 ~~~shell
 $ pip install pandoc-latex-french-spaces
 ~~~
```

### Comparing `pandoc_latex_french_spaces-1.0.0/pandoc_latex_french_spaces.py` & `pandoc_latex_french_spaces-1.0.0.1/pandoc_latex_french_spaces.py`

 * *Files identical despite different names*

### Comparing `pandoc_latex_french_spaces-1.0.0/pyproject.toml` & `pandoc_latex_french_spaces-1.0.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-    requires = ["poetry-core"]
+    requires = ["poetry-core>=1.2"]
     build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
     name = "pandoc-latex-french-spaces"
-    version = "1.0.0"
+    version = "1.0.0.1"
     description="A pandoc filter for dealing with french spacing rules"
     authors = ["Christophe Demko <chdemko@gmail.com>"]
     license = "BSD-3-Clause"
     readme = "README.md"
     homepage="https://github.com/chdemko/pandoc-latex-french-spaces"
     keywords=["pandoc", "filters", "latex", "french", "spaces"]
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
@@ -39,34 +39,34 @@
 
 
 [tool.poetry.dependencies]
     python = "^3.9"
     panflute = "^2.3.0"
 
 [tool.poetry.group.dev.dependencies]
-    tox = "^4.6.1"
+    tox = "^4.6.2"
 
     # Formatter
     black = "^23.3.0"
 
     # Tests
     pytest = "^7.3.2"
-    pytest-cov = "^4.0.0"
+    pytest-cov = "^4.1.0"
 
     # Style checkers
     doc8 = "^0.11.2"
     mypy = "^1.3.0"
     flake8 = "^6.0.0"
     flake8-annotations-complexity = "^0.0.7"
     flake8-black = "^0.3.6"
     flake8-blind-except = "^0.2.1"
-    flake8-bugbear = "^23.5.9"
+    flake8-bugbear = "^23.6.5"
     flake8-builtins = "^2.1.0"
     flake8-cognitive-complexity = "^0.1.0"
-    flake8-comprehensions = "^3.12.0"
+    flake8-comprehensions = "^3.13.0"
     flake8-docstrings = "^1.7.0"
     flake8-expression-complexity = "^0.0.11"
     flake8-fixme = "^1.1.1"
     flake8-functions = "^0.0.7"
     flake8-import-order = "^0.18.2"
     flake8-mypy = "^17.8.0"
     flake8-pyi = "^23.5.0"
```

### Comparing `pandoc_latex_french_spaces-1.0.0/PKG-INFO` & `pandoc_latex_french_spaces-1.0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandoc-latex-french-spaces
-Version: 1.0.0
+Version: 1.0.0.1
 Summary: A pandoc filter for dealing with french spacing rules
 Home-page: https://github.com/chdemko/pandoc-latex-french-spaces
 License: BSD-3-Clause
 Keywords: pandoc,filters,latex,french,spaces
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -32,14 +32,16 @@
 [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-latex-french-spaces/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-latex-french-spaces?branch=develop)
 [![Scrutinizer](https://img.shields.io/scrutinizer/g/chdemko/pandoc-latex-french-spaces.svg?logo=scrutinizer)](https://scrutinizer-ci.com/g/chdemko/pandoc-latex-french-spaces/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-latex-french-spaces.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-latex-french-spaces/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-latex-french-spaces.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-latex-french-spaces/)
 [![License](https://img.shields.io/pypi/l/pandoc-latex-french-spaces.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-latex-french-spaces/develop/LICENSE)
 [![Repo Size](https://img.shields.io/github/repo-size/chdemko/pandoc-latex-french-spaces.svg)](http://pandoc-latex-french-spaces.readthedocs.io/en/latest/)
 [![Python version](https://img.shields.io/pypi/pyversions/pandoc-latex-french-spaces.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-latex-french-spaces/)
+[![Poetry version](https://img.shields.io/badge/poetry-1.2%20|%201.3%20|%201.4%20|%201.5-blue.svg)](https://python-poetry.org/)
+[![Pandoc version](https://img.shields.io/badge/pandoc-2.11%20|%202.12%20|%202.13%20|%202.14%20|%202.15%20|%202.16%20|%202.17%20|%202.18%20|%202.19%20|%203.0%20|%203.1-blue.svg)](https://pandoc.org/)
 [![Downloads](https://pepy.tech/badge/pandoc-latex-french-spaces)](https://pepy.tech/project/pandoc-latex-french-spaces)
 [![Source Rank](https://img.shields.io/librariesio/sourcerank/pypi/pandoc-latex-french-spaces.svg?logo=koding&logoColor=white)](https://libraries.io/pypi/pandoc-latex-french-spaces)
 [![Development Status](https://img.shields.io/pypi/status/pandoc-latex-french-spaces.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiUnX5lXMAAAAlBJREFUeNrt3b1qlEEUBuB3TNDCP7wDOwv/cgv+pDC3YcDe+xBFFFLoDWhhpxiD12Ch1mJsg7irjRLGYjcKEbLC92n223meMgQSzrx7Zs6wMAkAAAAAAAAAAAAAAAAAAAAw78r+H9RaLyZZT3Itydkkx5XpUH1L8iHJVpJHpZS3/yQAtdZjSe4muZXkiLrPpd0kG0lul1K+9xaA6eK/SHJFjQfhdZIbfYRg75N+z+IPytUkd3rpANM9/422P8jt4HIp5V3XDrBu8QdpKcnNPraA62o5WKt9bAHjJCfUcpDGpZRTXQNQ1fGAApVSDvPvz1qfrv+fvb9xAiAACACDVf80qrU+q7Wecwhs4BB4gM+ZXBRt6wBtOpO/uC7WARa3AyTJqJRyWgdo18xLIgEwBSAACABt3hOYAhZ7Cph9TyAAzQYgSZ4KQNsBGAlA2wFwCDQFIAAIAAKAACAACAACgAAgAAgAAoAAIAAIAIvniwC07aVvBM2wwN8I2kmyogO0Z5TkSZKVUsqnZfVou4PpAKYABAABYDHnfAFofM6feUh0D7Cw9wA7e6OeDtDwnD/rl90DNN6hdABTAAJAs5aTjJOcVIreT+H/68DXuQNsW+bB+thHAF6p42Btdp4iaq0XMnk2bkk9B2U3yaVSyvtOHWD6Fu2Geg7Ow66Ln/x+OvZokueZPBjN/NtKslZK+dHLGDh9g3YtyYNpa2F+2/79vhb/VwfYN/acz+RFytVMno/3puDh+prJ8/GbSR730fYBAAAAAAAAAAAAAAAAAACAYfkJuHbYr8dtGYwAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-latex-french-spaces/)
 [![Docs](https://img.shields.io/readthedocs/pandoc-latex-french-spaces.svg?logo=read-the-docs&logoColor=white)](http://pandoc-latex-french-spaces.readthedocs.io/en/latest/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAYAAABXAvmHAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAAOxAAADsQBlSsOGwAAABl0RVh0U29mdHdhcmUAd3d3Lmlua3NjYXBlLm9yZ5vuPBoAAANwSURBVGiB7Zndi1VlFIefNZPR9GkTmSkOhIZYeBFiIDEYNUREXVQEQUhK4hdEf0GQf0IUU2BdhHUjNQTpRRdl0NdFXYRZCA0SJTZ9CJEDmY49Xewzw57Xfc7+OGfOEJzn5vCuvfbav/Wutd+993tgwIAB/2ui3xdUVwKPAbcDPwDHIuJiv3XURr1HPaTOuphpdeNy6ytEvUbdoX5pZ75Xr15uvQuoa9WX1N9KhOfZsdyih9QJ9Yg6V0P4PF8sl/CV6gvq6QaiU7b0U/g29bB6oQfC5znUD+HXqu/2UHSeWbNltjJDDXKYBJ4EfgFeBo42iNGO64BnexhvMeoqsxt0Vh3L2V/tYRVOqZUfsHUrcCcwDJyKiJ9y9g9rxunERuDBqs51Ezjb+t2UrwDwcM04Zeyv6lj7XUj9GtgCzABHgA3AI3XjlDAH3BERZ3ocF9TnetjvnThYRU+TCowAZ4DRuufWZAYYi4hLnZxqL6MR8TfwVlNVNVgNPL4kkdUN6uU+tNEnZVo6VkC9tcgeEdPAR83Sr8V29e5ODmUttLvDscn6ehpReUldhLpebTvL6rD6Yx/a6C/1xnY6OlVgf6fjEXEZeKPSbHTHDcAztc5QR9Q/1OOJfSgZr1b/6UMVTrTT2m6GnwZuKbBvVRfW/4iYAaaqT01jNqvjRQfaJdDuxhkBdia21xqKqku1m9ls+2OetIXuN9sGSVvpRB/a6KK6JtVbVIHnS3JcD0wktterTE6XrAB2pcZ0JkfJ+r+MA8n4MHC+sbTq7FGH84a0AjvJ+ryMR819D0TEeeDtruWVMwbcmzcsJGD2GbevYqBhYE9i69eTeVV+kK/ANrJPxqrsNrcdGBEngU+701aJb/ODfAJ1xAPcBjyR2Ja6Cu9FxOm8IZ/AdIOA6c08RfYhshQcB/amxnwCXwHf1Qw6rm6eH7T2+d9sJK+YObJJmYiIByLiXEfv1kPs15IHWcpk4rPOZpu7ec6qB9W1tVNWR9UX1Z8LEhgvuNgVr7vq+w1E/6t+rD6lrqgtvCCRq0x2i9U1rQulHEj8Hqoh/E/1FXVT16IrJjZVIOJk4hPqZyXCv1H3qtf3RXhO3M3qsQJB2xO/dS2ReS6o76j39UpP438p1QlgK3BTy/R5RHyQ+AyRbTveBZwDjkbE702vOWDAgCv5DyyzjR7/CUzHAAAAAElFTkSuQmCC)](https://pypi.org/project/black/)
 
 license icon by [Daniel Bruce](https://www.iconfinder.com/icons/216659/license_icon),
@@ -50,15 +52,15 @@
 *pandoc-latex-french-spaces* is a [pandoc] filter for dealing with french spacing rules for ponctuations in *LaTeX*.
 
 [pandoc]: http://pandoc.org/
 
 Instructions
 ------------
 
-*pandoc-latex-french-spaces* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows]. python 3.x will do.
+*pandoc-latex-french-spaces* requires [python], a programming language that comes pre-installed on linux and Mac OS X, and which is easily installed [on Windows].
 
 Install *pandoc-latex-french-spaces* as using the bash command
 
 ~~~shell
 $ pip install pandoc-latex-french-spaces
 ~~~
```

