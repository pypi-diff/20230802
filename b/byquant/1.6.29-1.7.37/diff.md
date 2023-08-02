# Comparing `tmp/byquant-1.6.29.tar.gz` & `tmp/byquant-1.7.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byquant-1.6.29.tar", last modified: Fri Jun 30 01:22:15 2023, max compression
+gzip compressed data, was "byquant-1.7.37.tar", last modified: Wed Aug  2 05:23:47 2023, max compression
```

## Comparing `byquant-1.6.29.tar` & `byquant-1.7.37.tar`

### file list

```diff
@@ -1,138 +1,228 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 01:22:15.952640 byquant-1.6.29/
--rw-rw-rw-   0        0        0     1328 2023-06-30 01:22:15.951638 byquant-1.6.29/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.6.29/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 01:22:15.231770 byquant-1.6.29/byquant/
--rw-rw-rw-   0        0        0    21865 2023-06-30 01:20:38.000000 byquant-1.6.29/byquant/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:22:15.280367 byquant-1.6.29/byquant/crypto/
--rw-rw-rw-   0        0        0       63 2023-06-27 01:17:34.000000 byquant-1.6.29/byquant/crypto/__init__.py
--rw-rw-rw-   0        0        0    17167 2023-06-27 01:17:45.000000 byquant-1.6.29/byquant/crypto/broker.py
--rw-rw-rw-   0        0        0     8092 2023-06-27 01:17:57.000000 byquant-1.6.29/byquant/crypto/feed.py
--rw-rw-rw-   0        0        0     7942 2021-09-04 05:54:05.000000 byquant-1.6.29/byquant/crypto/store.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:22:15.940193 byquant-1.6.29/byquant/exchange/
--rw-rw-rw-   0        0        0        0 2023-05-16 08:03:11.000000 byquant-1.6.29/byquant/exchange/__init__.py
--rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.6.29/byquant/exchange/ace.py
--rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/alpaca.py
--rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/ascendex.py
--rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bequant.py
--rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bigone.py
--rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/binance.py
--rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/binancecoinm.py
--rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/binanceus.py
--rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/binanceusdm.py
--rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bit2c.py
--rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitbank.py
--rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitbay.py
--rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitbns.py
--rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitcoincom.py
--rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitfinex.py
--rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitfinex2.py
--rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitflyer.py
--rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitforex.py
--rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitget.py
--rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bithumb.py
--rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitmart.py
--rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitmex.py
--rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitopro.py
--rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitpanda.py
--rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitrue.py
--rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitso.py
--rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitstamp.py
--rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitstamp1.py
--rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bittrex.py
--rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bitvavo.py
--rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bkex.py
--rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bl3p.py
--rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/blockchaincom.py
--rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/btcalpha.py
--rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/btcbox.py
--rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/btcex.py
--rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/btcmarkets.py
--rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/btctradeua.py
--rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/btcturk.py
--rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/buda.py
--rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/bybit.py
--rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/cex.py
--rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/coinbase.py
--rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/coinbaseprime.py
--rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/coinbasepro.py
--rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/coincheck.py
--rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/coinex.py
--rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/coinfalcon.py
--rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/coinmate.py
--rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/coinone.py
--rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/coinsph.py
--rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/coinspot.py
--rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/cryptocom.py
--rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/currencycom.py
--rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/delta.py
--rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/deribit.py
--rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/digifinex.py
--rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/exmo.py
--rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/flowbtc.py
--rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/fmfwio.py
--rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/gate.py
--rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/gateio.py
--rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/gemini.py
--rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/hitbtc.py
--rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/hitbtc3.py
--rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/hollaex.py
--rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/huobi.py
--rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/huobijp.py
--rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/huobipro.py
--rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/idex.py
--rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/independentreserve.py
--rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/indodax.py
--rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/itbit.py
--rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/kraken.py
--rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/krakenfutures.py
--rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/kucoin.py
--rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/kucoinfutures.py
--rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/kuna.py
--rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/latoken.py
--rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/lbank.py
--rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/lbank2.py
--rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/luno.py
--rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/lykke.py
--rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/mercado.py
--rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/mexc.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/mexc3.py
--rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/ndax.py
--rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/novadax.py
--rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/oceanex.py
--rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/okcoin.py
--rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/okex.py
--rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/okex5.py
--rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.6.29/byquant/exchange/okx.py
--rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/paymium.py
--rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/phemex.py
--rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/poloniex.py
--rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/poloniexfutures.py
--rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/probit.py
--rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/ripio.py
--rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/stex.py
--rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/tidex.py
--rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/timex.py
--rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/tokocrypto.py
--rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/upbit.py
--rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/wavesexchange.py
--rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/wazirx.py
--rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/whitebit.py
--rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/woo.py
--rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/xt.py
--rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/yobit.py
--rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/zaif.py
--rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/zb.py
--rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.6.29/byquant/exchange/zonda.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:22:15.948170 byquant-1.6.29/byquant/tool/
--rw-rw-rw-   0        0        0        0 2023-06-27 01:25:40.000000 byquant-1.6.29/byquant/tool/__init__.py
--rw-rw-rw-   0        0        0     3427 2023-02-15 05:30:28.000000 byquant-1.6.29/byquant/tool/tawPlus.py
-drwxrwxrwx   0        0        0        0 2023-06-30 01:22:15.260420 byquant-1.6.29/byquant.egg-info/
--rw-rw-rw-   0        0        0     1328 2023-06-30 01:22:15.000000 byquant-1.6.29/byquant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3561 2023-06-30 01:22:15.000000 byquant-1.6.29/byquant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 01:22:15.000000 byquant-1.6.29/byquant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-06-30 01:22:15.000000 byquant-1.6.29/byquant.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 01:22:15.000000 byquant-1.6.29/byquant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.6.29/byquant.egg-info/zip-safe
--rw-rw-rw-   0        0        0      190 2023-06-30 01:21:46.000000 byquant-1.6.29/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 01:22:15.954635 byquant-1.6.29/setup.cfg
--rw-rw-rw-   0        0        0     2760 2023-06-30 01:21:25.000000 byquant-1.6.29/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:23:47.046999 byquant-1.7.37/
+-rw-rw-rw-   0        0        0     1451 2023-08-02 05:23:47.046002 byquant-1.7.37/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-16 07:39:16.000000 byquant-1.7.37/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 05:23:45.964098 byquant-1.7.37/byquant/
+-rw-rw-rw-   0        0        0     7817 2023-08-02 02:09:08.000000 byquant-1.7.37/byquant/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:23:46.001997 byquant-1.7.37/byquant/chart/
+-rw-rw-rw-   0        0        0      971 2023-08-01 10:34:29.000000 byquant-1.7.37/byquant/chart/__init__.py
+-rw-rw-rw-   0        0        0     1061 2023-08-01 10:34:31.000000 byquant-1.7.37/byquant/chart/matplotlib.py
+-rw-rw-rw-   0        0        0     1089 2023-08-01 10:34:29.000000 byquant-1.7.37/byquant/chart/seaborn.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:23:46.019950 byquant-1.7.37/byquant/crypto/
+-rw-rw-rw-   0        0        0       63 2023-06-27 01:17:34.000000 byquant-1.7.37/byquant/crypto/__init__.py
+-rw-rw-rw-   0        0        0    17167 2023-06-27 01:17:45.000000 byquant-1.7.37/byquant/crypto/broker.py
+-rw-rw-rw-   0        0        0     8092 2023-06-27 01:17:57.000000 byquant-1.7.37/byquant/crypto/feed.py
+-rw-rw-rw-   0        0        0     7942 2021-09-04 05:54:05.000000 byquant-1.7.37/byquant/crypto/store.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:23:46.029923 byquant-1.7.37/byquant/data/
+-rw-rw-rw-   0        0        0     1462 2023-08-02 04:37:02.000000 byquant-1.7.37/byquant/data/__init__.py
+-rw-rw-rw-   0        0        0    27227 2023-08-02 04:37:22.000000 byquant-1.7.37/byquant/data/get.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:23:46.666065 byquant-1.7.37/byquant/exchange/
+-rw-rw-rw-   0        0        0    14497 2023-07-28 11:41:17.000000 byquant-1.7.37/byquant/exchange/__init__.py
+-rw-rw-rw-   0        0        0    41329 2023-05-15 07:52:05.000000 byquant-1.7.37/byquant/exchange/ace.py
+-rw-rw-rw-   0        0        0    33161 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/alpaca.py
+-rw-rw-rw-   0        0        0   129270 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/ascendex.py
+-rw-rw-rw-   0        0        0     1136 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bequant.py
+-rw-rw-rw-   0        0        0    62340 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bigone.py
+-rw-rw-rw-   0        0        0   378516 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/binance.py
+-rw-rw-rw-   0        0        0     1645 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/binancecoinm.py
+-rw-rw-rw-   0        0        0     2151 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/binanceus.py
+-rw-rw-rw-   0        0        0     2480 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/binanceusdm.py
+-rw-rw-rw-   0        0        0    35482 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bit2c.py
+-rw-rw-rw-   0        0        0    39008 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitbank.py
+-rw-rw-rw-   0        0        0      448 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitbay.py
+-rw-rw-rw-   0        0        0    45973 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitbns.py
+-rw-rw-rw-   0        0        0      467 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitcoincom.py
+-rw-rw-rw-   0        0        0    69312 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitfinex.py
+-rw-rw-rw-   0        0        0   111509 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitfinex2.py
+-rw-rw-rw-   0        0        0    37741 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitflyer.py
+-rw-rw-rw-   0        0        0    28316 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitforex.py
+-rw-rw-rw-   0        0        0   204946 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitget.py
+-rw-rw-rw-   0        0        0    42572 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bithumb.py
+-rw-rw-rw-   0        0        0   131429 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitmart.py
+-rw-rw-rw-   0        0        0   119564 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitmex.py
+-rw-rw-rw-   0        0        0    63261 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitopro.py
+-rw-rw-rw-   0        0        0    87308 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitpanda.py
+-rw-rw-rw-   0        0        0    88097 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitrue.py
+-rw-rw-rw-   0        0        0    68449 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitso.py
+-rw-rw-rw-   0        0        0    82190 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitstamp.py
+-rw-rw-rw-   0        0        0    17785 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitstamp1.py
+-rw-rw-rw-   0        0        0    93397 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bittrex.py
+-rw-rw-rw-   0        0        0    76761 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bitvavo.py
+-rw-rw-rw-   0        0        0    74167 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bkex.py
+-rw-rw-rw-   0        0        0    16241 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bl3p.py
+-rw-rw-rw-   0        0        0    47120 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/blockchaincom.py
+-rw-rw-rw-   0        0        0    35160 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/btcalpha.py
+-rw-rw-rw-   0        0        0    22489 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/btcbox.py
+-rw-rw-rw-   0        0        0   110784 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/btcex.py
+-rw-rw-rw-   0        0        0    48547 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/btcmarkets.py
+-rw-rw-rw-   0        0        0    22177 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/btctradeua.py
+-rw-rw-rw-   0        0        0    35384 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/btcturk.py
+-rw-rw-rw-   0        0        0    45591 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/buda.py
+-rw-rw-rw-   0        0        0   393944 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/bybit.py
+-rw-rw-rw-   0        0        0    64922 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/cex.py
+-rw-rw-rw-   0        0        0   124582 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/coinbase.py
+-rw-rw-rw-   0        0        0     1219 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/coinbaseprime.py
+-rw-rw-rw-   0        0        0    73787 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/coinbasepro.py
+-rw-rw-rw-   0        0        0    34208 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/coincheck.py
+-rw-rw-rw-   0        0        0   191859 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/coinex.py
+-rw-rw-rw-   0        0        0    38956 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/coinfalcon.py
+-rw-rw-rw-   0        0        0    39461 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/coinmate.py
+-rw-rw-rw-   0        0        0    34455 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/coinone.py
+-rw-rw-rw-   0        0        0    81092 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/coinsph.py
+-rw-rw-rw-   0        0        0    18778 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/coinspot.py
+-rw-rw-rw-   0        0        0   108248 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/cryptocom.py
+-rw-rw-rw-   0        0        0    79611 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/currencycom.py
+-rw-rw-rw-   0        0        0    84060 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/delta.py
+-rw-rw-rw-   0        0        0   119018 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/deribit.py
+-rw-rw-rw-   0        0        0   152160 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/digifinex.py
+-rw-rw-rw-   0        0        0    88724 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/exmo.py
+-rw-rw-rw-   0        0        0     1169 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/flowbtc.py
+-rw-rw-rw-   0        0        0     1238 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/fmfwio.py
+-rw-rw-rw-   0        0        0   221725 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/gate.py
+-rw-rw-rw-   0        0        0      445 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/gateio.py
+-rw-rw-rw-   0        0        0    69001 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/gemini.py
+-rw-rw-rw-   0        0        0    62241 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/hitbtc.py
+-rw-rw-rw-   0        0        0   116511 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/hitbtc3.py
+-rw-rw-rw-   0        0        0    69194 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/hollaex.py
+-rw-rw-rw-   0        0        0   362643 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/huobi.py
+-rw-rw-rw-   0        0        0    86605 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/huobijp.py
+-rw-rw-rw-   0        0        0      572 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/huobipro.py
+-rw-rw-rw-   0        0        0    67332 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/idex.py
+-rw-rw-rw-   0        0        0    29810 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/independentreserve.py
+-rw-rw-rw-   0        0        0    42437 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/indodax.py
+-rw-rw-rw-   0        0        0    34960 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/itbit.py
+-rw-rw-rw-   0        0        0   101404 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/kraken.py
+-rw-rw-rw-   0        0        0    81722 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/krakenfutures.py
+-rw-rw-rw-   0        0        0   160363 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/kucoin.py
+-rw-rw-rw-   0        0        0   101171 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/kucoinfutures.py
+-rw-rw-rw-   0        0        0    37750 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/kuna.py
+-rw-rw-rw-   0        0        0    70007 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/latoken.py
+-rw-rw-rw-   0        0        0    33717 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/lbank.py
+-rw-rw-rw-   0        0        0    97857 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/lbank2.py
+-rw-rw-rw-   0        0        0    40473 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/luno.py
+-rw-rw-rw-   0        0        0    48461 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/lykke.py
+-rw-rw-rw-   0        0        0    34639 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/mercado.py
+-rw-rw-rw-   0        0        0   209226 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/mexc.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/mexc3.py
+-rw-rw-rw-   0        0        0   106106 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/ndax.py
+-rw-rw-rw-   0        0        0    61638 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/novadax.py
+-rw-rw-rw-   0        0        0    37055 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/oceanex.py
+-rw-rw-rw-   0        0        0   177794 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/okcoin.py
+-rw-rw-rw-   0        0        0      434 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/okex.py
+-rw-rw-rw-   0        0        0      441 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/okex5.py
+-rw-rw-rw-   0        0        0   264399 2023-06-15 05:48:33.000000 byquant-1.7.37/byquant/exchange/okx.py
+-rw-rw-rw-   0        0        0    22745 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/paymium.py
+-rw-rw-rw-   0        0        0   191805 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/phemex.py
+-rw-rw-rw-   0        0        0    88311 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/poloniex.py
+-rw-rw-rw-   0        0        0    75104 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/poloniexfutures.py
+-rw-rw-rw-   0        0        0    69774 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/probit.py
+-rw-rw-rw-   0        0        0    47325 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/ripio.py
+-rw-rw-rw-   0        0        0   117868 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/stex.py
+-rw-rw-rw-   0        0        0    42407 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/tidex.py
+-rw-rw-rw-   0        0        0    65452 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/timex.py
+-rw-rw-rw-   0        0        0   119250 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/tokocrypto.py
+-rw-rw-rw-   0        0        0    75531 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/upbit.py
+-rw-rw-rw-   0        0        0   103453 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/wavesexchange.py
+-rw-rw-rw-   0        0        0    35544 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/wazirx.py
+-rw-rw-rw-   0        0        0    92139 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/whitebit.py
+-rw-rw-rw-   0        0        0    94453 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/woo.py
+-rw-rw-rw-   0        0        0   196488 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/xt.py
+-rw-rw-rw-   0        0        0    51368 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/yobit.py
+-rw-rw-rw-   0        0        0    28777 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/zaif.py
+-rw-rw-rw-   0        0        0   183857 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/zb.py
+-rw-rw-rw-   0        0        0    74036 2023-05-14 16:20:52.000000 byquant-1.7.37/byquant/exchange/zonda.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:23:46.967582 byquant-1.7.37/byquant/indicator/
+-rw-rw-rw-   0        0        0     1120 2023-08-01 10:34:25.000000 byquant-1.7.37/byquant/indicator/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:19.000000 byquant-1.7.37/byquant/indicator/ad.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:19.000000 byquant-1.7.37/byquant/indicator/adosc.py
+-rw-rw-rw-   0        0        0     1099 2023-08-01 10:33:20.000000 byquant-1.7.37/byquant/indicator/adx.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:21.000000 byquant-1.7.37/byquant/indicator/adxr.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:22.000000 byquant-1.7.37/byquant/indicator/apo.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:23.000000 byquant-1.7.37/byquant/indicator/aroon.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:25.000000 byquant-1.7.37/byquant/indicator/aroonosc.py
+-rw-rw-rw-   0        0        0     1097 2023-08-01 10:33:25.000000 byquant-1.7.37/byquant/indicator/atr.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:27.000000 byquant-1.7.37/byquant/indicator/avgprice.py
+-rw-rw-rw-   0        0        0     1444 2023-08-01 10:33:29.000000 byquant-1.7.37/byquant/indicator/bbands.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:30.000000 byquant-1.7.37/byquant/indicator/beta.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:31.000000 byquant-1.7.37/byquant/indicator/bop.py
+-rw-rw-rw-   0        0        0     1099 2023-08-01 10:33:32.000000 byquant-1.7.37/byquant/indicator/cci.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:32.000000 byquant-1.7.37/byquant/indicator/cmo.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:34.000000 byquant-1.7.37/byquant/indicator/correl.py
+-rw-rw-rw-   0        0        0     1126 2023-08-01 10:33:34.000000 byquant-1.7.37/byquant/indicator/dema.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:35.000000 byquant-1.7.37/byquant/indicator/dx.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:37.000000 byquant-1.7.37/byquant/indicator/ema.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:38.000000 byquant-1.7.37/byquant/indicator/ht_dcperiod.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:39.000000 byquant-1.7.37/byquant/indicator/ht_dcphase.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:40.000000 byquant-1.7.37/byquant/indicator/ht_phasor.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:42.000000 byquant-1.7.37/byquant/indicator/ht_sine.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:43.000000 byquant-1.7.37/byquant/indicator/ht_trendmode.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:44.000000 byquant-1.7.37/byquant/indicator/kama.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:44.000000 byquant-1.7.37/byquant/indicator/linearreg.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:46.000000 byquant-1.7.37/byquant/indicator/linearreg_angle.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:47.000000 byquant-1.7.37/byquant/indicator/linearreg_intercept.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:48.000000 byquant-1.7.37/byquant/indicator/linearreg_slope.py
+-rw-rw-rw-   0        0        0     1074 2023-08-01 10:33:48.000000 byquant-1.7.37/byquant/indicator/ma.py
+-rw-rw-rw-   0        0        0     1161 2023-08-01 10:33:51.000000 byquant-1.7.37/byquant/indicator/macd.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:51.000000 byquant-1.7.37/byquant/indicator/macdext.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:52.000000 byquant-1.7.37/byquant/indicator/medprice.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:52.000000 byquant-1.7.37/byquant/indicator/mfi.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:54.000000 byquant-1.7.37/byquant/indicator/midprice.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:54.000000 byquant-1.7.37/byquant/indicator/minus_di.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:56.000000 byquant-1.7.37/byquant/indicator/minus_dm.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:56.000000 byquant-1.7.37/byquant/indicator/mom.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:57.000000 byquant-1.7.37/byquant/indicator/natr.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:58.000000 byquant-1.7.37/byquant/indicator/obv.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:33:59.000000 byquant-1.7.37/byquant/indicator/plus_di.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:00.000000 byquant-1.7.37/byquant/indicator/plus_dm.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:02.000000 byquant-1.7.37/byquant/indicator/pro.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:03.000000 byquant-1.7.37/byquant/indicator/roc.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:04.000000 byquant-1.7.37/byquant/indicator/rocp.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:05.000000 byquant-1.7.37/byquant/indicator/rocr.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:06.000000 byquant-1.7.37/byquant/indicator/rocr100.py
+-rw-rw-rw-   0        0        0     1105 2023-08-01 10:34:08.000000 byquant-1.7.37/byquant/indicator/rsi.py
+-rw-rw-rw-   0        0        0     1298 2023-08-01 10:34:09.000000 byquant-1.7.37/byquant/indicator/sar.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:10.000000 byquant-1.7.37/byquant/indicator/sarext.py
+-rw-rw-rw-   0        0        0     1205 2023-08-01 10:34:11.000000 byquant-1.7.37/byquant/indicator/sma.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:12.000000 byquant-1.7.37/byquant/indicator/stddev.py
+-rw-rw-rw-   0        0        0     1870 2023-08-01 10:34:13.000000 byquant-1.7.37/byquant/indicator/stoch.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:14.000000 byquant-1.7.37/byquant/indicator/stochf.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:15.000000 byquant-1.7.37/byquant/indicator/stochrsi.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:16.000000 byquant-1.7.37/byquant/indicator/t3.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:17.000000 byquant-1.7.37/byquant/indicator/tema.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:18.000000 byquant-1.7.37/byquant/indicator/trange.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:19.000000 byquant-1.7.37/byquant/indicator/trix.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:19.000000 byquant-1.7.37/byquant/indicator/tsf.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:20.000000 byquant-1.7.37/byquant/indicator/typprice.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:21.000000 byquant-1.7.37/byquant/indicator/ultosc.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:22.000000 byquant-1.7.37/byquant/indicator/var.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:22.000000 byquant-1.7.37/byquant/indicator/wclprice.py
+-rw-rw-rw-   0        0        0     1102 2023-08-01 10:34:23.000000 byquant-1.7.37/byquant/indicator/willr.py
+-rw-rw-rw-   0        0        0     1081 2023-08-01 10:34:24.000000 byquant-1.7.37/byquant/indicator/wma.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:23:47.028050 byquant-1.7.37/byquant/indicators/
+-rw-rw-rw-   0        0        0     1132 2023-08-01 10:33:11.000000 byquant-1.7.37/byquant/indicators/__init__.py
+-rw-rw-rw-   0        0        0     1134 2023-08-01 10:33:02.000000 byquant-1.7.37/byquant/indicators/adx.py
+-rw-rw-rw-   0        0        0     1253 2023-08-01 10:33:03.000000 byquant-1.7.37/byquant/indicators/atr.py
+-rw-rw-rw-   0        0        0     1144 2023-08-01 10:33:04.000000 byquant-1.7.37/byquant/indicators/bollinger.py
+-rw-rw-rw-   0        0        0     1253 2023-08-01 10:33:05.000000 byquant-1.7.37/byquant/indicators/cci.py
+-rw-rw-rw-   0        0        0     1828 2023-08-01 10:33:06.000000 byquant-1.7.37/byquant/indicators/macd.py
+-rw-rw-rw-   0        0        0     1245 2023-08-01 10:33:07.000000 byquant-1.7.37/byquant/indicators/rsi.py
+-rw-rw-rw-   0        0        0     1503 2023-08-01 10:33:08.000000 byquant-1.7.37/byquant/indicators/sar.py
+-rw-rw-rw-   0        0        0     1408 2023-08-01 10:33:09.000000 byquant-1.7.37/byquant/indicators/sma.py
+-rw-rw-rw-   0        0        0     1144 2023-08-01 10:33:09.000000 byquant-1.7.37/byquant/indicators/stochastic.py
+-rw-rw-rw-   0        0        0     1143 2023-08-01 10:33:11.000000 byquant-1.7.37/byquant/indicators/williams.py
+-rw-rw-rw-   0        0        0     2369 2023-08-02 05:23:17.000000 byquant-1.7.37/byquant/metabacktest.py
+-rw-rw-rw-   0        0        0     1117 2023-07-30 04:29:44.000000 byquant-1.7.37/byquant/metastrategy.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:23:47.031042 byquant-1.7.37/byquant/strategy/
+-rw-rw-rw-   0        0        0      922 2023-07-30 04:49:12.000000 byquant-1.7.37/byquant/strategy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:23:47.041016 byquant-1.7.37/byquant/tool/
+-rw-rw-rw-   0        0        0        0 2023-06-27 01:25:40.000000 byquant-1.7.37/byquant/tool/__init__.py
+-rw-rw-rw-   0        0        0     3427 2023-02-15 05:30:28.000000 byquant-1.7.37/byquant/tool/tawPlus.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:23:45.990029 byquant-1.7.37/byquant.egg-info/
+-rw-rw-rw-   0        0        0     1451 2023-08-02 05:23:45.000000 byquant-1.7.37/byquant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5903 2023-08-02 05:23:45.000000 byquant-1.7.37/byquant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 05:23:45.000000 byquant-1.7.37/byquant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-08-02 05:23:45.000000 byquant-1.7.37/byquant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 05:23:45.000000 byquant-1.7.37/byquant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 09:08:59.000000 byquant-1.7.37/byquant.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      190 2023-08-02 05:22:58.000000 byquant-1.7.37/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 05:23:47.047997 byquant-1.7.37/setup.cfg
+-rw-rw-rw-   0        0        0     2880 2023-08-02 05:23:01.000000 byquant-1.7.37/setup.py
```

### Comparing `byquant-1.6.29/PKG-INFO` & `byquant-1.7.37/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.6.29
-Summary: ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community
+Version: 1.7.37
+Summary: ByQuant.com is AI Quantitative Strategy Competition Training Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
-License: MIT
+License: GPL
 Project-URL: Homepage, https://byquant.com
 Keywords: quant,strategy,algorithmic,algotrading
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Build Tools
@@ -18,14 +18,17 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: PHP
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Description-Content-Type: text/markdown
 
 ByQuant.com
