# Comparing `tmp/kraken-rebalance-bot-0.5.7.3.tar.gz` & `tmp/kraken-rebalance-bot-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken-rebalance-bot-0.5.7.3.tar", last modified: Sun Apr  2 19:51:02 2023, max compression
+gzip compressed data, was "kraken-rebalance-bot-1.0.0.tar", last modified: Sun Jun 18 08:11:49 2023, max compression
```

## Comparing `kraken-rebalance-bot-0.5.7.3.tar` & `kraken-rebalance-bot-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,33 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-02 19:51:02.295178 kraken-rebalance-bot-0.5.7.3/
--rw-r--r--   0 benjamin   (501) staff       (20)    33149 2022-11-30 07:24:35.000000 kraken-rebalance-bot-0.5.7.3/LICENSE
--rw-r--r--   0 benjamin   (501) staff       (20)       26 2022-11-30 12:52:55.000000 kraken-rebalance-bot-0.5.7.3/MANIFEST.in
--rw-r--r--   0 benjamin   (501) staff       (20)    12163 2023-04-02 19:51:02.294805 kraken-rebalance-bot-0.5.7.3/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)    11462 2023-01-25 18:58:42.000000 kraken-rebalance-bot-0.5.7.3/README.md
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-02 19:51:02.292398 kraken-rebalance-bot-0.5.7.3/krakenRebalanceBot/
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2022-11-30 07:17:47.000000 kraken-rebalance-bot-0.5.7.3/krakenRebalanceBot/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)    14701 2023-01-25 18:52:23.000000 kraken-rebalance-bot-0.5.7.3/krakenRebalanceBot/bot.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-04-02 19:51:02.294337 kraken-rebalance-bot-0.5.7.3/kraken_rebalance_bot.egg-info/
--rw-r--r--   0 benjamin   (501) staff       (20)    12163 2023-04-02 19:51:02.000000 kraken-rebalance-bot-0.5.7.3/kraken_rebalance_bot.egg-info/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)      314 2023-04-02 19:51:02.000000 kraken-rebalance-bot-0.5.7.3/kraken_rebalance_bot.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin   (501) staff       (20)        1 2023-04-02 19:51:02.000000 kraken-rebalance-bot-0.5.7.3/kraken_rebalance_bot.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       50 2023-04-02 19:51:02.000000 kraken-rebalance-bot-0.5.7.3/kraken_rebalance_bot.egg-info/requires.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       19 2023-04-02 19:51:02.000000 kraken-rebalance-bot-0.5.7.3/kraken_rebalance_bot.egg-info/top_level.txt
--rw-r--r--   0 benjamin   (501) staff       (20)       38 2023-04-02 19:51:02.297154 kraken-rebalance-bot-0.5.7.3/setup.cfg
--rwxr-xr-x   0 benjamin   (501) staff       (20)     4398 2023-04-02 19:51:00.000000 kraken-rebalance-bot-0.5.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:11:49.241355 kraken-rebalance-bot-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:11:49.237355 kraken-rebalance-bot-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:11:49.241355 kraken-rebalance-bot-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/.github/workflows/_build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/.github/workflows/_codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/.github/workflows/_pre_commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/.github/workflows/_pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21154 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    33149 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    49842 2023-06-18 08:11:49.241355 kraken-rebalance-bot-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   234803 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/backtesting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/example_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:11:49.241355 kraken-rebalance-bot-1.0.0/kraken_rebalance_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49842 2023-06-18 08:11:49.000000 kraken-rebalance-bot-1.0.0/kraken_rebalance_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-18 08:11:49.000000 kraken-rebalance-bot-1.0.0/kraken_rebalance_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 08:11:49.000000 kraken-rebalance-bot-1.0.0/kraken_rebalance_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-18 08:11:49.000000 kraken-rebalance-bot-1.0.0/kraken_rebalance_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 08:11:49.000000 kraken-rebalance-bot-1.0.0/kraken_rebalance_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-18 08:11:49.000000 kraken-rebalance-bot-1.0.0/kraken_rebalance_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 08:11:49.241355 kraken-rebalance-bot-1.0.0/rebalance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/rebalance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-18 08:11:49.000000 kraken-rebalance-bot-1.0.0/rebalance/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-06-18 08:11:39.000000 kraken-rebalance-bot-1.0.0/rebalance/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 08:11:49.241355 kraken-rebalance-bot-1.0.0/setup.cfg
```

### Comparing `kraken-rebalance-bot-0.5.7.3/LICENSE` & `kraken-rebalance-bot-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken-rebalance-bot-0.5.7.3/PKG-INFO` & `kraken-rebalance-bot-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,61 @@
-Metadata-Version: 2.1
-Name: kraken-rebalance-bot
-Version: 0.5.7.3
-Summary: A basic rebalance trading bot for the Kraken Cryptocurrency Exchange.
-Home-page: https://github.com/btschwertfeger/Kraken-Rebalance-Bot
-Author: Benjamin Thomas Schwertfeger
-Author-email: development@b-schwertfeger.de
-License: GPLv3
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 <h1 align=center>
-    Welcome to the Spot Rebalance Bot for the Kraken Cryptocurrency Exchange 🐙
+    Welcome to the Spot rebalance bot for the Kraken Cryptocurrency Exchange 🐙
 </h1>
 
 <div align="center">
 
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/btschwertfeger/Kraken-Rebalance-Bot)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-orange.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Generic badge](https://img.shields.io/badge/python-3.7+-blue.svg)](https://shields.io/)
-
-<!-- [![Downloads](https://static.pepy.tech/personalized-badge/kraken-rebalance-bot?period=total&units=abbreviation&left_color=grey&right_color=orange&left_text=downloads)](https://pepy.tech/project/kraken-rebalance-bot) -->
-
-![ql-workflow](https://github.com/btschwertfeger/Kraken-Rebalance-Bot/actions/workflows/codeql.yml/badge.svg)
-![python-package](https://github.com/btschwertfeger/Kraken-Rebalance-Bot/actions/workflows/python-package.yml/badge.svg)
+[![Generic badge](https://img.shields.io/badge/python-3.11+-blue.svg)](https://shields.io/)
+![release](https://shields.io/github/release-date/btschwertfeger/kraken-rebalance-bot)
+[![release](https://img.shields.io/pypi/v/kraken-rebalance-bot)](https://pypi.org/project/kraken-rebalance-bot/)
+[![Typing](https://img.shields.io/badge/typing-mypy-informational)](https://mypy-lang.org/)
+![ql-workflow](https://github.com/btschwertfeger/Kraken-Rebalance-Bot/actions/workflows/codeql.yaml/badge.svg)
 
 </div>
 
-<h3>
-This is an unofficial trading bot that performs buys and sells on the Kraken cryptocurrency exchange using Python.
-</h3>
+> ⚠️ This is an unofficial trading bot that performs buys and sells
+> on the Kraken cryptocurrency exchange using Python.
+
+Backend to access the Kraken API: [python-kraken-sdk](https://github.com/btschwertfeger/python-kraken-sdk)
 
 ---
 
 ## 📌 Disclaimer
 
-There is no guarantee that this software will work flawlessly at this or later times. Of course, no responsibility is taken for possible profits or losses. This software probably has some errors in it, so use it at your own risk. Also no one should be motivated or tempted to invest assets in speculative forms of investment. By using this software you release the author(s) from any liability regarding the use of this software.
+There is no guarantee that this software will work flawlessly at this or
+later times. Of course, no responsibility is taken for possible profits or
+losses. This software probably has some errors in it, so use it at your own
+risk. Also no one should be motivated or tempted to invest assets in
+speculative forms of investment. By using this software you release the
+author(s) from any liability regarding the use of this software.
 
 It is not certain that this software will ever lead to profits.
 
-## Package Update
-
-- January 25, 2023
-
 ---
 
 ## 📝 The Strategy
 
 This algorithm can buy and sell one or more Spot assets without leverage.
 
-The goal is to hold a certain amount of each base currency so that, for example, there is always about $1000 worth of BTC in the portfolio. If the price of Bitocoin increases so that there is now $1050 worth of Bitcoin in the portfolio, the excess $50 is sold. If the price of Bitcoin falls, so that the Bitcoin in the portfolio are only worth $950, the algorithm buys Bitcoin, to hold a value of about $1000 in Bitcoin in the portfolio again.
-
-The algorithm checks the price range every 6 hours by default. The margin, from how many percent price difference the algorithm becomes active, can also be adjusted.
+The goal is to hold a certain amount of each base currency so that, for
+example, there is always about $1000 worth of BTC in the portfolio. If
+the price of Bitcoin increases so that there is now $1050 worth of
+Bitcoin in the portfolio, the excess $50 is sold. If the price of
+Bitcoin falls, so that the Bitcoin in the portfolio are only worth $950,
+the algorithm buys Bitcoin, to hold a value of about $1000 in Bitcoin
+in the portfolio again.
+
+The algorithm checks the price range every 6 hours by default. The
+margin, from how many percent price difference the algorithm becomes
+active, can also be adjusted.
 
-Actions can be logged on the command-line using the logging module with active INFO-level and can also be sent to a telegram bot.
+Actions can be logged on the command-line using the logging module with
+active INFO-level and can also be sent to a telegram bot.
 
 ---
 
 ## ⚙️ Quick start and configuration
 
 ### 0. Check the source code of this algorithm on GitHub and read the README.md carefully
 
@@ -81,112 +71,126 @@
 
 - https://www.kraken.com/u/security/api
 
 ### 3. (optional) Create a Telegram Bot to get notified when the algorithm takes action
 
 1. Create a bot using <a href="https://t.me/BotFather" target="_blank">@BotFather</a>
 2. Write down/remember the token
-3. Start <a href="https://t.me/RawDataBot" target="_blank">@RawDataBot</a> and write down your personal chat id
+3. Start <a href="https://t.me/RawDataBot" target="_blank">@RawDataBot</a>
+   and write down your personal `chat_id`
 
 ### 4. Setup the configuration and start the algorithm
 
-#### a.) Using docker
-
-Build an image and pass a config when starting the container:
+An example configuration can be found in `example_config.json` and looks like
+this:
 
-```bash
-docker build -t krb:latest examples/docker
-docker run --env-file examples/docker/.docker.env krb
+```json
+{
+  "base_currency": ["ETH", "XBT"],    # base asset(s) to maintain
+  "quote_currency": ["USD", "USD"],   # quote asset(s) to trade with
+  "target_quantity": [500, 500],      # how many of the base to hold (value in quote)
+  "quote_to_maintain": [200, 200],    # freezed quote
+  "margin": [0.035, 0.035],           # buy/sell threshold
+  "lowest_buy_price": [1000, 15000],  # don't buy below this price
+  "times": ["06:00", "18:00"],        # has no effect if use_build_in_scheduler is true
+  "use_build_in_scheduler": false,    # if set to false, the script will only run once
+  "demo": true,                       # set to false to enable trading
+  "telegram": {                       # optional to get notified via telegram
+      "token": "telegram-bot-token",
+      "chat_id": "your-telegram-chat-id"
+  }
+}
 ```
 
-(`examples/docker/.docker.env` contains the configuration for this bot)
-
-Output:
+In the following a minimal working example is shown that uses this strategy
+to hold a `target_quantity` of $500 of ETH and $500 worth of XBT (as in the
+example config above). Both are traded against USD. The `demo` key must be
+set to `False` to enable the trading functionality. Of course, this also works
+with only one asset, too.
 
 ```bash
-2023/01/25 18:54:29 main,line: 42  WARNING | Not using telegram.
-2023/01/25 18:54:29 bot,line: 59     INFO | Starting the `kraken-rebalance-bot`
-2023/01/25 18:54:29 bot,line: 62     INFO | Using scheduled times @['00:00', '06:00', '12:00', '18:00']
-...
+rebalance \
+  --api-key "your-kraken-api-key-here" \
+  --secret-key "secret-key-here" \
+  --config config.json
 ```
 
-#### b.) Using a Python script
-
-In the following a minimal working example is shown that uses this strategy to hold a `target_quantity` of $500 of ETH and $500 worth of XBT. Both are traded agains USD. The `demo` key must be set to `False` to enable the trading functionality. Of course, this also works with only one asset, too.
-
-```python
-from krakenRebalanceBot.bot import RebalanceBot
-
-def main() -> None:
-    bot = RebalanceBot(
-        key='kraken-api-key',
-        secret='kraken-secret-key',
-        config={
-            'base_currency': ['ETH', 'XBT'],    # base assets to maintain
-            'quote_currency': ['USD', 'USD'],   # quote assets to trade with
-            'target_quantity': [500, 500],      # how many of the base to hold (value in quote)
-            'quote_to_maintain': [200, 200],    # freezed quote/dont trade with this
-            'margin': [0.035, 0.035],           # buy/sell threshold
-            'lowest_buy_price': [1000, 15000],  # dont buy below this price
-            'times': ['06:00', '18:00'],        # optional of use_build_in_sheduler is True
-            'use_build_in_sheduler': False,     # if set to False, the script will only run once
-            'demo': True,                       # set to false to enable trading
-            'telegram': {                       # optional to get notified via telegram
-                'token': 'telegram-bot-token',
-                'chat_id': 'your-telegram-chat-id'
-            }
-    })
-    bot.run()  # start the bot
-
-if __name__ == '__main__': main()
-```
-
-The file `/examples/main.py` serves as an example on how to initialize and run this trading algorithm using the `.env` and `config.json` files (see <a href="https://github.com/btschwertfeger/Kraken-Rebalance-Bot" target="_blank">GitHub</a>). There is also a Jupyter notebook in which one can test the algorithm without risking any assets.
-
-- <b>To see the output on the command line you need to enable logging with level INFO as shown in the example script.</b>
-- <b>If `use_build_in_sheduler` is enabled, there will be no output until the time is one of `times`.</b>
+Note: If `use_build_in_scheduler` is enabled, there will be no output until
+the time is one of `times`.
 
 ---
 
-## 📖 Documentation of configuration arguments:
+## 📖 Configuration
 
-| Key                     | Type                             | Description                                                                                                                                                             |
-| ----------------------- | -------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `base_currency`         | `List[str]`                      | Array of base currrncies to trade and hold.                                                                                                                             |
-| `quote_currency`        | `List[str]`                      | Array of quote currencies to trade the base currency with.                                                                                                              |
-| `target_quantity`       | `List[float] \| List[int]`       | Defines how much of a base currency should be held. This value is the worth of the base currency in quote currency.                                                     |
-| `quote_to_maintain`     | `List[float] \| List[int]`       | How much of quote currency should not be touched in the portfolio.                                                                                                      |
-| `margin`                | `List[float]`                    | Rebalance levels e.g. 0.035 = 3.5%: at a change of 3.5% the algorithm will buy or sell the missing/surplus quantity                                                     |
-| `lowest_buy_price`      | `List[float]`                    | (optional) The bot will not buy if the price falls below this price to avoid catching a falling knife. Acts Kind of stop loss, but without selling.                     |
-| `times`                 | `List[str]`                      | (optional, default: `['00:00', '06:00', '12:00', '18:00']`) At which time the bot should check the balances.                                                            |
-| `use_build_in_sheduler` | `bool`                           | (optional, default: `False`) Checks the balances once and exits if set to False. Otherwise the program will run forever and check the balances at the specified `times` |
-| `demo`                  | `bool`                           | Trade or not sample trade output. Set to True if you know what this algorithm does.                                                                                     |
-| `telegram`              | `{'chat_id': str, 'token': str}` | (optional) Specify token and chat id to get notified when the bot does something.                                                                                       |
-
-If `use_build_in_sheduler` is set to `False`, the program is executed once and ends after the iteration over all assets. This offers the possibility to create own scripts, which execute this algorithm at individual times (e.g. using <a href="https://wiki.ubuntuusers.de/Cron/" target="_blank">cron</a>).
+| Key                      | Type                             | Description                                                                                                                                                             |
+| ------------------------ | -------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `base_currency`          | `list[str]`                      | List of base currencies to trade and hold.                                                                                                                              |
+| `quote_currency`         | `list[str]`                      | List of quote currencies to trade the base currency with.                                                                                                               |
+| `target_quantity`        | `list[float] \| list[int]`       | Defines how much of a base currency should be held. This value is the worth of the base currency in quote currency.                                                     |
+| `quote_to_maintain`      | `list[float] \| list[int]`       | How much of quote currency should not be touched in the portfolio.                                                                                                      |
+| `margin`                 | `list[float]`                    | Rebalance levels e.g. 0.035 = 3.5%: at a change of 3.5% the algorithm will buy or sell the missing/surplus quantity                                                     |
+| `lowest_buy_price`       | `list[float]`                    | (optional) The bot will not buy if the price falls below this price to avoid catching a falling knife. Acts Kind of stop loss, but without selling.                     |
+| `times`                  | `list[str]`                      | (optional, default: `['00:00', '06:00', '12:00', '18:00']`) At which time the bot should check the balances.                                                            |
+| `use_build_in_scheduler` | `bool`                           | (optional, default: `False`) Checks the balances once and exits if set to False. Otherwise the program will run forever and check the balances at the specified `times` |
+| `demo`                   | `bool`                           | Trade or not sample trade output. Set to True if you know what this algorithm does.                                                                                     |
+| `telegram`               | `{'chat_id': str, 'token': str}` | (optional) Specify token and chat id to get notified when the bot does something.                                                                                       |
+
+If `use_build_in_scheduler` is set to `false`, the program is executed once
+and ends after the iteration over all assets. This offers the possibility to
+create own scripts, which execute this algorithm at individual times
+(e.g. using <a href="https://wiki.ubuntuusers.de/Cron/" target="_blank">cron</a>).
 
 ---
 
 ## 📍 Notes
 
-- Make sure to always have enough quote currency in your Kraken portfolio. Too low `target_quantity` values can cause the bot not to trade or even crash. Therefore, pay attention to the <a href="https://support.kraken.com/hc/en-us/articles/360050845612-Minimum-order-size-volume-for-trading-and-decimal-precision-for-residents-of-Japan-" target="_blank">minimum order sizes</a>.
-
-  - Example:
-    - situation:
-      - minimal order size of ETH is 0.01
-      - price of ETH: $1300
-      - `margin` is set to 0.04
-      - `target_quantity` is 200
-    - what will happen:
-      - If your actual holdings of ETH is $192 the bot tries to buy Ethereum with a volume of $8 because $200 - $200 \* 0.04 will trigger the buy order. But the minimum ordersize of Ethereum is 0.01 ETH (see <a href="https://support.kraken.com/hc/en-us/articles/360050845612-Minimum-order-size-volume-for-trading-and-decimal-precision-for-residents-of-Japan-" target="_blank">here</a>), and with a price of $1300 0.01 ETH equals $13 so: $13 < $8 will raise an error.
-  - So make sure that the minimum order sizes of the respective assets are consistent with the `margin` value and the `target_quantity`. The example would work if the `targe_quantity` is set to 500, because $500 _ 0.04 = $20 which is larger than $1300 _ 0.01 = $13.
-  - Also make sure that there is enough quote currency, otherwise the bot cannot buy anything.
-
-- This strategy is one of the simplest and most basic approaches for trading cryptocurrencies. For this reason, it should be noted here that this does not necessarily lead to profits. Before running such an algorithm, everyone should be clear about what products are being traded, what these products are for in the first place, and what makes them valuable. Even the best companies, stocks, materials, and also cryptocurrencies can become worthless from one day to the next, so everyone should do their own research and make their decisions based on these results.
+- Make sure to always have enough quote currency in your Kraken portfolio. Too
+  low `target_quantity` values can cause the bot not to trade or even crash.
+  Therefore, pay attention to the <a href="https://support.kraken.com/hc/en-us/articles/360050845612-Minimum-order-size-volume-for-trading-and-decimal-precision-for-residents-of-Japan-" target="_blank">minimum order sizes</a>.
+
+**Example situation**:
+
+- minimal order size of ETH is 0.01
+- price of ETH: $1300
+- `margin` is set to 0.04
+- `target_quantity` is 200
+- what will happen:
+
+  - If your actual holdings of ETH is $192 the bot tries to buy Ethereum
+    with a volume of $8 because $200 - $200 \* 0.04 will trigger the buy
+    order. But the minimum order size of Ethereum is 0.01 ETH
+    (see <a href="https://support.kraken.com/hc/en-us/articles/360050845612-Minimum-order-size-volume-for-trading-and-decimal-precision-for-residents-of-Japan-" target="_blank">here</a>),
+    and with a price of $1300 => 0.01 ETH equals $13 so: $13 < $8 will
+    raise an error.
+  - So make sure that the minimum order sizes of the respective assets
+    are consistent with the `margin` value and the `target_quantity`.
+    The example would work if the `targe_quantity` is set to 500,
+    because $500 _ 0.04 = $20 which is larger than $1300 _ 0.01 = $13.
+  - Also make sure that there is enough quote currency, otherwise the
+    bot cannot buy anything.
+
+- This strategy is one of the simplest and most basic approaches for trading
+  cryptocurrencies. For this reason, it should be noted here that this does not
+  necessarily lead to profits. Before running such an algorithm, everyone
+  should be clear about what products are being traded, what these products are
+  for in the first place, and what makes them valuable. Even the best companies,
+  stocks, materials, and also cryptocurrencies can become worthless from one day
+  to the next, so everyone should do their own research and make their decisions
+  based on these results.
+
+- It has been decided here not to present any material regarding the profitability
+  of this algorithm, as this could lead you to make your decisions based on my
+  successes and failures. What works once or over a long period of time does not
+  necessarily work in the future. But please let me know what you think about this
+  basic algorithm and what could be improved.
+
+- For any problems or suggestions - please open an issue.
 
-- It has been decided here not to present any material regarding the profitability of this algorithm, as this could lead you to make your decisions based on my successes and failures. What works once or over a long period of time does not necessarily work in the future. But please let me know what you think about this basic algorithm and what could be improved.
+---
 
-- For any problems, issues, and errors, please open an issue.
+## 🆕 Contributions
 
----
+… are welcome!
 
+## 🔭 References
 
+- https://python-kraken-sdk.readthedocs.io/en/stable
```

#### html2text {}

```diff
@@ -1,130 +1,112 @@
-Metadata-Version: 2.1 Name: kraken-rebalance-bot Version: 0.5.7.3 Summary: A
-basic rebalance trading bot for the Kraken Cryptocurrency Exchange. Home-page:
-https://github.com/btschwertfeger/Kraken-Rebalance-Bot Author: Benjamin Thomas
-Schwertfeger Author-email: development@b-schwertfeger.de License: GPLv3
-Platform: UNKNOWN Classifier: License :: OSI Approved :: GNU General Public
-License v3 (GPLv3) Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3.7 Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS Classifier: Operating System :: Unix
-Requires-Python: >=3.7.0 Description-Content-Type: text/markdown License-File:
-LICENSE
-****** Welcome to the Spot Rebalance Bot for the Kraken Cryptocurrency Exchange
+****** Welcome to the Spot rebalance bot for the Kraken Cryptocurrency Exchange
                                   ð ******
  [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://
  github.com/btschwertfeger/Kraken-Rebalance-Bot) [![License: GPL v3](https://
  img.shields.io/badge/License-GPLv3-orange.svg)](https://www.gnu.org/licenses/
-gpl-3.0) [![Generic badge](https://img.shields.io/badge/python-3.7+-blue.svg)]
-(https://shields.io/)  ![ql-workflow](https://github.com/btschwertfeger/Kraken-
-Rebalance-Bot/actions/workflows/codeql.yml/badge.svg) ![python-package](https:/
-   /github.com/btschwertfeger/Kraken-Rebalance-Bot/actions/workflows/python-
-                            package.yml/badge.svg)
-**** This is an unofficial trading bot that performs buys and sells on the
-Kraken cryptocurrency exchange using Python. ****
---- ## ð Disclaimer There is no guarantee that this software will work
+gpl-3.0) [![Generic badge](https://img.shields.io/badge/python-3.11+-blue.svg)]
+   (https://shields.io/) ![release](https://shields.io/github/release-date/
+btschwertfeger/kraken-rebalance-bot) [![release](https://img.shields.io/pypi/v/
+   kraken-rebalance-bot)](https://pypi.org/project/kraken-rebalance-bot/) [!
+[Typing](https://img.shields.io/badge/typing-mypy-informational)](https://mypy-
+ lang.org/) ![ql-workflow](https://github.com/btschwertfeger/Kraken-Rebalance-
+                 Bot/actions/workflows/codeql.yaml/badge.svg)
+> â ï¸ This is an unofficial trading bot that performs buys and sells > on
+the Kraken cryptocurrency exchange using Python. Backend to access the Kraken
+API: [python-kraken-sdk](https://github.com/btschwertfeger/python-kraken-sdk) -
+-- ## ð Disclaimer There is no guarantee that this software will work
 flawlessly at this or later times. Of course, no responsibility is taken for
 possible profits or losses. This software probably has some errors in it, so
 use it at your own risk. Also no one should be motivated or tempted to invest
 assets in speculative forms of investment. By using this software you release
 the author(s) from any liability regarding the use of this software. It is not
-certain that this software will ever lead to profits. ## Package Update -
-January 25, 2023 --- ## ð The Strategy This algorithm can buy and sell one
-or more Spot assets without leverage. The goal is to hold a certain amount of
-each base currency so that, for example, there is always about $1000 worth of
-BTC in the portfolio. If the price of Bitocoin increases so that there is now
-$1050 worth of Bitcoin in the portfolio, the excess $50 is sold. If the price
-of Bitcoin falls, so that the Bitcoin in the portfolio are only worth $950, the
-algorithm buys Bitcoin, to hold a value of about $1000 in Bitcoin in the
-portfolio again. The algorithm checks the price range every 6 hours by default.
-The margin, from how many percent price difference the algorithm becomes
-active, can also be adjusted. Actions can be logged on the command-line using
-the logging module with active INFO-level and can also be sent to a telegram
-bot. --- ## âï¸ Quick start and configuration ### 0. Check the source code
-of this algorithm on GitHub and read the README.md carefully - https://
-github.com/btschwertfeger/Kraken-Rebalance-Bot ### 1. Install the Python
-module: ```bash python3 -m pip install kraken-rebalance-bot ``` ### 2. Register
-at Kraken and generate API keys with trading access: - https://www.kraken.com/
-u/security/api ### 3. (optional) Create a Telegram Bot to get notified when the
-algorithm takes action 1. Create a bot using @BotFather 2. Write down/remember
-the token 3. Start @RawDataBot and write down your personal chat id ### 4.
-Setup the configuration and start the algorithm #### a.) Using docker Build an
-image and pass a config when starting the container: ```bash docker build -
-t krb:latest examples/docker docker run --env-file examples/docker/.docker.env
-krb ``` (`examples/docker/.docker.env` contains the configuration for this bot)
-Output: ```bash 2023/01/25 18:54:29 main,line: 42 WARNING | Not using telegram.
-2023/01/25 18:54:29 bot,line: 59 INFO | Starting the `kraken-rebalance-bot`
-2023/01/25 18:54:29 bot,line: 62 INFO | Using scheduled times @['00:00', '06:
-00', '12:00', '18:00'] ... ``` #### b.) Using a Python script In the following
-a minimal working example is shown that uses this strategy to hold a
-`target_quantity` of $500 of ETH and $500 worth of XBT. Both are traded agains
+certain that this software will ever lead to profits. --- ## ð The Strategy
+This algorithm can buy and sell one or more Spot assets without leverage. The
+goal is to hold a certain amount of each base currency so that, for example,
+there is always about $1000 worth of BTC in the portfolio. If the price of
+Bitcoin increases so that there is now $1050 worth of Bitcoin in the portfolio,
+the excess $50 is sold. If the price of Bitcoin falls, so that the Bitcoin in
+the portfolio are only worth $950, the algorithm buys Bitcoin, to hold a value
+of about $1000 in Bitcoin in the portfolio again. The algorithm checks the
+price range every 6 hours by default. The margin, from how many percent price
+difference the algorithm becomes active, can also be adjusted. Actions can be
+logged on the command-line using the logging module with active INFO-level and
+can also be sent to a telegram bot. --- ## âï¸ Quick start and configuration
+### 0. Check the source code of this algorithm on GitHub and read the README.md
+carefully - https://github.com/btschwertfeger/Kraken-Rebalance-Bot ### 1.
+Install the Python module: ```bash python3 -m pip install kraken-rebalance-bot
+``` ### 2. Register at Kraken and generate API keys with trading access: -
+https://www.kraken.com/u/security/api ### 3. (optional) Create a Telegram Bot
+to get notified when the algorithm takes action 1. Create a bot using
+@BotFather 2. Write down/remember the token 3. Start @RawDataBot and write down
+your personal `chat_id` ### 4. Setup the configuration and start the algorithm
+An example configuration can be found in `example_config.json` and looks like
+this: ```json { "base_currency": ["ETH", "XBT"], # base asset(s) to maintain
+"quote_currency": ["USD", "USD"], # quote asset(s) to trade with
+"target_quantity": [500, 500], # how many of the base to hold (value in quote)
+"quote_to_maintain": [200, 200], # freezed quote "margin": [0.035, 0.035], #
+buy/sell threshold "lowest_buy_price": [1000, 15000], # don't buy below this
+price "times": ["06:00", "18:00"], # has no effect if use_build_in_scheduler is
+true "use_build_in_scheduler": false, # if set to false, the script will only
+run once "demo": true, # set to false to enable trading "telegram": { #
+optional to get notified via telegram "token": "telegram-bot-token", "chat_id":
+"your-telegram-chat-id" } } ``` In the following a minimal working example is
+shown that uses this strategy to hold a `target_quantity` of $500 of ETH and
+$500 worth of XBT (as in the example config above). Both are traded against
 USD. The `demo` key must be set to `False` to enable the trading functionality.
-Of course, this also works with only one asset, too. ```python from
-krakenRebalanceBot.bot import RebalanceBot def main() -> None: bot =
-RebalanceBot( key='kraken-api-key', secret='kraken-secret-key', config=
-{ 'base_currency': ['ETH', 'XBT'], # base assets to maintain 'quote_currency':
-['USD', 'USD'], # quote assets to trade with 'target_quantity': [500, 500], #
-how many of the base to hold (value in quote) 'quote_to_maintain': [200, 200],
-# freezed quote/dont trade with this 'margin': [0.035, 0.035], # buy/sell
-threshold 'lowest_buy_price': [1000, 15000], # dont buy below this price
-'times': ['06:00', '18:00'], # optional of use_build_in_sheduler is True
-'use_build_in_sheduler': False, # if set to False, the script will only run
-once 'demo': True, # set to false to enable trading 'telegram': { # optional to
-get notified via telegram 'token': 'telegram-bot-token', 'chat_id': 'your-
-telegram-chat-id' } }) bot.run() # start the bot if __name__ == '__main__':
-main() ``` The file `/examples/main.py` serves as an example on how to
-initialize and run this trading algorithm using the `.env` and `config.json`
-files (see GitHub). There is also a Jupyter notebook in which one can test the
-algorithm without risking any assets. - To see the output on the command line
-you need to enable logging with level INFO as shown in the example script. - If
-`use_build_in_sheduler` is enabled, there will be no output until the time is
-one of `times`. --- ## ð Documentation of configuration arguments: | Key |
-Type | Description | | ----------------------- | ------------------------------
--- | --------------------------------------------------------------------------
+Of course, this also works with only one asset, too. ```bash rebalance \ --api-
+key "your-kraken-api-key-here" \ --secret-key "secret-key-here" \ --config
+config.json ``` Note: If `use_build_in_scheduler` is enabled, there will be no
+output until the time is one of `times`. --- ## ð Configuration | Key | Type
+| Description | | ------------------------ | -------------------------------- |
 -------------------------------------------------------------------------------
--------------- | | `base_currency` | `List[str]` | Array of base currrncies to
-trade and hold. | | `quote_currency` | `List[str]` | Array of quote currencies
-to trade the base currency with. | | `target_quantity` | `List[float] \| List
+-------------------------------------------------------------------------------
+--------- | | `base_currency` | `list[str]` | List of base currencies to trade
+and hold. | | `quote_currency` | `list[str]` | List of quote currencies to
+trade the base currency with. | | `target_quantity` | `list[float] \| list
 [int]` | Defines how much of a base currency should be held. This value is the
-worth of the base currency in quote currency. | | `quote_to_maintain` | `List
-[float] \| List[int]` | How much of quote currency should not be touched in the
-portfolio. | | `margin` | `List[float]` | Rebalance levels e.g. 0.035 = 3.5%:
+worth of the base currency in quote currency. | | `quote_to_maintain` | `list
+[float] \| list[int]` | How much of quote currency should not be touched in the
+portfolio. | | `margin` | `list[float]` | Rebalance levels e.g. 0.035 = 3.5%:
 at a change of 3.5% the algorithm will buy or sell the missing/surplus quantity
-| | `lowest_buy_price` | `List[float]` | (optional) The bot will not buy if the
+| | `lowest_buy_price` | `list[float]` | (optional) The bot will not buy if the
 price falls below this price to avoid catching a falling knife. Acts Kind of
-stop loss, but without selling. | | `times` | `List[str]` | (optional, default:
+stop loss, but without selling. | | `times` | `list[str]` | (optional, default:
 `['00:00', '06:00', '12:00', '18:00']`) At which time the bot should check the
-balances. | | `use_build_in_sheduler` | `bool` | (optional, default: `False`)
+balances. | | `use_build_in_scheduler` | `bool` | (optional, default: `False`)
 Checks the balances once and exits if set to False. Otherwise the program will
 run forever and check the balances at the specified `times` | | `demo` | `bool`
 | Trade or not sample trade output. Set to True if you know what this algorithm
 does. | | `telegram` | `{'chat_id': str, 'token': str}` | (optional) Specify
 token and chat id to get notified when the bot does something. | If
-`use_build_in_sheduler` is set to `False`, the program is executed once and
+`use_build_in_scheduler` is set to `false`, the program is executed once and
 ends after the iteration over all assets. This offers the possibility to create
 own scripts, which execute this algorithm at individual times (e.g. using
 cron). --- ## ð Notes - Make sure to always have enough quote currency in
 your Kraken portfolio. Too low `target_quantity` values can cause the bot not
-to trade or even crash. Therefore, pay attention to the minimum_order_sizes. -
-Example: - situation: - minimal order size of ETH is 0.01 - price of ETH: $1300
-- `margin` is set to 0.04 - `target_quantity` is 200 - what will happen: - If
-your actual holdings of ETH is $192 the bot tries to buy Ethereum with a volume
-of $8 because $200 - $200 \* 0.04 will trigger the buy order. But the minimum
-ordersize of Ethereum is 0.01 ETH (see here), and with a price of $1300 0.01
-ETH equals $13 so: $13 < $8 will raise an error. - So make sure that the
-minimum order sizes of the respective assets are consistent with the `margin`
-value and the `target_quantity`. The example would work if the `targe_quantity`
-is set to 500, because $500 _ 0.04 = $20 which is larger than $1300 _ 0.01 =
-$13. - Also make sure that there is enough quote currency, otherwise the bot
-cannot buy anything. - This strategy is one of the simplest and most basic
-approaches for trading cryptocurrencies. For this reason, it should be noted
-here that this does not necessarily lead to profits. Before running such an
-algorithm, everyone should be clear about what products are being traded, what
-these products are for in the first place, and what makes them valuable. Even
-the best companies, stocks, materials, and also cryptocurrencies can become
-worthless from one day to the next, so everyone should do their own research
-and make their decisions based on these results. - It has been decided here not
-to present any material regarding the profitability of this algorithm, as this
-could lead you to make your decisions based on my successes and failures. What
-works once or over a long period of time does not necessarily work in the
-future. But please let me know what you think about this basic algorithm and
-what could be improved. - For any problems, issues, and errors, please open an
-issue. ---
+to trade or even crash. Therefore, pay attention to the minimum_order_sizes.
+**Example situation**: - minimal order size of ETH is 0.01 - price of ETH:
+$1300 - `margin` is set to 0.04 - `target_quantity` is 200 - what will happen:
+- If your actual holdings of ETH is $192 the bot tries to buy Ethereum with a
+volume of $8 because $200 - $200 \* 0.04 will trigger the buy order. But the
+minimum order size of Ethereum is 0.01 ETH (see here), and with a price of
+$1300 => 0.01 ETH equals $13 so: $13 < $8 will raise an error. - So make sure
+that the minimum order sizes of the respective assets are consistent with the
+`margin` value and the `target_quantity`. The example would work if the
+`targe_quantity` is set to 500, because $500 _ 0.04 = $20 which is larger than
+$1300 _ 0.01 = $13. - Also make sure that there is enough quote currency,
+otherwise the bot cannot buy anything. - This strategy is one of the simplest
+and most basic approaches for trading cryptocurrencies. For this reason, it
+should be noted here that this does not necessarily lead to profits. Before
+running such an algorithm, everyone should be clear about what products are
+being traded, what these products are for in the first place, and what makes
+them valuable. Even the best companies, stocks, materials, and also
+cryptocurrencies can become worthless from one day to the next, so everyone
+should do their own research and make their decisions based on these results. -
+It has been decided here not to present any material regarding the
+profitability of this algorithm, as this could lead you to make your decisions
+based on my successes and failures. What works once or over a long period of
+time does not necessarily work in the future. But please let me know what you
+think about this basic algorithm and what could be improved. - For any problems
+or suggestions - please open an issue. --- ## ð Contributions â¦ are
+welcome! ## ð­ References - https://python-kraken-sdk.readthedocs.io/en/
+stable
```

### Comparing `kraken-rebalance-bot-0.5.7.3/krakenRebalanceBot/bot.py` & `kraken-rebalance-bot-1.0.0/rebalance/bot.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,315 +1,385 @@
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# Copyright (C) 2023 Benjamin Thomas Schwertfeger
+# GitHub: https://github.com/btschwertfeger
+# pylint: disable=too-many-branches,too-many-statements
+
+"""Module that implements the rebalance strategy"""
+
+import logging
 import sys
 import time
-import logging
-import schedule
-import numpy as np
+
 import requests
-from kraken.spot.client import User, Market, Trade
+import schedule
+from kraken.spot import Market, Trade, User
 
 
-class RebalanceBot():
-    '''
-        Class that implements the Rebalance Strategy
-
-        ===== PARAMETERS =====
-
-        key: str
-            Kraken API Public Key
-        secret: str
-            Kraken API Secret Key
-        config: dict
-            Configurations
-
-        ===== EXAMPLE =====
-
-        bot = RebalanceBot(
-            key='public-key',
-            secret='secret-key',
-            config={
-                'base_currency': ['ETH'],
-                'quote_currency': ['USD'],
-                'target_quantity': [1000],
-                'quote_to_maintain': [500],
-                'margin': [0.05],
-                'demo': false, 
-                "telegram": { # optional
-                    "token": "your telegram token",
-                    "chat_id": "your telegram chat id"
-                },
-                'use_build_in_sheduler': false, # optional    
-            }
-        )
-        bot.run()
-    '''
+class RebalanceBot:
+    """
+    Class that implements the Rebalance Strategy
+
+    ===== PARAMETERS =====
+
+    key: str
+        Kraken API Public Key
+    secret: str
+        Kraken API Secret Key
+    config: dict
+        Configurations
+
+    ===== EXAMPLE =====
+
+    bot = RebalanceBot(
+        key='public-key',
+        secret='secret-key',
+        config={
+            'base_currency': ['ETH'],
+            'quote_currency': ['USD'],
+            'target_quantity': [1000],
+            'quote_to_maintain': [500],
+            'margin': [0.05],
+            'demo': false,
+            "telegram": { # optional
+                "token": "your telegram token",
+                "chat_id": "your telegram chat id"
+            },
+            'use_build_in_scheduler': false, # optional
+        }
+    )
+    bot.run()
+    """
 
-    TIMES = ['00:00', '06:00', '12:00', '18:00']
+    TIMES: list[str] = ["00:00", "06:00", "12:00", "18:00"]
 
     def __init__(self, key: str, secret: str, config: dict):
-        self.__market = Market()
-        self.__trade = Trade(key=key, secret=secret)
-        self.__user = User(key=key, secret=secret)
-        
-        self.__use_telegram = False
-        self.__demo = True
-        self.__config = config
+        self.__market: Market = Market()
+        self.__trade: Trade = Trade(key=key, secret=secret)
+        self.__user: User = User(key=key, secret=secret)
+
+        self.__use_telegram: bool = False
+        self.__demo: bool = True
+        self.__config: dict = config
         self.__check_config()
-        
-    def run(self) -> None:
-        '''Runs the bot'''
-        logging.info('Starting the `kraken-rebalance-bot`')
-        
-        if self.__config.get('use_build_in_sheduler', False):
+
+    def run(self: "RebalanceBot") -> None:
+        """Runs the bot"""
+        logging.info("Starting the kraken-rebalance-bot")
+
+        if self.__config.get("use_build_in_scheduler", False):
             logging.info(f'Using scheduled times @{self.__config["times"]}')
-            for schedule_time in self.__config['times']:
+            for schedule_time in self.__config["times"]:
                 schedule.every().day.at(schedule_time).do(self.__check_balances)
 
             while True:
                 schedule.run_pending()
                 time.sleep(60)
 
-        else: 
+        else:
             self.__check_balances()
             sys.exit(0)
 
-    def __check_balances(self) -> None:
-        '''Checks if buy or sell order must be placed'''
-        logging.info('Checking balances ...')
-
-        for i, base_currency in enumerate(self.__config['base_currency']):
-            quote_to_maintain = self.__config['quote_to_maintain'][i]
-            target_quantity = self.__config['target_quantity'][i]
-            quote_currency = self.__config['quote_currency'][i]
-            margin = self.__config['margin'][i]
-
-            available_balance_base = float(self.__user.get_balances(currency=base_currency)['available_balance'])
-            available_balance_quote = float(self.__user.get_balances(currency=quote_currency)['available_balance'])
-
-            ticker = self.__market.get_ticker(pair=f'{base_currency}{quote_currency}')
-            symbol = list(ticker.keys())[0]
-            price = float(ticker[symbol]['c'][0])
-            value = available_balance_base * price
-
-            msg = f'\n👑 {symbol} Rebalance Bot'
-            msg += f'\n├ Price: {price} '
-            msg += f'\n├ Available {base_currency} » {available_balance_base} ({value} {quote_currency} / {target_quantity} {quote_currency})'
-            msg += f'\n└ Available {quote_currency} » {available_balance_quote}'
-            logging.info(f'\n{msg}')
+    def __check_balances(self: "RebalanceBot") -> None:
+        """Checks if buy or sell order must be placed"""
+        logging.info("Checking balances ...")
+
+        for i, base_currency in enumerate(self.__config["base_currency"]):
+            quote_to_maintain = self.__config["quote_to_maintain"][i]
+            target_quantity = self.__config["target_quantity"][i]
+            quote_currency = self.__config["quote_currency"][i]
+            margin = self.__config["margin"][i]
 
-            rebalanced = False
+            available_balance_base: float = float(
+                self.__user.get_balance(currency=base_currency)["available_balance"]
+            )
+            available_balance_quote: float = float(
+                self.__user.get_balance(currency=quote_currency)["available_balance"]
+            )
+
+            ticker: dict = self.__market.get_ticker(
+                pair=f"{base_currency}{quote_currency}"
+            )
+            symbol: str = list(ticker.keys())[0]
+            price: float = float(ticker[symbol]["c"][0])
+            value_of_base: float = available_balance_base * price
+
+            msg: str = f"\n👑 {symbol} Rebalance Bot"
+            msg += f"\n├ Price: {price} "
+            msg += f"\n├ Available {base_currency} » {available_balance_base} ({value_of_base} {quote_currency} / {target_quantity} {quote_currency})"
+            msg += f"\n└ Available {quote_currency} » {available_balance_quote}"
+            logging.info(f"\n{msg}")
+
+            rebalanced: bool = False
             # check range is left
-            if value <= target_quantity - target_quantity * margin: 
+            if value_of_base <= target_quantity - target_quantity * margin:
                 # check if buy would not break quantity to maintain
-                if available_balance_quote > quote_to_maintain + target_quantity - value: 
+                if (
+                    available_balance_quote
+                    > quote_to_maintain + target_quantity - value_of_base
+                ):
                     # check if price is higher than the defined max buy price to avoid catching the falling knife
-                    if price >= self.__config['lowest_buy_price'][i]:
+                    if price >= self.__config["lowest_buy_price"][i]:
                         self.__rebalance(
                             symbol=symbol,
-                            side='buy',
+                            side="buy",
                             index=i,
                             available={
-                                'base': available_balance_base, 
-                                'quote': available_balance_quote
+                                "base": available_balance_base,
+                                "quote": available_balance_quote,
                             },
-                            last_price=float(ticker[symbol]['c'][0])
+                            last_price=float(ticker[symbol]["c"][0]),
                         )
                         rebalanced = True
                     else:
                         msg = f'{symbol}: not buying because price ({price} {quote_currency}) is lower than the specified lowest buy price ({self.__config["lowest_buy_price"][i]} {quote_currency}).'
                         logging.info(msg)
 
                 else:
-                    msg = f'{symbol}: Not enough {quote_currency} to buy more {base_currency}. Noting changed.'
+                    msg = f"{symbol}: Not enough {quote_currency} to buy more {base_currency}. Noting changed."
                     logging.info(msg)
-            
+
             # check if new sell
-            elif value >= target_quantity + target_quantity * margin:
+            elif value_of_base >= target_quantity + target_quantity * margin:
                 self.__rebalance(
                     symbol=symbol,
-                    side='sell',
+                    side="sell",
                     index=i,
-                    available={ 
-                        'base': available_balance_base, 
-                        'quote': available_balance_quote
+                    available={
+                        "base": available_balance_base,
+                        "quote": available_balance_quote,
                     },
-                    last_price=float(ticker[symbol]['c'[0]])
+                    last_price=float(ticker[symbol]["c"[0]]),
                 )
                 rebalanced = True
             if rebalanced:
                 # wait to ensure that Krakens backend swallowed all requests
                 # to ensure the fetched balances match the actual balances
                 time.sleep(3)
-                available_balance_base = float(self.__user.get_balances(currency=base_currency)['available_balance'])
-                value = available_balance_base * float(self.__market.get_ticker(pair=symbol)[symbol]['c'][0])
-                
-                msg = f'👑 {symbol} Rebalance Bot updated values'
-                msg += f'\n├ Available {base_currency} » {available_balance_base} ({value} {quote_currency} / {target_quantity} {quote_currency})'
-                msg += f'\n└ Available {quote_currency} » {self.__user.get_balances(currency=quote_currency)["available_balance"]}'
-                logging.info(f'\n{msg}')
+                available_balance_base = self.__user.get_balance(
+                    currency=base_currency
+                )["available_balance"]
+
+                value_of_base = available_balance_base * float(
+                    self.__market.get_ticker(pair=symbol)[symbol]["c"][0]
+                )
+
+                msg = f"👑 {symbol} Rebalance Bot updated values"
+                msg += f"\n├ Available {base_currency} » {available_balance_base} ({value_of_base} {quote_currency} / {target_quantity} {quote_currency})"
+                msg += f'\n└ Available {quote_currency} » {self.__user.get_balance(currency=quote_currency)["available_balance"]}'
+                logging.info(f"\n{msg}")
             else:
-                msg += f'\n... nothing changed.'
-            
+                msg += "\n... nothing changed."
+
             self.send_to_telegram(message=msg)
             time.sleep(1)
 
-    def __rebalance(self, symbol: str, side: str, index: int, available: dict, last_price: float) -> None:
-        '''Places buy and sell orders'''
-        msg = f'Rebalancing {symbol} ...'
-        self.__new_message += f'\n\n{msg}'
-        
-        quote_volume = self.__config['target_quantity'][index] - (available['base'] * last_price)
-
-        # get information about the symbol to calculate the buying or selling size
-        symbol_data = self.__market.get_tradable_asset_pair(pair=symbol)[symbol]
-        ordermin = float(symbol_data['ordermin'])
-
-        base_factor = int(f'1{symbol_data["lot_decimals"]*str(0)}')
-        if base_factor == 0: baseIncrementSize = int(symbol_data['lot_multiplier'])
-        else: baseIncrementSize = float(int(symbol_data['lot_multiplier']) / base_factor)
-
-        baseRoundVal = self.__get_decimal_round_value(baseIncrementSize)
-        order_size =  self.__floor(abs(quote_volume) / float(last_price), baseRoundVal)
- 
-        if ordermin > order_size: 
-            msg = '❌ Ordermin > order size. Please check if your symbols or asset pairs \
-                minimum trade sizes match up with your target holdings, margins, and available quote balances. \
-                \n- also see: https://support.kraken.com/hc/en-us/articles/360050845612-Minimum-order-size-volume-for-trading-and-decimal-precision-for-residents-of-Japan-\
-                \n- and https://github.com/btschwertfeger/Kraken-Rebalance-Bot'
-            self.send_to_telegram(message=msg)
-            raise ValueError(msg)
+    def __rebalance(
+        self: "RebalanceBot",
+        symbol: str,
+        side: str,
+        index: int,
+        available: dict,
+        last_price: float,
+    ) -> None:
+        """Places buy and sell orders"""
+        msg: str = f"Rebalancing {symbol} ..."
+        logging.info(msg)
+
+        quote_volume: float = float(self.__config["target_quantity"][index]) - (
+            available["base"] * last_price
+        )
 
-        msg = f'✅ {side[0].upper()}{side[1:]} {order_size} {self.__config["base_currency"][index]} around {last_price} '
+        base_volume: str = self.__trade.truncate(
+            amount=abs(quote_volume) / float(last_price),
+            amount_type="volume",
+            pair=symbol,
+        )
+
+        msg = f'✅ {side[0].upper()}{side[1:]} {base_volume} {self.__config["base_currency"][index]} around {last_price} '
         msg += f'{self.__config["quote_currency"][index]} (volume: {quote_volume} {self.__config["quote_currency"][index]})'
         logging.info(msg)
         self.send_to_telegram(message=msg)
 
-        if self.__demo: return 
+        if self.__demo:
+            return
 
-        if side == 'buy': 
+        if side == "buy":
             response = self.__trade.create_order(
-                ordertype='market',
-                side='buy',
-                pair=symbol,
-                volume=order_size
+                ordertype="market", side="buy", pair=symbol, volume=base_volume
             )
-            logging.debug(f'Placed order response: {response}')
+            logging.debug(f"Placed order response: {response}")
 
-        if side == 'sell':
+        if side == "sell":
             response = self.__trade.create_order(
-                ordertype='market',
-                side='sell',
-                pair=symbol,
-                volume=order_size
+                ordertype="market", side="sell", pair=symbol, volume=base_volume
             )
-            logging.debug(f'Placed order response: {response}')
+            logging.debug(f"Placed order response: {response}")
+
+    def __check_config(self: "RebalanceBot") -> None:
+        """Checks the config for missing or wrong values"""
 
-    def __floor(self, value: float, precision: int=0) -> float:
-        ''' floor to precision '''
-        return np.true_divide(np.floor(value * 10.0 ** precision), 10.0 ** precision)
-
-    def __get_decimal_round_value(self, x: float) -> float:
-        ''' returns the number on how often to multiply x by 10 to get x >= 1
-        '''
-        roundVal = 0
-        while x < 1:
-            x *= 10
-            roundVal += 1
-        return roundVal
-
-    def __check_config(self) -> None:
-        '''Checks the config for missing or wrong values'''
-        # ___base_currency____
-        if 'base_currency' in self.__config:
-            if not isinstance(self.__config['base_currency'], list):
-                raise ValueError('base_currency must be type List[str] in config.')
-            if len(self.__config['base_currency']) == 0:
-                raise ValueError('No pair(s) specified in config.')
-            if len([pair for pair in self.__config['base_currency'] if not isinstance(pair, str)]) != 0:
-                raise ValueError('Each pair in config must be type str.')
+        if "base_currency" in self.__config:
+            if not isinstance(self.__config["base_currency"], list):
+                raise TypeError("base_currency must be type List[str] in config.")
+            if len(self.__config["base_currency"]) == 0:
+                raise TypeError("No pair(s) specified in config.")
+            if (
+                len(
+                    [
+                        pair
+                        for pair in self.__config["base_currency"]
+                        if not isinstance(pair, str)
+                    ]
+                )
+                != 0
+            ):
+                raise TypeError("Each pair in config must be type str.")
         else:
-            raise ValueError('Missing base_currency in config file.')
+            raise TypeError("Missing base_currency in config file.")
 
-        if 'quote_currency' in self.__config:
-            if not isinstance(self.__config['quote_currency'], list):
-                raise ValueError('quote_currency must be type List[str] in config.')
-            if len(self.__config['quote_currency']) == 0:
-                raise ValueError('No pair(s) specified in config.')
-            if len([pair for pair in self.__config['quote_currency'] if not isinstance(pair, str)]) != 0:
-                raise ValueError('Each pair in config must be type str.')
+        if "quote_currency" in self.__config:
+            if not isinstance(self.__config["quote_currency"], list):
+                raise TypeError("quote_currency must be type List[str] in config.")
+            if len(self.__config["quote_currency"]) == 0:
+                raise ValueError("No pair(s) specified in config.")
+            if (
+                len(
+                    [
+                        pair
+                        for pair in self.__config["quote_currency"]
+                        if not isinstance(pair, str)
+                    ]
+                )
+                != 0
+            ):
+                raise TypeError("Each pair in config must be type str.")
         else:
-            raise ValueError('Missing quote_currency in config file.')
+            raise TypeError("Missing quote_currency in config file.")
 
         # ___quantity____
-        if 'target_quantity' in self.__config:
-            if not isinstance(self.__config['target_quantity'], list): 
-                raise ValueError('No quantity in config must be type List[float].')
-            if len(self.__config['target_quantity']) == 0:
-                raise ValueError('No quantity defined in config.')
-            if len([q for q in self.__config['target_quantity'] if not isinstance(q, int) and not isinstance(q, float)]) != 0:
-                raise ValueError('target_quantity must be type int or float in config.')
+        if "target_quantity" in self.__config:
+            if not isinstance(self.__config["target_quantity"], list):
+                raise TypeError("No quantity in config must be type list[float].")
+            if len(self.__config["target_quantity"]) == 0:
+                raise TypeError("No quantity defined in config.")
+            if (
+                len(
+                    [
+                        q
+                        for q in self.__config["target_quantity"]
+                        if not isinstance(q, int) and not isinstance(q, float)
+                    ]
+                )
+                != 0
+            ):
+                raise TypeError("target_quantity must be type int or float in config.")
         else:
-            raise ValueError('No target_quantity defined in config.')
+            raise TypeError("No target_quantity defined in config.")
 
         # ___QUOTE_TO_MAINTAIN____
-        if 'quote_to_maintain' in self.__config:
-            if not isinstance(self.__config['quote_to_maintain'], list):
-                raise ValueError('No quote_to_maintain in config must be type List[float].')
-            if len(self.__config['quote_to_maintain']) == 0:
-                raise ValueError('No quote_to_maintain specified.')
-            if len([q for q in self.__config['quote_to_maintain'] if not isinstance(q, float) and not isinstance(q, int)]) != 0:
-                raise ValueError('quote_to_maintain must be type int or float in config.')
+        if "quote_to_maintain" in self.__config:
+            if not isinstance(self.__config["quote_to_maintain"], list):
+                raise TypeError(
+                    "No quote_to_maintain in config must be type List[float]."
+                )
+            if len(self.__config["quote_to_maintain"]) == 0:
+                raise TypeError("No quote_to_maintain specified.")
+            if (
+                len(
+                    [
+                        q
+                        for q in self.__config["quote_to_maintain"]
+                        if not isinstance(q, float) and not isinstance(q, int)
+                    ]
+                )
+                != 0
+            ):
+                raise TypeError(
+                    "quote_to_maintain must be type int or float in config."
+                )
         else:
-            raise ValueError('No quote_to_maintain defined in config.')
-        
+            raise ValueError("No quote_to_maintain defined in config.")
+
         # ___MARGIN___
-        if 'margin' in self.__config:
-            if not isinstance(self.__config['margin'], list):
-                raise ValueError('margin should be type List[str].')
-            if len([m for m in self.__config['margin'] if not isinstance(m, float) or m >= .99]) != 0:
-                raise ValueError('Margin should be less than 0.99, e.g. 0.04 for a 4% rebalance.')
-        else: 
-            ValueError('No margin defined in config.')
-
-        if 'lowest_buy_price' in self.__config:
-            if not isinstance(self.__config['lowest_buy_price'], list):
-                raise ValueError('lowest_buy_price should be type List[float].')
+        if "margin" in self.__config:
+            if not isinstance(self.__config["margin"], list):
+                raise TypeError("margin should be type list[str].")
+            if (
+                len(
+                    [
+                        m
+                        for m in self.__config["margin"]
+                        if not isinstance(m, float) or m >= 0.99
+                    ]
+                )
+                != 0
+            ):
+                raise TypeError(
+                    "Margin should be less than 0.99, e.g. 0.04 for a 4% rebalance."
+                )
+        else:
+            raise TypeError("No margin defined in config.")
+
+        if "lowest_buy_price" in self.__config:
+            if not isinstance(self.__config["lowest_buy_price"], list):
+                raise TypeError("lowest_buy_price should be type List[float].")
         else:
-            self.__config['lowest_buy_price'] = [0.0] * len(self.__config['target_quantity'])
+            self.__config["lowest_buy_price"] = [0.0] * len(
+                self.__config["target_quantity"]
+            )
 
         # ___MATCHING_PARAMETERS____
-        if len(self.__config['base_currency']) != len(self.__config['target_quantity'])                 \
-            or len(self.__config['base_currency']) != len(self.__config['quote_currency'])              \
-            or len(self.__config['base_currency']) != len(self.__config['margin'])                      \
-            or len(self.__config['base_currency']) != len(self.__config['quote_to_maintain'])           \
-            or len(self.__config['base_currency']) != len(self.__config['lowest_buy_price']):
-            raise ValueError('Lengths of: base_currency, quantity, margin, quote_to_maintain, and lowest_buy_price must be the same.')
-
-        if 'times' in self.__config:
-            if not isinstance(self.__config['times'], list) \
-                or len([t for t in self.__config['times'] if not isinstance(t, str)]) != 0:
-                raise ValueError('times must be type List[str] in config.')
+        if (
+            len(self.__config["base_currency"]) != len(self.__config["target_quantity"])
+            or len(self.__config["base_currency"])
+            != len(self.__config["quote_currency"])
+            or len(self.__config["base_currency"]) != len(self.__config["margin"])
+            or len(self.__config["base_currency"])
+            != len(self.__config["quote_to_maintain"])
+            or len(self.__config["base_currency"])
+            != len(self.__config["lowest_buy_price"])
+        ):
+            raise ValueError(
+                "Lengths of: base_currency, quantity, margin, quote_to_maintain, and lowest_buy_price must be the same."
+            )
+
+        if "times" in self.__config:
+            if (
+                not isinstance(self.__config["times"], list)
+                or len([t for t in self.__config["times"] if not isinstance(t, str)])
+                != 0
+            ):
+                raise TypeError("times must be type List[str] in config.")
         else:
-            logging.warning('No times specfied in config. Default ["00:00", "06:00", "12:00", "18:00"] will be used.')
-            self.__config['times'] = self.TIMES
+            logging.warning(
+                'No times specfied in config. Default ["00:00", "06:00", "12:00", "18:00"] will be used.'
+            )
+            self.__config["times"] = self.TIMES
 
-        if 'telegram' in self.__config:
-            if 'token' in self.__config['telegram'] and self.__config['telegram']['token'] \
-                and 'chat_id' in self.__config['telegram'] and self.__config['telegram']['chat_id']:
+        if "telegram" in self.__config:
+            if (
+                "token" in self.__config["telegram"]
+                and self.__config["telegram"]["token"]
+                and "chat_id" in self.__config["telegram"]
+                and self.__config["telegram"]["chat_id"]
+            ):
                 self.__use_telegram = True
 
-        if 'demo' in self.__config and isinstance(self.__config['demo'], bool):
-            self.__demo = self.__config['demo']
-            logging.info('Demo mode active, not trading.')
-
-    def send_to_telegram(self, message: str) -> None:
-        '''Send a Message to telegram'''
-        if not self.__use_telegram: return
+        if "demo" in self.__config and isinstance(self.__config["demo"], bool):
+            self.__demo = self.__config["demo"]
+            logging.info("Demo mode active, not trading.")
+
+    def send_to_telegram(self: "RebalanceBot", message: str) -> None:
+        """Send a Message to telegram"""
+        if not self.__use_telegram:
+            return
 
         requests.post(
             f'https://api.telegram.org/bot{self.__config["telegram"]["token"]}/sendMessage?chat_id={self.__config["telegram"]["chat_id"]}&text={message}',
-            timeout=10
+            timeout=10,
         )
 
-    def save_exit(self, reason: str='') -> None:
-        '''Exits the bot'''
+    def save_exit(self: "RebalanceBot", reason: str = "") -> None:
+        """Exits the bot"""
         logging.warning(reason)
         sys.exit(1)
```

