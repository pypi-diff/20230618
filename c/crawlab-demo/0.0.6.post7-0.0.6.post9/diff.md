# Comparing `tmp/crawlab-demo-0.0.6.post7.tar.gz` & `tmp/crawlab-demo-0.0.6.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlab-demo-0.0.6.post7.tar", last modified: Fri Dec 23 06:56:28 2022, max compression
+gzip compressed data, was "crawlab-demo-0.0.6.post9.tar", last modified: Fri Dec 23 08:09:45 2022, max compression
```

## Comparing `crawlab-demo-0.0.6.post7.tar` & `crawlab-demo-0.0.6.post9.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      444 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.470059 crawlab-demo-0.0.6.post7/crawlab_demo/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.470059 crawlab-demo-0.0.6.post7/crawlab_demo/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/actions/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/actions/import_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/actions/reimport_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/actions/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.470059 crawlab-demo-0.0.6.post7/crawlab_demo/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.470059 crawlab-demo-0.0.6.post7/crawlab_demo/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/demo.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.470059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.466059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.470059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/basic/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/basic/crawlab.json
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/basic/go.mod
--rw-r--r--   0 runner    (1001) docker     (123)    23756 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/basic/go.sum
--rw-r--r--   0 runner    (1001) docker     (123)      235 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/basic/main.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/colly_scrapy_docs/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/colly_scrapy_docs/crawlab.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/colly_scrapy_docs/go.mod
--rw-r--r--   0 runner    (1001) docker     (123)    27283 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/colly_scrapy_docs/go.sum
--rw-r--r--   0 runner    (1001) docker     (123)      843 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/colly_scrapy_docs/main.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/rod_github/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/rod_github/crawlab.json
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/rod_github/go.mod
--rw-r--r--   0 runner    (1001) docker     (123)    23275 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/rod_github/go.sum
--rw-r--r--   0 runner    (1001) docker     (123)      810 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/rod_github/main.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.470059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/node/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/node/basic/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/node/basic/crawlab.json
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/node/basic/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/node/puppeteer_163_tech_news/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/node/puppeteer_163_tech_news/crawlab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/node/puppeteer_163_tech_news/main.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.470059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/basic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/basic/crawlab.json
--rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/basic/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/spiders/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/spiders/books.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/crawlab.json
--rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/scrapy.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/spiders/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/spiders/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/scrapy.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/spiders/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/spiders/news.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/scrapy.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.474059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/spiders/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/spiders/news.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/scrapy.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/playwright_bing/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/playwright_bing/crawlab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/playwright_bing/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/crawlab.json
--rw-r--r--   0 runner    (1001) docker     (123)      267 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/spiders/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/spiders/baidu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/crawlab.json
--rw-r--r--   0 runner    (1001) docker     (123)      269 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/spiders/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/spiders/quotes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/selenium_36kr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/selenium_36kr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/selenium_36kr/crawlab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/selenium_36kr/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/crawlab_demo/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/models/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/models/spider.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/crawlab_demo/test/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/crawlab_demo/test/demo_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:56:28.470059 crawlab-demo-0.0.6.post7/crawlab_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2022-12-23 06:56:28.000000 crawlab-demo-0.0.6.post7/crawlab_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2022-12-23 06:56:28.000000 crawlab-demo-0.0.6.post7/crawlab_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 06:56:28.000000 crawlab-demo-0.0.6.post7/crawlab_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-23 06:56:28.000000 crawlab-demo-0.0.6.post7/crawlab_demo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-23 06:56:28.000000 crawlab-demo-0.0.6.post7/crawlab_demo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-23 06:56:28.000000 crawlab-demo-0.0.6.post7/crawlab_demo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 06:56:28.478059 crawlab-demo-0.0.6.post7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      925 2022-12-23 06:56:04.000000 crawlab-demo-0.0.6.post7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.599964 crawlab-demo-0.0.6.post9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2022-12-23 08:09:45.595964 crawlab-demo-0.0.6.post9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.579964 crawlab-demo-0.0.6.post9/crawlab_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.583963 crawlab-demo-0.0.6.post9/crawlab_demo/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/actions/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/actions/import_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/actions/reimport_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/actions/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.583963 crawlab-demo-0.0.6.post9/crawlab_demo/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.583963 crawlab-demo-0.0.6.post9/crawlab_demo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/demo.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.575964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.575964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.583963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/basic/crawlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/basic/go.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    23756 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/basic/go.sum
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/basic/main.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.583963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/colly_scrapy_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/colly_scrapy_docs/crawlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/colly_scrapy_docs/go.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    27283 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/colly_scrapy_docs/go.sum
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/colly_scrapy_docs/main.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.587963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/rod_github/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/rod_github/crawlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/rod_github/go.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    23275 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/rod_github/go.sum
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/rod_github/main.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.575964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/node/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.587963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/node/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/node/basic/crawlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/node/basic/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.587963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/node/puppeteer_163_tech_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/node/puppeteer_163_tech_news/crawlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/node/puppeteer_163_tech_news/main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.579964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.587963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/basic/crawlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/basic/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.587963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.587963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.587963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/spiders/books.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/crawlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/scrapy.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.587963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.587963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.587963 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/spiders/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/scrapy.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.591964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.591964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.591964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/spiders/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/scrapy.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.591964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.591964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.591964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/spiders/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/scrapy.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.591964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/playwright_bing/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/playwright_bing/crawlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/playwright_bing/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.591964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/crawlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.595964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.595964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/spiders/baidu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.595964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/crawlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.595964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.595964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/spiders/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/spiders/quotes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.595964 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/selenium_36kr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/selenium_36kr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/selenium_36kr/crawlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/selenium_36kr/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.595964 crawlab-demo-0.0.6.post9/crawlab_demo/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/models/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/models/spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.595964 crawlab-demo-0.0.6.post9/crawlab_demo/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/crawlab_demo/test/demo_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 08:09:45.583963 crawlab-demo-0.0.6.post9/crawlab_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2022-12-23 08:09:45.000000 crawlab-demo-0.0.6.post9/crawlab_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2022-12-23 08:09:45.000000 crawlab-demo-0.0.6.post9/crawlab_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 08:09:45.000000 crawlab-demo-0.0.6.post9/crawlab_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-23 08:09:45.000000 crawlab-demo-0.0.6.post9/crawlab_demo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-23 08:09:45.000000 crawlab-demo-0.0.6.post9/crawlab_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-23 08:09:45.000000 crawlab-demo-0.0.6.post9/crawlab_demo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 08:09:45.599964 crawlab-demo-0.0.6.post9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2022-12-23 08:09:18.000000 crawlab-demo-0.0.6.post9/setup.py
```

### Comparing `crawlab-demo-0.0.6.post7/LICENSE` & `crawlab-demo-0.0.6.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/actions/validate.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/actions/validate.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/cli/main.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/cli/main.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/demo.json` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/demo.json`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/basic/go.sum` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/basic/go.sum`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/colly_scrapy_docs/go.sum` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/colly_scrapy_docs/go.sum`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/colly_scrapy_docs/main.go` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/colly_scrapy_docs/main.go`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/rod_github/go.sum` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/rod_github/go.sum`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/golang/rod_github/main.go` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/golang/rod_github/main.go`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/node/puppeteer_163_tech_news/main.js` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/node/puppeteer_163_tech_news/main.js`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/middlewares.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/middlewares.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/settings.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/settings.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/bookdepository/bookdepository/spiders/books.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/bookdepository/bookdepository/spiders/books.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/middlewares.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/middlewares.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/settings.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/settings.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/github_search/github_search/spiders/github.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/github_search/github_search/spiders/github.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/middlewares.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/middlewares.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/settings.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/settings.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hackernews/hackernews/spiders/news.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hackernews/hackernews/spiders/news.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/middlewares.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/middlewares.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/settings.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/settings.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/hsph/hsph/spiders/news.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/hsph/hsph/spiders/news.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/playwright_bing/main.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/playwright_bing/main.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/middlewares.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/middlewares.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/settings.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/settings.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/spiders/baidu.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_baidu/scrapy_baidu/spiders/baidu.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/middlewares.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/middlewares.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/settings.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/settings.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/spiders/quotes.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/scrapy_quotes/scrapy_quotes/spiders/quotes.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/data/spiders/python/selenium_36kr/main.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/data/spiders/python/selenium_36kr/main.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/demo.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/demo.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/models/spider.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/models/spider.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo/test/demo_test.py` & `crawlab-demo-0.0.6.post9/crawlab_demo/test/demo_test.py`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/crawlab_demo.egg-info/SOURCES.txt` & `crawlab-demo-0.0.6.post9/crawlab_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlab-demo-0.0.6.post7/setup.py` & `crawlab-demo-0.0.6.post9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open('requirements.txt', 'r') as f:
     install_requires = f.read().split('\n')
 
 setup(
     name='crawlab-demo',
-    version='0.0.6-7',
+    version='0.0.6-9',
     packages=find_packages(),
     url='https://github.com/crawlab-team/crawlab-demo',
     license='BSD-3-Clause',
     author='tikazyq',
     author_email='tikazyq@163.com',
     description='Demo for Crawlab',
     long_description=long_description,
```