```

### Comparing `byquant-1.6.29/byquant/crypto/broker.py` & `byquant-1.7.37/byquant/crypto/broker.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/crypto/feed.py` & `byquant-1.7.37/byquant/crypto/feed.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/crypto/store.py` & `byquant-1.7.37/byquant/crypto/store.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/ace.py` & `byquant-1.7.37/byquant/exchange/ace.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/alpaca.py` & `byquant-1.7.37/byquant/exchange/alpaca.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/ascendex.py` & `byquant-1.7.37/byquant/exchange/ascendex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bequant.py` & `byquant-1.7.37/byquant/exchange/bequant.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bigone.py` & `byquant-1.7.37/byquant/exchange/bigone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/binance.py` & `byquant-1.7.37/byquant/exchange/binance.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/binancecoinm.py` & `byquant-1.7.37/byquant/exchange/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/binanceus.py` & `byquant-1.7.37/byquant/exchange/binanceus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/binanceusdm.py` & `byquant-1.7.37/byquant/exchange/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bit2c.py` & `byquant-1.7.37/byquant/exchange/bit2c.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitbank.py` & `byquant-1.7.37/byquant/exchange/bitbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitbns.py` & `byquant-1.7.37/byquant/exchange/bitbns.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitfinex.py` & `byquant-1.7.37/byquant/exchange/bitfinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitfinex2.py` & `byquant-1.7.37/byquant/exchange/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitflyer.py` & `byquant-1.7.37/byquant/exchange/bitflyer.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitforex.py` & `byquant-1.7.37/byquant/exchange/bitforex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitget.py` & `byquant-1.7.37/byquant/exchange/bitget.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bithumb.py` & `byquant-1.7.37/byquant/exchange/bithumb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitmart.py` & `byquant-1.7.37/byquant/exchange/bitmart.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitmex.py` & `byquant-1.7.37/byquant/exchange/bitmex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitopro.py` & `byquant-1.7.37/byquant/exchange/bitopro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitpanda.py` & `byquant-1.7.37/byquant/exchange/bitpanda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitrue.py` & `byquant-1.7.37/byquant/exchange/bitrue.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitso.py` & `byquant-1.7.37/byquant/exchange/bitso.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitstamp.py` & `byquant-1.7.37/byquant/exchange/bitstamp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitstamp1.py` & `byquant-1.7.37/byquant/exchange/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bittrex.py` & `byquant-1.7.37/byquant/exchange/bittrex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bitvavo.py` & `byquant-1.7.37/byquant/exchange/bitvavo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bkex.py` & `byquant-1.7.37/byquant/exchange/bkex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bl3p.py` & `byquant-1.7.37/byquant/exchange/bl3p.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/blockchaincom.py` & `byquant-1.7.37/byquant/exchange/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/btcalpha.py` & `byquant-1.7.37/byquant/exchange/btcalpha.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/btcbox.py` & `byquant-1.7.37/byquant/exchange/btcbox.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/btcex.py` & `byquant-1.7.37/byquant/exchange/btcex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/btcmarkets.py` & `byquant-1.7.37/byquant/exchange/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/btctradeua.py` & `byquant-1.7.37/byquant/exchange/btctradeua.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/btcturk.py` & `byquant-1.7.37/byquant/exchange/btcturk.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/buda.py` & `byquant-1.7.37/byquant/exchange/buda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/bybit.py` & `byquant-1.7.37/byquant/exchange/bybit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/cex.py` & `byquant-1.7.37/byquant/exchange/cex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/coinbase.py` & `byquant-1.7.37/byquant/exchange/coinbase.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/coinbaseprime.py` & `byquant-1.7.37/byquant/exchange/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/coinbasepro.py` & `byquant-1.7.37/byquant/exchange/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/coincheck.py` & `byquant-1.7.37/byquant/exchange/coincheck.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/coinex.py` & `byquant-1.7.37/byquant/exchange/coinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/coinfalcon.py` & `byquant-1.7.37/byquant/exchange/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/coinmate.py` & `byquant-1.7.37/byquant/exchange/coinmate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/coinone.py` & `byquant-1.7.37/byquant/exchange/coinone.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/coinsph.py` & `byquant-1.7.37/byquant/exchange/coinsph.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/coinspot.py` & `byquant-1.7.37/byquant/exchange/coinspot.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/cryptocom.py` & `byquant-1.7.37/byquant/exchange/cryptocom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/currencycom.py` & `byquant-1.7.37/byquant/exchange/currencycom.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/delta.py` & `byquant-1.7.37/byquant/exchange/delta.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/deribit.py` & `byquant-1.7.37/byquant/exchange/deribit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/digifinex.py` & `byquant-1.7.37/byquant/exchange/digifinex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/exmo.py` & `byquant-1.7.37/byquant/exchange/exmo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/flowbtc.py` & `byquant-1.7.37/byquant/exchange/flowbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/fmfwio.py` & `byquant-1.7.37/byquant/exchange/fmfwio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/gate.py` & `byquant-1.7.37/byquant/exchange/gate.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/gemini.py` & `byquant-1.7.37/byquant/exchange/gemini.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/hitbtc.py` & `byquant-1.7.37/byquant/exchange/hitbtc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/hitbtc3.py` & `byquant-1.7.37/byquant/exchange/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/hollaex.py` & `byquant-1.7.37/byquant/exchange/hollaex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/huobi.py` & `byquant-1.7.37/byquant/exchange/huobi.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/huobijp.py` & `byquant-1.7.37/byquant/exchange/huobijp.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/huobipro.py` & `byquant-1.7.37/byquant/exchange/huobipro.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/idex.py` & `byquant-1.7.37/byquant/exchange/idex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/independentreserve.py` & `byquant-1.7.37/byquant/exchange/independentreserve.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/indodax.py` & `byquant-1.7.37/byquant/exchange/indodax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/itbit.py` & `byquant-1.7.37/byquant/exchange/itbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/kraken.py` & `byquant-1.7.37/byquant/exchange/kraken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/krakenfutures.py` & `byquant-1.7.37/byquant/exchange/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/kucoin.py` & `byquant-1.7.37/byquant/exchange/kucoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/kucoinfutures.py` & `byquant-1.7.37/byquant/exchange/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/kuna.py` & `byquant-1.7.37/byquant/exchange/kuna.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/latoken.py` & `byquant-1.7.37/byquant/exchange/latoken.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/lbank.py` & `byquant-1.7.37/byquant/exchange/lbank.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/lbank2.py` & `byquant-1.7.37/byquant/exchange/lbank2.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/luno.py` & `byquant-1.7.37/byquant/exchange/luno.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/lykke.py` & `byquant-1.7.37/byquant/exchange/lykke.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/mercado.py` & `byquant-1.7.37/byquant/exchange/mercado.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/mexc.py` & `byquant-1.7.37/byquant/exchange/mexc.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/ndax.py` & `byquant-1.7.37/byquant/exchange/ndax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/novadax.py` & `byquant-1.7.37/byquant/exchange/novadax.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/oceanex.py` & `byquant-1.7.37/byquant/exchange/oceanex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/okcoin.py` & `byquant-1.7.37/byquant/exchange/okcoin.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/okx.py` & `byquant-1.7.37/byquant/exchange/okx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/paymium.py` & `byquant-1.7.37/byquant/exchange/paymium.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/phemex.py` & `byquant-1.7.37/byquant/exchange/phemex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/poloniex.py` & `byquant-1.7.37/byquant/exchange/poloniex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/poloniexfutures.py` & `byquant-1.7.37/byquant/exchange/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/probit.py` & `byquant-1.7.37/byquant/exchange/probit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/ripio.py` & `byquant-1.7.37/byquant/exchange/ripio.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/stex.py` & `byquant-1.7.37/byquant/exchange/stex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/tidex.py` & `byquant-1.7.37/byquant/exchange/tidex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/timex.py` & `byquant-1.7.37/byquant/exchange/timex.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/tokocrypto.py` & `byquant-1.7.37/byquant/exchange/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/upbit.py` & `byquant-1.7.37/byquant/exchange/upbit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/wavesexchange.py` & `byquant-1.7.37/byquant/exchange/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/wazirx.py` & `byquant-1.7.37/byquant/exchange/wazirx.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/whitebit.py` & `byquant-1.7.37/byquant/exchange/whitebit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/woo.py` & `byquant-1.7.37/byquant/exchange/woo.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/xt.py` & `byquant-1.7.37/byquant/exchange/xt.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/yobit.py` & `byquant-1.7.37/byquant/exchange/yobit.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/zaif.py` & `byquant-1.7.37/byquant/exchange/zaif.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/zb.py` & `byquant-1.7.37/byquant/exchange/zb.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/exchange/zonda.py` & `byquant-1.7.37/byquant/exchange/zonda.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant/tool/tawPlus.py` & `byquant-1.7.37/byquant/tool/tawPlus.py`

 * *Files identical despite different names*

### Comparing `byquant-1.6.29/byquant.egg-info/PKG-INFO` & `byquant-1.7.37/byquant.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: byquant
-Version: 1.6.29
-Summary: ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community
+Version: 1.7.37
+Summary: ByQuant.com is AI Quantitative Strategy Competition Training Community
 Home-page: https://byquant.com
 Author: Uakeey
 Author-email: uakee@outlook.com
-License: MIT
+License: GPL
 Project-URL: Homepage, https://byquant.com
 Keywords: quant,strategy,algorithmic,algotrading
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Build Tools
@@ -18,14 +18,17 @@
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: PHP
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Description-Content-Type: text/markdown
 
 ByQuant.com
```

### Comparing `byquant-1.6.29/setup.py` & `byquant-1.7.37/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 
 here = path.abspath(path.dirname(__file__))
 root = path.dirname(here)
 
 readme = path.join(here, 'README.md')
 package = {
   "name": "byquant",
-  "version": "1.6.29",
-  "description": "ByQuant.com is a Artificial Intelligence Quantitative Investment Trading Competition Learning Community",
+  "version": "1.7.37",
+  "description": "ByQuant.com is AI Quantitative Strategy Competition Training Community",
   "type": "module",
   "readme": "README.md",
   "package_json": "package.json",
   "author": {
     "name": "Uakeey",
     "email": "uakee@outlook.com",
     "url": "https://github.com/byquantcom/"
   },
-  "license": "MIT",
+  "license": "GPL",
   "bugs": {
     "url": "https://github.com/byquantcom/byquant/issues"
   },
   "homepage": "https://byquant.com",
   "keywords": [
     "quant",
     "strategy",
@@ -75,14 +75,17 @@
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: JavaScript',
         'Programming Language :: PHP',
         'Operating System :: OS Independent',
         'Environment :: Console'
     ],
     keywords=package['keywords'],
     packages=find_packages(exclude=['byquant.async_support*'] if is_python_2 else []),
```

