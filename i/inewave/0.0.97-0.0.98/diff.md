# Comparing `tmp/inewave-0.0.97.tar.gz` & `tmp/inewave-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inewave-0.0.97.tar", last modified: Tue Jul 25 00:12:29 2023, max compression
+gzip compressed data, was "inewave-0.0.98.tar", last modified: Wed Aug  2 01:19:17 2023, max compression
```

## Comparing `inewave-0.0.97.tar` & `inewave-0.0.98.tar`

### file list

```diff
@@ -1,695 +1,702 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:29.032600 inewave-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 00:08:24.000000 inewave-0.0.97/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-25 00:12:29.032600 inewave-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-25 00:08:24.000000 inewave-0.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.860597 inewave-0.0.97/inewave/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.860597 inewave-0.0.97/inewave/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/_utils/leituracsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.868597 inewave-0.0.97/inewave/newave/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/abertura.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/bid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/cortes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    75043 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/elnino.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)    42179 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/forwarh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/gee.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/manutt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.880597 inewave-0.0.97/inewave/newave/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/abertura.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/arquivos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.880597 inewave-0.0.97/inewave/newave/modelos/arquivoscsv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/arquivoscsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/arquivoscsv/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/bid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.880597 inewave-0.0.97/inewave/newave/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/blocos/versaomodelo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/cortes.py
--rw-r--r--   0 runner    (1001) docker     (123)    30466 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)   135879 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/elnino.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)    87572 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/forwarh.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/gee.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/manutt.py
--rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/perda.py
--rw-r--r--   0 runner    (1001) docker     (123)    24454 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/selcor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)    20506 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/tecno.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/perda.py
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/selcor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/tecno.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/vazpast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.880597 inewave-0.0.97/inewave/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8174 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/estados.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.880597 inewave-0.0.97/inewave/nwlistcf/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/estados.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/nwlistcfrel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/nwlistcfrel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.892598 inewave-0.0.97/inewave/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/gtert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/merclsin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.904598 inewave-0.0.97/inewave/nwlistop/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.904598 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivousina.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.904598 inewave-0.0.97/inewave/nwlistop/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/parsubmercados.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/submercado.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/usina.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/valoresserie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/def.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dflppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dflpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/gtert.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.860597 inewave-0.0.97/inewave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-25 00:12:28.000000 inewave-0.0.97/inewave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21445 2023-07-25 00:12:28.000000 inewave-0.0.97/inewave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 00:12:28.000000 inewave-0.0.97/inewave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 00:12:28.000000 inewave-0.0.97/inewave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 00:12:28.000000 inewave-0.0.97/inewave.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 00:12:29.032600 inewave-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-25 00:08:24.000000 inewave-0.0.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.908598 inewave-0.0.97/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.908598 inewave-0.0.97/tests/_arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/_arquivos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.908598 inewave-0.0.97/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.996600 inewave-0.0.97/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/arquivos_nwlistcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)    46951 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/caso_nwlistcf_nwlistop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    30063 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)   847210 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)   295249 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)   295245 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105146 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)   295190 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)   295196 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   847164 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)   120243 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)   267099 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267152 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)   267153 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267144 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)   291239 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)   291240 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14002 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicaconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)    56476 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/estados.py
--rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)   267138 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104654 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)   120990 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104650 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105178 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105179 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105181 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   847144 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105136 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105139 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105141 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105140 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105189 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105190 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)    49768 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/gtert.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105188 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105191 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1087195 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)    49720 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/manutt.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    57012 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (123)    76521 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwlistcfrel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)   378349 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    50087 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)   267136 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   380918 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/selcor.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/term.py
--rw-r--r--   0 runner    (1001) docker     (123)   271157 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)   283139 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   283209 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)    32259 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)   847200 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267158 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267117 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105173 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105174 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105176 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   847195 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   847135 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:29.012600 inewave-0.0.97/tests/newave/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_cortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    49743 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_exph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_expt.py
--rw-r--r--   0 runner    (1001) docker     (123)    36320 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_forwarh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_manutt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_parp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_selcor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_shist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_vazpast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:29.012600 inewave-0.0.97/tests/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/test_arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/test_caso.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/test_estados.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/test_nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/test_nwlistcfrel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:29.032600 inewave-0.0.97/tests/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_coper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_evert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_exces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_geol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_gtert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_invade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vento.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vturuh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.484546 inewave-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 01:14:29.000000 inewave-0.0.98/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-02 01:19:17.484546 inewave-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-02 01:14:29.000000 inewave-0.0.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.348545 inewave-0.0.98/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-02 01:14:29.000000 inewave-0.0.98/examples/plot_dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-02 01:14:29.000000 inewave-0.0.98/examples/plot_modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-02 01:14:29.000000 inewave-0.0.98/examples/plot_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-08-02 01:14:29.000000 inewave-0.0.98/examples/plot_sistema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.352545 inewave-0.0.98/inewave/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.352545 inewave-0.0.98/inewave/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/_utils/formatacao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/_utils/leituracsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.360545 inewave-0.0.98/inewave/newave/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81481 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42179 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/gee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/manutt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.368545 inewave-0.0.98/inewave/newave/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/arquivos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.368545 inewave-0.0.98/inewave/newave/modelos/arquivoscsv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/arquivoscsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/arquivoscsv/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/bid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.368545 inewave-0.0.98/inewave/newave/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/blocos/versaomodelo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30466 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135879 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87572 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/gee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30603 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/perda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24463 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20585 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/perda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/vazpast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.368545 inewave-0.0.98/inewave/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/estados.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.372546 inewave-0.0.98/inewave/nwlistcf/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/nwlistcfrel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/nwlistcfrel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.380545 inewave-0.0.98/inewave/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/merclsin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/inewave/nwlistop/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivousina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/inewave/nwlistop/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/parsubmercados.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/submercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/usina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresserie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dflppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dflpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.352545 inewave-0.0.98/inewave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-02 01:19:17.000000 inewave-0.0.98/inewave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-08-02 01:19:17.000000 inewave-0.0.98/inewave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 01:19:17.000000 inewave-0.0.98/inewave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 01:19:17.000000 inewave-0.0.98/inewave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 01:19:17.000000 inewave-0.0.98/inewave.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 01:19:17.484546 inewave-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 01:14:29.000000 inewave-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/tests/_arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/_arquivos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.464546 inewave-0.0.98/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/arquivos_nwlistcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46951 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/caso_nwlistcf_nwlistop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30063 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847210 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295249 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295245 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105146 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295196 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847164 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120243 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267099 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267152 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267153 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267144 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   291239 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   291240 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14002 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicaconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56476 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267138 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104654 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120990 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104650 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105178 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105179 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105181 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847144 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105136 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105141 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105140 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105189 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49768 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105188 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105191 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1087195 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49720 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57012 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76521 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwlistcfrel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)   378349 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50087 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267136 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   380918 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)   271157 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283209 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32259 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847200 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267158 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267117 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105173 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105174 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105176 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847195 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847135 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.476546 inewave-0.0.98/tests/newave/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49743 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36320 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_manutt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_vazpast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.476546 inewave-0.0.98/tests/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/test_estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/test_nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/test_nwlistcfrel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.484546 inewave-0.0.98/tests/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vturuh.py
```

### Comparing `inewave-0.0.97/LICENSE.md` & `inewave-0.0.98/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/PKG-INFO` & `inewave-0.0.98/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 0.0.97
+Version: 0.0.98
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,28 +20,31 @@
 
 O `inewave` é um pacote Python para manipulação dos arquivos de entrada e saída do programa [NEWAVE](http://www.cepel.br/pt_br/produtos/newave-modelo-de-planejamento-da-operacao-de-sistemas-hidrotermicos-interligados-de-longo-e-medio-prazo.htm). O NEWAVE é desenvolvido pelo [CEPEL](http://www.cepel.br) e utilizado para os estudos de planejamento e operação do Sistema Interligado Nacional (SIN).
 
 O inewave oferece:
 
 - Meios para leitura dos arquivos de entrada e saída do NEWAVE e programas associados: NWLISTCF e NWLISTOP
 
-- Armazenamento e processamento de dados otimizados com o uso de NumPy e Pandas
+- Facilidades para estudo e análise dos dados utilizando DataFrames do pandas
 
 - Dados estruturados em modelos com o uso do paradigma de orientação a objetos (OOP)
 
-- Utilidades de escritas dos arquivos de entrada do NEWAVE para elaboração automatizada de estudos
-
-Com inewave é possível ler os arquivos de texto, característicos do NEWAVE, para poupar processamento futuro e reduzir o tempo de execução.
 
 ## Instalação
 
-O inewave é compatível com versões de Python >= 3.8 e é construído com base no framework [cfinterface](https://github.com/rjmalves/cfi), que deve sempre ser mantido na versão mais atualizada para a distribuição de Python instalada.
+O inewave é compatível com versões de Python >= 3.8.
 
-Em posse de uma instalação local de Python, é recomendado que se use um ambiente virtual para instalação de módulos de terceiros, sendo que o inewave não é uma exceção. Para mais detalhes sobre o uso de ambientes virtuais, recomenda-se a leitura do recurso oficial de Python para ambientes virtuais: [venv](https://docs.python.org/3/library/venv.html).
+É possível instalar a versão distribuída oficialmente com pip:
 
 ```
 python -m pip install inewave
 ```
 
+É possível realizar a instalação da versão de desenvolvimento fazendo o uso do Git.
+
+```
+pip install git+https://github.com/rjmalves/inewave
+```
+
 ## Documentação
 
 Guias, tutoriais e as referências podem ser encontrados no site oficial do pacote: https://rjmalves.github.io/inewave
```

### Comparing `inewave-0.0.97/README.md` & `inewave-0.0.98/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 
 O `inewave` é um pacote Python para manipulação dos arquivos de entrada e saída do programa [NEWAVE](http://www.cepel.br/pt_br/produtos/newave-modelo-de-planejamento-da-operacao-de-sistemas-hidrotermicos-interligados-de-longo-e-medio-prazo.htm). O NEWAVE é desenvolvido pelo [CEPEL](http://www.cepel.br) e utilizado para os estudos de planejamento e operação do Sistema Interligado Nacional (SIN).
 
 O inewave oferece:
 
 - Meios para leitura dos arquivos de entrada e saída do NEWAVE e programas associados: NWLISTCF e NWLISTOP
 
-- Armazenamento e processamento de dados otimizados com o uso de NumPy e Pandas
+- Facilidades para estudo e análise dos dados utilizando DataFrames do pandas
 
 - Dados estruturados em modelos com o uso do paradigma de orientação a objetos (OOP)
 
-- Utilidades de escritas dos arquivos de entrada do NEWAVE para elaboração automatizada de estudos
-
-Com inewave é possível ler os arquivos de texto, característicos do NEWAVE, para poupar processamento futuro e reduzir o tempo de execução.
 
 ## Instalação
 
-O inewave é compatível com versões de Python >= 3.8 e é construído com base no framework [cfinterface](https://github.com/rjmalves/cfi), que deve sempre ser mantido na versão mais atualizada para a distribuição de Python instalada.
+O inewave é compatível com versões de Python >= 3.8.
 
-Em posse de uma instalação local de Python, é recomendado que se use um ambiente virtual para instalação de módulos de terceiros, sendo que o inewave não é uma exceção. Para mais detalhes sobre o uso de ambientes virtuais, recomenda-se a leitura do recurso oficial de Python para ambientes virtuais: [venv](https://docs.python.org/3/library/venv.html).
+É possível instalar a versão distribuída oficialmente com pip:
 
 ```
 python -m pip install inewave
 ```
 
+É possível realizar a instalação da versão de desenvolvimento fazendo o uso do Git.
+
+```
+pip install git+https://github.com/rjmalves/inewave
+```
+
 ## Documentação
 
 Guias, tutoriais e as referências podem ser encontrados no site oficial do pacote: https://rjmalves.github.io/inewave
```

### Comparing `inewave-0.0.97/inewave/_utils/leituracsv.py` & `inewave-0.0.98/inewave/_utils/leituracsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/config.py` & `inewave-0.0.98/inewave/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,26 +30,26 @@
     "AGOSTO",
     "SETEMBRO",
     "OUTUBRO",
     "NOVEMBRO",
     "DEZEMBRO",
 ]
 MESES_DF = [
-    "Janeiro",
-    "Fevereiro",
-    "Março",
-    "Abril",
-    "Maio",
-    "Junho",
-    "Julho",
-    "Agosto",
-    "Setembro",
-    "Outubro",
-    "Novembro",
-    "Dezembro",
+    "janeiro",
+    "fevereiro",
+    "março",
+    "abril",
+    "maio",
+    "junho",
+    "julho",
+    "agosto",
+    "setembro",
+    "outubro",
+    "novembro",
+    "dezembro",
 ]
 MESES_ABREV = [
     "JAN",
     "FEV",
     "MAR",
     "ABR",
     "MAI",
```

### Comparing `inewave-0.0.97/inewave/newave/__init__.py` & `inewave-0.0.98/inewave/newave/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # Inclui os membros
 
 from .abertura import Abertura  # noqa
-from .adterm import AdTerm  # noqa
+from .adterm import Adterm  # noqa
 from .agrint import Agrint  # noqa
 from .arquivos import Arquivos  # noqa
 from .bid import BID  # noqa
-from .cadic import CAdic  # noqa
+from .cadic import Cadic  # noqa
 from .caso import Caso  # noqa
-from .clasgas import ClasGas  # noqa
-from .clast import ClasT  # noqa
+from .clasgas import Clasgas  # noqa
+from .clast import Clast  # noqa
 from .confhd import Confhd  # noqa
-from .conft import ConfT  # noqa
+from .conft import Conft  # noqa
 from .curva import Curva  # noqa
-from .cvar import CVAR  # noqa
-from .dger import DGer  # noqa
-from .dsvagua import DSVAgua  # noqa
-from .eafpast import EafPast  # noqa
+from .cvar import Cvar  # noqa
+from .dger import Dger  # noqa
+from .dsvagua import Dsvagua  # noqa
+from .eafpast import Eafpast  # noqa
 from .elnino import ElNino  # noqa
 from .ensoaux import ENSOAux  # noqa
 from .exph import Exph  # noqa
 from .expt import Expt  # noqa
 from .gee import GEE  # noqa
 from .ghmin import Ghmin  # noqa
-from .gtminpat import GTMinPat  # noqa
+from .gtminpat import Gtminpat  # noqa
 from .hidr import Hidr  # noqa
 from .itaipu import Itaipu  # noqa
 from .manutt import Manutt  # noqa
 from .modif import Modif  # noqa
-from .newavetim import NewaveTim  # noqa
-from .parp import PARp  # noqa
-from .parpvaz import PARpvaz  # noqa
-from .parpeol import PARpeol  # noqa
+from .newavetim import Newavetim  # noqa
+from .parp import Parp  # noqa
+from .parpvaz import Parpvaz  # noqa
+from .parpeol import Parpeol  # noqa
 from .patamar import Patamar  # noqa
 from .penalid import Penalid  # noqa
 from .perda import Perda  # noqa
-from .pmo import PMO  # noqa
-from .re import RE  # noqa
-from .ree import REE  # noqa
-from .sar import SAR  # noqa
+from .pmo import Pmo  # noqa
+from .re import Re  # noqa
+from .ree import Ree  # noqa
+from .sar import Sar  # noqa
 from .shist import Shist  # noqa
 from .selcor import Selcor  # noqa
 from .sistema import Sistema  # noqa
 from .tecno import Tecno  # noqa
 from .term import Term  # noqa
 from .vazoes import Vazoes  # noqa
-from .vazpast import VazPast  # noqa
+from .vazpast import Vazpast  # noqa
 from .eolicacadastro import EolicaCadastro  # noqa
 from .eolicaconfiguracao import EolicaConfiguracao  # noqa
 from .eolicafte import EolicaFTE  # noqa
 from .eolicageracao import EolicaGeracao  # noqa
 from .eolicahistorico import EolicaHistorico  # noqa
 from .eolicasubmercado import EolicaSubmercado  # noqa
```

### Comparing `inewave-0.0.97/inewave/newave/abertura.py` & `inewave-0.0.98/inewave/newave/abertura.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/adterm.py` & `inewave-0.0.98/inewave/newave/adterm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from inewave.newave.modelos.adterm import BlocoUTEAdTerm
 
 from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class AdTerm(SectionFile):
+class Adterm(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às térmicas de
     despacho antecipado disponíveis.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS = [BlocoUTEAdTerm]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="adterm.dat") -> "AdTerm":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="adterm.dat") -> "Adterm":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
@@ -37,50 +37,32 @@
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def despachos(self) -> Optional[pd.DataFrame]:
         """
         A tabela de espachos antecipados das térmicas GNL.
 
-        - Código UTE (`int`)
-        - Nome UTE (`str`)
-        - Lag (`int`)
-        - Patamar [1-p] (`float`), onde p é o número de patamares.
+        - codigo_usina (`int`)
+        - nome_usina (`str`)
+        - lag (`int`)
+        - patamar_1 (`float`)
+        - ...
+        - patamar_N (`float`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoUTEAdTerm, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoUTEAdTerm)
+        if isinstance(b, BlocoUTEAdTerm):
             return b.data
         return None
 
     @despachos.setter
     def despachos(self, d: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoUTEAdTerm, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoUTEAdTerm)
+        if isinstance(b, BlocoUTEAdTerm):
             b.data = d
```

### Comparing `inewave-0.0.97/inewave/newave/arquivos.py` & `inewave-0.0.98/inewave/newave/arquivos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from inewave.newave.modelos.arquivos import BlocoNomesArquivos
 
 from cfinterface.files.sectionfile import SectionFile
 
-from typing import List, TypeVar, Type, Optional
+from typing import List, TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
@@ -41,56 +41,36 @@
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     def __le_nome_por_indice(self, indice: int) -> Optional[str]:
-        b = self.__bloco_por_tipo(BlocoNomesArquivos, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoNomesArquivos)
+        if isinstance(b, BlocoNomesArquivos):
             if indice in b.data.index:
                 dado = b.data.iloc[indice, 1]
                 if isinstance(dado, str):
                     return dado
         return None
 
     def __atualiza_nome_por_indice(self, indice: int, nome: str):
-        b = self.__bloco_por_tipo(BlocoNomesArquivos, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoNomesArquivos)
+        if isinstance(b, BlocoNomesArquivos):
             dif = indice - b.data.shape[0] + 1
             if dif > 0:
                 col_vazia = [None] * dif
                 b.data = pd.concat(
                     [
                         b.data,
                         pd.DataFrame(
                             data={
-                                "Legenda": col_vazia,
-                                "Nome": col_vazia,
+                                "legenda": col_vazia,
+                                "nome": col_vazia,
                             }
                         ),
                     ],
                     ignore_index=True,
                 )
             b.data.iloc[indice, 1] = nome
 
@@ -98,16 +78,18 @@
     def arquivos(self) -> List[str]:
         """
         Os nomes dos arquivos utilizados.
 
         :return: Os arquivos na mesma ordem em que são declarados
         :rtype: List[str]
         """
-        b = self.__bloco_por_tipo(BlocoNomesArquivos, 0)
-        return [] if b is None else b.data.iloc[:, 1]
+        b = self.data.get_sections_of_type(BlocoNomesArquivos)
+        return (
+            [] if not isinstance(b, BlocoNomesArquivos) else b.data.iloc[:, 1]
+        )
 
     @property
     def dger(self) -> Optional[str]:
         """
         Nome do arquivo de dados gerais utilizado pelo NEWAVE.
         """
         return self.__le_nome_por_indice(0)
```

### Comparing `inewave-0.0.97/inewave/newave/avl_cortesfpha_nwv.py` & `inewave-0.0.98/inewave/newave/avl_cortesfpha_nwv.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         return cls.read(join(diretorio, arquivo))
 
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
-        - indice_usina (`int`)
+        - codigo_usina (`int`)
         - periodo (`int`)
         - nome_usina (`str`)
         - indice_corte (`int`)
         - fator_correcao (`float`)
         - rhs_energia (`float`)
         - coeficiente_volume_util_MW_hm3 (`float`)
         - coeficiente_vazao_turbinada_MW_m3s (`float`)
```

### Comparing `inewave-0.0.97/inewave/newave/avl_desvfpha_s.py` & `inewave-0.0.98/inewave/newave/avl_desvfpha_v_q.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,94 +1,73 @@
 from inewave.newave.modelos.blocos.versaomodelo import VersaoModelo
-from inewave.newave.modelos.avl_desvfpha_s import TabelaAvlDesvFphaS
+from inewave.newave.modelos.avl_desvfpha_v_q import TabelaAvlDesvFphaVQ
 
 from cfinterface.files.blockfile import BlockFile
-from typing import Optional, TypeVar, Type
+from typing import Optional, TypeVar
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class AvlDesvFphaS(BlockFile):
+class AvlDesvFphaVQ(BlockFile):
     """
-    Arquivo com os desvios da função de produção no plano de
-    vazão vertida (S).
+    Arquivo com os desvios da função de produção nos planos de
+    volume armazenado e vazão turbinada (V-Q).
     """
 
-    BLOCKS = [VersaoModelo, TabelaAvlDesvFphaS]
+    BLOCKS = [VersaoModelo, TabelaAvlDesvFphaVQ]
     ENCODING = "iso-8859-1"
 
     T = TypeVar("T")
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__df_completo: Optional[pd.DataFrame] = None
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, arquivo: str = "avl_desvfpha_s_001.dat"
-    ) -> "AvlDesvFphaS":
+        cls, diretorio: str, arquivo: str = "avl_desvfpha_v_q_001.dat"
+    ) -> "AvlDesvFphaVQ":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, arquivo))
 
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
-        - indice_usina (`int`)
+        - codigo_usina (`int`)
         - nome_usina (`str`)
         - volume_armazenado_percentual (`float`)
         - vazao_turbinada_m3s (`float`)
-        - vazao_vertida_m3s (`float`)
         - desvio_percentual (`float`)
 
         :return: A tabela como um dataframe
         :rtype: pd.DataFrame | None
         """
         if self.__df_completo is None:
-            tabelas = self.data.of_type(TabelaAvlDesvFphaS)
+            tabelas = self.data.of_type(TabelaAvlDesvFphaVQ)
             self.__df_completo = pd.DataFrame()
             for t in tabelas:
                 self.__df_completo = pd.concat(
                     [self.__df_completo, t.data], ignore_index=True
                 )
         return self.__df_completo
 
-    def _bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def versao(self) -> Optional[str]:
         """
         A versão do modelo utilizada para executar o caso.
 
         :return: A versão do modelo
         :rtype: str | None
         """
-        b = self._bloco_por_tipo(VersaoModelo, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(VersaoModelo)
+        if isinstance(b, VersaoModelo):
             return b.data
         return None
```

### Comparing `inewave-0.0.97/inewave/newave/avl_desvfpha_v_q.py` & `inewave-0.0.98/inewave/newave/avl_desvfpha_s.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,74 @@
 from inewave.newave.modelos.blocos.versaomodelo import VersaoModelo
-from inewave.newave.modelos.avl_desvfpha_v_q import TabelaAvlDesvFphaVQ
+from inewave.newave.modelos.avl_desvfpha_s import TabelaAvlDesvFphaS
 
 from cfinterface.files.blockfile import BlockFile
-from typing import Optional, TypeVar, Type
+from typing import Optional, TypeVar
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class AvlDesvFphaVQ(BlockFile):
+class AvlDesvFphaS(BlockFile):
     """
-    Arquivo com os desvios da função de produção nos planos de
-    volume armazenado e vazão turbinada (V-Q).
+    Arquivo com os desvios da função de produção no plano de
+    vazão vertida (S).
     """
 
-    BLOCKS = [VersaoModelo, TabelaAvlDesvFphaVQ]
+    BLOCKS = [VersaoModelo, TabelaAvlDesvFphaS]
     ENCODING = "iso-8859-1"
 
     T = TypeVar("T")
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__df_completo: Optional[pd.DataFrame] = None
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, arquivo: str = "avl_desvfpha_v_q_001.dat"
-    ) -> "AvlDesvFphaVQ":
+        cls, diretorio: str, arquivo: str = "avl_desvfpha_s_001.dat"
+    ) -> "AvlDesvFphaS":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, arquivo))
 
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
-        - indice_usina (`int`)
+        - codigo_usina (`int`)
         - nome_usina (`str`)
         - volume_armazenado_percentual (`float`)
         - vazao_turbinada_m3s (`float`)
+        - vazao_vertida_m3s (`float`)
         - desvio_percentual (`float`)
 
         :return: A tabela como um dataframe
         :rtype: pd.DataFrame | None
         """
         if self.__df_completo is None:
-            tabelas = self.data.of_type(TabelaAvlDesvFphaVQ)
+            tabelas = self.data.of_type(TabelaAvlDesvFphaS)
             self.__df_completo = pd.DataFrame()
             for t in tabelas:
                 self.__df_completo = pd.concat(
                     [self.__df_completo, t.data], ignore_index=True
                 )
         return self.__df_completo
 
-    def _bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def versao(self) -> Optional[str]:
         """
         A versão do modelo utilizada para executar o caso.
 
         :return: A versão do modelo
         :rtype: str | None
         """
-        b = self._bloco_por_tipo(VersaoModelo, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(VersaoModelo)
+        if isinstance(b, VersaoModelo):
             return b.data
         return None
```

### Comparing `inewave-0.0.97/inewave/newave/bid.py` & `inewave-0.0.98/inewave/newave/bid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/cadic.py` & `inewave-0.0.98/inewave/newave/confhd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,77 @@
-from inewave.newave.modelos.cadic import BlocoCargasAdicionais
+from inewave.newave.modelos.confhd import BlocoConfUHE
 
 from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class CAdic(SectionFile):
+class Confhd(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às cargas
-    adicionais.
+    Armazena os dados de entrada do NEWAVE referentes às
+    configurações das usinas hidrelétricas.
+
+    Esta classe lida com informações de entrada fornecidas ao NEWAVE e
+    que podem ser modificadas através do arquivo `modif.dat`.
 
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [BlocoCargasAdicionais]
+    SECTIONS = [BlocoConfUHE]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="c_adic.dat") -> "CAdic":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="confhd.dat") -> "Confhd":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="c_adic.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="confhd.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
-    def cargas(self) -> Optional[pd.DataFrame]:
+    def usinas(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com as cargas adicionais por mês/ano e por subsistema
-        para cada razão de carga adicional. As colunas são:
+        Tabela com as usinas.
 
-        - Código Subsistema (`int`)
-        - Nome Subsistema (`str`)
-        - Razão (`str`)
-        - Ano (`str`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - codigo_usina (`int`)
+        - nome_usina (`str`)
+        - posto (`int`)
+        - codigo_usina_jusante (`int`)
+        - ree (`int`)
+        - volume_inicial_percentual (`float`)
+        - usina_existente (`str`)
+        - usina_modificada (`int`)
+        - ano_inicio_historico (`int`)
+        - ano_fim_historico (`int`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoCargasAdicionais, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoConfUHE)
+        if isinstance(b, BlocoConfUHE):
             return b.data
         return None
 
-    @cargas.setter
-    def cargas(self, valor: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoCargasAdicionais, 0)
-        if b is not None:
+    @usinas.setter
+    def usinas(self, valor: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoConfUHE)
+        if isinstance(b, BlocoConfUHE):
             b.data = valor
         else:
             raise ValueError("Campo não lido")
```

### Comparing `inewave-0.0.97/inewave/newave/caso.py` & `inewave-0.0.98/inewave/nwlistcf/caso.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from inewave.newave.modelos.caso import NomeCaso, CaminhoGerenciadorProcessos
+from inewave.nwlistcf.modelos.caso import NomeCaso
 
 from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
 class Caso(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes ao caso de estudo.
+    Armazena os dados de entrada do NWLISTCF referentes ao caso de estudo.
 
-    Esta classe lida com informações de entrada fornecidas ao NEWAVE e
+    Esta classe lida com informações de entrada fornecidas ao NWLISTCF e
     que podem ser modificadas através do arquivo `caso.dat`.
 
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [NomeCaso, CaminhoGerenciadorProcessos]
+    SECTIONS = [NomeCaso]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="caso.dat") -> "Caso":
         msg = (
@@ -38,64 +38,25 @@
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def arquivos(self) -> Optional[str]:
         """
-        Caminho para o arquivo `arquivos.dat` de entrada do NEWAVE.
+        Caminho para o arquivo `arquivos.dat` de entrada do NWLISTCF.
 
         :return: O caminho para o arquivo
         :rtype: str | None
         """
-        b = self.__bloco_por_tipo(NomeCaso, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(NomeCaso)
+        if isinstance(b, NomeCaso):
             return b.data
         return None
 
     @arquivos.setter
     def arquivos(self, a: str):
-        b = self.__bloco_por_tipo(NomeCaso, 0)
-        if b is not None:
-            b.data = a
-
-    @property
-    def gerenciador_processos(self) -> Optional[str]:
-        """
-        Caminho para o gerenciador de processos do NEWAVE.
-
-        :return: O caminho para o arquivo
-        :rtype: str | None
-        """
-        b = self.__bloco_por_tipo(CaminhoGerenciadorProcessos, 0)
-        if b is not None:
-            return b.data
-        return None
-
-    @gerenciador_processos.setter
-    def gerenciador_processos(self, a: str):
-        b = self.__bloco_por_tipo(CaminhoGerenciadorProcessos, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(NomeCaso)
+        if isinstance(b, NomeCaso):
             b.data = a
```

### Comparing `inewave-0.0.97/inewave/newave/clasgas.py` & `inewave-0.0.98/inewave/newave/clasgas.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TypeVar, List, Type
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class ClasGas(SectionFile):
+class Clasgas(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às classes
     de gás.
 
     """
 
     T = TypeVar("T")
@@ -20,15 +20,15 @@
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="clasgas.dat"
-    ) -> "ClasGas":
+    ) -> "Clasgas":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/newave/clast.py` & `inewave-0.0.98/inewave/newave/cvar.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,121 +1,114 @@
-from inewave.newave.modelos.clast import (
-    BlocoUTEClasT,
-    BlocoModificacaoUTEClasT,
+from inewave.newave.modelos.cvar import (
+    BlocoValoresConstantesCVAR,
+    BlocoAlfaVariavelNoTempo,
+    BlocoLambdaVariavelNoTempo,
 )
 
-from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from cfinterface.files.blockfile import BlockFile
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class ClasT(SectionFile):
+class Cvar(BlockFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às classes de
-    usinas térmicas.
-
+    Armazena os dados de entrada do NEWAVE referentes à curva para
+    penalização por volume mínimo dos reservatórios.
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [BlocoUTEClasT, BlocoModificacaoUTEClasT]
+    BLOCKS = [
+        BlocoValoresConstantesCVAR,
+        BlocoAlfaVariavelNoTempo,
+        BlocoLambdaVariavelNoTempo,
+    ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="clast.dat") -> "ClasT":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="cvar.dat") -> "Cvar":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="clast.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="cvar.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
+    @property
+    def valores_constantes(self) -> Optional[list]:
+        """
+        Valores constantes dos parâmetros ALFA e LAMBDA do CVAR.
+
+        :return: Os valores dos campos da linha como uma lista.
+        :rtype: list | None
+        """
+        b = self.data.get_blocks_of_type(BlocoValoresConstantesCVAR)
+        if isinstance(b, BlocoValoresConstantesCVAR):
+            return b.data
+        return None
+
+    @valores_constantes.setter
+    def valores_constantes(self, valores: list):
         """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
+        Valores constantes dos parâmetros ALFA e LAMBDA do CVAR.
 
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
+        :return: Os valores dos campos da linha como uma lista.
+        :rtype: list | None
+        """
+        b = self.data.get_blocks_of_type(BlocoValoresConstantesCVAR)
+        if isinstance(b, BlocoValoresConstantesCVAR):
+            b.data = valores
+        else:
+            raise ValueError("Bloco não lido")
 
     @property
-    def usinas(self) -> Optional[pd.DataFrame]:
+    def alfa_variavel(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com as usinas e seus custos.
+        Tabela com os valores variáveis do CVAR para o parâmetro ALFA.
 
-        - Número (`int`)
-        - Nome (`str`)
-        - Tipo Combustível (`str`)
-        - Custo [1-5] (`float`)
+        - ano (`str`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
+        - ...
+        - dezembro (`float`)
 
-        :return: A tabela como um DataFrame
+        :return: O valor de ALFA por estágio em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoUTEClasT, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(BlocoAlfaVariavelNoTempo)
+        if isinstance(b, BlocoAlfaVariavelNoTempo):
             return b.data
         return None
 
-    @usinas.setter
-    def usinas(self, valor: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoUTEClasT, 0)
-        if b is not None:
-            b.data = valor
-        else:
-            raise ValueError("Campo não lido")
-
     @property
-    def modificacoes(self) -> Optional[pd.DataFrame]:
+    def lambda_variavel(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com as modificações de custos das usinas
-        organizadas por usina.
+        Tabela com os valores variáveis do CVAR para o parâmetro LAMBDA.
 
-        - Número (`int`)
-        - Custo (`float`)
-        - Mês Início (`int`)
-        - Ano Início (`int`)
-        - Mês Fim (`int`)
-        - Ano Fim (`int`)
-        - Nome (`str`)
+        - ano (`str`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
+        - ...
+        - dezembro (`float`)
 
-        :return: A tabela como um DataFrame
+        :return: O valor de LAMBDA por estágio em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoModificacaoUTEClasT, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(BlocoLambdaVariavelNoTempo)
+        if isinstance(b, BlocoLambdaVariavelNoTempo):
             return b.data
         return None
-
-    @modificacoes.setter
-    def modificacoes(self, valor: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoModificacaoUTEClasT, 0)
-        if b is not None:
-            b.data = valor
-        else:
-            raise ValueError("Campo não lido")
```

### Comparing `inewave-0.0.97/inewave/newave/confhd.py` & `inewave-0.0.98/inewave/newave/dsvagua.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,76 @@
-from inewave.newave.modelos.confhd import BlocoConfUHE
+from inewave.newave.modelos.dsvagua import BlocoDsvUHE
 
 from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Confhd(SectionFile):
+class Dsvagua(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às
-    configurações das usinas hidrelétricas.
+    Armazena os dados de entrada do NEWAVE referentes aos
+    desvios de água por usina.
 
     Esta classe lida com informações de entrada fornecidas ao NEWAVE e
-    que podem ser modificadas através do arquivo `modif.dat`.
+    que podem ser modificadas através do arquivo `dsvagua.dat`.
 
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [BlocoConfUHE]
+    SECTIONS = [BlocoDsvUHE]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="confhd.dat") -> "Confhd":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="dsvagua.dat"
+    ) -> "Dsvagua":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="confhd.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="dsvagua.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
-    def usinas(self) -> Optional[pd.DataFrame]:
+    def desvios(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com as usinas.
+        Tabela com os desvios de água por usina e por estágio.
 
-        - Número (`int`)
-        - Nome (`str`)
-        - Posto (`int`)
-        - Jusante (`int`)
-        - REE (`int`)
-        - Volume Inicial (`float`)
-        - Usina Existente (`str`)
-        - Modificada (`int`)
-        - Início do Histórico (`int`)
-        - Fim do Histórico (`int`)
+        - ano (`int`)
+        - codigo_usina (`int`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
+        - ...
+        - dezembro (`float`)
+        - considera_desvio_usina_NC (`int`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoConfUHE, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoDsvUHE)
+        if isinstance(b, BlocoDsvUHE):
             return b.data
         return None
 
-    @usinas.setter
-    def usinas(self, valor: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoConfUHE, 0)
-        if b is not None:
+    @desvios.setter
+    def desvios(self, valor: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoDsvUHE)
+        if isinstance(b, BlocoDsvUHE):
             b.data = valor
         else:
             raise ValueError("Campo não lido")
```

### Comparing `inewave-0.0.97/inewave/newave/conft.py` & `inewave-0.0.98/inewave/newave/conft.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from inewave.newave.modelos.conft import BlocoConfUTE
 
 from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class ConfT(SectionFile):
+class Conft(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às configurações das
     usinas térmicas.
     """
 
     T = TypeVar("T")
 
     SECTIONS = [BlocoConfUTE]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="conft.dat") -> "ConfT":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="conft.dat") -> "Conft":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
@@ -36,53 +36,33 @@
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def usinas(self) -> Optional[pd.DataFrame]:
         """
         Tabela com as usinas.
 
-        - Número (`int`)
-        - Nome (`str`)
-        - Subsistema (`int`)
-        - Usina Existente (`str`)
-        - Classe (`int`)
+        - codigo_usina (`int`)
+        - nome_usina (`str`)
+        - submercado (`int`)
+        - usina_existente (`str`)
+        - classe (`int`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoConfUTE, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoConfUTE)
+        if isinstance(b, BlocoConfUTE):
             return b.data
         return None
 
     @usinas.setter
     def usinas(self, valor: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoConfUTE, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoConfUTE)
+        if isinstance(b, BlocoConfUTE):
             b.data = valor
         else:
             raise ValueError("Campo não lido")
```

### Comparing `inewave-0.0.97/inewave/newave/cortes.py` & `inewave-0.0.98/inewave/newave/cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/cortesh.py` & `inewave-0.0.98/inewave/newave/cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/curva.py` & `inewave-0.0.98/inewave/newave/curva.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from inewave.newave.modelos.curva import (
     BlocoConfiguracoesPenalizacaoCurva,
     BlocoPenalidadesViolacaoREECurva,
-    BlocoCurvaSegurancaSubsistema,
+    BlocoCurvaSegurancaREE,
     BlocoMaximoIteracoesProcessoIterativoEtapa2,
     BlocoIteracaoAPartirProcessoIterativoEtapa2,
     BlocoToleranciaProcessoIterativoEtapa2,
     BlocoImpressaoRelatorioProcessoIterativoEtapa2,
 )
 
 from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
@@ -24,15 +24,15 @@
     """
 
     T = TypeVar("T")
 
     SECTIONS = [
         BlocoConfiguracoesPenalizacaoCurva,
         BlocoPenalidadesViolacaoREECurva,
-        BlocoCurvaSegurancaSubsistema,
+        BlocoCurvaSegurancaREE,
         BlocoMaximoIteracoesProcessoIterativoEtapa2,
         BlocoIteracaoAPartirProcessoIterativoEtapa2,
         BlocoToleranciaProcessoIterativoEtapa2,
         BlocoImpressaoRelatorioProcessoIterativoEtapa2,
     ]
 
     def __init__(self, data=...) -> None:
@@ -52,199 +52,183 @@
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def configuracoes_penalizacao(self) -> Optional[list]:
         """
         Linha de configuração das opções de penalização do
         arquivo curva.dat.
 
         :return: Os valores dos campos da linha como uma lista.
         :rtype: Optional[list]
         """
-        b = self.__bloco_por_tipo(BlocoConfiguracoesPenalizacaoCurva, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoConfiguracoesPenalizacaoCurva)
+        if isinstance(b, BlocoConfiguracoesPenalizacaoCurva):
             return b.data
         return None
 
     @configuracoes_penalizacao.setter
     def configuracoes_penalizacao(self, valor: list):
-        b = self.__bloco_por_tipo(BlocoConfiguracoesPenalizacaoCurva, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoConfiguracoesPenalizacaoCurva)
+        if isinstance(b, BlocoConfiguracoesPenalizacaoCurva):
             b.data = valor
         else:
             raise ValueError("Campo não lido")
 
     @property
     def custos_penalidades(self) -> Optional[pd.DataFrame]:
         """
         Tabela com os custos para penalização em cada REE.
 
-        - Subsistema (`int`)
-        - Custo (`float`)
+        - ree (`int`)
+        - penalidade (`float`)
 
         :return: Os custos por REE em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoPenalidadesViolacaoREECurva, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoPenalidadesViolacaoREECurva)
+        if isinstance(b, BlocoPenalidadesViolacaoREECurva):
             return b.data
         return None
 
     @custos_penalidades.setter
     def custos_penalidades(self, valor: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoPenalidadesViolacaoREECurva, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoPenalidadesViolacaoREECurva)
+        if isinstance(b, BlocoPenalidadesViolacaoREECurva):
             b.data = valor
         else:
             raise ValueError("Campo não lido")
 
     @property
     def curva_seguranca(self) -> Optional[pd.DataFrame]:
         """
         Tabela da curva de segurança por REE.
 
-        - REE (`int`)
-        - Ano (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - ree (`int`)
+        - ano (`int`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: Os valores dos campos da linha como uma lista.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoCurvaSegurancaSubsistema, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoCurvaSegurancaREE)
+        if isinstance(b, BlocoCurvaSegurancaREE):
             return b.data
         return None
 
     @curva_seguranca.setter
     def curva_seguranca(self, valor: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoCurvaSegurancaSubsistema, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoCurvaSegurancaREE)
+        if isinstance(b, BlocoCurvaSegurancaREE):
             b.data = valor
         else:
             raise ValueError("Campo não lido")
 
     @property
     def maximo_iteracoes_etapa2(self) -> Optional[int]:
         """
         Número máximo de iterações no processo iterativo de 2ª
         etapa.
 
         :return: O valor como um int
         :rtype: Optional[int]
         """
-        b = self.__bloco_por_tipo(
-            BlocoMaximoIteracoesProcessoIterativoEtapa2, 0
+        b = self.data.get_sections_of_type(
+            BlocoMaximoIteracoesProcessoIterativoEtapa2
         )
-        if b is not None:
+        if isinstance(b, BlocoMaximoIteracoesProcessoIterativoEtapa2):
             return b.data
         return None
 
     @maximo_iteracoes_etapa2.setter
     def maximo_iteracoes_etapa2(self, valor: int):
-        b = self.__bloco_por_tipo(
-            BlocoMaximoIteracoesProcessoIterativoEtapa2, 0
+        b = self.data.get_sections_of_type(
+            BlocoMaximoIteracoesProcessoIterativoEtapa2
         )
-        if b is not None:
+        if isinstance(b, BlocoMaximoIteracoesProcessoIterativoEtapa2):
             b.data = valor
         else:
             raise ValueError("Campo não lido")
 
     @property
     def iteracao_a_partir_etapa2(self) -> Optional[int]:
         """
         Iteração a partir da qual ocorre o processo iterativo de 2ª
         etapa.
 
         :return: O valor como um int
         :rtype: Optional[int]
         """
-        b = self.__bloco_por_tipo(
-            BlocoIteracaoAPartirProcessoIterativoEtapa2, 0
+        b = self.data.get_sections_of_type(
+            BlocoIteracaoAPartirProcessoIterativoEtapa2
         )
-        if b is not None:
+        if isinstance(b, BlocoIteracaoAPartirProcessoIterativoEtapa2):
             return b.data
         return None
 
     @iteracao_a_partir_etapa2.setter
     def iteracao_a_partir_etapa2(self, valor: int):
-        b = self.__bloco_por_tipo(
-            BlocoIteracaoAPartirProcessoIterativoEtapa2, 0
+        b = self.data.get_sections_of_type(
+            BlocoIteracaoAPartirProcessoIterativoEtapa2
         )
-        if b is not None:
+        if isinstance(b, BlocoIteracaoAPartirProcessoIterativoEtapa2):
             b.data = valor
         else:
             raise ValueError("Campo não lido")
 
     @property
     def tolerancia_processo_etapa2(self) -> Optional[float]:
         """
         Tolerância para a execução do processo iterativo de etapa 2.
 
         :return: O valor como um float
         :rtype: Optional[float]
         """
-        b = self.__bloco_por_tipo(BlocoToleranciaProcessoIterativoEtapa2, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(
+            BlocoToleranciaProcessoIterativoEtapa2
+        )
+        if isinstance(b, BlocoToleranciaProcessoIterativoEtapa2):
             return b.data
         return None
 
     @tolerancia_processo_etapa2.setter
     def tolerancia_processo_etapa2(self, valor: int):
-        b = self.__bloco_por_tipo(BlocoToleranciaProcessoIterativoEtapa2, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(
+            BlocoToleranciaProcessoIterativoEtapa2
+        )
+        if isinstance(b, BlocoToleranciaProcessoIterativoEtapa2):
             b.data = valor
         else:
             raise ValueError("Campo não lido")
 
     @property
     def impressao_relatorio_etapa2(self) -> Optional[int]:
         """
         Opção de impressão ou não do relatório do
         processo iterativo de 2ª etapa.
 
         :return: O valor como um int
         :rtype: Optional[int]
         """
-        b = self.__bloco_por_tipo(
-            BlocoImpressaoRelatorioProcessoIterativoEtapa2, 0
+        b = self.data.get_sections_of_type(
+            BlocoImpressaoRelatorioProcessoIterativoEtapa2
         )
-        if b is not None:
+        if isinstance(b, BlocoImpressaoRelatorioProcessoIterativoEtapa2):
             return b.data
         return None
 
     @impressao_relatorio_etapa2.setter
     def impressao_relatorio_etapa2(self, valor: int):
-        b = self.__bloco_por_tipo(
-            BlocoImpressaoRelatorioProcessoIterativoEtapa2, 0
+        b = self.data.get_sections_of_type(
+            BlocoImpressaoRelatorioProcessoIterativoEtapa2
         )
-        if b is not None:
+        if isinstance(b, BlocoImpressaoRelatorioProcessoIterativoEtapa2):
             b.data = valor
         else:
             raise ValueError("Campo não lido")
```

### Comparing `inewave-0.0.97/inewave/newave/dsvagua.py` & `inewave-0.0.98/inewave/newave/eafpast.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,96 +1,73 @@
-from inewave.newave.modelos.dsvagua import BlocoDsvUHE
+from inewave.newave.modelos.eafpast import BlocoEafPast
 
 from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class DSVAgua(SectionFile):
+class Eafpast(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes aos
-    desvios de água por usina.
+    Armazena os dados de entrada do NEWAVE referentes às
+    vazões anteriores ao período de planejamento por REE.
 
     Esta classe lida com informações de entrada fornecidas ao NEWAVE e
-    que podem ser modificadas através do arquivo `dsvagua.dat`.
+    que são usadas junto das contidas no arquivo `vazoes.dat`.
 
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [BlocoDsvUHE]
+    SECTIONS = [BlocoEafPast]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dsvagua.dat"
-    ) -> "DSVAgua":
+        cls, diretorio: str, nome_arquivo="eafpast.dat"
+    ) -> "Eafpast":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="dsvagua.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="eafpast.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
-    def desvios(self) -> Optional[pd.DataFrame]:
+    def tendencia(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com os desvios de água por usina e por estágio.
+        Tabela com a tendência hidrológica por REE.
 
-        - Ano (`int`)
-        - Usina (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - codigo_ree (`int`)
+        - nome_ree (`str`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
-        - Flag (`int`)
+        - dezembro (`float`)
 
         :return: A tabela como um DataFrame
-        :rtype: pd.DataFrame | None
+        :rtype: Optional[pd.DataFrame]
         """
-        b = self.__bloco_por_tipo(BlocoDsvUHE, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoEafPast)
+        if isinstance(b, BlocoEafPast):
             return b.data
         return None
 
-    @desvios.setter
-    def desvios(self, valor: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoDsvUHE, 0)
-        if b is not None:
-            b.data = valor
-        else:
-            raise ValueError("Campo não lido")
+    @tendencia.setter
+    def tendencia(self, df: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoEafPast)
+        if isinstance(b, BlocoEafPast):
+            b.data = df
```

### Comparing `inewave-0.0.97/inewave/newave/eafpast.py` & `inewave-0.0.98/inewave/newave/vazpast.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,72 @@
-from inewave.newave.modelos.eafpast import BlocoEafPast
+from inewave.newave.modelos.vazpast import BlocoVazPast
 
 from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class EafPast(SectionFile):
+class Vazpast(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às
-    vazões anteriores ao período de planejamento por REE.
+    vazões anteriores ao período de planejamento.
 
     Esta classe lida com informações de entrada fornecidas ao NEWAVE e
-    que são usadas junto das contidas no arquivo `vazoes.dat`.
+    que são usadas juntos das contidas no arquivo `vazoes.dat`.
 
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [BlocoEafPast]
+    SECTIONS = [BlocoVazPast]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="eafpast.dat"
-    ) -> "EafPast":
+        cls, diretorio: str, nome_arquivo="vazpast.dat"
+    ) -> "Vazpast":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="eafpast.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="vazpast.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def tendencia(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com a tendência hidrológica por REE.
+        Tabela com a tendência hidrológica por UHE.
 
-        - Índice (`int`)
-        - REE (`str`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - codigo_usina (`int`)
+        - nome_usina (`str`)
+        - janeiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: A tabela como um DataFrame
-        :rtype: Optional[pd.DataFrame]
+        :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoEafPast, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoVazPast)
+        if isinstance(b, BlocoVazPast):
             return b.data
         return None
 
     @tendencia.setter
     def tendencia(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoEafPast, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoVazPast)
+        if isinstance(b, BlocoVazPast):
             b.data = df
```

### Comparing `inewave-0.0.97/inewave/newave/elnino.py` & `inewave-0.0.98/inewave/newave/elnino.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/enavazb.py` & `inewave-0.0.98/inewave/newave/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/enavazf.py` & `inewave-0.0.98/inewave/newave/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/energiab.py` & `inewave-0.0.98/inewave/newave/energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/energiaf.py` & `inewave-0.0.98/inewave/newave/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/energias.py` & `inewave-0.0.98/inewave/newave/energias.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/engnat.py` & `inewave-0.0.98/inewave/newave/engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/ensoaux.py` & `inewave-0.0.98/inewave/newave/ensoaux.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/eolicacadastro.py` & `inewave-0.0.98/inewave/newave/modif.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,389 +1,470 @@
-from typing import Type, TypeVar, List, Optional, Union
-from datetime import datetime
-
 from cfinterface.components.register import Register
 from cfinterface.files.registerfile import RegisterFile
-from inewave.newave.modelos.eolicacadastro import (
-    RegistroEolicaCadastro,
-    RegistroEolicaCadastroConjuntoAerogeradores,
-    RegistroEolicaCadastroAerogerador,
-    RegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo,
-    RegistroEolicaConjuntoAerogeradoresPotenciaEfetiva,
-    RegistroPEECadastro,
-    RegistroPEEPotenciaInstaladaPeriodo,
+from inewave.newave.modelos.modif import (
+    USINA,
+    VOLMIN,
+    VOLMAX,
+    NUMCNJ,
+    NUMMAQ,
+    VAZMIN,
+    CFUGA,
+    CMONT,
+    VMAXT,
+    VMINT,
+    VMINP,
+    VAZMINT,
+    VAZMAXT,
+    TURBMAXT,
+    TURBMINT,
 )
 
+
+from typing import TypeVar, List, Optional, Union
+import pandas as pd  # type: ignore
+
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class EolicaCadastro(RegisterFile):
+class Modif(RegisterFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes ao cadastro
-    das usinas eólicas do sistema.
+    Armazena os dados de entrada do NEWAVE referentes às alterações nas
+    configurações das usinas hidroelétricas.
     """
 
     T = TypeVar("T")
 
     REGISTERS = [
-        RegistroEolicaCadastroAerogerador,
-        RegistroEolicaCadastroConjuntoAerogeradores,
-        RegistroEolicaCadastro,
-        RegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo,
-        RegistroEolicaConjuntoAerogeradoresPotenciaEfetiva,
-        RegistroPEECadastro,
-        RegistroPEEPotenciaInstaladaPeriodo,
+        USINA,
+        VOLMIN,
+        VOLMAX,
+        NUMCNJ,
+        NUMMAQ,
+        VAZMIN,
+        CFUGA,
+        CMONT,
+        VMAXT,
+        VMINT,
+        VMINP,
+        VAZMINT,
+        VAZMAXT,
+        TURBMAXT,
+        TURBMINT,
     ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="eolica-cadastro.csv"
-    ) -> "EolicaCadastro":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="modif.dat") -> "Modif":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(
-        self, diretorio: str, nome_arquivo="eolica-cadastro.csv"
-    ):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="modif.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
+    def usina(
+        self,
+        codigo: Optional[int] = None,
+        nome: Optional[str] = None,
+        df: bool = False,
+    ) -> Optional[Union[USINA, List[USINA], pd.DataFrame]]:
+        """
+        Obtém um registro que define a usina modificada.
+
+        :param codigo: código da usina modificada
+        :type codigo: int | None
+        :param nome: nome da usina
+        :type nome: str | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`USINA` | list[:class:`USINA`] | :class:`pd.DataFrame` | None
         """
-        Obtém os registro de um tipo, se houver algum no arquivo.
-
-        :param registro: Um tipo de registro para ser lido
-        :type registro: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-
-        """
-        return [b for b in self.data.of_type(registro)]
-
-    def __obtem_registros(self, tipo: Type[T]) -> List[T]:
-        return self.__registros_por_tipo(tipo)
-
-    def __obtem_registros_com_filtros(
-        self, tipo_registro: Type[T], **kwargs
-    ) -> Optional[Union[T, List[T]]]:
-        def __atende(r) -> bool:
-            condicoes: List[bool] = []
-            for k, v in kwargs.items():
-                if v is not None:
-                    condicoes.append(getattr(r, k) == v)
-            return all(condicoes)
-
-        regs_filtro = [
-            r for r in self.__obtem_registros(tipo_registro) if __atende(r)
-        ]
-        if len(regs_filtro) == 0:
-            return None
-        elif len(regs_filtro) == 1:
-            return regs_filtro[0]
+        if df:
+            return self._as_df(USINA)
         else:
-            return regs_filtro
+            return self.data.get_registers_of_type(
+                USINA, codigo=codigo, nome=nome
+            )
 
-    def cria_registro(self, anterior: Register, registro: Register):
+    def volmin(
+        self,
+        volume: Optional[float] = None,
+        unidade: Optional[str] = None,
+        df: bool = False,
+    ) -> Optional[Union[VOLMIN, List[VOLMIN], pd.DataFrame]]:
+        """
+        Obtém um registro que define um volume mínimo.
+
+        :param volume: volume mínimo
+        :type volume: float | None
+        :param unidade: unidade do volume
+        :type unidade: str | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`VOLMIN` | list[:class:`VOLMIN`] | :class:`pd.DataFrame` | None
         """
-        Adiciona um registro ao arquivo após um outro registro previamente
-        existente.
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                VOLMIN, volume=volume, unidade=unidade
+            )
 
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
+    def volmax(
+        self,
+        volume: Optional[float] = None,
+        unidade: Optional[str] = None,
+        df: bool = False,
+    ) -> Optional[Union[VOLMAX, List[VOLMAX], pd.DataFrame]]:
+        """
+        Obtém um registro que define um volume máximo.
+
+        :param volume: volume máximo
+        :type volume: float | None
+        :param unidade: unidade do volume
+        :type unidade: str | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`VOLMAX` | list[:class:`VOLMAX`] | :class:`pd.DataFrame` | None
         """
-        self.data.add_after(anterior, registro)
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                VOLMAX, volume=volume, unidade=unidade
+            )
 
-    def deleta_registro(self, registro: Register):
+    def numcnj(
+        self,
+        numero: Optional[int] = None,
+        df: bool = False,
+    ) -> Optional[Union[NUMCNJ, List[NUMCNJ], pd.DataFrame]]:
         """
-        Remove um registro existente no arquivo.
+        Obtém um registro que um número de conjuntos de máquinas.
 
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
+        :param numero: o número
+        :type numero: int | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`NUMCNJ` | list[:class:`NUMCNJ`] | :class:`pd.DataFrame` | None
         """
-        self.data.remove(registro)
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(NUMCNJ, numero=numero)
 
-    def append_registro(self, registro: Register):
+    def nummaq(
+        self,
+        conjunto: Optional[int] = None,
+        numero_maquinas: Optional[int] = None,
+        df: bool = False,
+    ) -> Optional[Union[NUMMAQ, List[NUMMAQ], pd.DataFrame]]:
+        """
+        Obtém um registro que um número de máquinas por
+            conjunto de máquinas.
+
+        :param conjunto: o conjunto
+        :type conjunto: int | None
+        :param numero_maquinas: o número de máquinas
+        :type numero_maquinas: int | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`NUMMAQ` | list[:class:`NUMMAQ`] | :class:`pd.DataFrame` | None
         """
-        Adiciona um registro ao arquivo na última posição.
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                NUMMAQ, conjunto=conjunto, numero_maquinas=numero_maquinas
+            )
+
+    def vazmin(
+        self,
+        vazao: Optional[float] = None,
+        df: bool = False,
+    ) -> Optional[Union[VAZMIN, List[VAZMIN], pd.DataFrame]]:
         """
-        self.data.append(registro)
+        Obtém um registro que define uma vazão mínima.
 
-    def preppend_registro(self, registro: Register):
+        :param vazao: vazão mínima
+        :type vazao: float | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`VAZMIN` | list[:class:`VAZMIN`] | :class:`pd.DataFrame` | None
         """
-        Adiciona um registro ao arquivo na primeira posição.
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(VAZMIN, vazao=vazao)
+
+    def cfuga(
+        self,
+        mes: Optional[int] = None,
+        ano: Optional[int] = None,
+        nivel: Optional[float] = None,
+        df: bool = False,
+    ) -> Optional[Union[CFUGA, List[CFUGA], pd.DataFrame]]:
+        """
+        Obtém um registro que define o nível do canal de fuga.
+
+        :param mes: mês de validade do nível
+        :type mes: int | None
+        :param ano: ano de validade do nível
+        :type ano: int | None
+        :param nivel: o nível
+        :type nivel: float | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`CFUGA` | list[:class:`CFUGA`] | :class:`pd.DataFrame` | None
         """
-        self.data.preppend(registro)
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                CFUGA, mes=mes, ano=ano, nivel=nivel
+            )
 
-    def eolica_cadastro(
+    def cmont(
         self,
-        codigo_eolica: Optional[int] = None,
-        nome_eolica: Optional[str] = None,
-        quantidade_conjuntos: Optional[str] = None,
-    ) -> Optional[Union[RegistroEolicaCadastro, List[RegistroEolicaCadastro]]]:
+        mes: Optional[int] = None,
+        ano: Optional[int] = None,
+        nivel: Optional[float] = None,
+        df: bool = False,
+    ) -> Optional[Union[CMONT, List[CMONT], pd.DataFrame]]:
+        """
+        Obtém um registro que define o nível do canal de montante.
+
+        :param mes: mês de validade do nível
+        :type mes: int | None
+        :param ano: ano de validade do nível
+        :type ano: int | None
+        :param nivel: o nível
+        :type nivel: float | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`CMONT` | list[:class:`CMONT`] | :class:`pd.DataFrame` | None
         """
-        Obtém um registro que cadastra uma usina eólica.
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                CMONT, mes=mes, ano=ano, nivel=nivel
+            )
 
-        :param codigo_eolica: código que especifica a usina
-        :type codigo_eolica: int | None
-        :param nome_eolica: nome da usina
-        :type nome_eolica: str | None
-        :param quantidade_conjuntos: quantidade de conjuntos de geradores
-        :type quantidade_conjuntos: int | None
+    def vmaxt(
+        self,
+        mes: Optional[int] = None,
+        ano: Optional[int] = None,
+        volume: Optional[float] = None,
+        unidade: Optional[str] = None,
+        df: bool = False,
+    ) -> Optional[Union[VMAXT, List[VMAXT], pd.DataFrame]]:
+        """
+        Obtém um registro que define o volume máximo por período.
+
+        :param mes: mês de validade do volume
+        :type mes: int | None
+        :param ano: ano de validade do volume
+        :type ano: int | None
+        :param volume: o volume
+        :type volume: float | None
+        :param unidade: a unidade do volume
+        :type unidade: str | None
         :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroEolicaCadastro` |
-            list[:class:`RegistroEolicaCadastro`] | None
+        :rtype: :class:`VMAXT` | list[:class:`VMAXT`] | :class:`pd.DataFrame` | None
         """
-        return self.__obtem_registros_com_filtros(
-            RegistroEolicaCadastro,
-            codigo_eolica=codigo_eolica,
-            nome_eolica=nome_eolica,
-            quantidade_conjuntos=quantidade_conjuntos,
-        )
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                VMAXT, mes=mes, ano=ano, volume=volume, unidade=unidade
+            )
 
-    def eolica_cadastro_conjunto_aerogeradores(
+    def vmint(
         self,
-        codigo_eolica: Optional[int] = None,
-        indice_conjunto: Optional[int] = None,
-        nome_conjunto: Optional[str] = None,
-        quantidade_aerogeradores: Optional[int] = None,
-    ) -> Optional[
-        Union[
-            RegistroEolicaCadastroConjuntoAerogeradores,
-            List[RegistroEolicaCadastroConjuntoAerogeradores],
-        ]
-    ]:
-        """
-        Obtém um registro que cadastra um conjunto de aerogeradores
-        de uma usina.
-
-        :param codigo_eolica: código que especifica a usina
-        :type codigo_eolica: int | None
-        :param indice_conjunto: código do conjunto de geradores da usina
-        :type indice_conjunto: int | None
-        :param nome_conjunto: nome do conjunto
-        :type nome_conjunto: str | None
-        :param quantidade_aerogeradores: quantidade de geradores no conjunto
-        :type quantidade_aerogeradores: int | None
-        :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroEolicaCadastroConjuntoAerogeradores` |
-            list[:class:`RegistroEolicaCadastroConjuntoAerogeradores`] | None
-        """
-        return self.__obtem_registros_com_filtros(
-            RegistroEolicaCadastroConjuntoAerogeradores,
-            codigo_eolica=codigo_eolica,
-            indice_conjunto=indice_conjunto,
-            nome_conjunto=nome_conjunto,
-            quantidade_aerogeradores=quantidade_aerogeradores,
-        )
+        mes: Optional[int] = None,
+        ano: Optional[int] = None,
+        volume: Optional[float] = None,
+        unidade: Optional[str] = None,
+        df: bool = False,
+    ) -> Optional[Union[VMINT, List[VMINT], pd.DataFrame]]:
+        """
+        Obtém um registro que define o volume mínimo por período.
+
+        :param mes: mês de validade do volume
+        :type mes: int | None
+        :param ano: ano de validade do volume
+        :type ano: int | None
+        :param volume: o volume
+        :type volume: float | None
+        :param unidade: a unidade do volume
+        :type unidade: str | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`VMINT` | list[:class:`VMINT`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                VMINT, mes=mes, ano=ano, volume=volume, unidade=unidade
+            )
 
-    def eolica_cadastro_aerogerador(
+    def vminp(
         self,
-        codigo_eolica: Optional[int] = None,
-        indice_conjunto: Optional[int] = None,
-        velocidade_cutin: Optional[float] = None,
-        velocidade_nominal: Optional[float] = None,
-        velocidade_cutout: Optional[float] = None,
-        potencia_velocidade_cutin: Optional[float] = None,
-        potencia_velocidade_nominal: Optional[float] = None,
-        potencia_velocidade_cutout: Optional[float] = None,
-        altura_torre: Optional[float] = None,
-    ) -> Optional[
-        Union[
-            RegistroEolicaCadastroAerogerador,
-            List[RegistroEolicaCadastroAerogerador],
-        ]
-    ]:
-        """
-        Obtém um registro que o cadastro de um conjunto de aerogeradores
-        de uma usina.
-
-        :param codigo_eolica: código que especifica a usina
-        :type codigo_eolica: float | None
-        :param indice_conjunto: código do conjunto de geradores da usina
-        :type indice_conjunto: float | None
-        :param velocidade_cutin: velocidade de cutin do gerador
-        :type velocidade_cutin: float | None
-        :param velocidade_nominal: velocidade nominal do gerador
-        :type velocidade_nominal: float | None
-        :param velocidade_cutout: velocidade de cutout do gerador
-        :type velocidade_cutout: float | None
-        :param potencia_velocidade_cutin: potência na velocidade de cutin
-        :type potencia_velocidade_cutin: float | None
-        :param potencia_velocidade_nominal: potência na velocidade nominal
-        :type potencia_velocidade_nominal: float | None
-        :param potencia_velocidade_cutout: potência na velocidade cutout
-        :type potencia_velocidade_cutout: float | None
-        :param altura_torre: altura da torre do gerador
-        :type altura_torre: float | None
-
-        :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroEolicaCadastroAerogerador` |
-            list[:class:`RegistroEolicaCadastroAerogerador`] | None
-        """
-        return self.__obtem_registros_com_filtros(
-            RegistroEolicaCadastroAerogerador,
-            codigo_eolica=codigo_eolica,
-            indice_conjunto=indice_conjunto,
-            velocidade_cutin=velocidade_cutin,
-            velocidade_nominal=velocidade_nominal,
-            velocidade_cutout=velocidade_cutout,
-            potencia_velocidade_cutin=potencia_velocidade_cutin,
-            potencia_velocidade_nominal=potencia_velocidade_nominal,
-            potencia_velocidade_cutout=potencia_velocidade_cutout,
-            altura_torre=altura_torre,
-        )
+        mes: Optional[int] = None,
+        ano: Optional[int] = None,
+        volume: Optional[float] = None,
+        unidade: Optional[str] = None,
+        df: bool = False,
+    ) -> Optional[Union[VMINP, List[VMINP], pd.DataFrame]]:
+        """
+        Obtém um registro que define o volume mínimo para penalidade.
+
+        :param mes: mês de validade do volume
+        :type mes: int | None
+        :param ano: ano de validade do volume
+        :type ano: int | None
+        :param volume: o volume
+        :type volume: float | None
+        :param unidade: a unidade do volume
+        :type unidade: str | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`VMINP` | list[:class:`VMINP`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                VMINP, mes=mes, ano=ano, volume=volume, unidade=unidade
+            )
 
-    def eolica_conjunto_aerogeradores_quantidade_operando_periodo(
+    def vazmint(
         self,
-        codigo_eolica: Optional[int] = None,
-        indice_conjunto: Optional[int] = None,
-        periodo_inicial: Optional[datetime] = None,
-        periodo_final: Optional[datetime] = None,
-        numero_aerogeradores: Optional[int] = None,
-    ) -> Optional[
-        Union[
-            RegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo,
-            List[RegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo],
-        ]
-    ]:
-        """
-        Obtém um registro que o cadastro de um conjunto de aerogeradores
-        de uma usina.
-
-        :param codigo_eolica: código que especifica a usina
-        :type codigo_eolica: int | None
-        :param indice_conjunto: código do conjunto de geradores da usina
-        :type indice_conjunto: int | None
-        :param periodo_inicial: período de início de operação
-        :type periodo_inicial: datetime | None
-        :param periodo_final: período de fim de operação
-        :type periodo_final: datetime | None
-        :param numero_aerogeradores: número de geradores operando
-        :type numero_aerogeradores: int | None
-        :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo` |
-            list[:class:`RegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo`] | None
-        """
-        return self.__obtem_registros_com_filtros(
-            RegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo,
-            codigo_eolica=codigo_eolica,
-            indice_conjunto=indice_conjunto,
-            periodo_inicial=periodo_inicial,
-            periodo_final=periodo_final,
-            numero_aerogeradores=numero_aerogeradores,
-        )
+        mes: Optional[int] = None,
+        ano: Optional[int] = None,
+        vazao: Optional[float] = None,
+        df: bool = False,
+    ) -> Optional[Union[VAZMINT, List[VAZMINT], pd.DataFrame]]:
+        """
+        Obtém um registro que define a vazão mínima por período.
+
+        :param mes: mês de validade da vazão
+        :type mes: int | None
+        :param ano: ano de validade da vazão
+        :type ano: int | None
+        :param vazao: a vazão mínima
+        :type vazao: float | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`VAZMINT` | list[:class:`VAZMINT`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                VAZMINT, mes=mes, ano=ano, vazao=vazao
+            )
 
-    def eolica_conjunto_aerogeradores_potencia_efetiva_periodo(
+    def vazmaxt(
         self,
-        codigo_eolica: Optional[int] = None,
-        indice_conjunto: Optional[int] = None,
-        periodo_inicial: Optional[datetime] = None,
-        periodo_final: Optional[datetime] = None,
-        potencia_efetiva: Optional[float] = None,
-    ) -> Optional[
-        Union[
-            RegistroEolicaConjuntoAerogeradoresPotenciaEfetiva,
-            List[RegistroEolicaConjuntoAerogeradoresPotenciaEfetiva],
-        ]
-    ]:
-        """
-        Obtém um registro que contém a potência efetiva por período
-        para um conjunto de aerogeradores.
-
-        :param codigo_eolica: código que especifica a usina
-        :type codigo_eolica: int | None
-        :param indice_conjunto: código do conjunto de geradores da usina
-        :type indice_conjunto: int | None
-        :param periodo_inicial: período de início de operação
-        :type periodo_inicial: datetime | None
-        :param periodo_final: período de fim de operação
-        :type periodo_final: datetime | None
-        :param potencia_efetiva: potência efetiva do conjunto de aerogeradores
-        :type potencia_efetiva: float | None
-        :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroEolicaConjuntoAerogeradoresPotenciaEfetiva` |
-            list[:class:`RegistroEolicaConjuntoAerogeradoresPotenciaEfetiva`] | None
-        """
-        return self.__obtem_registros_com_filtros(
-            RegistroEolicaConjuntoAerogeradoresPotenciaEfetiva,
-            codigo_eolica=codigo_eolica,
-            indice_conjunto=indice_conjunto,
-            periodo_inicial=periodo_inicial,
-            periodo_final=periodo_final,
-            potencia_efetiva=potencia_efetiva,
-        )
+        mes: Optional[int] = None,
+        ano: Optional[int] = None,
+        vazao: Optional[float] = None,
+        df: bool = False,
+    ) -> Optional[Union[VAZMAXT, List[VAZMAXT], pd.DataFrame]]:
+        """
+        Obtém um registro que define a vazão máxima por período.
+
+        :param mes: mês de validade da vazão
+        :type mes: int | None
+        :param ano: ano de validade da vazão
+        :type ano: int | None
+        :param vazao: a vazão máxima
+        :type vazao: float | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`VAZMAXT` | list[:class:`VAZMAXT`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                VAZMAXT, mes=mes, ano=ano, vazao=vazao
+            )
 
-    def pee_cad(
+    def turbmaxt(
         self,
-        codigo_pee: Optional[int] = None,
-        nome_pee: Optional[str] = None,
-    ) -> Optional[Union[RegistroPEECadastro, List[RegistroPEECadastro]]]:
-        """
-        Obtém um registro que cadastra um PEE.
-
-        :param codigo_pee: código que especifica o PEE
-        :type codigo_pee: int | None
-        :param nome_pee: nome do PEE
-        :type nome_pee: str | None
-        :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroPEECadastro` |
-            list[:class:`RegistroPEECadastro`] | None
-        """
-        return self.__obtem_registros_com_filtros(
-            RegistroPEECadastro,
-            codigo_pee=codigo_pee,
-            nome_pee=nome_pee,
-        )
+        mes: Optional[int] = None,
+        ano: Optional[int] = None,
+        turbinamento: Optional[float] = None,
+        df: bool = False,
+    ) -> Optional[Union[TURBMAXT, List[TURBMAXT], pd.DataFrame]]:
+        """
+        Obtém um registro que define o turbinamento máximo por período.
+
+        :param mes: mês de validade do turbinamento
+        :type mes: int | None
+        :param ano: ano de validade do turbinamento
+        :type ano: int | None
+        :param turbinamento: o turbinamento máximo
+        :type turbinamento: float | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`TURBMAXT` | list[:class:`TURBMAXT`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                TURBMAXT, mes=mes, ano=ano, turbinamento=turbinamento
+            )
 
-    def pee_pot_inst_per(
+    def turbmint(
         self,
-        codigo_pee: Optional[int] = None,
-        periodo_inicial: Optional[datetime] = None,
-        periodo_final: Optional[datetime] = None,
-        potencia_instalada: Optional[float] = None,
-    ) -> Optional[
-        Union[
-            RegistroPEEPotenciaInstaladaPeriodo,
-            List[RegistroPEEPotenciaInstaladaPeriodo],
-        ]
-    ]:
-        """
-        Obtém um registro que contém a potência instalada por período
-        para um PEE.
-
-        :param codigo_pee: código que especifica o PEE
-        :type codigo_pee: int | None
-        :param periodo_inicial: período de início de operação
-        :type periodo_inicial: datetime | None
-        :param periodo_final: período de fim de operação
-        :type periodo_final: datetime | None
-        :param potencia_instalada: potência efetiva do PEE
-        :type potencia_instalada: float | None
-        :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroPEEPotenciaInstaladaPeriodo` |
-            list[:class:`RegistroPEEPotenciaInstaladaPeriodo`] | None
-        """
-        return self.__obtem_registros_com_filtros(
-            RegistroPEEPotenciaInstaladaPeriodo,
-            codigo_pee=codigo_pee,
-            periodo_inicial=periodo_inicial,
-            periodo_final=periodo_final,
-            potencia_instalada=potencia_instalada,
+        mes: Optional[int] = None,
+        ano: Optional[int] = None,
+        turbinamento: Optional[float] = None,
+        df: bool = False,
+    ) -> Optional[Union[TURBMINT, List[TURBMINT], pd.DataFrame]]:
+        """
+        Obtém um registro que define o turbinamento mínimo por período.
+        :param mes: mês de validade do turbinamento
+        :type mes: int | None
+        :param ano: ano de validade do turbinamento
+        :type ano: int | None
+        :param turbinamento: o turbinamento mínimo
+        :type turbinamento: float | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`TURBMINT` | list[:class:`TURBMINT`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(USINA)
+        else:
+            return self.data.get_registers_of_type(
+                TURBMINT, mes=mes, ano=ano, turbinamento=turbinamento
+            )
+
+    def modificacoes_usina(self, codigo: int) -> Optional[List[Register]]:
+        """
+        Filtra os registros que são associados a uma usina específica.
+
+        :param codigo: O código da usina
+        :type codigo: int
+        :return: Os registros que modificam a usina
+        :rtype: List[Register]
+        """
+        usinas = self.usina()
+        if usinas is None or isinstance(usinas, USINA):
+            return None
+        reg_usina: List[USINA] = list(
+            filter(lambda r: r.codigo == codigo, usinas)
         )
+        modificacoes_usina: List[Register] = []
+        if len(reg_usina) > 0:
+            r = reg_usina[0].next
+            while not (isinstance(r, USINA) or r.is_last):
+                modificacoes_usina.append(r)
+                r = r.next
+
+        return modificacoes_usina
```

### Comparing `inewave-0.0.97/inewave/newave/eolicahistorico.py` & `inewave-0.0.98/inewave/newave/eolicahistorico.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Type, TypeVar, List, Optional, Union
+from typing import TypeVar, List, Optional, Union
 from datetime import datetime
 
-from cfinterface.components.register import Register
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.eolicahistorico import (
     RegistroEolicaHistoricoVentoHorizonte,
     RegistroEolicaHistoricoVento,
     RegistroHistoricoVentoHorizonte,
     RegistroHistoricoVento,
 )
@@ -49,84 +48,14 @@
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
-        """
-        Obtém os registro de um tipo, se houver algum no arquivo.
-
-        :param registro: Um tipo de registro para ser lido
-        :type registro: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-
-        """
-        return [b for b in self.data.of_type(registro)]
-
-    def __obtem_registros(self, tipo: Type[T]) -> List[T]:
-        return self.__registros_por_tipo(tipo)
-
-    def __obtem_registros_com_filtros(
-        self, tipo_registro: Type[T], **kwargs
-    ) -> Optional[Union[T, List[T]]]:
-        def __atende(r) -> bool:
-            condicoes: List[bool] = []
-            for k, v in kwargs.items():
-                if v is not None:
-                    condicoes.append(getattr(r, k) == v)
-            return all(condicoes)
-
-        regs_filtro = [
-            r for r in self.__obtem_registros(tipo_registro) if __atende(r)
-        ]
-        if len(regs_filtro) == 0:
-            return None
-        elif len(regs_filtro) == 1:
-            return regs_filtro[0]
-        else:
-            return regs_filtro
-
-    def cria_registro(self, anterior: Register, registro: Register):
-        """
-        Adiciona um registro ao arquivo após um outro registro previamente
-        existente.
-
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.add_after(anterior, registro)
-
-    def deleta_registro(self, registro: Register):
-        """
-        Remove um registro existente no arquivo.
-
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.remove(registro)
-
-    def append_registro(self, registro: Register):
-        """
-        Adiciona um registro ao arquivo na última posição.
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.append(registro)
-
-    def preppend_registro(self, registro: Register):
-        """
-        Adiciona um registro ao arquivo na primeira posição.
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.preppend(registro)
-
     def eolica_historico_vento_horizonte(
         self,
         data_inicial: Optional[datetime] = None,
         data_final: Optional[datetime] = None,
     ) -> Optional[
         Union[
             RegistroEolicaHistoricoVentoHorizonte,
@@ -140,15 +69,15 @@
         :type data_inicial: datetime | None
         :param data_final: data de fim do histórico
         :type data_final: datetime | None
         :return: Um ou mais registros, se existirem.
         :rtype: :class:`RegistroEolicaHistoricoVentoHorizonte` |
             list[:class:`RegistroEolicaHistoricoVentoHorizonte`] | None
         """
-        return self.__obtem_registros_com_filtros(
+        return self.data.get_registers_of_type(
             RegistroEolicaHistoricoVentoHorizonte,
             data_inicial=data_inicial,
             data_final=data_final,
         )
 
     def eolica_historico_vento(
         self,
@@ -177,15 +106,15 @@
         :type velocidade: float | None
         :param direcao: direção do vento
         :type direcao: float | None
         :return: Um ou mais registros, se existirem.
         :rtype: :class:`RegistroEolicaHistoricoVento` |
             list[:class:`RegistroEolicaHistoricoVento`] | None
         """
-        return self.__obtem_registros_com_filtros(
+        return self.data.get_registers_of_type(
             RegistroEolicaHistoricoVento,
             codigo_eolica=codigo_eolica,
             data_inicial=data_inicial,
             data_final=data_final,
             velocidade=velocidade,
             direcao=direcao,
         )
@@ -207,15 +136,15 @@
         :type data_inicial: datetime | None
         :param data_final: data de fim do histórico
         :type data_final: datetime | None
         :return: Um ou mais registros, se existirem.
         :rtype: :class:`RegistroHistoricoVentoHorizonte` |
             list[:class:`RegistroHistoricoVentoHorizonte`] | None
         """
-        return self.__obtem_registros_com_filtros(
+        return self.data.get_registers_of_type(
             RegistroHistoricoVentoHorizonte,
             data_inicial=data_inicial,
             data_final=data_final,
         )
 
     def vento_hist(
         self,
@@ -244,15 +173,15 @@
         :type velocidade: float | None
         :param direcao: direção do vento
         :type direcao: float | None
         :return: Um ou mais registros, se existirem.
         :rtype: :class:`RegistroHistoricoVento` |
             list[:class:`RegistroHistoricoVento`] | None
         """
-        return self.__obtem_registros_com_filtros(
+        return self.data.get_registers_of_type(
             RegistroHistoricoVento,
             codigo_eolica=codigo_eolica,
             data_inicial=data_inicial,
             data_final=data_final,
             velocidade=velocidade,
             direcao=direcao,
         )
```

### Comparing `inewave-0.0.97/inewave/newave/eolicasubmercado.py` & `inewave-0.0.98/inewave/newave/restricaoenergia.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,167 +1,134 @@
-from typing import Type, TypeVar, List, Optional, Union
+from typing import TypeVar, List, Optional, Union
+from datetime import datetime
 
-from cfinterface.components.register import Register
 from cfinterface.files.registerfile import RegisterFile
-from inewave.newave.modelos.eolicasubmercado import (
-    RegistroEolicaSubmercado,
-    RegistroPEESubmercado,
+from inewave.newave.modelos.restricaoenergia import (
+    RegistroRHE,
+    RegistroRHEHorizPer,
+    RegistroRHELsLPPEarmi,
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class EolicaSubmercado(RegisterFile):
+class RestricaoEnergia(RegisterFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes ao mapeamento
-    de usinas eólicas e submercados.
+    Armazena os dados de entrada do NEWAVE referentes ao cadastro
+    das restrições lineares por partes no domínio de energia (REE).
     """
 
     T = TypeVar("T")
 
-    REGISTERS = [RegistroEolicaSubmercado, RegistroPEESubmercado]
+    REGISTERS = [
+        RegistroRHELsLPPEarmi,
+        RegistroRHEHorizPer,
+        RegistroRHE,
+    ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="eolica-submercado.csv"
-    ) -> "EolicaSubmercado":
+        cls, diretorio: str, nome_arquivo="restricao-energia.csv"
+    ) -> "RestricaoEnergia":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(
-        self, diretorio: str, nome_arquivo="eolica-submercado.csv"
+        self, diretorio: str, nome_arquivo="restricao-energia.csv"
     ):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
-        """
-        Obtém os registro de um tipo, se houver algum no arquivo.
-
-        :param registro: Um tipo de registro para ser lido
-        :type registro: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-
-        """
-        return [b for b in self.data.of_type(registro)]
-
-    def __obtem_registros(self, tipo: Type[T]) -> List[T]:
-        return self.__registros_por_tipo(tipo)
-
-    def __obtem_registros_com_filtros(
-        self, tipo_registro: Type[T], **kwargs
-    ) -> Optional[Union[T, List[T]]]:
-        def __atende(r) -> bool:
-            condicoes: List[bool] = []
-            for k, v in kwargs.items():
-                if v is not None:
-                    condicoes.append(getattr(r, k) == v)
-            return all(condicoes)
-
-        regs_filtro = [
-            r for r in self.__obtem_registros(tipo_registro) if __atende(r)
-        ]
-        if len(regs_filtro) == 0:
-            return None
-        elif len(regs_filtro) == 1:
-            return regs_filtro[0]
-        else:
-            return regs_filtro
-
-    def cria_registro(self, anterior: Register, registro: Register):
-        """
-        Adiciona um registro ao arquivo após um outro registro previamente
-        existente.
-
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.add_after(anterior, registro)
-
-    def deleta_registro(self, registro: Register):
-        """
-        Remove um registro existente no arquivo.
-
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.remove(registro)
-
-    def append_registro(self, registro: Register):
-        """
-        Adiciona um registro ao arquivo na última posição.
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.append(registro)
-
-    def preppend_registro(self, registro: Register):
-        """
-        Adiciona um registro ao arquivo na primeira posição.
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
+    def rhe(
+        self,
+        codigo_restricao: Optional[int] = None,
+        formula: Optional[str] = None,
+    ) -> Optional[Union[RegistroRHE, List[RegistroRHE]]]:
+        """
+        Obtém um registro que cadastra uma usina restrição linear por
+        partes de energia (REE).
+
+        :param codigo_restricao: código que especifica a restrição
+        :type codigo_restricao: int | None
+        :param formula: equação da restrição
+        :type formula: str | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`RegistroRHE` |
+            list[:class:`RegistroRHE`] | None
         """
-        self.data.preppend(registro)
+        return self.data.get_registers_of_type(
+            RegistroRHE,
+            codigo_restricao=codigo_restricao,
+            formula=formula,
+        )
 
-    def eolica_submercado(
+    def rhe_horiz_per(
         self,
-        codigo_eolica: Optional[int] = None,
-        codigo_submercado: Optional[int] = None,
-    ) -> Optional[
-        Union[
-            RegistroEolicaSubmercado,
-            List[RegistroEolicaSubmercado],
-        ]
-    ]:
-        """
-        Obtém um registro que contém o mapeamento usina-submercado.
-
-        :param codigo_eolica: código que especifica a usina
-        :type codigo_eolica: int | None
-        :param codigo_submercado: código que especifica o submercado
-        :type codigo_submercado: int | None
+        codigo_restricao: Optional[int] = None,
+        data_inicial: Optional[datetime] = None,
+        data_final: Optional[datetime] = None,
+    ) -> Optional[Union[RegistroRHEHorizPer, List[RegistroRHEHorizPer]]]:
+        """
+        Obtém um registro que cadastra o horizonte de validade de uma
+        restrição linear por partes de energia.
+
+        :param codigo_restricao: código que especifica a restrição
+        :type codigo_restricao: int | None
+        :param data_inicial: data inicial de validade da restrição
+        :type data_inicial: datetime | None
+        :param data_final: data final de validade da restrição
+        :type data_final: datetime | None
         :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroEolicaSubmercado` |
-            list[:class:`RegistroEolicaSubmercado`] | None
+        :rtype: :class:`RegistroRHEHorizPer` |
+            list[:class:`RegistroRHEHorizPer`] | None
         """
-        return self.__obtem_registros_com_filtros(
-            RegistroEolicaSubmercado,
-            codigo_eolica=codigo_eolica,
-            codigo_submercado=codigo_submercado,
+        return self.data.get_registers_of_type(
+            RegistroRHEHorizPer,
+            codigo_restricao=codigo_restricao,
+            data_inicial=data_inicial,
+            data_final=data_final,
         )
 
-    def pee_subm(
+    def rhe_ls_lpp_earmi(
         self,
-        codigo_pee: Optional[int] = None,
-        codigo_submercado: Optional[int] = None,
-    ) -> Optional[Union[RegistroPEESubmercado, List[RegistroPEESubmercado]]]:
-        """
-        Obtém um registro que contém o mapeamento PEE-submercado.
-
-        :param codigo_pee: código que especifica o PEE
-        :type codigo_pee: int | None
-        :param codigo_submercado: código que especifica o submercado
-        :type codigo_submercado: int | None
+        codigo_restricao: Optional[int] = None,
+        indice_reta: Optional[int] = None,
+        coeficiente_angular: Optional[float] = None,
+        coeficiente_linear: Optional[float] = None,
+    ) -> Optional[Union[RegistroRHELsLPPEarmi, List[RegistroRHELsLPPEarmi]]]:
+        """
+        Obtém um registro que cadastra as retas da restrição linear
+        por partes de energia.
+
+        :param codigo_restricao: código que especifica a restrição
+        :type codigo_restricao: int | None
+        :param indice_reta: índice da reta definida
+        :type indice_reta: int | None
+        :param coeficiente_angular: coeficiente angular da reta
+        :type coeficiente_angular: float | None
+        :param coeficiente_linear: coeficiente linear da reta
+        :type coeficiente_linear: float | None
         :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroPEESubmercado` |
-            list[:class:`RegistroPEESubmercado`] | None
+        :rtype: :class:`RegistroRHELsLPPEarmi` |
+            list[:class:`RegistroRHELsLPPEarmi`] | None
         """
-        return self.__obtem_registros_com_filtros(
-            RegistroPEESubmercado,
-            codigo_pee=codigo_pee,
-            codigo_submercado=codigo_submercado,
+        return self.data.get_registers_of_type(
+            RegistroRHELsLPPEarmi,
+            codigo_restricao=codigo_restricao,
+            indice_reta=indice_reta,
+            coeficiente_angular=coeficiente_angular,
+            coeficiente_linear=coeficiente_linear,
         )
```

### Comparing `inewave-0.0.97/inewave/newave/exph.py` & `inewave-0.0.98/inewave/newave/cadic.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,73 @@
-from inewave.newave.modelos.exph import BlocoUHEExph
+from inewave.newave.modelos.cadic import BlocoCargasAdicionais
 
 from cfinterface.files.sectionfile import SectionFile
-from cfinterface.components.section import Section
-from typing import TypeVar, List, Type, Optional
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Exph(SectionFile):
+class Cadic(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes à expansão
-    hidraulica do sistema.
+    Armazena os dados de entrada do NEWAVE referentes às cargas
+    adicionais.
 
     """
 
     T = TypeVar("T")
 
-    SECTIONS: List[Type[Section]] = [BlocoUHEExph]
+    SECTIONS = [BlocoCargasAdicionais]
+
+    def __init__(self, data=...) -> None:
+        super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="exph.dat") -> "Exph":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="c_adic.dat") -> "Cadic":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="exph.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="c_adic.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
-    def expansoes(self) -> Optional[pd.DataFrame]:
+    def cargas(self) -> Optional[pd.DataFrame]:
         """
-        A tabela de expansões de máquinas das UHEs.
+        Tabela com as cargas adicionais por mês/ano e por subsistema
+        para cada razão de carga adicional. As colunas são:
 
-        - Código UHE (`int`)
-        - Nome UHE (`str`)
-        - Início Enchimento (`datetime`)
-        - Duração (`int`)
-        - Volume Morto (`float`)
-        - Data de Entrada (`datetime`)
-        - Potência (`float`)
-        - Máquina (`int`)
-        - Conjunto (`int`)
+        - codigo_subsistema (`int`)
+        - nome_subsistema (`str`)
+        - razao (`str`)
+        - ano (`str`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
+        - ...
+        - dezembro (`float`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoUHEExph, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoCargasAdicionais)
+        if isinstance(b, BlocoCargasAdicionais):
             return b.data
         return None
 
-    @expansoes.setter
-    def expansoes(self, d: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoUHEExph, 0)
-        if b is not None:
-            b.data = d
+    @cargas.setter
+    def cargas(self, valor: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoCargasAdicionais)
+        if isinstance(b, BlocoCargasAdicionais):
+            b.data = valor
+        else:
+            raise ValueError("Campo não lido")
```

### Comparing `inewave-0.0.97/inewave/newave/expt.py` & `inewave-0.0.98/inewave/newave/ghmin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,72 @@
-from inewave.newave.modelos.expt import BlocoUTEExpt
-
 from cfinterface.files.sectionfile import SectionFile
 from cfinterface.components.section import Section
 from typing import TypeVar, List, Type, Optional
+
+from inewave.newave.modelos.ghmin import BlocoUHEGhmin
+
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Expt(SectionFile):
+class Ghmin(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes à expansão
-    térmica do sistema.
+    Armazena os dados de entrada do NEWAVE referentes à geração hidráulica
+    mínima por usina.
 
     """
 
     T = TypeVar("T")
 
-    SECTIONS: List[Type[Section]] = [BlocoUTEExpt]
+    SECTIONS: List[Type[Section]] = [BlocoUHEGhmin]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="expt.dat") -> "Expt":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="ghmin.dat") -> "Ghmin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="expt.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghmin.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
-    def expansoes(self) -> Optional[pd.DataFrame]:
+    def geracoes(self) -> Optional[pd.DataFrame]:
         """
-        A tabela de expansões das UTEs.
+        Tabela com as gerações mínimas das usinas
+        hidráulicas.
 
         - codigo_usina (`int`)
-        - tipo (`str`)
-        - modificacao (`float`)
-        - data_inicio (`datetime`)
-        - data_fim (`datetime`)
-        - nome_usina (`str`)
+        - mes (`int`)
+        - ano (`str`)
+        - patamar (`int`)
+        - geracao (`float`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoUTEExpt, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoUHEGhmin)
+        if isinstance(b, BlocoUHEGhmin):
             return b.data
         return None
 
-    @expansoes.setter
-    def expansoes(self, d: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoUTEExpt, 0)
-        if b is not None:
-            b.data = d
+    @geracoes.setter
+    def geracoes(self, valor: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoUHEGhmin)
+        if isinstance(b, BlocoUHEGhmin):
+            b.data = valor
+        else:
+            raise ValueError("Campo não lido")
```

### Comparing `inewave-0.0.97/inewave/newave/forward.py` & `inewave-0.0.98/inewave/newave/forward.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/forwarh.py` & `inewave-0.0.98/inewave/newave/forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/gee.py` & `inewave-0.0.98/inewave/newave/gee.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/gtminpat.py` & `inewave-0.0.98/inewave/newave/gtminpat.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TypeVar, List, Type
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class GTMinPat(SectionFile):
+class Gtminpat(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes à geração térmica
     mínima por patamar.
 
     """
 
     T = TypeVar("T")
@@ -20,15 +20,15 @@
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="gtminpat.dat"
-    ) -> "GTMinPat":
+    ) -> "Gtminpat":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/newave/hidr.py` & `inewave-0.0.98/inewave/newave/hidr.py`

 * *Files 23% similar despite different names*

```diff
@@ -52,59 +52,59 @@
         registros: List[RegistroUHEHidr] = [
             r for r in self.data.of_type(RegistroUHEHidr)
         ]
         if len(registros) == 0:
             return None
         df = pd.DataFrame(
             columns=[
-                "Nome",
-                "Posto",
-                "Subsistema",
-                "Empresa",
-                "Jusante",
-                "Desvio",
-                "Volume Mínimo",
-                "Volume Máximo",
-                "Volume Vertedouro",
-                "Volume Desvio",
-                "Cota Mínima",
-                "Cota Máxima",
-                *[f"A{i} VC" for i in range(5)],
-                *[f"A{i} CA" for i in range(5)],
-                *[f"Evaporação {m}" for m in MESES_ABREV],
-                "Num. Conjuntos Máquinas",
-                *[f"Num. Máquinas Conjunto {i}" for i in range(1, 6)],
-                *[f"PotEf Conjunto {i}" for i in range(1, 6)],
-                *[f"HEf Conjunto {i}" for i in range(1, 6)],
-                *[f"QEf Conjunto {i}" for i in range(1, 6)],
-                "Produtibilidade Específica",
-                "Perdas",
-                "Número PJUS",
-                *[f"A{i} PJUS1" for i in range(5)],
-                *[f"A{i} PJUS2" for i in range(5)],
-                *[f"A{i} PJUS3" for i in range(5)],
-                *[f"A{i} PJUS4" for i in range(5)],
-                *[f"A{i} PJUS5" for i in range(5)],
-                *[f"A{i} PJUS6" for i in range(5)],
-                *[f"REF PJUS {i}" for i in range(1, 7)],
-                "Canal de Fuga Médio",
-                "Influencia Vert. Cfuga",
-                "Fator Carga Max.",
-                "Fator Carga Min.",
-                "Vazão Mínima Histórica",
-                "Num. Unidades Base",
-                "Tipo Turbina",
-                "Representação Conjunto",
-                "TEIF",
-                "IP",
-                "Tipo de Perda",
-                "Data",
-                "Observação",
-                "Volume de Referência",
-                "Tipo de Regulação",
+                "nome_usina",
+                "posto",
+                "submercado",
+                "empresa",
+                "codigo_usina_jusante",
+                "desvio",
+                "volume_minimo",
+                "volume_maximo",
+                "volume_vertedouro",
+                "volume_desvio",
+                "cota_minima",
+                "cota_maxima",
+                *[f"a{i}_volume_cota" for i in range(5)],
+                *[f"a{i}_cota_area" for i in range(5)],
+                *[f"evaporacao_{m}" for m in MESES_ABREV],
+                "numero_conjuntos_maquinas",
+                *[f"maquinas_conjunto_{i}" for i in range(1, 6)],
+                *[f"potencia_nominal_conjunto_{i}" for i in range(1, 6)],
+                *[f"queda_nominal_conjunto_{i}" for i in range(1, 6)],
+                *[f"vazao_nominal_conjunto_{i}" for i in range(1, 6)],
+                "produtibilidade_especifica",
+                "perdas",
+                "numero_polinomios_jusante",
+                *[f"a{i}_jusante_1" for i in range(5)],
+                *[f"a{i}_jusante_2" for i in range(5)],
+                *[f"a{i}_jusante_3" for i in range(5)],
+                *[f"a{i}_jusante_4" for i in range(5)],
+                *[f"a{i}_jusante_5" for i in range(5)],
+                *[f"a{i}_jusante_6" for i in range(5)],
+                *[f"referencia_jusante_{i}" for i in range(1, 7)],
+                "canal_fuga_medio",
+                "influencia_vertimento_canal_fuga",
+                "fator_carga_maximo",
+                "fator_carga_minimo",
+                "vazao_minima_historica",
+                "numero_unidades_base",
+                "tipo_turbina",
+                "representacao_conjunto",
+                "teif",
+                "ip",
+                "tipo_perda",
+                "data",
+                "observacao",
+                "volume_referencia",
+                "tipo_regulacao",
             ]
         )
         for i, r in enumerate(registros):
             df.loc[i + 1] = [
                 r.nome,
                 r.posto,
                 r.subsistema,
@@ -141,161 +141,161 @@
                 r.ip,
                 r.tipo_perda,
                 r.data_referencia,
                 r.observacao,
                 r.volume_referencia,
                 r.tipo_regulacao,
             ]
-        df.index.name = "Código"
+        df.index.name = "codigo_usina"
 
         df = df.astype(
             {
-                "Nome": str,
-                "Posto": int,
-                "Subsistema": int,
-                "Empresa": int,
-                "Jusante": int,
-                "Desvio": int,
-                "Volume Mínimo": float,
-                "Volume Máximo": float,
-                "Volume Vertedouro": float,
-                "Volume Desvio": float,
-                "Cota Mínima": float,
-                "Cota Máxima": float,
-                "Produtibilidade Específica": float,
-                "Perdas": float,
-                "Canal de Fuga Médio": float,
-                "Influencia Vert. Cfuga": int,
-                "Fator Carga Max.": float,
-                "Fator Carga Min.": float,
-                "Vazão Mínima Histórica": int,
-                "Num. Unidades Base": int,
-                "Tipo Turbina": int,
-                "Representação Conjunto": int,
-                "TEIF": float,
-                "IP": float,
-                "Tipo de Perda": int,
-                "Data": str,
-                "Observação": str,
-                "Volume de Referência": float,
-                "Tipo de Regulação": str,
+                "nome_usina": str,
+                "posto": int,
+                "submercado": int,
+                "empresa": int,
+                "codigo_usina_jusante": int,
+                "desvio": int,
+                "volume_minimo": float,
+                "volume_maximo": float,
+                "volume_vertedouro": float,
+                "volume_desvio": float,
+                "cota_minima": float,
+                "cota_maxima": float,
+                "produtibilidade_especifica": float,
+                "perdas": float,
+                "canal_fuga_medio": float,
+                "influencia_vertimento_canal_fuga": int,
+                "fator_carga_maximo": float,
+                "fator_carga_minimo": float,
+                "vazao_minima_historica": int,
+                "numero_unidades_base": int,
+                "tipo_turbina": int,
+                "representacao_conjunto": int,
+                "teif": float,
+                "ip": float,
+                "tipo_perda": int,
+                "data": str,
+                "observacao": str,
+                "volume_referencia": float,
+                "tipo_regulacao": str,
             },
         )
         return df
 
     def __atualiza_registros(self):
         registros: List[RegistroUHEHidr] = [r for r in self.data][1:]
         for (_, linha), r in zip(self.cadastro.iterrows(), registros):
-            r.nome = linha["Nome"]
-            r.posto = linha["Posto"]
-            r.subsistema = linha["Subsistema"]
-            r.empresa = linha["Empresa"]
-            r.jusante = linha["Jusante"]
-            r.desvio = linha["Desvio"]
-            r.volume_minimo = linha["Volume Mínimo"]
-            r.volume_maximo = linha["Volume Máximo"]
-            r.volume_vertedouro = linha["Volume Vertedouro"]
-            r.volume_desvio = linha["Volume Desvio"]
-            r.cota_minima = linha["Cota Mínima"]
-            r.cota_maxima = linha["Cota Máxima"]
+            r.nome = linha["nome_usina"]
+            r.posto = linha["posto"]
+            r.subsistema = linha["submercado"]
+            r.empresa = linha["empresa"]
+            r.jusante = linha["codigo_usina_jusante"]
+            r.desvio = linha["desvio"]
+            r.volume_minimo = linha["volume_minimo"]
+            r.volume_maximo = linha["volume_maximo"]
+            r.volume_vertedouro = linha["volume_vertedouro"]
+            r.volume_desvio = linha["volume_desvio"]
+            r.cota_minima = linha["cota_minima"]
+            r.cota_maxima = linha["cota_maxima"]
             r.polinomio_volume_cota = linha[
-                [f"A{i} VC" for i in range(5)]
+                [f"a{i}_volume_cota" for i in range(5)]
             ].tolist()
             r.polinomio_cota_area = linha[
-                [f"A{i} CA" for i in range(5)]
+                [f"a{i}_cota_area" for i in range(5)]
             ].tolist()
             r.evaporacao = linha[
-                [f"Evaporação {m}" for m in MESES_ABREV]
+                [f"evaporacao_{m}" for m in MESES_ABREV]
             ].tolist()
-            r.numero_conjuntos_maquinas = linha["Num. Conjuntos Máquinas"]
+            r.numero_conjuntos_maquinas = linha["numero_conjuntos_maquinas"]
             r.potef_conjunto = linha[
-                [f"PotEf Conjunto {i}" for i in range(1, 6)]
+                [f"potencia_nominal_conjunto_{i}" for i in range(1, 6)]
             ].tolist()
             r.hef_conjunto = linha[
-                [f"HEf Conjunto {i}" for i in range(1, 6)]
+                [f"queda_nominal_conjunto_{i}" for i in range(1, 6)]
             ].tolist()
             r.qef_conjunto = linha[
-                [f"QEf Conjunto {i}" for i in range(1, 6)]
+                [f"vazao_nominal_conjunto_{i}" for i in range(1, 6)]
             ].tolist()
-            r.produtibilidade_especifica = linha["Produtibilidade Específica"]
-            r.perdas = linha["Perdas"]
-            r.numero_polinomios_jusante = linha["Número PJUS"]
+            r.produtibilidade_especifica = linha["produtibilidade_especifica"]
+            r.perdas = linha["perdas"]
+            r.numero_polinomios_jusante = linha["numero_polinomios_jusante"]
             r.polinomios_jusante = linha[
-                [f"A{i} PJUS1" for i in range(5)]
-                + [f"A{i} PJUS2" for i in range(5)]
-                + [f"A{i} PJUS3" for i in range(5)]
-                + [f"A{i} PJUS4" for i in range(5)]
-                + [f"A{i} PJUS5" for i in range(5)]
-                + [f"A{i} PJUS6" for i in range(5)]
-                + [f"REF PJUS {i}" for i in range(1, 7)]
+                [f"a{i}_jusante_1" for i in range(5)]
+                + [f"a{i}_jusante_2" for i in range(5)]
+                + [f"a{i}_jusante_3" for i in range(5)]
+                + [f"a{i}_jusante_4" for i in range(5)]
+                + [f"a{i}_jusante_5" for i in range(5)]
+                + [f"a{i}_jusante_6" for i in range(5)]
+                + [f"referencia_jusante_{i}" for i in range(1, 7)]
             ].tolist()
-            r.canal_fuga_medio = linha["Canal de Fuga Médio"]
+            r.canal_fuga_medio = linha["canal_fuga_medio"]
             r.influencia_vertimento_canal_fuga = linha[
-                "Influencia Vert. Cfuga"
+                "influencia_vertimento_canal_fuga"
             ]
-            r.fator_carga_maximo = linha["Fator Carga Max."]
-            r.fator_carga_minimo = linha["Fator Carga Min."]
-            r.vazao_minima_historica = linha["Vazão Mínima Histórica"]
-            r.numero_unidades_base = linha["Num. Unidades Base"]
-            r.tipo_turbina = linha["Tipo Turbina"]
-            r.representacao_conjunto = linha["Representação Conjunto"]
-            r.teif = linha["TEIF"]
-            r.ip = linha["IP"]
-            r.tipo_perda = linha["Tipo de Perda"]
-            r.data_referencia = linha["Data"]
-            r.observacao = linha["Observação"]
-            r.volume_referencia = linha["Volume de Referência"]
-            r.tipo_regulacao = linha["Tipo de Regulação"]
+            r.fator_carga_maximo = linha["fator_carga_maximo"]
+            r.fator_carga_minimo = linha["fator_carga_minimo"]
+            r.vazao_minima_historica = linha["vazao_minima_historica"]
+            r.numero_unidades_base = linha["numero_unidades_base"]
+            r.tipo_turbina = linha["tipo_turbina"]
+            r.representacao_conjunto = linha["representacao_conjunto"]
+            r.teif = linha["teif"]
+            r.ip = linha["ip"]
+            r.tipo_perda = linha["tipo_perda"]
+            r.data_referencia = linha["data"]
+            r.observacao = linha["observacao"]
+            r.volume_referencia = linha["volume_referencia"]
+            r.tipo_regulacao = linha["tipo_regulacao"]
 
     @property
     def cadastro(self) -> pd.DataFrame:
         """
         Obtém a tabela com os dados cadastrais existentes no arquivo
         binário.
 
-        - Nome (`str`): nome da usina (12 caracteres)
-        - Posto (`int`): posto de vazão natural da usina
-        - Subsistema (`int`): subsistema da usina
-        - Empresa (`int`): agente responsável pela usina
-        - Jusante (`int`): posto à jusante da usina
-        - Desvio (`float`): TODO
-        - Volume Mínimo (`float`): volume mínimo da usina (hm3)
-        - Volume Máximo (`float`): volume máximo da usina (hm3)
-        - Volume Vertedouro (`float`): volume do vertedouro da usina (hm3)
-        - Volume Desvio (`float`): TODO
-        - Cota Mínima (`float`): cota mínima da usina (m)
-        - Cota Máxima (`float`): cota máxima da usina (m)
-        - A[0-4] VC (`float`): coeficientes do polinômio volume-cota
-        - A[0-4] CA (`float`): coeficientes do polinômio cota-área
-        - Evaporação [JAN..DEZ] (`float`): coeficientes de evaporação (mm)
-        - Num Conjunto Máquinas (`int`): número de conjuntos de máquinas
-        - Num Máquinas Conjunto [1-5] (`int`): máquinas por conjunto
-        - PotEf. Conjunto [1-5] (`float`): potência das máquinas (MWmed)
-        - HEf Conjunto [1-5]: alturas nominais de queda por conjunto (m)
-        - QEf Conjunto [1-5]: vazões nominais por conjunto (m3/s)
-        - Produtibilidade Específica (`float`): produtibilidade específica
-        - Perdas (`float`): perdas da usina
-        - Número PJUS (`int`): número de polinômios de jusante
-        - C[0-4] PJUS[1-6] (`float`): coeficientes de cada polinjus
-        - REF PJUS [1-6] (`float`): coeficientes do polinjus de referência
-        - Canal de Fuga Médio (`float`): cota média do canal de fuga (m)
-        - Influencia Vert. Cfuga (`int`): TODO (0 ou 1)
-        - Fator Carga Max. (`float`): TODO (%)
-        - Fator Carga Min. (`float`): TODO (%)
-        - Vazão Mínima Histórica (`float`): vazão mínima da usina (m3/s)
-        - Num. Unidades Base (`int`): TODO
-        - Tipo Turbina (`int`): TODO
-        - Representação Conjunto (`int`): TODO
-        - TEIF (`float`): TODO (%)
-        - IP (`float`): TODO (%)
-        - Tipo de Perda (`int`): TODO
-        - Data (`str`): DD-MM-AA
-        - Observação (`str`): observação qualquer sobre a usina
-        - Volume de Referência (`float`): TODO (hm3)
-        - Tipo de Regulação (`str`): D, S ou M
+        - nome_usina (`str`): nome da usina (12 caracteres)
+        - posto (`int`): posto de vazão natural da usina
+        - submercado (`int`): submercado da usina
+        - empresa (`int`): agente responsável pela usina
+        - codigo_usina_jusante (`int`): posto à jusante da usina
+        - desvio (`float`): TODO
+        - volume_minimo (`float`): volume mínimo da usina (hm3)
+        - volume_maximo (`float`): volume máximo da usina (hm3)
+        - volume_vertedouro (`float`): volume do vertedouro da usina (hm3)
+        - volume_desvio (`float`): TODO
+        - cota_minima (`float`): cota mínima da usina (m)
+        - cota_maxima (`float`): cota máxima da usina (m)
+        - a[0-4]_volume_cota (`float`): coeficientes do polinômio volume-cota
+        - a[0-4]_cota_area (`float`): coeficientes do polinômio cota-área
+        - evaporacao_[JAN..DEZ] (`float`): coeficientes de evaporação (mm)
+        - numero_conjuntos_maquinas (`int`): número de conjuntos de máquinas
+        - maquinas_conjunto_[1-5] (`int`): máquinas por conjunto
+        - potencia_nominal_conjunto_[1-5] (`float`): potência das máquinas (MWmed)
+        - queda_nominal_conjunto_[1-5]: alturas nominais de queda por conjunto (m)
+        - vazao_nominal_conjunto_[1-5]: vazões nominais por conjunto (m3/s)
+        - produtibilidade_especifica (`float`): produtibilidade específica
+        - perdas (`float`): perdas da usina
+        - numero_polinomios_jusante (`int`): número de polinômios de jusante
+        - a[0-4]_jusante_[1-6] (`float`): coeficientes de cada polinjus
+        - referencia_jusante_[1-6] (`float`): coeficientes do polinjus de referência
+        - canal_fuga_medio (`float`): cota média do canal de fuga (m)
+        - influencia_vertimento_canal_fuga (`int`): TODO (0 ou 1)
+        - fator_carga_maximo (`float`): TODO (%)
+        - fator_carga_minimo (`float`): TODO (%)
+        - vazao_minima_historica (`float`): vazão mínima da usina (m3/s)
+        - numero_unidades_base (`int`): TODO
+        - tipo_turbina (`int`): TODO
+        - representacao_conjunto (`int`): TODO
+        - teif (`float`): TODO (%)
+        - ip (`float`): TODO (%)
+        - tipo_perda (`int`): TODO
+        - data (`str`): DD-MM-AA
+        - observacao (`str`): observação qualquer sobre a usina
+        - volume_referencia (`float`): TODO (hm3)
+        - tipo_regulacao (`str`): D, S ou M
 
         :return: A tabela com os dados cadastrais
         :rtype: pd.DataFrame | None
         """
         if self.__df is None:
             self.__df = self.__monta_df_de_registros()
         return self.__df
```

### Comparing `inewave-0.0.97/inewave/newave/itaipu.py` & `inewave-0.0.98/inewave/newave/itaipu.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/manutt.py` & `inewave-0.0.98/inewave/newave/manutt.py`

 * *Files 21% similar despite different names*

```diff
@@ -38,34 +38,14 @@
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def manutencoes(self) -> Optional[pd.DataFrame]:
         """
         Tabela com as manutenções por usinas.
 
         - codigo_empresa (`int`)
         - nome_empresa (`str`)
@@ -75,19 +55,19 @@
         - data_inicio (`datetime`)
         - duracao (`int`)
         - potencia (`float`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoManutencaoUTE, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoManutencaoUTE)
+        if isinstance(b, BlocoManutencaoUTE):
             return b.data
         return None
 
     @manutencoes.setter
     def manutencoes(self, valor: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoManutencaoUTE, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoManutencaoUTE)
+        if isinstance(b, BlocoManutencaoUTE):
             b.data = valor
         else:
             raise ValueError("Campo não lido")
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/adterm.py` & `inewave-0.0.98/inewave/newave/modelos/adterm.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,20 +38,20 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            cols = [f"Patamar {i}" for i in range(1, n_pat + 1)]
+            cols = [f"patamar_{i}" for i in range(1, n_pat + 1)]
             df = pd.DataFrame(tabela, columns=cols)
-            df["Código UTE"] = codigo_utes
-            df["Nome UTE"] = nome_utes
-            df["Lag"] = lag_utes
-            df = df[["Código UTE", "Nome UTE", "Lag"] + cols]
+            df["codigo_usina"] = codigo_utes
+            df["nome_usina"] = nome_utes
+            df["lag"] = lag_utes
+            df = df[["codigo_usina", "nome_usina", "lag"] + cols]
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
 
         # Obtem o número de patamares e constroi a linha de despachos
@@ -100,22 +100,24 @@
     def write(self, file: IO, *args, **kwargs):
         for linha in self.__cabecalhos:
             file.write(linha)
         if not isinstance(self.data, pd.DataFrame):
             raise ValueError("Dados do adterm.dat não foram lidos com sucesso")
 
         ultima_ute = 0
-        cols_despachos = [c for c in list(self.data.columns) if "Patamar" in c]
+        cols_despachos = [c for c in list(self.data.columns) if "patamar" in c]
         for _, linha in self.data.iterrows():
             linha_lida: pd.Series = linha
-            if linha_lida["Código UTE"] != ultima_ute:
-                ultima_ute = linha_lida["Código UTE"]
+            if linha_lida["codigo_usina"] != ultima_ute:
+                ultima_ute = linha_lida["codigo_usina"]
                 file.write(
                     self.__linha_ute.write(
-                        linha_lida[["Código UTE", "Nome UTE", "Lag"]].tolist()
+                        linha_lida[
+                            ["codigo_usina", "nome_usina", "lag"]
+                        ].tolist()
                     )
                 )
             file.write(
                 self.__linha_despachos.write(
                     linha_lida[cols_despachos].tolist()
                 )
             )
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/agrint.py` & `inewave-0.0.98/inewave/newave/modelos/agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/arquivos.py` & `inewave-0.0.98/inewave/newave/modelos/arquivos.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            df = pd.DataFrame(data={"Legenda": legendas, "Nome": nomes})
+            df = pd.DataFrame(data={"legenda": legendas, "nome": nomes})
             return df
 
         legendas: List[str] = []
         nomes: List[str] = []
         while True:
             linha = file.readline()
             if len(linha) < 3:
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/arquivoscsv/arquivocsv.py` & `inewave-0.0.98/inewave/newave/modelos/arquivoscsv/arquivocsv.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,51 +21,31 @@
     """
 
     BLOCKS: List[Type[Block]] = [VersaoModelo]
     ENCODING = "iso-8859-1"
 
     T = TypeVar("T")
 
-    def _bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def versao(self) -> Optional[str]:
         """
         A versão do modelo utilizada para executar o caso.
 
         :return: A versão do modelo
         :rtype: str | None
         """
-        b = self._bloco_por_tipo(VersaoModelo, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(VersaoModelo)
+        if isinstance(b, VersaoModelo):
             return b.data
         return None
 
     def _tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
         :return: A tabela como um dataframe
         :rtype: pd.DataFrame | None
         """
-        b = self._bloco_por_tipo(TabelaCSV, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(TabelaCSV)
+        if isinstance(b, TabelaCSV):
             return b.data
         return None
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/avl_cortesfpha_nwv.py` & `inewave-0.0.98/inewave/newave/modelos/avl_cortesfpha_nwv.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             FloatField(size=16, decimal_digits=8),
             FloatField(size=16, decimal_digits=8),
             FloatField(size=16, decimal_digits=8),
         ],
         delimiter=";",
     )
     COLUMN_NAMES = [
-        "indice_usina",
+        "codigo_usina",
         "periodo",
         "nome_usina",
         "indice_corte",
         "fator_correcao",
         "rhs_energia",
         "coeficiente_volume_util_MW_hm3",
         "coeficiente_vazao_turbinada_MW_m3s",
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/avl_desvfpha_s.py` & `inewave-0.0.98/inewave/newave/modelos/avl_desvfpha_s.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Bloco com os desvios da função de produção no plano de
     vazão vertida (S).
     """
 
     BEGIN_PATTERN = "-----;--------------;--------;"
 
     COLUMN_NAMES = [
-        "indice_usina",
+        "codigo_usina",
         "nome_usina",
         "volume_armazenado_percentual",
         "vazao_turbinada_m3s",
         "vazao_vertida_m3s",
         "desvio_percentual",
     ]
     END_PATTERN = ""
@@ -30,15 +30,15 @@
         return pd.DataFrame(data=dados, columns=self.__class__.COLUMN_NAMES)
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, TabelaAvlDesvFphaS):
             return False
         else:
             if not all(
-                [type(self.data) == pd.DataFrame, type(o.data) == pd.DataFrame]
+                [type(self.data) is pd.DataFrame, type(o.data) is pd.DataFrame]
             ):
                 return False
             else:
                 return self.data.equals(o.data)
 
     def read(self, file: IO, *args, **kwargs):
         # Espera o fim do cabeçalho
@@ -74,15 +74,15 @@
         dados: Dict[str, List] = {c: [] for c in self.__class__.COLUMN_NAMES}
         while True:
             linha = file.readline()
             if len(linha) < 3 or "-----;--------------;------;" in linha:
                 self.data = self._monta_df(dados)
                 return
             dados_linha = self.__linha.read(linha)
-            dados["indice_usina"] += [dados_linha[0]] * num_valores_vert
+            dados["codigo_usina"] += [dados_linha[0]] * num_valores_vert
             dados["nome_usina"] += [dados_linha[1]] * num_valores_vert
             dados["volume_armazenado_percentual"] += [
                 dados_linha[2]
             ] * num_valores_vert
             dados["vazao_turbinada_m3s"] += [dados_linha[3]] * num_valores_vert
             dados["vazao_vertida_m3s"] += valores_vert
             dados["desvio_percentual"] += dados_linha[4:]
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/avl_desvfpha_v_q.py` & `inewave-0.0.98/inewave/newave/modelos/avl_desvfpha_v_q.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Bloco com os desvios da função de produção nos planos de
     volume armazenado e vazão turbinada (V-Q).
     """
 
     BEGIN_PATTERN = "-----;--------------;------;"
 
     COLUMN_NAMES = [
-        "indice_usina",
+        "codigo_usina",
         "nome_usina",
         "volume_armazenado_percentual",
         "vazao_turbinada_m3s",
         "desvio_percentual",
     ]
     END_PATTERN = ""
 
@@ -29,15 +29,15 @@
         return pd.DataFrame(data=dados, columns=self.__class__.COLUMN_NAMES)
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, TabelaAvlDesvFphaVQ):
             return False
         else:
             if not all(
-                [type(self.data) == pd.DataFrame, type(o.data) == pd.DataFrame]
+                [type(self.data) is pd.DataFrame, type(o.data) is pd.DataFrame]
             ):
                 return False
             else:
                 return self.data.equals(o.data)
 
     def read(self, file: IO, *args, **kwargs):
         # Espera o fim do cabeçalho
@@ -73,14 +73,14 @@
         dados: Dict[str, List] = {c: [] for c in self.__class__.COLUMN_NAMES}
         while True:
             linha = file.readline()
             if len(linha) < 3 or "-----;--------------;------;" in linha:
                 self.data = self._monta_df(dados)
                 return
             dados_linha = self.__linha.read(linha)
-            dados["indice_usina"] += [dados_linha[0]] * num_valores_turb
+            dados["codigo_usina"] += [dados_linha[0]] * num_valores_turb
             dados["nome_usina"] += [dados_linha[1]] * num_valores_turb
             dados["volume_armazenado_percentual"] += [
                 dados_linha[3]
             ] * num_valores_turb
             dados["vazao_turbinada_m3s"] += valores_turb
             dados["desvio_percentual"] += dados_linha[4:]
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/blocos/tabelacsv.py` & `inewave-0.0.98/inewave/newave/modelos/blocos/tabelacsv.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return pd.DataFrame(data=dados, columns=self.__class__.COLUMN_NAMES)
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, TabelaCSV):
             return False
         else:
             if not all(
-                [type(self.data) == pd.DataFrame, type(o.data) == pd.DataFrame]
+                [type(self.data) is pd.DataFrame, type(o.data) is pd.DataFrame]
             ):
                 return False
             else:
                 return self.data.equals(o.data)
 
     def read(self, file: IO, *args, **kwargs):
         if len(self.__class__.LINE_MODEL.fields) != len(
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/cadic.py` & `inewave-0.0.98/inewave/newave/modelos/cadic.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,20 +49,20 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
-            df["Código Subsistema"] = codigo_subsis
-            df["Nome Subsistema"] = nome_subsis
-            df["Razão"] = razao
-            df["Ano"] = anos
+            df["codigo_subsistema"] = codigo_subsis
+            df["nome_subsistema"] = nome_subsis
+            df["comentario"] = razao
+            df["ano"] = anos
             df = df[
-                ["Código Subsistema", "Nome Subsistema", "Razão", "Ano"]
+                ["codigo_subsistema", "nome_subsistema", "comentario", "ano"]
                 + MESES_DF
             ]
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
@@ -111,32 +111,32 @@
         if not isinstance(self.data, pd.DataFrame):
             raise ValueError("Dados do c_adic.dat não foram lidos com sucesso")
 
         for _, linha in self.data.iterrows():
             linha_lida: pd.Series = linha
             if any(
                 [
-                    linha_lida["Código Subsistema"] != ultimo_codigo,
-                    linha_lida["Nome Subsistema"] != ultimo_subsis,
-                    linha_lida["Razão"] != ultima_razao,
+                    linha_lida["codigo_subsistema"] != ultimo_codigo,
+                    linha_lida["nome_subsistema"] != ultimo_subsis,
+                    linha_lida["comentario"] != ultima_razao,
                 ]
             ):
-                ultimo_codigo = linha_lida["Código Subsistema"]
-                ultimo_subsis = linha_lida["Nome Subsistema"]
-                ultima_razao = linha_lida["Razão"]
+                ultimo_codigo = linha_lida["codigo_subsistema"]
+                ultimo_subsis = linha_lida["nome_subsistema"]
+                ultima_razao = linha_lida["comentario"]
                 file.write(
                     self.__linha_subsis.write(
                         linha_lida[
                             [
-                                "Código Subsistema",
-                                "Nome Subsistema",
-                                "Razão",
+                                "codigo_subsistema",
+                                "nome_subsistema",
+                                "comentario",
                             ]
                         ].tolist()
                     )
                 )
-            linha_saida = linha_lida[["Ano"] + MESES_DF]
+            linha_saida = linha_lida[["ano"] + MESES_DF]
             valores_saida = []
             for valor, vazio in zip(linha_saida, linha_saida.isna()):
                 valores_saida.append(None if vazio else valor)
             file.write(self.__linha_cargas.write(valores_saida))
         file.write(BlocoCargasAdicionais.FIM_BLOCO)
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/caso.py` & `inewave-0.0.98/inewave/newave/modelos/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/clast.py` & `inewave-0.0.98/inewave/newave/modelos/clast.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,28 +45,28 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            cols = [f"Custo {i}" for i in range(1, 6)]
+            cols = [f"custo_{i}" for i in range(1, 6)]
             df = pd.DataFrame(tabela, columns=cols)
-            df["Número"] = numero_ute
-            df["Nome"] = nome_ute
-            df["Tipo Combustível"] = tipo_combustivel
-            df = df[["Número", "Nome", "Tipo Combustível"] + cols]
+            df["codigo"] = codigo_ute
+            df["nome"] = nome_ute
+            df["tipo_combustivel"] = tipo_combustivel
+            df = df[["codigo", "nome", "tipo_combustivel"] + cols]
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
 
         # Variáveis auxiliares
-        numero_ute: List[int] = []
+        codigo_ute: List[int] = []
         nome_ute: List[str] = []
         tipo_combustivel: List[str] = []
         tabela = np.zeros((MAX_UTES, 5))
         i = 0
         while True:
             linha = file.readline()
             # Confere se acabou
@@ -74,15 +74,15 @@
                 break
             if BlocoUTEClasT.FIM_BLOCO in linha:
                 tabela = tabela[:i, :]
                 self.data = converte_tabela_em_df()
                 break
             dados = self.__linha.read(linha)
             tabela[i, :] = dados[3:]
-            numero_ute.append(dados[0])
+            codigo_ute.append(dados[0])
             nome_ute.append(dados[1])
             tipo_combustivel.append(dados[2])
             i += 1
 
     # Override
     def write(self, file: IO, *args, **kwargs):
         for linha in self.__cabecalhos:
@@ -131,46 +131,46 @@
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(
                 data={
-                    "Número": numero_ute,
-                    "Custo": custo,
-                    "Mês Início": mes_ini,
-                    "Ano Início": ano_ini,
-                    "Mês Fim": mes_fim,
-                    "Ano Fim": ano_fim,
-                    "Nome": nomes,
+                    "codigo": codigo_ute,
+                    "custo": custo,
+                    "mes_inicio": mes_ini,
+                    "ano_inicio": ano_ini,
+                    "mes_fim": mes_fim,
+                    "ano_fim": ano_fim,
+                    "nome": nomes,
                 }
             )
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
 
         # Variáveis auxiliares
-        numero_ute: List[int] = []
+        codigo_ute: List[int] = []
         custo: List[float] = []
         mes_ini: List[int] = []
         ano_ini: List[int] = []
         mes_fim: List[int] = []
         ano_fim: List[int] = []
         nomes: List[str] = []
         while True:
             linha = file.readline()
             # Confere se acabou
             if len(linha) < 3:
-                if len(numero_ute) > 0:
+                if len(codigo_ute) > 0:
                     self.data = converte_tabela_em_df()
                 break
             dados = self.__linha.read(linha)
-            numero_ute.append(dados[0])
+            codigo_ute.append(dados[0])
             custo.append(dados[1])
             mes_ini.append(dados[2])
             ano_ini.append(dados[3])
             mes_fim.append(dados[4])
             ano_fim.append(dados[5])
             nomes.append(dados[6])
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/confhd.py` & `inewave-0.0.98/inewave/newave/modelos/confhd.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,24 +59,24 @@
             col_ree = extrai_coluna_de_listas(dados_uhes, 4)
             col_vinic = extrai_coluna_de_listas(dados_uhes, 5)
             col_exis = extrai_coluna_de_listas(dados_uhes, 6)
             col_modif = extrai_coluna_de_listas(dados_uhes, 7)
             col_inic_hist = extrai_coluna_de_listas(dados_uhes, 8)
             col_fim_hist = extrai_coluna_de_listas(dados_uhes, 9)
             dados = {
-                "Número": col_num,
-                "Nome": col_nome,
-                "Posto": col_posto,
-                "Jusante": col_jus,
-                "REE": col_ree,
-                "Volume Inicial": col_vinic,
-                "Usina Existente": col_exis,
-                "Modificada": col_modif,
-                "Início do Histórico": col_inic_hist,
-                "Fim do Histórico": col_fim_hist,
+                "codigo_usina": col_num,
+                "nome_usina": col_nome,
+                "posto": col_posto,
+                "codigo_usina_jusante": col_jus,
+                "ree": col_ree,
+                "volume_inicial_percentual": col_vinic,
+                "usina_existente": col_exis,
+                "usina_modificada": col_modif,
+                "ano_inicio_historico": col_inic_hist,
+                "ano_fim_historico": col_fim_hist,
             }
             return pd.DataFrame(data=dados)
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/conft.py` & `inewave-0.0.98/inewave/newave/modelos/conft.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,19 +48,19 @@
             # Converte as informações de cada linha em colunas
             col_num = extrai_coluna_de_listas(dados_utes, 0)
             col_nome = extrai_coluna_de_listas(dados_utes, 1)
             col_subsis = extrai_coluna_de_listas(dados_utes, 2)
             col_exis = extrai_coluna_de_listas(dados_utes, 3)
             col_clas = extrai_coluna_de_listas(dados_utes, 4)
             dados = {
-                "Número": col_num,
-                "Nome": col_nome,
-                "Subsistema": col_subsis,
-                "Usina Existente": col_exis,
-                "Classe": col_clas,
+                "codigo_usina": col_num,
+                "nome_usina": col_nome,
+                "submercado": col_subsis,
+                "usina_existente": col_exis,
+                "classe": col_clas,
             }
             return pd.DataFrame(data=dados)
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/cortes.py` & `inewave-0.0.98/inewave/newave/modelos/cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/cortesh.py` & `inewave-0.0.98/inewave/newave/modelos/cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/curva.py` & `inewave-0.0.98/inewave/newave/modelos/curva.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from typing import List, IO
 import pandas as pd  # type: ignore
 import numpy as np  # type: ignore
 
 
 class BlocoConfiguracoesPenalizacaoCurva(Section):
     """
-    Bloco de informações das usinas cadastradas
-    no arquivo do NEWAVE `conft.dat`.
+    Bloco com as configurações de penalização da curva de aversão,
+    existente no arquivo do NEWAVE `curva.dat`.
     """
 
     def __init__(self, previous=None, next=None, data=None) -> None:
         super().__init__(previous, next, data)
         self.__linha = Line(
             [
                 IntegerField(3, 1),
@@ -88,16 +88,16 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            df = pd.DataFrame(tabela, columns=["Sistema", "Custo"])
-            df = df.astype({"Sistema": "int64"})
+            df = pd.DataFrame(tabela, columns=["ree", "penalidade"])
+            df = df.astype({"ree": "int64"})
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
 
         i = 0
@@ -122,23 +122,23 @@
         for linha in self.__cabecalhos:
             file.write(linha)
         if not isinstance(self.data, pd.DataFrame):
             raise ValueError("Dados do curva.dat não foram lidos com sucesso")
 
         for _, lin in self.data.iterrows():
             file.write(
-                self.__linha.write([int(lin["Sistema"])] + [lin["Custo"]])
+                self.__linha.write([int(lin["ree"])] + [lin["penalidade"]])
             )
         file.write(BlocoPenalidadesViolacaoREECurva.FIM_BLOCO + "\n")
 
 
-class BlocoCurvaSegurancaSubsistema(Section):
+class BlocoCurvaSegurancaREE(Section):
     """
     Bloco com informações da curva de segurança de operação por mês/ano
-    e por subsistema.
+    e por REE.
     """
 
     FIM_BLOCO = "9999"
 
     def __init__(self, previous=None, next=None, data=None) -> None:
         super().__init__(previous, next, data)
         self.__linha_subsis = Line([IntegerField(3, 1)])
@@ -146,50 +146,47 @@
         campos_curva: List[Field] = [
             FloatField(5, i * 6 + 6, 1) for i in range(len(MESES_DF))
         ]
         self.__linha = Line(campo_ano + campos_curva)
         self.__cabecalhos: List[str] = []
 
     def __eq__(self, o: object) -> bool:
-        if not isinstance(o, BlocoCurvaSegurancaSubsistema):
+        if not isinstance(o, BlocoCurvaSegurancaREE):
             return False
-        bloco: BlocoCurvaSegurancaSubsistema = o
+        bloco: BlocoCurvaSegurancaREE = o
         if not all(
             [
                 isinstance(self.data, pd.DataFrame),
                 isinstance(o.data, pd.DataFrame),
             ]
         ):
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            df = pd.DataFrame(tabela, columns=["REE", "Ano"] + MESES_DF)
-            df = df.astype({"REE": "int64", "Ano": "int64"})
+            df = pd.DataFrame(tabela, columns=["ree", "ano"] + MESES_DF)
+            df = df.astype({"ree": "int64", "ano": "int64"})
             return df
 
         # Salta as linhas adicionais
         for _ in range(3):
             self.__cabecalhos.append(file.readline())
 
         i = 0
         subsis_atual = 0
         tabela = np.zeros(
             (MAX_SUBMERCADOS * MAX_ANOS_ESTUDO, len(MESES_DF) + 2)
         )
         while True:
             linha = file.readline()
             # Confere se terminaram
-            if (
-                len(linha) < 3
-                or BlocoCurvaSegurancaSubsistema.FIM_BLOCO in linha
-            ):
+            if len(linha) < 3 or BlocoCurvaSegurancaREE.FIM_BLOCO in linha:
                 # Converte para df e salva na variável
                 if i > 0:
                     tabela = tabela[:i, :]
                     self.data = converte_tabela_em_df()
                 break
             # Confere se é uma linha de subsistema ou tabela
             if len(linha) < 10:
@@ -205,24 +202,24 @@
             file.write(linha)
         if not isinstance(self.data, pd.DataFrame):
             raise ValueError("Dados do curva.dat não foram lidos com sucesso")
 
         ultimo_ree = 0
         for _, linha in self.data.iterrows():
             linha_lida: pd.Series = linha
-            if linha_lida["REE"] != ultimo_ree:
-                ultimo_ree = linha_lida["REE"]
+            if linha_lida["ree"] != ultimo_ree:
+                ultimo_ree = linha_lida["ree"]
                 file.write(self.__linha_subsis.write([int(ultimo_ree)]))
             file.write(
                 self.__linha.write(
-                    [int(linha_lida["Ano"])] + linha_lida[MESES_DF].tolist()
+                    [int(linha_lida["ano"])] + linha_lida[MESES_DF].tolist()
                 )
             )
 
-        file.write(BlocoCurvaSegurancaSubsistema.FIM_BLOCO + "\n")
+        file.write(BlocoCurvaSegurancaREE.FIM_BLOCO + "\n")
 
 
 class BlocoMaximoIteracoesProcessoIterativoEtapa2(Section):
     """
     Bloco com informações do número máximo de iterações da
     segunda etapa do processo iterativo no cálculo da curva de aversão.
     """
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/cvar.py` & `inewave-0.0.98/inewave/newave/modelos/cvar.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,17 +89,17 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
-            df["Ano"] = anos
+            df["ano"] = anos
             df = df
-            df = df[["Ano"] + MESES_DF]
+            df = df[["ano"] + MESES_DF]
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
 
         i = 0
@@ -164,17 +164,17 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
-            df["Ano"] = anos
+            df["ano"] = anos
             df = df
-            df = df[["Ano"] + MESES_DF]
+            df = df[["ano"] + MESES_DF]
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
 
         i = 0
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/dger.py` & `inewave-0.0.98/inewave/newave/modelos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/dsvagua.py` & `inewave-0.0.98/inewave/newave/modelos/dsvagua.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,21 +47,31 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df() -> pd.DataFrame:
-            cols = ["Ano", "Usina"] + MESES_DF + ["Flag"]
+            cols = (
+                ["ano", "codigo_usina"]
+                + MESES_DF
+                + ["considera_desvio_usina_NC"]
+            )
             df = pd.DataFrame(
                 tabela,
                 columns=cols,
             )
             df["Comentário"] = comentarios
-            df = df.astype({"Ano": "int64", "Usina": "int64", "Flag": "int64"})
+            df = df.astype(
+                {
+                    "ano": "int64",
+                    "codigo_usina": "int64",
+                    "considera_desvio_usina_NC": "int64",
+                }
+            )
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
 
         i = 0
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/eafpast.py` & `inewave-0.0.98/inewave/newave/modelos/eafpast.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,22 +38,22 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df() -> pd.DataFrame:
-            cols = ["Índice"] + MESES_DF
+            cols = ["codigo_ree"] + MESES_DF
             df = pd.DataFrame(
                 tabela,
                 columns=cols,
             )
-            df["REE"] = rees
-            df = df.astype({"Índice": "int64"})
-            df = df[["Índice", "REE"] + MESES_DF]
+            df["nome_ree"] = rees
+            df = df.astype({"codigo_ree": "int64"})
+            df = df[["codigo_ree", "nome_ree"] + MESES_DF]
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
 
         i = 0
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/enavazb.py` & `inewave-0.0.98/inewave/newave/modelos/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/enavazf.py` & `inewave-0.0.98/inewave/newave/modelos/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/energiab.py` & `inewave-0.0.98/inewave/newave/modelos/energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/energiaf.py` & `inewave-0.0.98/inewave/newave/modelos/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/energias.py` & `inewave-0.0.98/inewave/newave/modelos/energias.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/engnat.py` & `inewave-0.0.98/inewave/newave/modelos/engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/eolicacadastro.py` & `inewave-0.0.98/inewave/newave/modelos/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/eolicaconfiguracao.py` & `inewave-0.0.98/inewave/newave/modelos/eolicaconfiguracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/eolicafte.py` & `inewave-0.0.98/inewave/newave/modelos/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/eolicageracao.py` & `inewave-0.0.98/inewave/newave/modelos/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/eolicahistorico.py` & `inewave-0.0.98/inewave/newave/modelos/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/eolicaposto.py` & `inewave-0.0.98/inewave/newave/modelos/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/eolicasubmercado.py` & `inewave-0.0.98/inewave/newave/modelos/eolicasubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/exph.py` & `inewave-0.0.98/inewave/newave/modelos/exph.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,23 +47,23 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame()
-            df["Código UHE"] = codigo_uhes
-            df["Nome UHE"] = nome_uhes
-            df["Início Enchimento"] = inicio_enchimento
-            df["Duração"] = duracao
-            df["Volume Morto"] = volume_morto
-            df["Data de Entrada"] = data_entrada
-            df["Potência"] = potencia
-            df["Máquina"] = maquina
-            df["Conjunto"] = conjunto
+            df["codigo_usina"] = codigo_uhes
+            df["nome_usina"] = nome_uhes
+            df["data_inicio_enchimento"] = inicio_enchimento
+            df["duracao_enchimento"] = duracao
+            df["volume_morto"] = volume_morto
+            df["data_entrada_operacao"] = data_entrada
+            df["potencia_instalada"] = potencia
+            df["maquina_entrada"] = maquina
+            df["conjunto_maquina_entrada"] = conjunto
             return df
 
         # Salta as linhas adicionais
         for _ in range(3):
             self.__cabecalhos.append(file.readline())
 
         # Variáveis auxiliares
@@ -129,17 +129,17 @@
             file.write(linha)
         if not isinstance(self.data, pd.DataFrame):
             raise ValueError("Dados do exph.dat não foram lidos com sucesso")
 
         ultima_uhe = 0
         for _, linha in self.data.iterrows():
             linha_lida: pd.Series = linha
-            if linha_lida["Código UHE"] != ultima_uhe and ultima_uhe != 0:
+            if linha_lida["codigo_usina"] != ultima_uhe and ultima_uhe != 0:
                 file.write(f"{BlocoUHEExph.FIM_BLOCO}\n")
-            ultima_uhe = int(linha_lida["Código UHE"])
+            ultima_uhe = int(linha_lida["codigo_usina"])
             dados_linha = linha_lida.tolist()
             # Corrige posições opcionais
             for i in [3, -1, -2]:
                 dados_linha[i] = (
                     int(dados_linha[i])
                     if not pd.isnull(dados_linha[i])
                     else None
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/expt.py` & `inewave-0.0.98/inewave/newave/modelos/expt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/forward.py` & `inewave-0.0.98/inewave/newave/modelos/forward.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/forwarh.py` & `inewave-0.0.98/inewave/newave/modelos/forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/ghmin.py` & `inewave-0.0.98/inewave/newave/modelos/ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/hidr.py` & `inewave-0.0.98/inewave/newave/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/manutt.py` & `inewave-0.0.98/inewave/newave/modelos/manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/modif.py` & `inewave-0.0.98/inewave/newave/modelos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/newavetim.py` & `inewave-0.0.98/inewave/newave/modelos/newavetim.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df() -> pd.DataFrame:
-            df = pd.DataFrame(data={"Etapa": etapas, "Tempo": tempos})
+            df = pd.DataFrame(data={"etapa": etapas, "tempo": tempos})
             return df
 
         # Variáveis auxiliares
         etapas: List[str] = []
         tempos: List[timedelta] = []
 
         # Leitura das etapas
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/nwv_avl_evap.py` & `inewave-0.0.98/inewave/newave/modelos/nwv_avl_evap.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             FloatField(size=10, decimal_digits=3),
             FloatField(size=10, decimal_digits=2),
         ],
         delimiter=";",
     )
     COLUMN_NAMES = [
         "periodo",
-        "indice_usina",
+        "codigo_usina",
         "nome_usina",
         "volume_armazenado_hm3",
         "evaporacao_calculada_hm3",
         "evaporacao_modelo_hm3",
         "desvio_absoluto_hm3",
         "desvio_percentual",
     ]
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/nwv_cortes_evap.py` & `inewave-0.0.98/inewave/newave/modelos/nwv_cortes_evap.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             FloatField(size=17, decimal_digits=10),
             FloatField(size=12, decimal_digits=14),
         ],
         delimiter=";",
     )
     COLUMN_NAMES = [
         "periodo",
-        "indice_usina",
+        "codigo_usina",
         "nome_usina",
         "derivada_cota_area",
         "derivada_volume_cota",
         "volume_referencia_hm3",
         "evaporacao_referencia_hm3",
         "coeficiente_volume",
         "rhs_volume",
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/nwv_eco_evap.py` & `inewave-0.0.98/inewave/newave/modelos/nwv_eco_evap.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             IntegerField(size=11),
             IntegerField(size=15),
         ],
         delimiter=";",
     )
     COLUMN_NAMES = [
         "periodo",
-        "indice_usina",
+        "codigo_usina",
         "nome_usina",
         "volume_referencia_hm3",
         "evaporacao_referencia_hm3",
         "coeficiente_evaporacao_mm_mes",
         "flag_evaporacao",
         "evaporacao_linear",
         "tipo_volume_referencia",
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/parp.py` & `inewave-0.0.98/inewave/newave/modelos/parp.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,19 +54,19 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            df = pd.DataFrame(tabela, columns=["Ano"] + MESES_DF)
-            df["REE"] = ree
-            df["Configuração"] = cfg
-            df = df[["REE", "Configuração", "Ano"] + MESES_DF]
-            df = df.astype({"Ano": "int64"})
+            df = pd.DataFrame(tabela, columns=["ano"] + MESES_DF)
+            df["ree"] = ree
+            df["configuracao"] = cfg
+            df = df[["ree", "configuracao", "ano"] + MESES_DF]
+            df = df.astype({"ano": "int64"})
             return df
 
         # Identifica o REE e a configuração
         linha = file.readline()
         ree = self.__campo_ree.read(linha)
         cfg = self.__campo_cfg.read(linha)
 
@@ -147,23 +147,23 @@
                 anos[idx_i:idx_f] = [str(ano)] * 12
             return [int(a) for a in anos]
 
         def converte_vetor_meses(meses: List[str]) -> List[int]:
             return [MESES_ABREV.index(m) + 1 for m in meses]
 
         def converte_tabela_em_df():
-            cols = [f"Lag {i}" for i in range(1, 12)]
+            cols = [f"lag_{i}" for i in range(1, 12)]
             df = pd.DataFrame(tabela, columns=cols)
             anos_conv = converte_vetor_anos(anos)
             meses_conv = converte_vetor_meses(meses)
-            df["Data"] = [
+            df["data"] = [
                 date(year=a, month=m, day=1)
                 for a, m in zip(anos_conv, meses_conv)
             ]
-            df = df[["Data"] + cols]
+            df = df[["data"] + cols]
             return df
 
         # Salta as linhas adicionais
         for _ in range(5):
             file.readline()
 
         # Variáveis auxiliares
@@ -244,23 +244,23 @@
                 anos[idx_i:idx_f] = [str(ano)] * 12
             return [int(a) for a in anos]
 
         def converte_vetor_meses(meses: List[str]) -> List[int]:
             return [MESES_ABREV.index(m) + 1 for m in meses]
 
         def converte_tabela_em_df():
-            cols = [f"Lag {i}" for i in range(1, 12)]
+            cols = [f"lag_{i}" for i in range(1, 12)]
             df = pd.DataFrame(tabela, columns=cols)
             anos_conv = converte_vetor_anos(anos)
             meses_conv = converte_vetor_meses(meses)
-            df["Data"] = [
+            df["data"] = [
                 date(year=a, month=m, day=1)
                 for a, m in zip(anos_conv, meses_conv)
             ]
-            df = df[["Data"] + cols]
+            df = df[["data"] + cols]
             return df
 
         # Salta as linhas adicionais
         for _ in range(3):
             file.readline()
 
         # Variáveis auxiliares
@@ -336,17 +336,17 @@
                 idx = indice_inicio_pos + a
                 ano = ultimo_ano_estudo + a + 1
                 anos[idx] = str(ano)
             return [int(a) for a in anos]
 
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
-            df["Tipo"] = self.__tipo
-            df["Ano"] = converte_vetor_anos(anos)
-            df = df[["Tipo", "Ano"] + MESES_DF]
+            df["tipo"] = self.__tipo
+            df["ano"] = converte_vetor_anos(anos)
+            df = df[["tipo", "ano"] + MESES_DF]
             return df
 
         # Salta as linhas adicionais
         linha = file.readline()
         self.__tipo = linha.split("ORDEM")[1].split("DO MODELO")[0].strip()
         for _ in range(3):
             file.readline()
@@ -398,18 +398,18 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             cols = (
-                [f"Psi {i}" for i in range(1, len(MESES_DF))]
-                + ["Psi A"]
-                + [f"Psi Norm {i}" for i in range(1, len(MESES_DF))]
-                + ["Psi Norm A"]
+                [f"psi_{i}" for i in range(1, len(MESES_DF))]
+                + ["psi_A"]
+                + [f"psi_norm_{i}" for i in range(1, len(MESES_DF))]
+                + ["psi_norm_A"]
             )
             return pd.DataFrame(tabela, columns=cols)
 
         linha = file.readline()
 
         tabela = np.zeros((1, 2 * len(MESES_DF)))
         # Processa os dados
@@ -461,17 +461,17 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
-            df["Ano"] = ano
-            df["Série"] = list(range(i))
-            df = df[["Ano", "Série"] + MESES_DF]
+            df["ano"] = ano
+            df["serie"] = list(range(i))
+            df = df[["ano", "serie"] + MESES_DF]
             return df
 
         # Identifica o ano em questão
         linha = file.readline()
         ano = self.__campo_ano.read(linha)
 
         # Salta as linhas adicionais
@@ -551,23 +551,23 @@
                 anos[idx_i:idx_f] = [str(ano)] * 12
             return [int(a) for a in anos]
 
         def converte_vetor_meses(meses: List[str]) -> List[int]:
             return [MESES_ABREV.index(m) + 1 for m in meses]
 
         def converte_tabela_em_df():
-            cols = [f"Lag {i}" for i in range(1, 12)]
+            cols = [f"lag_{i}" for i in range(1, 12)]
             df = pd.DataFrame(tabela, columns=cols)
             anos_conv = converte_vetor_anos(anos)
             meses_conv = converte_vetor_meses(meses)
-            df["Data"] = [
+            df["data"] = [
                 date(year=a, month=m, day=1)
                 for a, m in zip(anos_conv, meses_conv)
             ]
-            df = df[["Data"] + cols]
+            df = df[["data"] + cols]
             return df
 
         # Salta as linhas adicionais
         for _ in range(4):
             file.readline()
 
         # Variáveis auxiliares
@@ -622,17 +622,17 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
-            df["Ano"] = ano
-            df["Série"] = list(range(i))
-            df = df[["Ano", "Série"] + MESES_DF]
+            df["ano"] = ano
+            df["serie"] = list(range(i))
+            df = df[["ano", "serie"] + MESES_DF]
             return df
 
         # Identifica o ano em questão
         linha = file.readline()
         ano = self.__campo_ano.read(linha)
 
         # Salta as linhas adicionais
@@ -715,19 +715,19 @@
         def converte_vetor_meses(meses: List[str]) -> List[int]:
             return [MESES_ABREV.index(m) + 1 for m in meses]
 
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
             anos_conv = converte_vetor_anos(anos)
             meses_conv = converte_vetor_meses(meses)
-            df["Data"] = [
+            df["data"] = [
                 date(year=a, month=m, day=1)
                 for a, m in zip(anos_conv, meses_conv)
             ]
-            df = df[["Data"] + MESES_DF]
+            df = df[["data"] + MESES_DF]
             return df
 
         # Salta as linhas adicionais
         for _ in range(5):
             file.readline()
 
         # Variáveis auxiliares
@@ -778,17 +778,17 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=rees)
-            df["REE"] = rees
-            df["Configuração"] = cfg
-            df = df[["Configuração", "REE"] + rees]
+            df["ree"] = rees
+            df["configuracao"] = cfg
+            df = df[["configuracao", "ree"] + rees]
             return df
 
         # Identifica a configuração
         linha = file.readline()
         cfg = self.__campo_cfg.read(linha)
 
         file.readline()
@@ -842,18 +842,19 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=rees)
-            df["REE"] = valores_rees
-            df["Configuração"] = cfg
-            df = df[["Configuração", "REE"] + rees]
-            df = df.astype({"MES": "int64"})
+            df["ree"] = valores_rees
+            df["configuracao"] = cfg
+            df = df[["configuracao", "ree"] + rees]
+            df = df.rename(columns={"MES": "mes"})
+            df = df.astype({"mes": "int64"})
             return df
 
         # Identifica a configuração
         linha = file.readline()
         cfg = self.__campo_cfg.read(linha)
 
         file.readline()
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/parpeol.py` & `inewave-0.0.98/inewave/newave/modelos/parpeol.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,19 +54,19 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            df = pd.DataFrame(tabela, columns=["Ano"] + MESES_DF)
-            df["UEE"] = uee
-            df["Configuração"] = cfg
-            df = df[["UEE", "Configuração", "Ano"] + MESES_DF]
-            df = df.astype({"Ano": "int64"})
+            df = pd.DataFrame(tabela, columns=["ano"] + MESES_DF)
+            df["uee"] = uee
+            df["configuracao"] = cfg
+            df = df[["uee", "configuracao", "ano"] + MESES_DF]
+            df = df.astype({"ano": "int64"})
             return df
 
         # Identifica a usina e a configuração
         linha = file.readline()
         uee = self.__campo_uee.read(linha)
         cfg = self.__campo_cfg.read(linha)
 
@@ -147,23 +147,23 @@
                 anos[idx_i:idx_f] = [str(ano)] * 12
             return [int(a) for a in anos]
 
         def converte_vetor_meses(meses: List[str]) -> List[int]:
             return [MESES_ABREV.index(m) + 1 for m in meses]
 
         def converte_tabela_em_df():
-            cols = [f"Lag {i}" for i in range(1, 12)]
+            cols = [f"lag_{i}" for i in range(1, 12)]
             df = pd.DataFrame(tabela, columns=cols)
             anos_conv = converte_vetor_anos(anos)
             meses_conv = converte_vetor_meses(meses)
-            df["Data"] = [
+            df["data"] = [
                 date(year=a, month=m, day=1)
                 for a, m in zip(anos_conv, meses_conv)
             ]
-            df = df[["Data"] + cols]
+            df = df[["data"] + cols]
             return df
 
         # Salta as linhas adicionais
         for _ in range(5):
             file.readline()
 
         # Variáveis auxiliares
@@ -218,17 +218,17 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
-            df["Ano"] = ano
-            df["Série"] = list(range(i))
-            df = df[["Ano", "Série"] + MESES_DF]
+            df["ano"] = ano
+            df["serie"] = list(range(i))
+            df = df[["ano", "serie"] + MESES_DF]
             return df
 
         # Identifica o ano em questão
         linha = file.readline()
         ano = self.__campo_ano.read(linha)
 
         # Salta as linhas adicionais
@@ -308,23 +308,23 @@
                 anos[idx_i:idx_f] = [str(ano)] * 12
             return [int(a) for a in anos]
 
         def converte_vetor_meses(meses: List[str]) -> List[int]:
             return [MESES_ABREV.index(m) + 1 for m in meses]
 
         def converte_tabela_em_df():
-            cols = [f"Lag {i}" for i in range(1, 12)]
+            cols = [f"lag_{i}" for i in range(1, 12)]
             df = pd.DataFrame(tabela, columns=cols)
             anos_conv = converte_vetor_anos(anos)
             meses_conv = converte_vetor_meses(meses)
-            df["Data"] = [
+            df["data"] = [
                 date(year=a, month=m, day=1)
                 for a, m in zip(anos_conv, meses_conv)
             ]
-            df = df[["Data"] + cols]
+            df = df[["data"] + cols]
             return df
 
         # Salta as linhas adicionais
         for _ in range(4):
             file.readline()
 
         # Variáveis auxiliares
@@ -375,17 +375,17 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=rees_uees)
-            df["UEE"] = uees
-            df["Configuração"] = cfg
-            df = df[["Configuração", "UEE"] + rees_uees]
+            df["uee"] = uees
+            df["configuracao"] = cfg
+            df = df[["configuracao", "uee"] + rees_uees]
             return df
 
         # Identifica a configuração
         linha = file.readline()
         cfg = self.__campo_cfg.read(linha)
 
         file.readline()
@@ -443,18 +443,19 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=uees_rees)
-            df["UEE"] = uees
-            df["Configuração"] = cfg
-            df = df[["Configuração", "UEE"] + uees_rees]
-            df = df.astype({"MES": "int64"})
+            df["uee"] = uees
+            df["configuracao"] = cfg
+            df = df[["configuracao", "uee"] + uees_rees]
+            df = df.rename(columns={"MES": "mes"})
+            df = df.astype({"mes": "int64"})
             return df
 
         # Identifica a configuração
         linha = file.readline()
         cfg = self.__campo_cfg.read(linha)
 
         file.readline()
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/parpvaz.py` & `inewave-0.0.98/inewave/newave/modelos/parpvaz.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,19 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            df = pd.DataFrame(tabela, columns=["Ano"] + MESES_DF)
-            df["UHE"] = uhe
-            df["Configuração"] = cfg
-            df = df[["UHE", "Configuração", "Ano"] + MESES_DF]
-            df = df.astype({"Ano": "int64"})
+            df = pd.DataFrame(tabela, columns=["ano"] + MESES_DF)
+            df["uhe"] = uhe
+            df["configuracao"] = cfg
+            df = df[["uhe", "configuracao", "ano"] + MESES_DF]
+            df = df.astype({"ano": "int64"})
             return df
 
         # Identifica a usina e a configuração
         linha = file.readline()
         uhe = self.__campo_uhe.read(linha)
         cfg = self.__campo_cfg.read(linha)
 
@@ -151,23 +151,23 @@
                 anos[idx_i:idx_f] = [str(ano)] * 12
             return [int(a) for a in anos]
 
         def converte_vetor_meses(meses: List[str]) -> List[int]:
             return [MESES_ABREV.index(m) + 1 for m in meses]
 
         def converte_tabela_em_df():
-            cols = [f"Lag {i}" for i in range(1, 12)]
+            cols = [f"lag_{i}" for i in range(1, 12)]
             df = pd.DataFrame(tabela, columns=cols)
             anos_conv = converte_vetor_anos(anos)
             meses_conv = converte_vetor_meses(meses)
-            df["Data"] = [
+            df["data"] = [
                 date(year=a, month=m, day=1)
                 for a, m in zip(anos_conv, meses_conv)
             ]
-            df = df[["Data"] + cols]
+            df = df[["data"] + cols]
             return df
 
         # Salta as linhas adicionais
         for _ in range(5):
             file.readline()
 
         # Variáveis auxiliares
@@ -253,23 +253,23 @@
                 anos[idx_i:idx_f] = [str(ano)] * 12
             return [int(a) for a in anos]
 
         def converte_vetor_meses(meses: List[str]) -> List[int]:
             return [MESES_ABREV.index(m) + 1 for m in meses]
 
         def converte_tabela_em_df():
-            cols = [f"Lag {i}" for i in range(1, 12)]
+            cols = [f"lag_{i}" for i in range(1, 12)]
             df = pd.DataFrame(tabela, columns=cols)
             anos_conv = converte_vetor_anos(anos)
             meses_conv = converte_vetor_meses(meses)
-            df["Data"] = [
+            df["data"] = [
                 date(year=a, month=m, day=1)
                 for a, m in zip(anos_conv, meses_conv)
             ]
-            df = df[["Data"] + cols]
+            df = df[["data"] + cols]
             return df
 
         # Salta as linhas adicionais
         for _ in range(3):
             file.readline()
 
         # Variáveis auxiliares
@@ -350,17 +350,17 @@
                 idx = indice_inicio_pos + a
                 ano = ultimo_ano_estudo + a + 1
                 anos[idx] = str(ano)
             return [int(a) for a in anos]
 
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
-            df["Tipo"] = self.__tipo
-            df["Ano"] = converte_vetor_anos(anos)
-            df = df[["Tipo", "Ano"] + MESES_DF]
+            df["tipo"] = self.__tipo
+            df["ano"] = converte_vetor_anos(anos)
+            df = df[["tipo", "ano"] + MESES_DF]
             return df
 
         # Salta as linhas adicionais
         linha = file.readline()
         self.__tipo = linha.split("ORDEM")[1].split("DO MODELO")[0].strip()
         for _ in range(3):
             file.readline()
@@ -412,18 +412,18 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             cols = (
-                [f"Psi {i}" for i in range(1, len(MESES_DF))]
-                + ["Psi A"]
-                + [f"Psi Norm {i}" for i in range(1, len(MESES_DF))]
-                + ["Psi Norm A"]
+                [f"psi_{i}" for i in range(1, len(MESES_DF))]
+                + ["psi_A"]
+                + [f"psi_norm_{i}" for i in range(1, len(MESES_DF))]
+                + ["psi_norm_A"]
             )
             return pd.DataFrame(tabela, columns=cols)
 
         linha = file.readline()
 
         tabela = np.zeros((1, 2 * len(MESES_DF)))
         # Processa os dados
@@ -475,17 +475,17 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
-            df["Ano"] = ano
-            df["Série"] = list(range(i))
-            df = df[["Ano", "Série"] + MESES_DF]
+            df["ano"] = ano
+            df["serie"] = list(range(i))
+            df = df[["ano", "serie"] + MESES_DF]
             return df
 
         # Identifica o ano em questão
         linha = file.readline()
         ano = self.__campo_ano.read(linha)
 
         # Salta as linhas adicionais
@@ -570,23 +570,23 @@
                 anos[idx_i:idx_f] = [str(ano)] * 12
             return [int(a) for a in anos]
 
         def converte_vetor_meses(meses: List[str]) -> List[int]:
             return [MESES_ABREV.index(m) + 1 for m in meses]
 
         def converte_tabela_em_df():
-            cols = [f"Lag {i}" for i in range(1, 12)]
+            cols = [f"lag_{i}" for i in range(1, 12)]
             df = pd.DataFrame(tabela, columns=cols)
             anos_conv = converte_vetor_anos(anos)
             meses_conv = converte_vetor_meses(meses)
-            df["Data"] = [
+            df["data"] = [
                 date(year=a, month=m, day=1)
                 for a, m in zip(anos_conv, meses_conv)
             ]
-            df = df[["Data"] + cols]
+            df = df[["data"] + cols]
             return df
 
         # Salta as linhas adicionais
         for _ in range(4):
             file.readline()
 
         # Variáveis auxiliares
@@ -639,18 +639,18 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            df = pd.DataFrame(tabela, columns=MESES_DF + ["Anual"])
-            df["UHE 1"] = uhes1
-            df["UHE 2"] = uhes2
-            return df[["UHE 1", "UHE 2"] + MESES_DF + ["Anual"]]
+            df = pd.DataFrame(tabela, columns=MESES_DF + ["anual"])
+            df["uhe_1"] = uhes1
+            df["uhe_2"] = uhes2
+            return df[["uhe_1", "uhe_2"] + MESES_DF + ["anual"]]
 
         for _ in range(4):
             file.readline()
 
         # Variáveis auxiliares
         uhes1: List[str] = []
         uhes2: List[str] = []
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/patamar.py` & `inewave-0.0.98/inewave/newave/modelos/patamar.py`

 * *Files 6% similar despite different names*

```diff
@@ -288,21 +288,21 @@
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(
                 tabela,
-                columns=["Subsistema De", "Subsistema Para", "Ano"] + MESES_DF,
+                columns=["submercado_de", "submercado_para", "ano"] + MESES_DF,
             )
             df = df.astype(
                 {
-                    "Subsistema De": "int64",
-                    "Subsistema Para": "int64",
-                    "Ano": "int64",
+                    "submercado_de": "int64",
+                    "submercado_para": "int64",
+                    "ano": "int64",
                 }
             )
             return df
 
         # Salta as linhas adicionais
         for _ in range(5):
             self.__cabecalhos.append(file.readline())
@@ -356,35 +356,35 @@
         ultimo_subsistema_de = 0
         ultimo_subsistema_para = 0
 
         for _, linha in self.data.iterrows():
             linha_lida: pd.Series = linha
             if any(
                 [
-                    linha_lida["Subsistema De"] != ultimo_subsistema_de,
-                    linha_lida["Subsistema Para"] != ultimo_subsistema_para,
+                    linha_lida["submercado_de"] != ultimo_subsistema_de,
+                    linha_lida["submercado_para"] != ultimo_subsistema_para,
                 ]
             ):
                 ultimo_ano = 0
-                ultimo_subsistema_de = linha_lida["Subsistema De"]
-                ultimo_subsistema_para = linha_lida["Subsistema Para"]
+                ultimo_subsistema_de = linha_lida["submercado_de"]
+                ultimo_subsistema_para = linha_lida["submercado_para"]
                 file.write(
                     self.__linha_subsis.write(
                         [
                             int(ultimo_subsistema_de),
                             int(ultimo_subsistema_para),
                         ]
                     )
                 )
             ano_linha = (
-                int(linha_lida["Ano"])
-                if linha_lida["Ano"] != ultimo_ano
+                int(linha_lida["ano"])
+                if linha_lida["ano"] != ultimo_ano
                 else None
             )
-            ultimo_ano = int(linha_lida["Ano"])
+            ultimo_ano = int(linha_lida["ano"])
             file.write(
                 self.__linha.write([ano_linha] + linha_lida[MESES_DF].tolist())
             )
         file.write(BlocoIntercambioPatamarSubsistemas.FIM_BLOCO + "\n")
 
 
 class BlocoUsinasNaoSimuladas(Section):
@@ -418,22 +418,22 @@
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(
                 tabela,
-                columns=["Subsistema", "Patamar", "Bloco", "Ano"] + MESES_DF,
+                columns=["submercado", "patamar", "bloco", "ano"] + MESES_DF,
             )
             df = df.astype(
                 {
-                    "Subsistema": "int64",
-                    "Patamar": "int64",
-                    "Bloco": "int64",
-                    "Ano": "int64",
+                    "submercado": "int64",
+                    "patamar": "int64",
+                    "bloco": "int64",
+                    "ano": "int64",
                 }
             )
             return df
 
         # Salta as linhas adicionais
         for _ in range(4):
             self.__cabecalhos.append(file.readline())
@@ -489,32 +489,32 @@
         ultimo_subsistema = 0
         ultimo_bloco = 0
 
         for _, linha in self.data.iterrows():
             linha_lida: pd.Series = linha
             if any(
                 [
-                    linha_lida["Subsistema"] != ultimo_subsistema,
-                    linha_lida["Bloco"] != ultimo_bloco,
+                    linha_lida["submercado"] != ultimo_subsistema,
+                    linha_lida["bloco"] != ultimo_bloco,
                 ]
             ):
                 ultimo_ano = 0
-                ultimo_subsistema = linha_lida["Subsistema"]
-                ultimo_bloco = linha_lida["Bloco"]
+                ultimo_subsistema = linha_lida["submercado"]
+                ultimo_bloco = linha_lida["bloco"]
                 file.write(
                     self.__linha_subsis.write(
                         [
                             int(ultimo_subsistema),
                             int(ultimo_bloco),
                         ]
                     )
                 )
             ano_linha = (
-                int(linha_lida["Ano"])
-                if linha_lida["Ano"] != ultimo_ano
+                int(linha_lida["ano"])
+                if linha_lida["ano"] != ultimo_ano
                 else None
             )
-            ultimo_ano = int(linha_lida["Ano"])
+            ultimo_ano = int(linha_lida["ano"])
             file.write(
                 self.__linha.write([ano_linha] + linha_lida[MESES_DF].tolist())
             )
         file.write(BlocoIntercambioPatamarSubsistemas.FIM_BLOCO + "\n")
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/penalid.py` & `inewave-0.0.98/inewave/newave/modelos/penalid.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,26 +42,26 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             cols = [
-                "Penalidade 1",
-                "Penalidade 2",
-                "Subsistema",
+                "penalidade_1",
+                "penalidade_2",
+                "submercado",
             ]
             df = pd.DataFrame(tabela, columns=cols)
-            df["Chave"] = chaves
+            df["mnemonico"] = chaves
             df = df[
                 [
-                    "Chave",
-                    "Penalidade 1",
-                    "Penalidade 2",
-                    "Subsistema",
+                    "mnemonico",
+                    "penalidade_1",
+                    "penalidade_2",
+                    "submercado",
                 ]
             ]
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/pmo.py` & `inewave-0.0.98/inewave/newave/modelos/pmo.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
-            df["REE"] = rees
-            df = df[["REE"] + MESES_DF]
+            df["ree"] = rees
+            df = df[["ree"] + MESES_DF]
             return df
 
         # Pula as linhas iniciais
         for _ in range(4):
             file.readline()
 
         # Variáveis auxiliares
@@ -111,16 +111,16 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(tabela, columns=MESES_DF)
-            df["REE"] = rees
-            df = df[["REE"] + MESES_DF]
+            df["ree"] = rees
+            df = df[["ree"] + MESES_DF]
             return df
 
         # Pula as linhas iniciais
         for _ in range(4):
             file.readline()
 
         # Variáveis auxiliares
@@ -174,24 +174,24 @@
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df() -> pd.DataFrame:
             df = pd.DataFrame(tabela)
             df.columns = [
-                "Iteração",
-                "Lim. Inf. ZINF",
-                "ZINF",
-                "Lim. Sup. ZINF",
-                "ZSUP",
-                "Delta ZINF",
-                "ZSUP Iteração",
+                "iteracao",
+                "limite_inferior_zinf",
+                "zinf",
+                "limite_superior_zinf",
+                "zsup",
+                "delta_zinf",
+                "zsup_iteracap",
             ]
-            df = df.astype({"Iteração": "int64"})
-            df["Tempo"] = tempos
+            df = df.astype({"iteracao": "int64"})
+            df["tempo"] = tempos
             return df
 
         # Salta as duas linhas iniciais
         for _ in range(3):
             file.readline()
         # Variáveis auxiliares
         tabela = np.zeros((3 * MAX_ITERS, 7), dtype=np.float64)
@@ -249,15 +249,15 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            df = pd.DataFrame(tabela, columns=["Ano"] + MESES_DF)
+            df = pd.DataFrame(tabela, columns=["ano"] + MESES_DF)
             return df
 
         # Pula as linhas iniciais
         for _ in range(6):
             file.readline()
         # Variáveis auxiliares
         tabela = np.zeros((MAX_ANOS_ESTUDO, len(MESES_DF) + 1), dtype=np.int64)
@@ -311,19 +311,19 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            colunas = ["Reta", "Coeficiente Angular", "Constante"]
+            colunas = ["reta", "coeficiente_angular", "coeficiente_linear"]
             df = pd.DataFrame(tabela, columns=colunas)
-            df["REE"] = rees
-            df = df[["REE"] + colunas]
-            df = df.astype({"Reta": "int64"})
+            df["ree"] = rees
+            df = df[["ree"] + colunas]
+            df = df.astype({"reta": "int64"})
             return df
 
         # Variáveis auxiliares
         ree_atual = ""
         rees: List[str] = []
         tabela = np.zeros(
             (BlocoMARSPMO.MAX_RETAS_MARS * MAX_REES * MAX_MESES_ESTUDO, 3),
@@ -348,15 +348,15 @@
 
 class BlocoRiscoDeficitENSPMO(Block):
     """
     Bloco de informações sobre os riscos de déficit e
     ENS (energia não suprida) existentes no arquivo `pmo.dat`.
     """
 
-    BEGIN_PATTERN = "RISCO ANUAL DE DEFICIT E E\(ENS\) \(%\)"  # noqa
+    BEGIN_PATTERN = r"RISCO ANUAL DE DEFICIT E E\(ENS\) \(%\)"  # noqa
     END_PATTERN = ""
 
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, BlocoRiscoDeficitENSPMO):
             return False
         bloco: BlocoRiscoDeficitENSPMO = o
         if not all(
@@ -369,19 +369,19 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df() -> pd.DataFrame:
             df = pd.DataFrame(tabela)
-            cols = ["Ano"]
+            cols = ["ano"]
             for sub in subsistemas:
-                cols += [f"Risco - {sub}", f"EENS - {sub}"]
+                cols += [f"risco_{sub}", f"eens_{sub}"]
             df.columns = cols
-            df = df.astype({"Ano": "int64"})
+            df = df.astype({"ano": "int64"})
             return df
 
         # Pula as três linhas iniciais
         for _ in range(3):
             file.readline()
         # Identifica os subsistemas em questão e constroi
         # a estrutura da linha da tabela a ser lida
@@ -447,18 +447,18 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df() -> pd.DataFrame:
-            cols = ["Valor Esperado", "Desvio Padrão do VE", "(%)"]
+            cols = ["valor_esperado", "desvio_padrao", "percentual"]
             df = pd.DataFrame(tabela, columns=cols)
-            df["Parcela"] = parcelas
-            df = df[["Parcela"] + cols]
+            df["parcela"] = parcelas
+            df = df[["parcela"] + cols]
             return df
 
         # Salta duas linhas
         for _ in range(2):
             file.readline()
         parcelas: List[str] = []
         tabela = np.zeros((30, 3), dtype=np.float64)
@@ -691,15 +691,15 @@
                         "configuracao",
                         "produtibilidade_equivalente_volmin_volmax",
                     ]
                     + self.__colunas_produtibilidades_reservatorios()
                     + self.__colunas_produtibilidades_acumuladas()
                 ]
                 break
-            if "CONFIGURACAO :   " in linha:
+            if "CONFIGURACAO :" in linha:
                 if cfg_atual != 0:
                     df_atual = self.__fecha_configuracao(
                         df_usinas,
                         df_reservatorios,
                         df_acumuladas,
                         cfg_atual,
                         df_atual,
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/re.py` & `inewave-0.0.98/inewave/newave/modelos/re.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,17 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            cols = ["Conjunto"] + [f"Usina {i}" for i in range(1, 11)]
+            cols = ["conjunto"] + [f"codigo_usina_{i}" for i in range(1, 11)]
             df = pd.DataFrame(tabela, columns=cols)
-            df = df.astype({"Conjunto": "int64"})
+            df = df.astype({"conjunto": "int64"})
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
 
         i = 0
@@ -124,32 +124,32 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             cols = [
-                "Conjunto",
-                "Mês Início",
-                "Ano Início",
-                "Mês Fim",
-                "Ano Fim",
-                "Flag P",
-                "Restrição",
+                "conjunto",
+                "mes_inicio",
+                "ano_inicio",
+                "mes_fim",
+                "ano_fim",
+                "patamar",
+                "restricao",
             ]
             df = pd.DataFrame(tabela, columns=cols)
             df["Motivo"] = motivos
             df = df.astype(
                 {
-                    "Conjunto": "int64",
-                    "Mês Início": "int64",
-                    "Ano Início": "int64",
-                    "Mês Fim": "int64",
-                    "Ano Fim": "int64",
-                    "Flag P": "int64",
+                    "conjunto": "int64",
+                    "mes_inicio": "int64",
+                    "ano_inicio": "int64",
+                    "mes_fim": "int64",
+                    "ano_fim": "int64",
+                    "patamar": "int64",
                 }
             )
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/ree.py` & `inewave-0.0.98/inewave/newave/modelos/ree.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,29 +44,29 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             cols = [
-                "Número",
-                "Submercado",
-                "Mês Fim Individualizado",
-                "Ano Fim Individualizado",
+                "codigo",
+                "submercado",
+                "mes_fim_individualizado",
+                "ano_fim_individualizado",
             ]
             df = pd.DataFrame(tabela, columns=cols)
-            df["Nome"] = nomes
-            df = df.astype({"Submercado": np.int64, "Número": np.int64})
+            df["nome"] = nomes
+            df = df.astype({"submercado": np.int64, "codigo": np.int64})
             df = df[
                 [
-                    "Número",
-                    "Nome",
-                    "Submercado",
-                    "Mês Fim Individualizado",
-                    "Ano Fim Individualizado",
+                    "codigo",
+                    "nome",
+                    "submercado",
+                    "mes_fim_individualizado",
+                    "ano_fim_individualizado",
                 ]
             ]
             return df
 
         # Salta as linhas adicionais
         for _ in range(3):
             self.__cabecalhos.append(file.readline())
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/restricaoeletrica.py` & `inewave-0.0.98/inewave/newave/modelos/restricaoeletrica.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/restricaoenergia.py` & `inewave-0.0.98/inewave/newave/modelos/restricaoenergia.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/restricaovazao.py` & `inewave-0.0.98/inewave/newave/modelos/restricaovazao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/selcor.py` & `inewave-0.0.98/inewave/newave/modelos/selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/shist.py` & `inewave-0.0.98/inewave/newave/modelos/shist.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/sistema.py` & `inewave-0.0.98/inewave/newave/modelos/sistema.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,23 +94,25 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            cols = [f"Custo Pat. {p}" for p in range(1, 5)] + [
-                f"Corte Pat. {p}" for p in range(1, 5)
+            cols = [f"custo_deficit_patamar_{p}" for p in range(1, 5)] + [
+                f"corte_patamar_{p}" for p in range(1, 5)
             ]
             df = pd.DataFrame(
-                tabela, columns=["Num. Subsistema", "Fictício"] + cols
+                tabela, columns=["codigo_submercado", "ficticio"] + cols
             )
-            df["Nome"] = subsistemas
-            df = df[["Num. Subsistema", "Nome", "Fictício"] + cols]
-            df = df.astype({"Num. Subsistema": "int64", "Fictício": "int64"})
+            df["nome_submercado"] = subsistemas
+            df = df[
+                ["codigo_submercado", "nome_submercado", "ficticio"] + cols
+            ]
+            df = df.astype({"codigo_submercado": "int64", "ficticio": "int64"})
             return df
 
         # Salta as linhas adicionais
         for _ in range(3):
             self.__cabecalhos.append(file.readline())
 
         i = 0
@@ -137,16 +139,16 @@
     def write(self, file: IO, *args, **kwargs):
         for linha in self.__cabecalhos:
             file.write(linha)
         if not isinstance(self.data, pd.DataFrame):
             raise ValueError(
                 "Dados do sistema.dat não foram lidos com sucesso"
             )
-        cols = [f"Custo Pat. {p}" for p in range(1, 5)] + [
-            f"Corte Pat. {p}" for p in range(1, 5)
+        cols = [f"custo_deficit_patamar_{p}" for p in range(1, 5)] + [
+            f"corte_patamar_{p}" for p in range(1, 5)
         ]
         for _, linha_dados in self.data.iterrows():
             dados_linha = linha_dados[cols].tolist()
             dados_linha_escrita = linha_dados.tolist()[:3]
             for d in dados_linha:
                 dados_linha_escrita.append(d if not np.isnan(d) else None)
             file.write(self.__linha.write(dados_linha_escrita))
@@ -188,29 +190,29 @@
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(
                 tabela,
-                columns=["Ano"] + MESES_DF,
+                columns=["ano"] + MESES_DF,
             )
-            df["Subsistema De"] = subsistemas_de
-            df["Subsistema Para"] = subsistemas_para
-            df["Sentido"] = sentidos
+            df["submercado_de"] = subsistemas_de
+            df["submercado_para"] = subsistemas_para
+            df["sentido"] = sentidos
             df = df[
-                ["Subsistema De", "Subsistema Para", "Sentido", "Ano"]
+                ["submercado_de", "submercado_para", "sentido", "ano"]
                 + MESES_DF
             ]
             df = df.astype(
                 {
-                    "Subsistema De": "int64",
-                    "Subsistema Para": "int64",
-                    "Sentido": "int64",
-                    "Ano": "int64",
+                    "submercado_de": "int64",
+                    "submercado_para": "int64",
+                    "sentido": "int64",
+                    "ano": "int64",
                 }
             )
             return df
 
         # Salta as linhas adicionais
         for _ in range(3):
             self.__cabecalhos.append(file.readline())
@@ -278,38 +280,38 @@
         ultimo_subsistema_para = 0
         ultimo_sentido = -1
 
         for _, linha in self.data.iterrows():
             linha_lida: pd.Series = linha
             if any(
                 [
-                    linha_lida["Subsistema De"] != ultimo_subsistema_de,
-                    linha_lida["Subsistema Para"] != ultimo_subsistema_para,
-                    linha_lida["Sentido"] != ultimo_sentido,
+                    linha_lida["submercado_de"] != ultimo_subsistema_de,
+                    linha_lida["submercado_para"] != ultimo_subsistema_para,
+                    linha_lida["sentido"] != ultimo_sentido,
                 ]
             ):
                 ultimo_ano = 0
-                ultimo_subsistema_de = linha_lida["Subsistema De"]
-                ultimo_subsistema_para = linha_lida["Subsistema Para"]
-                ultimo_sentido = linha_lida["Sentido"]
+                ultimo_subsistema_de = linha_lida["submercado_de"]
+                ultimo_subsistema_para = linha_lida["submercado_para"]
+                ultimo_sentido = linha_lida["sentido"]
                 file.write(
                     self.__linha_subsis.write(
                         [
                             int(ultimo_subsistema_de),
                             int(ultimo_subsistema_para),
                             int(ultimo_sentido),
                         ]
                     )
                 )
             ano_linha = (
-                int(linha_lida["Ano"])
-                if linha_lida["Ano"] != ultimo_ano
+                int(linha_lida["ano"])
+                if linha_lida["ano"] != ultimo_ano
                 else None
             )
-            ultimo_ano = int(linha_lida["Ano"])
+            ultimo_ano = int(linha_lida["ano"])
             dados_linha = linha_lida[MESES_DF].tolist()
             dados_linha_escrita = []
             for d in dados_linha:
                 dados_linha_escrita.append(d if not np.isnan(d) else None)
             file.write(self.__linha.write([ano_linha] + dados_linha_escrita))
         file.write(BlocoIntercambioSubsistema.FIM_BLOCO + "\n")
 
@@ -347,23 +349,23 @@
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(
                 tabela,
-                columns=["Subsistema"] + MESES_DF,
+                columns=["submercado"] + MESES_DF,
             )
             df = df.astype(
                 {
-                    "Subsistema": "int64",
+                    "submercado": "int64",
                 }
             )
-            df["Ano"] = anos
-            df = df[["Subsistema", "Ano"] + MESES_DF]
+            df["ano"] = anos
+            df = df[["submercado", "ano"] + MESES_DF]
             return df
 
         # Salta as linhas adicionais
         for _ in range(3):
             self.__cabecalhos.append(file.readline())
 
         i = 0
@@ -412,30 +414,30 @@
 
         ultimo_subsistema = 0
 
         for _, linha in self.data.iterrows():
             linha_lida: pd.Series = linha
             if any(
                 [
-                    linha_lida["Subsistema"] != ultimo_subsistema,
+                    linha_lida["submercado"] != ultimo_subsistema,
                 ]
             ):
                 ultimo_ano = ""
-                ultimo_subsistema = linha_lida["Subsistema"]
+                ultimo_subsistema = linha_lida["submercado"]
                 file.write(
                     self.__linha_subsis.write(
                         [
                             int(ultimo_subsistema),
                         ]
                     )
                 )
             ano_linha = (
-                linha_lida["Ano"] if linha_lida["Ano"] != ultimo_ano else None
+                linha_lida["ano"] if linha_lida["ano"] != ultimo_ano else None
             )
-            ultimo_ano = linha_lida["Ano"]
+            ultimo_ano = linha_lida["ano"]
             dados_linha = linha_lida[MESES_DF].tolist()
             dados_linha_escrita = []
             for d in dados_linha:
                 dados_linha_escrita.append(d if not np.isnan(d) else None)
             file.write(self.__linha.write([ano_linha] + dados_linha_escrita))
         file.write(BlocoMercadoEnergiaSistema.FIM_BLOCO + "\n")
 
@@ -475,19 +477,19 @@
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
             df = pd.DataFrame(
-                tabela, columns=["Subsistema", "Bloco", "Ano"] + MESES_DF
+                tabela, columns=["submercado", "bloco", "ano"] + MESES_DF
             )
-            df["Razão"] = razoes
-            df = df.astype({"Subsistema": "int64", "Ano": "int64"})
-            df = df[["Subsistema", "Bloco", "Razão", "Ano"] + MESES_DF]
+            df["fonte"] = razoes
+            df = df.astype({"submercado": "int64", "ano": "int64"})
+            df = df[["submercado", "bloco", "fonte", "ano"] + MESES_DF]
             return df
 
         # Salta as linhas adicionais
         for _ in range(3):
             self.__cabecalhos.append(file.readline())
 
         i = 0
@@ -543,26 +545,26 @@
         ultimo_subsistema: Optional[int] = 0
         ultimo_bloco: Optional[int] = 0
         ultima_razao: Optional[str] = ""
 
         for _, linha in self.data.iterrows():
             linha_lida: pd.Series = linha
             novo_subsis = (
-                int(linha_lida["Subsistema"])
-                if not np.isnan(linha_lida["Subsistema"])
+                int(linha_lida["submercado"])
+                if not np.isnan(linha_lida["submercado"])
                 else None
             )
             novo_bloco = (
-                int(linha_lida["Bloco"])
-                if not np.isnan(linha_lida["Bloco"])
+                int(linha_lida["bloco"])
+                if not np.isnan(linha_lida["bloco"])
                 else None
             )
             nova_razao = (
-                str(linha_lida["Razão"])
-                if not linha_lida["Razão"] is None
+                str(linha_lida["fonte"])
+                if not linha_lida["fonte"] is None
                 else None
             )
             if any(
                 [
                     novo_subsis != ultimo_subsistema,
                     novo_bloco != ultimo_bloco,
                     nova_razao != ultima_razao,
@@ -578,18 +580,18 @@
                             novo_subsis,
                             novo_bloco,
                             nova_razao,
                         ]
                     )
                 )
             ano_linha = (
-                int(linha_lida["Ano"])
-                if linha_lida["Ano"] != ultimo_ano
+                int(linha_lida["ano"])
+                if linha_lida["ano"] != ultimo_ano
                 else None
             )
-            ultimo_ano = int(linha_lida["Ano"])
+            ultimo_ano = int(linha_lida["ano"])
             dados_linha = linha_lida[MESES_DF].tolist()
             dados_linha_escrita = []
             for d in dados_linha:
                 dados_linha_escrita.append(d if not np.isnan(d) else None)
             file.write(self.__linha.write([ano_linha] + dados_linha_escrita))
         file.write(BlocoGeracaoUsinasNaoSimuladas.FIM_BLOCO + "\n")
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/term.py` & `inewave-0.0.98/inewave/newave/modelos/term.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,30 +46,30 @@
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df() -> pd.DataFrame:
             cols = (
                 [
-                    "Potência Instalada",
-                    "FC Máximo",
-                    "TEIF",
-                    "Indisponibilidade Programada",
+                    "potencia_instalada",
+                    "fator_capacidade_maximo",
+                    "teif",
+                    "indisponibilidade_programada",
                 ]
-                + [f"GT Min {m}" for m in MESES_DF]
-                + ["GT Min D+ Anos"]
+                + [f"geracao_minima_{m}" for m in MESES_DF]
+                + ["geracao_minima_demais_anos"]
             )
             df = pd.DataFrame(
                 tabela,
                 columns=cols,
             )
-            df["Número"] = numeros
-            df["Nome"] = nomes
-            df = df[["Número", "Nome"] + cols]
-            df = df.astype({"Número": "int64"})
+            df["codigo_usina"] = numeros
+            df["nome_usina"] = nomes
+            df = df[["codigo_usina", "nome_usina"] + cols]
+            df = df.astype({"codigo_usina": "int64"})
             return df
 
         # Salta as linhas adicionais
         for _ in range(2):
             self.__cabecalhos.append(file.readline())
 
         i = 0
@@ -82,14 +82,15 @@
             if len(linha) < 3:
                 # Converte para df e salva na variável
                 if i > 0:
                     tabela = tabela[:i, :]
                     self.data = converte_tabela_em_df()
                 break
             dados = self.__linha.read(linha)
+            print(dados)
             tabela[i, :] = dados[2:]
             numeros.append(dados[0])
             nomes.append(dados[1])
             i += 1
 
     # Override
     def write(self, file: IO, *args, **kwargs):
```

### Comparing `inewave-0.0.97/inewave/newave/modelos/vazaob.py` & `inewave-0.0.98/inewave/newave/modelos/vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/vazaof.py` & `inewave-0.0.98/inewave/newave/modelos/vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/vazaos.py` & `inewave-0.0.98/inewave/newave/modelos/vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/vazoes.py` & `inewave-0.0.98/inewave/newave/modelos/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/modelos/vazpast.py` & `inewave-0.0.98/inewave/newave/modelos/vazpast.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,22 +38,22 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df() -> pd.DataFrame:
-            cols = ["Índice"] + MESES_DF
+            cols = ["codigo_usina"] + MESES_DF
             df = pd.DataFrame(
                 tabela,
                 columns=cols,
             )
-            df["Usina"] = usinas
-            df = df.astype({"Índice": "int64"})
-            df = df[["Índice", "Usina"] + MESES_DF]
+            df["nome_usina"] = usinas
+            df = df.astype({"codigo_usina": "int64"})
+            df = df[["codigo_usina", "nome_usina"] + MESES_DF]
             return df
 
         # Salta as linhas adicionais
         for _ in range(3):
             self.__cabecalhos.append(file.readline())
 
         i = 0
```

### Comparing `inewave-0.0.97/inewave/newave/nwv_avl_evap.py` & `inewave-0.0.98/inewave/newave/nwv_avl_evap.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
         - periodo (`int`)
-        - indice_usina (`int`)
+        - codigo_usina (`int`)
         - nome_usina (`str`)
         - volume_armazenado_hm3 (`float`)
         - evaporacao_calculada_hm3 (`float`)
         - evaporacao_modelo_hm3 (`float`)
         - desvio_absoluto_hm3 (`float`)
         - desvio_percentual (`float`)
```

### Comparing `inewave-0.0.97/inewave/newave/nwv_cortes_evap.py` & `inewave-0.0.98/inewave/newave/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/nwv_eco_evap.py` & `inewave-0.0.98/inewave/newave/nwv_eco_evap.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
         - periodo (`int`)
-        - indice_usina (`int`)
+        - codigo_usina (`int`)
         - nome_usina (`str`)
         - volume_referencia_hm3 (`float`)
         - evaporacao_referencia_hm3 (`float`)
         - coeficiente_evaporacao_mm_mes (`int`)
         - flag_evaporacao (`int`)
         - evaporacao_linear (`int`)
         - tipo_volume_referencia (`int`)
```

### Comparing `inewave-0.0.97/inewave/newave/parp.py` & `inewave-0.0.98/inewave/newave/parp.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class PARp(BlockFile):
+class Parp(BlockFile):
     """
     Armazena os dados de saída do NEWAVE referentes aos modelos e às
     séries sintéticas de energia geradas pelo PAR(p).
 
 
     Esta classe lida com informações de saída do NEWAVE e
     cujas saídas devem ser compatíveis com as observadas através
@@ -60,15 +60,15 @@
         self.__ordem_original_modelo = None
         self.__ordem_final_modelo = None
         self.__coeficientes = None
         self.__correl_espacial_anual = None
         self.__correl_espacial_mensal = None
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="parp.dat") -> "PARp":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="parp.dat") -> "Parp":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
@@ -78,35 +78,15 @@
 
         :return: Os nomes dos REEs
         :rtype: List[str]
         """
         if self.series_energia_ree is None:
             return None
         else:
-            return self.series_energia_ree["REE"].unique().tolist()
-
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
+            return self.series_energia_ree["ree"].unique().tolist()
 
     def __concatena_dados(self, bloco: Type[Block]) -> Optional[Any]:
         """
         Obtém os dados de um bloco se este existir dentre os blocos do arquivo.
 
         :param bloco: O tipo do bloco cujos dados serão extraídos
         :type bloco: Type[T]
@@ -149,16 +129,16 @@
                 f"{df.shape[0]} linhas não podem ser "
                 + f"divididas em {len(rees)} grupos"
             )
         cols = list(df.columns)
         col_ree: List[str] = []
         for ree in rees:
             col_ree += [ree] * int(linhas_por_ree)
-        df["REE"] = col_ree
-        return df[["REE"] + cols]
+        df["ree"] = col_ree
+        return df[["ree"] + cols]
 
     def __adiciona_coluna_ree_com_estagios(
         self, df: pd.DataFrame
     ) -> pd.DataFrame:
         """
         Adiciona uma coluna com os REEs de cada amostra e outra
         com o estágio de cada uma, assumindo
@@ -180,17 +160,17 @@
             )
         cols = list(df.columns)
         col_ree: List[str] = []
         col_estagio: List[int] = []
         for ree in rees:
             col_ree += [ree] * int(linhas_por_ree)
             col_estagio += list(range(1, int(linhas_por_ree) + 1))
-        df["REE"] = col_ree
-        df["Estágio"] = col_estagio
-        return df[["REE", "Estágio"] + cols]
+        df["ree"] = col_ree
+        df["estagio"] = col_estagio
+        return df[["ree", "estagio"] + cols]
 
     def __adiciona_coluna_ree_corrigindo_pre_pos(
         self, df: Optional[pd.DataFrame]
     ) -> Optional[pd.DataFrame]:
         """
         Adiciona uma coluna com os REEs de cada amostra e outra
         com o estágio de cada uma, assumindo
@@ -237,40 +217,40 @@
                 f"{df.shape[0]} linhas não podem ser "
                 + f"divididas em {len(rees)} grupos"
             )
         cols = list(df.columns)
         col_ree: List[str] = []
         for ree in rees:
             col_ree += [ree] * int(linhas_por_ree)
-        df["REE"] = col_ree
+        df["ree"] = col_ree
         ree0 = rees[0]
-        ano0 = df["Ano"].unique().tolist()[0]
-        filtro = (df["Ano"] == ano0) & (df["REE"] == ree0)
+        ano0 = df["ano"].unique().tolist()[0]
+        filtro = (df["ano"] == ano0) & (df["ree"] == ree0)
         n_series = df.loc[filtro].shape[0]
         for i, ree in enumerate(rees):
             i_i = i * int(linhas_por_ree)
             i_f = i_i + int(linhas_por_ree) - 1
-            df.loc[i_i:i_f, "Ano"] = converte_vetor_anos(
-                df.loc[i_i:i_f, "Ano"].tolist(), n_series
+            df.loc[i_i:i_f, "ano"] = converte_vetor_anos(
+                df.loc[i_i:i_f, "ano"].tolist(), n_series
             )
-        return df[["REE"] + cols]
+        return df[["ree"] + cols]
 
     @property
     def series_energia_ree(self) -> Optional[pd.DataFrame]:
         """
         A tabela de séries de energia para todas as configurações
         e REEs, no mesmo formato do arquivo `parp.dat`.
 
-        - REE (`str`)
-        - Configuração (`int`)
-        - Ano (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - ree (`str`)
+        - configuracao (`int`)
+        - ano (`int`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__series_energia is None:
             self.__series_energia = self.__concatena_dados(
                 BlocoSerieEnergiaREE
@@ -279,21 +259,21 @@
 
     @property
     def series_ruido_ree(self) -> Optional[pd.DataFrame]:
         """
         A tabela de séries de ruído para todos os REEs,
         no mesmo formato do arquivo `parp.dat`.
 
-        - REE (`str`)
-        - Ano (`int`)
-        - Série (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - ree (`str`)
+        - ano (`int`)
+        - serie (`int`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__series_ruido is None:
             self.__series_ruido = self.__concatena_dados(BlocoSerieRuidosREE)
             self.__series_ruido = (
@@ -305,21 +285,21 @@
 
     @property
     def series_media_ree(self) -> Optional[pd.DataFrame]:
         """
         A tabela de séries de médias para todos os REEs,
         no mesmo formato do arquivo `parp.dat`.
 
-        - REE (`str`)
-        - Ano (`int`)
-        - Série (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - ree (`str`)
+        - ano (`int`)
+        - serie (`int`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__series_media is None:
             self.__series_media = self.__concatena_dados(BlocoSerieMediasREE)
             self.__series_media = (
@@ -332,20 +312,20 @@
     @property
     def correlacao_series_energia_ree(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação das séries de energia para
         todas as configurações vigentes e REEs,
         no mesmo formato do arquivo `parp.dat`.
 
-        - REE (`str`)
-        - Data (`date`)
-        - Lag 1 (`float`)
-        - Lag 2 (`float`)
+        - ree (`str`)
+        - data (`date`)
+        - lag_1 (`float`)
+        - lag_2 (`float`)
         - ...
-        - Lag 11 (`float`)
+        - lag_11 (`float`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
         if self.__correl_series_energia is None:
             self.__correl_series_energia = self.__concatena_dados(
                 BlocoCorrelEnergiasREE
@@ -358,20 +338,20 @@
     @property
     def correlacao_parcial_series_energia_ree(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação parcial das séries de energia para
         todas as configurações vigentes e REEs,
         no mesmo formato do arquivo `parp.dat`.
 
-        - REE (`str`)
-        - Data (`date`)
-        - Lag 1 (`float`)
-        - Lag 2 (`float`)
+        - ree (`str`)
+        - data (`date`)
+        - lag_1 (`float`)
+        - lag_2 (`float`)
         - ...
-        - Lag 11 (`float`)
+        - lag_11 (`float`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
         if self.__correl_parcial_series_energia is None:
             self.__correl_parcial_series_energia = self.__concatena_dados(
                 BlocoCorrelParcialEnergiasREE
@@ -384,20 +364,20 @@
     @property
     def correlacao_series_ruidos_ree(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação das séries de ruídos para
         todas as configurações vigentes e REEs,
         no mesmo formato do arquivo `parp.dat`.
 
-        - REE (`str`)
-        - Data (`date`)
-        - Lag 1 (`float`)
-        - Lag 2 (`float`)
+        - ree (`str`)
+        - data (`date`)
+        - lag_1 (`float`)
+        - lag_2 (`float`)
         - ...
-        - Lag 11 (`float`)
+        - lag_11 (`float`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
         if self.__correl_series_ruido is None:
             self.__correl_series_ruido = self.__concatena_dados(
                 BlocoCorrelRuidosREE
@@ -410,20 +390,20 @@
     @property
     def correlacao_cruzada_media_ree(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação cruzada da variável anual com
         as séries de energia para todas as configurações vigentes e REEs,
         no mesmo formato do arquivo `parp.dat`.
 
-        - REE (`str`)
-        - Data (`date`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - ree (`str`)
+        - data (`date`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
         if self.__correl_cruzada_media is None:
             self.__correl_cruzada_media = self.__concatena_dados(
                 BlocoCorrelCruzadaMediaREE
@@ -436,87 +416,87 @@
     @property
     def ordem_original_modelo(self) -> Optional[pd.DataFrame]:
         """
         A tabela de ordens originais do modelo PAR ou PAR-A
         de cada REE, no mesmo formato do arquivo `parp.dat`,
         organizada por ano de estudo.
 
-        - REE (`str`)
-        - Ano (`int`)
-        - Janeiro (`int`)
-        - Fevereiro (`int`)
+        - ree (`str`)
+        - ano (`int`)
+        - janeiro (`int`)
+        - fevereiro (`int`)
         - ...
-        - Dezembro (`int`)
+        - dezembro (`int`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
 
         if self.__ordem_original_modelo is None:
             dados = self.__concatena_dados(BlocoOrdemModeloREE)
             if dados is not None:
                 dados = (
-                    dados.loc[dados["Tipo"] == "ORIGINAL", :]
-                    .drop(columns=["Tipo"])
+                    dados.loc[dados["tipo"] == "ORIGINAL", :]
+                    .drop(columns=["tipo"])
                     .copy()
                 )
                 dados = self.__adiciona_coluna_ree(dados)
                 self.__ordem_original_modelo = dados
 
         return self.__ordem_original_modelo
 
     @property
     def ordem_final_modelo(self) -> Optional[pd.DataFrame]:
         """
         A tabela de ordens finais do modelo PAR ou PAR-A
         de cada REE, no mesmo formato do arquivo `parp.dat`,
         organizada por ano de estudo.
 
-        - REE (`str`)
-        - Ano (`int`)
-        - Janeiro (`int`)
-        - Fevereiro (`int`)
+        - ree (`str`)
+        - ano (`int`)
+        - janeiro (`int`)
+        - fevereiro (`int`)
         - ...
-        - Dezembro (`int`)
+        - dezembro (`int`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__ordem_final_modelo is None:
             dados = self.__concatena_dados(BlocoOrdemModeloREE)
             if dados is not None:
                 dados = (
-                    dados.loc[dados["Tipo"] == "FINAL", :]
-                    .drop(columns=["Tipo"])
+                    dados.loc[dados["tipo"] == "FINAL", :]
+                    .drop(columns=["tipo"])
                     .copy()
                 )
                 dados = self.__adiciona_coluna_ree(dados)
                 self.__ordem_final_modelo = dados
 
         return self.__ordem_final_modelo
 
     @property
     def coeficientes(self) -> Optional[pd.DataFrame]:
         """
         Lista de coeficientes dos modelos PAR ou PAR-A
         de cada REE, no mesmo formato do arquivo `parp.dat`,
         organizada por período de estudo.
 
-        - REE (`str`)
-        - Estágio (`int`)
-        - Psi 1 (`int`)
-        - Psi 2 (`int`)
-        - ...
-        - Psi 11 (`int`)
-        - Psi A (`int`)
-        - Psi Norm 1 (`int`)
-        - Psi Norm 2 (`int`)
+        - ree (`str`)
+        - estagio (`int`)
+        - psi_1 (`int`)
+        - psi_2 (`int`)
+        - ...
+        - psi_11 (`int`)
+        - psi_A (`int`)
+        - psi_norm_1 (`int`)
+        - psi_norm_2 (`int`)
         - ...
-        - Psi Norm 11 (`int`)
-        - Psi Norm A (`int`)
+        - psi_norm_11 (`int`)
+        - psi_norm_A (`int`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__coeficientes is None:
             dados = self.__concatena_dados(BlocoCoeficientesModeloREE)
             if dados is not None:
@@ -527,16 +507,16 @@
 
     @property
     def correlacao_espacial_anual(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação para todas as configurações
         e REEs, no mesmo formato do arquivo `parp.dat`.
 
-        - Configuração (`int`)
-        - REE (`str`)
+        - configuracao (`int`)
+        - ree (`str`)
         - <Nome do REE 1> (`str`)
         - <Nome do REE 2> (`str`)
         - ...
         - <Nome do REE N> (`str`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
@@ -549,17 +529,17 @@
 
     @property
     def correlacao_espacial_mensal(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação para todas as configurações
         e REEs, no mesmo formato do arquivo `parp.dat`.
 
-        - Configuração (`int`)
-        - REE (`str`)
-        - MES (`int`)
+        - configuracao (`int`)
+        - ree (`str`)
+        - mes (`int`)
         - <Nome do REE 1> (`str`)
         - <Nome do REE 2> (`str`)
         - ...
         - <Nome do REE N> (`str`)
 
         :return: A tabela como um DataFrame.
         :rtype: Optional[pd.DataFrame]
```

### Comparing `inewave-0.0.97/inewave/newave/parpeol.py` & `inewave-0.0.98/inewave/newave/parpeol.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class PARpeol(BlockFile):
+class Parpeol(BlockFile):
     """
     Armazena os dados de saída do NEWAVE referentes às
     séries sintéticas de ventos geradas pelo PAR(p).
 
     Esta classe lida com informações de saída do NEWAVE e
     cujas saídas devem ser compatíveis com as observadas através
     do NWLISTOP.
@@ -45,15 +45,15 @@
         self.__correl_series_ruido = None
         self.__correl_espacial_anual = None
         self.__correl_espacial_mensal = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="parpeol.dat"
-    ) -> "PARpeol":
+    ) -> "Parpeol":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
@@ -63,35 +63,15 @@
 
         :return: Os nomes das UEEs
         :rtype: List[str]
         """
         if self.series_ventos_uee is None:
             return None
         else:
-            return self.series_ventos_uee["UEE"].unique().tolist()
-
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
+            return self.series_ventos_uee["uee"].unique().tolist()
 
     def __concatena_dados(self, bloco: Type[Block]) -> Optional[Any]:
         """
         Obtém os dados de um bloco se este existir dentre os blocos do arquivo.
 
         :param bloco: O tipo do bloco cujos dados serão extraídos
         :type bloco: Type[T]
@@ -134,16 +114,16 @@
                 f"{df.shape[0]} linhas não podem ser "
                 + f"divididas em {len(uees)} grupos"
             )
         cols = list(df.columns)
         col_uee: List[str] = []
         for uee in uees:
             col_uee += [uee] * int(linhas_por_uee)
-        df["UEE"] = col_uee
-        return df[["UEE"] + cols]
+        df["uee"] = col_uee
+        return df[["uee"] + cols]
 
     def __adiciona_coluna_uee_com_estagios(
         self, df: pd.DataFrame
     ) -> pd.DataFrame:
         """
         Adiciona uma coluna com as UEEs de cada amostra e outra
         com o estágio de cada uma, assumindo
@@ -165,17 +145,17 @@
             )
         cols = list(df.columns)
         col_uee: List[str] = []
         col_estagio: List[int] = []
         for uee in uees:
             col_uee += [uee] * int(linhas_por_uee)
             col_estagio += list(range(1, int(linhas_por_uee) + 1))
-        df["UEE"] = col_uee
-        df["Estágio"] = col_estagio
-        return df[["UEE", "Estágio"] + cols]
+        df["uee"] = col_uee
+        df["estagio"] = col_estagio
+        return df[["uee", "estagio"] + cols]
 
     def __adiciona_coluna_uee_corrigindo_pre_pos(
         self, df: Optional[pd.DataFrame]
     ) -> Optional[pd.DataFrame]:
         """
         Adiciona uma coluna com as UEEs de cada amostra e outra
         com o estágio de cada uma, assumindo
@@ -222,61 +202,61 @@
                 f"{df.shape[0]} linhas não podem ser "
                 + f"divididas em {len(uees)} grupos"
             )
         cols = list(df.columns)
         col_uee: List[str] = []
         for uee in uees:
             col_uee += [uee] * int(linhas_por_uee)
-        df["UEE"] = col_uee
+        df["uee"] = col_uee
         uee0 = uees[0]
-        ano0 = df["Ano"].unique().tolist()[0]
-        filtro = (df["Ano"] == ano0) & (df["UEE"] == uee0)
+        ano0 = df["ano"].unique().tolist()[0]
+        filtro = (df["ano"] == ano0) & (df["uee"] == uee0)
         n_series = df.loc[filtro].shape[0]
         for i, uee in enumerate(uees):
             i_i = i * int(linhas_por_uee)
             i_f = i_i + int(linhas_por_uee) - 1
-            df.loc[i_i:i_f, "Ano"] = converte_vetor_anos(
-                df.loc[i_i:i_f, "Ano"].tolist(), n_series
+            df.loc[i_i:i_f, "ano"] = converte_vetor_anos(
+                df.loc[i_i:i_f, "ano"].tolist(), n_series
             )
-        return df[["UEE"] + cols]
+        return df[["uee"] + cols]
 
     @property
     def series_ventos_uee(self) -> Optional[pd.DataFrame]:
         """
         A tabela de séries de ventos para todas as configurações
         e UEEs, no mesmo formato do arquivo `parpeol.dat`.
 
-        - UEE (`str`)
-        - Configuração (`int`)
-        - Ano (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - uee (`str`)
+        - configuracao (`int`)
+        - ano (`int`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__series_ventos is None:
             self.__series_ventos = self.__concatena_dados(BlocoSerieVentosUEE)
         return self.__series_ventos
 
     @property
     def series_ruido_uee(self) -> Optional[pd.DataFrame]:
         """
         A tabela de séries de ruído para todos os UEEs,
         no mesmo formato do arquivo `parpeol.dat`.
 
-        - UEE (`str`)
-        - Ano (`int`)
+        - uee (`str`)
+        - ano (`int`)
         - Série (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__series_ruido is None:
             self.__series_ruido = self.__concatena_dados(BlocoSerieRuidosUEE)
             self.__series_ruido = (
@@ -289,15 +269,15 @@
     @property
     def correlacao_series_ventos_uee(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação das séries de ventos para
         todas as configurações vigentes e UEEs,
         no mesmo formato do arquivo `parpeol.dat`.
 
-        - UEE (`str`)
+        - uee (`str`)
         - Data (`date`)
         - Lag 1 (`float`)
         - Lag 2 (`float`)
         - ...
         - Lag 11 (`float`)
 
         :return: A tabela como um DataFrame
@@ -315,15 +295,15 @@
     @property
     def correlacao_series_ruidos_uee(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação das séries de ruídos para
         todas as configurações vigentes e UEEs,
         no mesmo formato do arquivo `parpeol.dat`.
 
-        - UEE (`str`)
+        - uee (`str`)
         - Data (`date`)
         - Lag 1 (`float`)
         - Lag 2 (`float`)
         - ...
         - Lag 11 (`float`)
 
         :return: A tabela como um DataFrame
@@ -340,16 +320,16 @@
 
     @property
     def correlacao_espacial_anual(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação para todas as configurações
         e REEs / UEEs, no mesmo formato do arquivo `parpeol.dat`.
 
-        - Configuração (`int`)
-        - UEE (`str`)
+        - configuracao (`int`)
+        - uee (`str`)
         - <Nome do REE 1> (`str`)
         - <Nome do REE 2> (`str`)
         - ...
         - <Nome do REE N> (`str`)
         - <Nome da UEE 1> (`str`)
         - ...
         - <Nome da UEE M> (`str`)
@@ -365,17 +345,17 @@
 
     @property
     def correlacao_espacial_mensal(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação para todas as configurações
         e REEs / UEEs, no mesmo formato do arquivo `parpeol.dat`.
 
-        - Configuração (`int`)
-        - REE (`str`)
-        - MES (`int`)
+        - configuracao (`int`)
+        - uee (`str`)
+        - mes (`int`)
         - <Nome do REE 1> (`str`)
         - <Nome do REE 2> (`str`)
         - ...
         - <Nome do REE N> (`str`)
         - <Nome da UEE 1> (`str`)
         - ...
         - <Nome da UEE M> (`str`)
```

### Comparing `inewave-0.0.97/inewave/newave/parpvaz.py` & `inewave-0.0.98/inewave/newave/parpvaz.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class PARpvaz(BlockFile):
+class Parpvaz(BlockFile):
     """
     Armazena os dados de saída do NEWAVE referentes aos modelos e às
     séries sintéticas de vazões geradas pelo PAR(p).
 
 
     Esta classe lida com informações de saída do NEWAVE e
     cujas saídas devem ser compatíveis com as observadas através
@@ -53,15 +53,15 @@
         self.__ordem_final_modelo = None
         self.__coeficientes = None
         self.__correl_espacial_anual_mensal = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="parpvaz.dat"
-    ) -> "PARpvaz":
+    ) -> "Parpvaz":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
@@ -71,15 +71,15 @@
 
         :return: Os nomes das UHEs
         :rtype: List[str]
         """
         if self.series_vazoes_uhe is None:
             return None
         else:
-            return self.series_vazoes_uhe["UHE"].unique().tolist()
+            return self.series_vazoes_uhe["uhe"].unique().tolist()
 
     def __concatena_dados(self, bloco: Type[Block]) -> Optional[Any]:
         """
         Obtém os dados de um bloco se este existir dentre os blocos do arquivo.
 
         :param bloco: O tipo do bloco cujos dados serão extraídos
         :type bloco: Type[T]
@@ -122,16 +122,16 @@
                 f"{df.shape[0]} linhas não podem ser "
                 + f"divididas em {len(uhes)} grupos"
             )
         cols = list(df.columns)
         col_uhe: List[str] = []
         for uhe in uhes:
             col_uhe += [uhe] * int(linhas_por_uhe)
-        df["UHE"] = col_uhe
-        return df[["UHE"] + cols]
+        df["uhe"] = col_uhe
+        return df[["uhe"] + cols]
 
     def __adiciona_coluna_uhe_com_estagios(
         self, df: pd.DataFrame
     ) -> pd.DataFrame:
         """
         Adiciona uma coluna com as UHEs de cada amostra e outra
         com o estágio de cada uma, assumindo
@@ -153,17 +153,17 @@
             )
         cols = list(df.columns)
         col_uhe: List[str] = []
         col_estagio: List[int] = []
         for uhe in uhes:
             col_uhe += [uhe] * int(linhas_por_uhe)
             col_estagio += list(range(1, int(linhas_por_uhe) + 1))
-        df["UHE"] = col_uhe
-        df["Estágio"] = col_estagio
-        return df[["UHE", "Estágio"] + cols]
+        df["uhe"] = col_uhe
+        df["estagio"] = col_estagio
+        return df[["uhe", "estagio"] + cols]
 
     def __adiciona_coluna_uhe_corrigindo_pre_pos(
         self, df: Optional[pd.DataFrame]
     ) -> Optional[pd.DataFrame]:
         """
         Adiciona uma coluna com as UHEs de cada amostra e outra
         com o estágio de cada uma, assumindo
@@ -215,61 +215,61 @@
                 f"{df.shape[0]} linhas não podem ser "
                 + f"divididas em {len(uhes)} grupos"
             )
         cols = list(df.columns)
         col_uhe: List[str] = []
         for uhe in uhes:
             col_uhe += [uhe] * int(linhas_por_uhe)
-        df["UHE"] = col_uhe
+        df["uhe"] = col_uhe
         uhe0 = uhes[0]
-        ano0 = df["Ano"].unique().tolist()[0]
-        filtro = (df["Ano"] == ano0) & (df["UHE"] == uhe0)
+        ano0 = df["ano"].unique().tolist()[0]
+        filtro = (df["ano"] == ano0) & (df["uhe"] == uhe0)
         n_series = df.loc[filtro].shape[0]
         for i, uhe in enumerate(uhes):
             i_i = i * int(linhas_por_uhe)
             i_f = i_i + int(linhas_por_uhe) - 1
-            df.loc[i_i:i_f, "Ano"] = converte_vetor_anos(
-                df.loc[i_i:i_f, "Ano"].tolist(), n_series
+            df.loc[i_i:i_f, "ano"] = converte_vetor_anos(
+                df.loc[i_i:i_f, "ano"].tolist(), n_series
             )
-        return df[["UHE"] + cols]
+        return df[["uhe"] + cols]
 
     @property
     def series_vazoes_uhe(self) -> Optional[pd.DataFrame]:
         """
         A tabela de séries de vazões para todas as configurações
         e UHEs, no mesmo formato do arquivo `parpvaz.dat`.
 
-        - UHE (`str`)
-        - Configuração (`int`)
-        - Ano (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - uhe (`str`)
+        - configuracao (`int`)
+        - ano (`int`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__series_vazoes is None:
             self.__series_vazoes = self.__concatena_dados(BlocoSerieVazoesUHE)
         return self.__series_vazoes
 
     @property
     def series_ruido_uhe(self) -> Optional[pd.DataFrame]:
         """
         A tabela de séries de ruído para todas as UHEs,
         no mesmo formato do arquivo `parpvaz.dat`.
 
-        - UHE (`str`)
-        - Ano (`int`)
+        - uhe (`str`)
+        - ano (`int`)
         - Série (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__series_ruido is None:
             self.__series_ruido = self.__concatena_dados(BlocoSerieRuidosUHE)
             self.__series_ruido = (
@@ -282,20 +282,20 @@
     @property
     def correlacao_series_vazoes_uhe(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação das séries de vazões para
         todas as configurações vigentes e UHEs,
         no mesmo formato do arquivo `parpvaz.dat`.
 
-        - UHE (`str`)
-        - Data (`date`)
-        - Lag 1 (`float`)
-        - Lag 2 (`float`)
+        - uhe (`str`)
+        - data (`date`)
+        - lag_1 (`float`)
+        - lag_2 (`float`)
         - ...
-        - Lag 11 (`float`)
+        - lag_11 (`float`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
         if self.__correl_series_vazoes is None:
             self.__correl_series_vazoes = self.__concatena_dados(
                 BlocoCorrelVazoesUHE
@@ -308,20 +308,20 @@
     @property
     def correlacao_parcial_series_vazoes_uhe(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação das séries de vazões para
         todas as configurações vigentes e UHEs,
         no mesmo formato do arquivo `parpvaz.dat`.
 
-        - UHE (`str`)
-        - Data (`date`)
-        - Lag 1 (`float`)
-        - Lag 2 (`float`)
+        - uhe (`str`)
+        - data (`date`)
+        - lag_1 (`float`)
+        - lag_2 (`float`)
         - ...
-        - Lag 11 (`float`)
+        - lag_11 (`float`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
         if self.__correl_parcial_series_vazoes is None:
             self.__correl_parcial_series_vazoes = self.__concatena_dados(
                 BlocoCorrelParcialVazoesUHE
@@ -334,20 +334,20 @@
     @property
     def correlacao_series_ruidos_uhe(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação das séries de ruídos para
         todas as configurações vigentes e UHEs,
         no mesmo formato do arquivo `parpvaz.dat`.
 
-        - UHE (`str`)
-        - Data (`date`)
-        - Lag 1 (`float`)
-        - Lag 2 (`float`)
+        - uhe (`str`)
+        - data (`date`)
+        - lag_1 (`float`)
+        - lag_2 (`float`)
         - ...
-        - Lag 11 (`float`)
+        - lag_11 (`float`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
         if self.__correl_series_ruido is None:
             self.__correl_series_ruido = self.__concatena_dados(
                 BlocoCorrelRuidosUHE
@@ -360,87 +360,87 @@
     @property
     def ordem_original_modelo(self) -> Optional[pd.DataFrame]:
         """
         A tabela de ordens originais do modelo PAR ou PAR-A
         de cada UHE, no mesmo formato do arquivo `parpvaz.dat`,
         organizada por ano de estudo.
 
-        - UHE (`str`)
-        - Ano (`int`)
-        - Janeiro (`int`)
-        - Fevereiro (`int`)
+        - uhe (`str`)
+        - ano (`int`)
+        - janeiro (`int`)
+        - fevereiro (`int`)
         - ...
-        - Dezembro (`int`)
+        - dezembro (`int`)
 
         :return: A tabela como um DataFrame
         :rtype: pd.DataFrame | None
         """
 
         if self.__ordem_original_modelo is None:
             dados = self.__concatena_dados(BlocoOrdemModeloUHE)
             if dados is not None:
                 dados = (
-                    dados.loc[dados["Tipo"] == "ORIGINAL", :]
-                    .drop(columns=["Tipo"])
+                    dados.loc[dados["tipo"] == "ORIGINAL", :]
+                    .drop(columns=["tipo"])
                     .copy()
                 )
                 dados = self.__adiciona_coluna_uhe(dados)
                 self.__ordem_original_modelo = dados
 
         return self.__ordem_original_modelo
 
     @property
     def ordem_final_modelo(self) -> Optional[pd.DataFrame]:
         """
         A tabela de ordens finais do modelo PAR ou PAR-A
         de cada UHE, no mesmo formato do arquivo `parpvaz.dat`,
         organizada por ano de estudo.
 
-        - UHE (`str`)
-        - Ano (`int`)
-        - Janeiro (`int`)
-        - Fevereiro (`int`)
+        - uhe (`str`)
+        - ano (`int`)
+        - janeiro (`int`)
+        - fevereiro (`int`)
         - ...
-        - Dezembro (`int`)
+        - dezembro (`int`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__ordem_final_modelo is None:
             dados = self.__concatena_dados(BlocoOrdemModeloUHE)
             if dados is not None:
                 dados = (
-                    dados.loc[dados["Tipo"] == "FINAL", :]
-                    .drop(columns=["Tipo"])
+                    dados.loc[dados["tipo"] == "FINAL", :]
+                    .drop(columns=["tipo"])
                     .copy()
                 )
                 dados = self.__adiciona_coluna_uhe(dados)
                 self.__ordem_final_modelo = dados
 
         return self.__ordem_final_modelo
 
     @property
     def coeficientes(self) -> Optional[pd.DataFrame]:
         """
         Lista de coeficientes dos modelos PAR ou PAR-A
         de cada UHE, no mesmo formato do arquivo `parpvaz.dat`,
         organizada por período de estudo.
 
-        - UHE (`str`)
-        - Estágio (`int`)
-        - Psi 1 (`int`)
-        - Psi 2 (`int`)
+        - uhe (`str`)
+        - estagio (`int`)
+        - psi_1 (`int`)
+        - psi_2 (`int`)
         - ...
-        - Psi 11 (`int`)
-        - Psi A (`int`)
-        - Psi Norm 1 (`int`)
-        - Psi Norm 2 (`int`)
+        - psi_11 (`int`)
+        - psi_A (`int`)
+        - psi_norm_1 (`int`)
+        - psi_norm_2 (`int`)
         - ...
-        - Psi Norm 11 (`int`)
-        - Psi Norm A (`int`)
+        - psi_norm_11 (`int`)
+        - psi_norm_A (`int`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__coeficientes is None:
             dados = self.__concatena_dados(BlocoCoeficientesModeloUHE)
             if dados is not None:
@@ -451,21 +451,21 @@
 
     @property
     def correlacao_espacial_anual_mensal(self) -> Optional[pd.DataFrame]:
         """
         A tabela de correlação para todas as UHEs,
         no mesmo formato do arquivo `parpvaz.dat`.
 
-        - UHE 1 (`str`)
-        - UHE 2 (`str`)
-        - Janeiro (`str`)
-        - Fevereiro (`str`)
+        - uhe_1 (`str`)
+        - uhe_2 (`str`)
+        - janeiro (`str`)
+        - fevereiro (`str`)
         - ...
-        - Dezembro (`str`)
-        - Anual (`str`)
+        - dezembro (`str`)
+        - anual (`str`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
         if self.__correl_espacial_anual_mensal is None:
             self.__correl_espacial_anual_mensal = self.__concatena_dados(
                 BlocoCorrelEspacialAnualMensalUHE
```

### Comparing `inewave-0.0.97/inewave/newave/patamar.py` & `inewave-0.0.98/inewave/newave/sistema.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,201 +1,187 @@
-from inewave.newave.modelos.patamar import (
-    BlocoNumeroPatamares,
-    BlocoDuracaoPatamar,
-    BlocoCargaPatamar,
-    BlocoIntercambioPatamarSubsistemas,
-    BlocoUsinasNaoSimuladas,
+from inewave.newave.modelos.sistema import (
+    BlocoCustosDeficit,
+    BlocoGeracaoUsinasNaoSimuladas,
+    BlocoIntercambioSubsistema,
+    BlocoMercadoEnergiaSistema,
+    BlocoNumeroPatamaresDeficit,
 )
 
+
 from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Patamar(SectionFile):
+class Sistema(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes aos
-    patamares de carga por submercado.
+    Armazena os dados de entrada do NEWAVE referentes às configurações
+    dos subsistemas (submercados).
 
     """
 
     T = TypeVar("T")
 
     SECTIONS = [
-        BlocoNumeroPatamares,
-        BlocoDuracaoPatamar,
-        BlocoCargaPatamar,
-        BlocoIntercambioPatamarSubsistemas,
-        BlocoUsinasNaoSimuladas,
+        BlocoNumeroPatamaresDeficit,
+        BlocoCustosDeficit,
+        BlocoIntercambioSubsistema,
+        BlocoMercadoEnergiaSistema,
+        BlocoGeracaoUsinasNaoSimuladas,
     ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="patamar.dat"
-    ) -> "Patamar":
+        cls, diretorio: str, nome_arquivo="sistema.dat"
+    ) -> "Sistema":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="patamar.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="sistema.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
-    def numero_patamares(self) -> Optional[int]:
+    def numero_patamares_deficit(self) -> Optional[int]:
         """
-        O número de patamares utilizado no estudo.
+        O número de patamares de déficit utilizados no estudo.
 
         :return: O número de patamares como um inteiro
         :rtype: int | None
         """
-        b = self.__bloco_por_tipo(BlocoNumeroPatamares, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoNumeroPatamaresDeficit)
+        if isinstance(b, BlocoNumeroPatamaresDeficit):
             return b.data
         return None
 
-    @numero_patamares.setter
-    def numero_patamares(self, n: int):
-        b = self.__bloco_por_tipo(BlocoNumeroPatamares, 0)
-        if b is not None:
+    @numero_patamares_deficit.setter
+    def numero_patamares_deficit(self, n: int):
+        b = self.data.get_sections_of_type(BlocoNumeroPatamaresDeficit)
+        if isinstance(b, BlocoNumeroPatamaresDeficit):
             b.data = n
 
     @property
-    def duracao_mensal_patamares(self) -> Optional[pd.DataFrame]:
+    def custo_deficit(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com a duração mensal de cada patamar no horizonte
-        de estudo.
+        Tabela com o custo de cada patamar de déficit, por
+        subsistema.
 
-        - Ano (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - codigo_submercado (`int`)
+        - nome_submercado (`str`)
+        - ficticio (`int`)
+        - custo_deficit_patamar_1 (`float`)
         - ...
-        - Dezembro (`float`)
+        - custo_deficit_patamar_5 (`float`)
+        - corte_patamar_1 (`float`)
+        - ...
+        - corte_patamar_5 (`float`)
 
         :return: A duração por mês em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoDuracaoPatamar, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoCustosDeficit)
+        if isinstance(b, BlocoCustosDeficit):
             return b.data
         return None
 
-    @duracao_mensal_patamares.setter
-    def duracao_mensal_patamares(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoDuracaoPatamar, 0)
-        if b is not None:
+    @custo_deficit.setter
+    def custo_deficit(self, df: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoCustosDeficit)
+        if isinstance(b, BlocoCustosDeficit):
             b.data = df
 
     @property
-    def carga_patamares(self) -> Optional[pd.DataFrame]:
+    def limites_intercambio(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com a carga em P.U. por patamar.
+        Tabela com o limite de intercâmbio por par de
+        subsistemas.
 
-        - Ano (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - submercado_de (`int`)
+        - submercado_para (`int`)
+        - sentido (`int`)
+        - ano (`int`)
+        - janeiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
-        :return: A carga por mês em um DataFrame.
+        :return: A duração por mês em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoCargaPatamar, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoIntercambioSubsistema)
+        if isinstance(b, BlocoIntercambioSubsistema):
             return b.data
         return None
 
-    @carga_patamares.setter
-    def carga_patamares(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoCargaPatamar, 0)
-        if b is not None:
+    @limites_intercambio.setter
+    def limites_intercambio(self, df: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoIntercambioSubsistema)
+        if isinstance(b, BlocoIntercambioSubsistema):
             b.data = df
 
     @property
-    def intercambio_patamares(self) -> Optional[pd.DataFrame]:
+    def mercado_energia(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com a correção em P.U. do intercâmbio por patamar.
+        Tabela com o mercado total de energia por período de estudo.
 
-        - Subsistema De (`str`)
-        - Subsistema Para (`str`)
-        - Ano (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - submercado (`int`)
+        - ano (`int`)
+        - janeiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: A carga por mês em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoIntercambioPatamarSubsistemas, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoMercadoEnergiaSistema)
+        if isinstance(b, BlocoMercadoEnergiaSistema):
             return b.data
         return None
 
-    @intercambio_patamares.setter
-    def intercambio_patamares(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoIntercambioPatamarSubsistemas, 0)
-        if b is not None:
+    @mercado_energia.setter
+    def mercado_energia(self, df: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoMercadoEnergiaSistema)
+        if isinstance(b, BlocoMercadoEnergiaSistema):
             b.data = df
 
     @property
-    def usinas_nao_simuladas(self) -> Optional[pd.DataFrame]:
+    def geracao_usinas_nao_simuladas(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com os fatores das usinas não simuladas em P.U.
+        Tabela com a geração das usinas não simuladas por fonte
+        de geração.
 
-        - Subsistema (`int`)
-        - Patamar (`int`)
-        - Bloco (`int`)
-        - Ano (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - submercado (`int`)
+        - bloco (`int`)
+        - fonte (`str`)
+        - ano (`int`)
+        - janeiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
-        :return: Os valores por mês em um DataFrame.
+        :return: A carga por mês em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoUsinasNaoSimuladas, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoGeracaoUsinasNaoSimuladas)
+        if isinstance(b, BlocoGeracaoUsinasNaoSimuladas):
             return b.data
         return None
 
-    @usinas_nao_simuladas.setter
-    def usinas_nao_simuladas(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoUsinasNaoSimuladas, 0)
-        if b is not None:
+    @geracao_usinas_nao_simuladas.setter
+    def geracao_usinas_nao_simuladas(self, df: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoGeracaoUsinasNaoSimuladas)
+        if isinstance(b, BlocoGeracaoUsinasNaoSimuladas):
             b.data = df
```

### Comparing `inewave-0.0.97/inewave/newave/penalid.py` & `inewave-0.0.98/inewave/newave/penalid.py`

 * *Files 26% similar despite different names*

```diff
@@ -40,50 +40,30 @@
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def penalidades(self) -> Optional[pd.DataFrame]:
         """
         Tabela com as penalidades.
 
-        - Chave (`str`)
-        - Penalidade 1 (`float`)
-        - Penalidade 2 (`float`)
-        - Subsistema (`int`)
+        - mnemonico (`str`)
+        - penalidade_1 (`float`)
+        - penalidade_2 (`float`)
+        - submercado (`int`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoPenalidades, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoPenalidades)
+        if isinstance(b, BlocoPenalidades):
             return b.data
         return None
 
     @penalidades.setter
     def penalidades(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoPenalidades, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoPenalidades)
+        if isinstance(b, BlocoPenalidades):
             b.data = df
```

### Comparing `inewave-0.0.97/inewave/newave/perda.py` & `inewave-0.0.98/inewave/newave/perda.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/pmo.py` & `inewave-0.0.98/inewave/newave/pmo.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 from inewave.newave.modelos.pmo import BlocoConfiguracoesExpansaoPMO
 from inewave.newave.modelos.pmo import BlocoMARSPMO
 from inewave.newave.modelos.pmo import BlocoRiscoDeficitENSPMO
 from inewave.newave.modelos.pmo import BlocoCustoOperacaoPMO
 from inewave.newave.modelos.pmo import BlocoCustoOperacaoTotalPMO
 from inewave.newave.modelos.pmo import BlocoProdutibilidadesConfiguracaoPMO
 
-from cfinterface.components.block import Block
 from cfinterface.files.blockfile import BlockFile
-from typing import Type, TypeVar, Optional, Any
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class PMO(BlockFile):
+class Pmo(BlockFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao
     acompanhamento do programa.
 
     Esta classe lida com as informações de entrada fornecidas ao
     NEWAVE e reproduzidas no `pmo.dat`, bem como as saídas finais
     da execução: custos de operação, energias, déficit, etc.
@@ -43,271 +42,267 @@
         BlocoRiscoDeficitENSPMO,
         BlocoCustoOperacaoPMO,
         BlocoCustoOperacaoTotalPMO,
         BlocoProdutibilidadesConfiguracaoPMO,
     ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="pmo.dat") -> "PMO":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="pmo.dat") -> "Pmo":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
-    def __extrai_dados_se_existe(
-        self, bloco: Type[Block], indice: int = 0
-    ) -> Optional[Any]:
-        """
-        Obtém os dados de um bloco se este existir dentre os blocos do arquivo.
-
-        :param bloco: O tipo do bloco cujos dados serão extraídos
-        :type bloco: Type[T]
-        :param indice: Qual dos blocos do tipo será acessado
-        :type indice: int, optional
-        :return: Os dados do bloco, se existirem
-        :rtype: Any
-        """
-        b = self.__bloco_por_tipo(bloco, indice)
-        if b is not None:
-            return b.data
-        return None
-
     @property
     def eafpast_tendencia_hidrologica(self) -> Optional[pd.DataFrame]:
         """
         Energias afluentes passadas por REE para análise da tendência
         hidrológica, em relação à primeira configuração do sistema,
         em MWmes.
 
-        - REE (`str`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - ree (`str`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: A tendência hidrológica em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(BlocoEafPastTendenciaHidrolPMO)
+        b = self.data.get_blocks_of_type(BlocoEafPastTendenciaHidrolPMO)
+        if isinstance(b, BlocoEafPastTendenciaHidrolPMO):
+            return b.data
+        return None
 
     @property
     def eafpast_cfuga_medio(self) -> Optional[pd.DataFrame]:
         """
         Energias afluentes passadas por REE considerando canal de
         fuga médio, em relação à primeira configuração do sistema,
         em MWmes.
 
-        - REE (`str`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - ree (`str`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: As energias afluentes passadas.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(BlocoEafPastCfugaMedioPMO)
+        b = self.data.get_blocks_of_type(BlocoEafPastCfugaMedioPMO)
+        if isinstance(b, BlocoEafPastCfugaMedioPMO):
+            return b.data
+        return None
 
     @property
     def configuracoes_entrada_reservatorio(self) -> Optional[pd.DataFrame]:
         """
         Configurações do sistema em cada período devido a entrada
         de reservatórios e/ou potência de base.
 
-        - Ano (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - ano (`int`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: As configurações em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(BlocoConfiguracoesExpansaoPMO, 0)
+        b = self.data.get_blocks_of_type(BlocoConfiguracoesExpansaoPMO)
+        if isinstance(b, list):
+            return b[0].data
+        return None
 
     @property
     def configuracoes_alteracao_potencia(self) -> Optional[pd.DataFrame]:
         """
         Configurações do sistema em cada período devido a alterações
         de potência.
 
-        - Ano (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - ano (`int`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: As configurações em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(BlocoConfiguracoesExpansaoPMO, 1)
+        b = self.data.get_blocks_of_type(BlocoConfiguracoesExpansaoPMO)
+        if isinstance(b, list):
+            return b[1].data
+        return None
 
     @property
     def configuracoes_qualquer_modificacao(self) -> Optional[pd.DataFrame]:
         """
         Configurações do sistema em cada período devido a alterações
         de potência.
 
-        - Ano (`int`)
-        - Janeiro (`float`)
-        - Fevereiro (`float`)
+        - ano (`int`)
+        - janeiro (`float`)
+        - fevereiro (`float`)
         - ...
-        - Dezembro (`float`)
+        - dezembro (`float`)
 
         :return: As configurações em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(BlocoConfiguracoesExpansaoPMO, 2)
+        b = self.data.get_blocks_of_type(BlocoConfiguracoesExpansaoPMO)
+        if isinstance(b, list):
+            return b[2].data
+        return None
 
     def retas_perdas_engolimento(self, estagio: int) -> Optional[pd.DataFrame]:
         """
         Retas ajustadas segundo o modelo MARS para corrigir a
         energia fio d'água com as perdas por engolimento máximo.
 
-        - REE (`str`)
-        - Reta (`int`)
-        - Coeficiente Angular (`float`)
-        - Constante (`float`)
+        - ree (`str`)
+        - reta (`int`)
+        - coeficiente_angular (`float`)
+        - coeficiente_linear (`float`)
 
         :return: As retas em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(BlocoMARSPMO, estagio - 1)
+        b = self.data.get_blocks_of_type(BlocoMARSPMO)
+        if isinstance(b, list):
+            return b[estagio - 1].data
+        return None
 
     @property
     def convergencia(self) -> Optional[pd.DataFrame]:
         """
         Tabela de convergência da execução do NEWAVE.
 
-        - Iteração (`int`)
-        - Lim. Inf. ZINF (`float`)
-        - ZINF (`float`)
-        - Lim. Sup. ZINF (`float`)
-        - ZSUP (`float`)
-        - Delta ZINF (`float`)
-        - ZSUP Iteração (`float`)
+        - iteracao (`int`)
+        - limite_inferior_zinf (`float`)
+        - zinf (`float`)
+        - limite_superior_zinf (`float`)
+        - zsup (`float`)
+        - delta_zinf (`float`)
+        - zsup_iteracao (`float`)
+        - tempo (`timedelta`)
 
         :return: As convergência em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(BlocoConvergenciaPMO)
+        b = self.data.get_blocks_of_type(BlocoConvergenciaPMO)
+        if isinstance(b, BlocoConvergenciaPMO):
+            return b.data
+        return None
 
     @property
     def risco_deficit_ens(self) -> Optional[pd.DataFrame]:
         """
         Tabela de riscos de déficit e enegia não suprida (ENS).
 
-        - Ano (`int`)
-        - Risco - <nome_subsistema_1> (`float`)
-        - EENS - <nome_subsistema_1> (`float`)
+        - ano (`int`)
+        - risco_<nome_submercado_1> (`float`)
+        - eens_<nome_submercado_1> (`float`)
         - ...
-        - Risco - <nome_subsistema_N> (`float`)
-        - EENS - <nome_subsistema_N> (`float`)
+        - risco_<nome_submercado_N> (`float`)
+        - eens_<nome_submercado_N> (`float`)
 
         :return: Os ricos em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(BlocoRiscoDeficitENSPMO)
+        b = self.data.get_blocks_of_type(BlocoRiscoDeficitENSPMO)
+        if isinstance(b, BlocoRiscoDeficitENSPMO):
+            return b.data
+        return None
 
     @property
     def custo_operacao_series_simuladas(self) -> Optional[pd.DataFrame]:
         """
         Tabela de custos de operação categorizados para as
         séries simuladas.
 
-        - Parcela (`str`)
-        - Valor Esperado (`float`)
-        - Desvio Padrão do VE (`float`)
-        - (%) (`float`)
+        - parcela (`str`)
+        - valor_esperado (`float`)
+        - desvio_padrao (`float`)
+        - percentual (`float`)
 
         :return: Os custos em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(BlocoCustoOperacaoPMO, 0)
+        b = self.data.get_blocks_of_type(BlocoCustoOperacaoPMO)
+        if isinstance(b, list):
+            return b[0].data
+        return None
 
     @property
     def valor_esperado_periodo_estudo(self) -> Optional[pd.DataFrame]:
         """
         Tabela de custos de operação esperados para o período
         de estudo.
 
-        - Parcela (`str`)
-        - Valor Esperado (`float`)
-        - Desvio Padrão do VE (`float`)
-        - (%) (`float`)
+        - parcela (`str`)
+        - valor_esperado (`float`)
+        - desvio_padrao (`float`)
+        - percentual (`float`)
 
         :return: Os custos em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(BlocoCustoOperacaoPMO, 1)
+        b = self.data.get_blocks_of_type(BlocoCustoOperacaoPMO)
+        if isinstance(b, list):
+            return b[1].data
+        return None
 
     @property
     def custo_operacao_referenciado_primeiro_mes(
         self,
     ) -> Optional[pd.DataFrame]:
         """
         Tabela de custos de operação esperados para o período
         de estudo, referenciados ao primeiro mês.
 
-        - Parcela (`str`)
-        - Valor Esperado (`float`)
-        - Desvio Padrão do VE (`float`)
-        - (%) (`float`)
+        - parcela (`str`)
+        - valor_esperado (`float`)
+        - desvio_padrao (`float`)
+        - percentual (`float`)
 
         :return: Os custos em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(BlocoCustoOperacaoPMO, 2)
+        b = self.data.get_blocks_of_type(BlocoCustoOperacaoPMO)
+        if isinstance(b, list):
+            return b[2].data
+        return None
 
     @property
     def custo_operacao_total(self) -> Optional[float]:
         """
         Custo de operacao total da SF.
 
         :return: O custo total.
         :rtype: float | None
         """
-        b = self.__extrai_dados_se_existe(BlocoCustoOperacaoTotalPMO)
-        if isinstance(b, list):
-            return b[0]
+        b = self.data.get_blocks_of_type(BlocoCustoOperacaoTotalPMO)
+        if isinstance(b, BlocoCustoOperacaoTotalPMO):
+            return b.data[0]
         return None
 
     @property
     def desvio_custo_operacao_total(self) -> Optional[float]:
         """
         O desvio padrão do custo de operacao total da SF.
 
         :return: O desvio do custo total.
         :rtype: float | None
         """
-        b = self.__extrai_dados_se_existe(BlocoCustoOperacaoTotalPMO)
-        if isinstance(b, list):
-            return b[1]
+        b = self.data.get_blocks_of_type(BlocoCustoOperacaoTotalPMO)
+        if isinstance(b, BlocoCustoOperacaoTotalPMO):
+            return b.data[1]
         return None
 
     @property
     def produtibilidades_equivalentes(self) -> Optional[pd.DataFrame]:
         """
         Tabela de produtibilidades calculadas para diversos fins do NEWAVE
         por usina e por configuração.
@@ -329,10 +324,11 @@
         - produtibilidade_acumulada_calculo_evaporacao_altura_65 (`float`)
         - produtibilidade_acumulada_calculo_evaporacao_altura_maxima (`float`)
 
 
         :return: As produtibilidades em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        return self.__extrai_dados_se_existe(
-            BlocoProdutibilidadesConfiguracaoPMO, 0
-        )
+        b = self.data.get_blocks_of_type(BlocoProdutibilidadesConfiguracaoPMO)
+        if isinstance(b, BlocoProdutibilidadesConfiguracaoPMO):
+            return b.data
+        return None
```

### Comparing `inewave-0.0.97/inewave/newave/ree.py` & `inewave-0.0.98/inewave/newave/ree.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class REE(SectionFile):
+class Ree(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às configurações
     dos REEs.
 
     """
 
     T = TypeVar("T")
@@ -28,15 +28,15 @@
         BlocoFicticiasIndividualizado,
     ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="ree.dat") -> "REE":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="ree.dat") -> "Ree":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
@@ -45,70 +45,50 @@
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def rees(self) -> Optional[pd.DataFrame]:
         """
         Tabela com os REES e os submercados
 
-        - Número (`int`)
-        - Nome (`str`)
-        - Submercado (`int`)
-        - Mês Fim Individualizado (`int`)
-        - Ano Fim Individualizado (`int`)
+        - codigo (`int`)
+        - nome (`str`)
+        - submercado (`int`)
+        - mes_fim_individualizado (`int`)
+        - ano_fim_individualizado (`int`)
 
         :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoReesSubmercados, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoReesSubmercados)
+        if isinstance(b, BlocoReesSubmercados):
             return b.data
         return None
 
     @rees.setter
     def rees(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoReesSubmercados, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoReesSubmercados)
+        if isinstance(b, BlocoReesSubmercados):
             b.data = df
 
     @property
     def remocao_ficticias(self) -> Optional[int]:
         """
         Opção de remover usinas fictícias nos períodos individualizados.
 
         :return: O valor do campo.
         :rtype: int | None
         """
-        b = self.__bloco_por_tipo(BlocoFicticiasIndividualizado, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoFicticiasIndividualizado)
+        if isinstance(b, BlocoFicticiasIndividualizado):
             return b.data[1]
         return None
 
     @remocao_ficticias.setter
     def remocao_ficticias(self, d: int):
-        b = self.__bloco_por_tipo(BlocoFicticiasIndividualizado, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoFicticiasIndividualizado)
+        if isinstance(b, BlocoFicticiasIndividualizado):
             b.data[1] = d
```

### Comparing `inewave-0.0.97/inewave/newave/restricaoeletrica.py` & `inewave-0.0.98/inewave/newave/restricaoeletrica.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Type, TypeVar, List, Optional, Union
+from typing import TypeVar, List, Optional, Union
 from datetime import datetime
 
-from cfinterface.components.register import Register
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.restricaoeletrica import (
     RegistroRE,
     RegistroREHorizPer,
     RegistroRELimFormPer,
 )
 
@@ -49,84 +48,14 @@
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
-        """
-        Obtém os registro de um tipo, se houver algum no arquivo.
-
-        :param registro: Um tipo de registro para ser lido
-        :type registro: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-
-        """
-        return [b for b in self.data.of_type(registro)]
-
-    def __obtem_registros(self, tipo: Type[T]) -> List[T]:
-        return self.__registros_por_tipo(tipo)
-
-    def __obtem_registros_com_filtros(
-        self, tipo_registro: Type[T], **kwargs
-    ) -> Optional[Union[T, List[T]]]:
-        def __atende(r) -> bool:
-            condicoes: List[bool] = []
-            for k, v in kwargs.items():
-                if v is not None:
-                    condicoes.append(getattr(r, k) == v)
-            return all(condicoes)
-
-        regs_filtro = [
-            r for r in self.__obtem_registros(tipo_registro) if __atende(r)
-        ]
-        if len(regs_filtro) == 0:
-            return None
-        elif len(regs_filtro) == 1:
-            return regs_filtro[0]
-        else:
-            return regs_filtro
-
-    def cria_registro(self, anterior: Register, registro: Register):
-        """
-        Adiciona um registro ao arquivo após um outro registro previamente
-        existente.
-
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.add_after(anterior, registro)
-
-    def deleta_registro(self, registro: Register):
-        """
-        Remove um registro existente no arquivo.
-
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.remove(registro)
-
-    def append_registro(self, registro: Register):
-        """
-        Adiciona um registro ao arquivo na última posição.
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.append(registro)
-
-    def preppend_registro(self, registro: Register):
-        """
-        Adiciona um registro ao arquivo na primeira posição.
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.preppend(registro)
-
     def re(
         self,
         codigo_restricao: Optional[int] = None,
         formula: Optional[str] = None,
     ) -> Optional[Union[RegistroRE, List[RegistroRE]]]:
         """
         Obtém um registro que cadastra uma usina restrição elétrica (RE).
@@ -135,15 +64,15 @@
         :type codigo_restricao: int | None
         :param formula: equação da restrição
         :type formula: str | None
         :return: Um ou mais registros, se existirem.
         :rtype: :class:`RegistroRE` |
             list[:class:`RegistroRE`] | None
         """
-        return self.__obtem_registros_com_filtros(
+        return self.data.get_registers_of_type(
             RegistroRE,
             codigo_restricao=codigo_restricao,
             formula=formula,
         )
 
     def re_horiz_per(
         self,
@@ -161,15 +90,15 @@
         :type data_inicial: datetime | None
         :param data_final: data final de validade da restrição
         :type data_final: datetime | None
         :return: Um ou mais registros, se existirem.
         :rtype: :class:`RegistroREHorizPer` |
             list[:class:`RegistroREHorizPer`] | None
         """
-        return self.__obtem_registros_com_filtros(
+        return self.data.get_registers_of_type(
             RegistroREHorizPer,
             codigo_restricao=codigo_restricao,
             data_inicial=data_inicial,
             data_final=data_final,
         )
 
     def re_lim_form_per(
@@ -197,15 +126,15 @@
         :type limite_inferior: float | None
         :param limite_superior: limite superior da restrição
         :type limite_superior: float | None
         :return: Um ou mais registros, se existirem.
         :rtype: :class:`RegistroRELimFormPer` |
             list[:class:`RegistroRELimFormPer`] | None
         """
-        return self.__obtem_registros_com_filtros(
+        return self.data.get_registers_of_type(
             RegistroRELimFormPer,
             codigo_restricao=codigo_restricao,
             data_inicial=data_inicial,
             data_final=data_final,
             patamar=patamar,
             limite_inferior=limite_inferior,
             limite_superior=limite_superior,
```

### Comparing `inewave-0.0.97/inewave/newave/restricaoenergia.py` & `inewave-0.0.98/inewave/newave/restricaovazao.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,205 +1,134 @@
-from typing import Type, TypeVar, List, Optional, Union
+from typing import TypeVar, List, Optional, Union
 from datetime import datetime
 
-from cfinterface.components.register import Register
 from cfinterface.files.registerfile import RegisterFile
-from inewave.newave.modelos.restricaoenergia import (
-    RegistroRHE,
-    RegistroRHEHorizPer,
-    RegistroRHELsLPPEarmi,
+from inewave.newave.modelos.restricaovazao import (
+    RegistroRHQ,
+    RegistroRHQHorizPer,
+    RegistroRHQLsLPPVoli,
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class RestricaoEnergia(RegisterFile):
+class RestricaoVazao(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao cadastro
-    das restrições lineares por partes no domínio de energia (REE).
+    das restrições lineares por partes no domínio de vazão (RHQ).
     """
 
     T = TypeVar("T")
 
     REGISTERS = [
-        RegistroRHELsLPPEarmi,
-        RegistroRHEHorizPer,
-        RegistroRHE,
+        RegistroRHQLsLPPVoli,
+        RegistroRHQHorizPer,
+        RegistroRHQ,
     ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="restricao-energia.csv"
-    ) -> "RestricaoEnergia":
+        cls, diretorio: str, nome_arquivo="restricao-vazao.csv"
+    ) -> "RestricaoVazao":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
     def escreve_arquivo(
-        self, diretorio: str, nome_arquivo="restricao-energia.csv"
+        self, diretorio: str, nome_arquivo="restricao-vazao.csv"
     ):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __registros_por_tipo(self, registro: Type[T]) -> List[T]:
-        """
-        Obtém os registro de um tipo, se houver algum no arquivo.
-
-        :param registro: Um tipo de registro para ser lido
-        :type registro: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-
-        """
-        return [b for b in self.data.of_type(registro)]
-
-    def __obtem_registros(self, tipo: Type[T]) -> List[T]:
-        return self.__registros_por_tipo(tipo)
-
-    def __obtem_registros_com_filtros(
-        self, tipo_registro: Type[T], **kwargs
-    ) -> Optional[Union[T, List[T]]]:
-        def __atende(r) -> bool:
-            condicoes: List[bool] = []
-            for k, v in kwargs.items():
-                if v is not None:
-                    condicoes.append(getattr(r, k) == v)
-            return all(condicoes)
-
-        regs_filtro = [
-            r for r in self.__obtem_registros(tipo_registro) if __atende(r)
-        ]
-        if len(regs_filtro) == 0:
-            return None
-        elif len(regs_filtro) == 1:
-            return regs_filtro[0]
-        else:
-            return regs_filtro
-
-    def cria_registro(self, anterior: Register, registro: Register):
-        """
-        Adiciona um registro ao arquivo após um outro registro previamente
-        existente.
-
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.add_after(anterior, registro)
-
-    def deleta_registro(self, registro: Register):
-        """
-        Remove um registro existente no arquivo.
-
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.remove(registro)
-
-    def append_registro(self, registro: Register):
-        """
-        Adiciona um registro ao arquivo na última posição.
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.append(registro)
-
-    def preppend_registro(self, registro: Register):
-        """
-        Adiciona um registro ao arquivo na primeira posição.
-        Este método existe para retrocompatibilidade e deve ser substituído
-        quando for suportado na classe :class:`RegisterFile`.
-        """
-        self.data.preppend(registro)
-
-    def rhe(
+    def rhq(
         self,
         codigo_restricao: Optional[int] = None,
         formula: Optional[str] = None,
-    ) -> Optional[Union[RegistroRHE, List[RegistroRHE]]]:
+    ) -> Optional[Union[RegistroRHQ, List[RegistroRHQ]]]:
         """
         Obtém um registro que cadastra uma usina restrição linear por
-        partes de energia (REE).
+        partes de vazão (UHE).
 
         :param codigo_restricao: código que especifica a restrição
         :type codigo_restricao: int | None
         :param formula: equação da restrição
         :type formula: str | None
         :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroRHE` |
-            list[:class:`RegistroRHE`] | None
+        :rtype: :class:`RegistroRHQ` |
+            list[:class:`RegistroRHQ`] | None
         """
-        return self.__obtem_registros_com_filtros(
-            RegistroRHE,
+        return self.data.get_registers_of_type(
+            RegistroRHQ,
             codigo_restricao=codigo_restricao,
             formula=formula,
         )
 
-    def rhe_horiz_per(
+    def rhq_horiz_per(
         self,
         codigo_restricao: Optional[int] = None,
         data_inicial: Optional[datetime] = None,
         data_final: Optional[datetime] = None,
-    ) -> Optional[Union[RegistroRHEHorizPer, List[RegistroRHEHorizPer]]]:
+    ) -> Optional[Union[RegistroRHQHorizPer, List[RegistroRHQHorizPer]]]:
         """
         Obtém um registro que cadastra o horizonte de validade de uma
-        restrição linear por partes de energia.
+        restrição linear por partes de vazão.
 
         :param codigo_restricao: código que especifica a restrição
         :type codigo_restricao: int | None
         :param data_inicial: data inicial de validade da restrição
         :type data_inicial: datetime | None
         :param data_final: data final de validade da restrição
         :type data_final: datetime | None
         :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroRHEHorizPer` |
-            list[:class:`RegistroRHEHorizPer`] | None
+        :rtype: :class:`RegistroRHQHorizPer` |
+            list[:class:`RegistroRHQHorizPer`] | None
         """
-        return self.__obtem_registros_com_filtros(
-            RegistroRHEHorizPer,
+        return self.data.get_registers_of_type(
+            RegistroRHQHorizPer,
             codigo_restricao=codigo_restricao,
             data_inicial=data_inicial,
             data_final=data_final,
         )
 
-    def rhe_ls_lpp_earmi(
+    def rhq_ls_lpp_voli(
         self,
         codigo_restricao: Optional[int] = None,
         indice_reta: Optional[int] = None,
         coeficiente_angular: Optional[float] = None,
         coeficiente_linear: Optional[float] = None,
-    ) -> Optional[Union[RegistroRHELsLPPEarmi, List[RegistroRHELsLPPEarmi]]]:
+    ) -> Optional[Union[RegistroRHQLsLPPVoli, List[RegistroRHQLsLPPVoli]]]:
         """
         Obtém um registro que cadastra as retas da restrição linear
-        por partes de energia.
+        por partes de vazão.
 
         :param codigo_restricao: código que especifica a restrição
         :type codigo_restricao: int | None
         :param indice_reta: índice da reta definida
         :type indice_reta: int | None
         :param coeficiente_angular: coeficiente angular da reta
         :type coeficiente_angular: float | None
         :param coeficiente_linear: coeficiente linear da reta
         :type coeficiente_linear: float | None
         :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroRHELsLPPEarmi` |
-            list[:class:`RegistroRHELsLPPEarmi`] | None
+        :rtype: :class:`RegistroRHQLsLPPVoli` |
+            list[:class:`RegistroRHQLsLPPVoli`] | None
         """
-        return self.__obtem_registros_com_filtros(
-            RegistroRHELsLPPEarmi,
+        return self.data.get_registers_of_type(
+            RegistroRHQLsLPPVoli,
             codigo_restricao=codigo_restricao,
             indice_reta=indice_reta,
             coeficiente_angular=coeficiente_angular,
             coeficiente_linear=coeficiente_linear,
         )
```

### Comparing `inewave-0.0.97/inewave/newave/sar.py` & `inewave-0.0.98/inewave/newave/sar.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from typing import TypeVar, List, Type
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class SAR(SectionFile):
+class Sar(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes à superfície de
     aversão à risco (SAR).
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="sar.dat") -> "SAR":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="sar.dat") -> "Sar":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/newave/tecno.py` & `inewave-0.0.98/inewave/newave/tecno.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/term.py` & `inewave-0.0.98/inewave/newave/vazaob.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,74 @@
-from inewave.newave.modelos.term import BlocoTermUTE
-
 from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from inewave.newave.modelos.vazaob import SecaoDadosVazaob
 import pandas as pd  # type: ignore
 
+from typing import TypeVar, Optional
+
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Term(SectionFile):
+class Vazaob(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes aos dados das
-    usinas térmicas.
+    Armazena os dados de saída do NEWAVE referentes às séries sintéticas
+    de vazão para a etapa backward geradas pelo modelo.
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [BlocoTermUTE]
+    SECTIONS = [SecaoDadosVazaob]
+    STORAGE = "BINARY"
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="term.dat") -> "Term":
+    def le_arquivo(
+        cls,
+        diretorio: str,
+        nome_arquivo="vazaob.dat",
+        numero_forwards: int = 200,
+        numero_aberturas: int = 20,
+        numero_uhes: int = 164,
+        numero_estagios: int = 60,
+    ) -> "Vazaob":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="term.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
+        return cls.read(
+            join(diretorio, nome_arquivo),
+            numero_forwards=numero_forwards,
+            numero_aberturas=numero_aberturas,
+            numero_uhes=numero_uhes,
+            numero_estagios=numero_estagios,
         )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
 
     @property
-    def usinas(self) -> Optional[pd.DataFrame]:
+    def series(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com configurações e custos das usinas térmicas.
+        Obtém a tabela com os dados das séries de vazão
+        afluente por UHE, por estágio, série forward e abertura.
 
-        - Número (`int`)
-        - Nome (`str`)
-        - Potência Instalada (`float`)
-        - FC Máximo (`float`)
-        - TEIF (`float`)
-        - Indisponibilidade Programada (`float`)
-        - GT Min Janeiro (`float`)
-        - ...
-        - GT Min Dezembro (`float`)
-        - GT Min D+ Anos (`float`)
+        - estagio (`int`): estágio do cenário gerado
+        - uhe (`int`): UHE para a qual foi gerado
+        - serie (`int`): índice da série forward
+        - abertura (`int`): índice da abertura
+        - valor (`float`): energia em MWmes
 
-        :return: A tabela como um DataFrame
+        :return: A tabela com os dados das séries
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoTermUTE, 0)
-        if b is not None:
-            return b.data
-        return None
-
-    @usinas.setter
-    def usinas(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoTermUTE, 0)
-        if b is not None:
-            b.data = df
+        sections = [r for r in self.data.of_type(SecaoDadosVazaob)]
+        if len(sections) > 0:
+            return sections[0].data
+        else:
+            return None
+
+    @series.setter
+    def series(self, df: pd.DataFrame):
+        sections = [r for r in self.data.of_type(SecaoDadosVazaob)]
+        if len(sections) > 0:
+            sections[0].data = df
```

### Comparing `inewave-0.0.97/inewave/newave/vazaob.py` & `inewave-0.0.98/inewave/newave/vazaof.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,73 @@
 from cfinterface.files.sectionfile import SectionFile
-from inewave.newave.modelos.vazaob import SecaoDadosVazaob
+from inewave.newave.modelos.vazaof import SecaoDadosVazaof
 import pandas as pd  # type: ignore
 
 from typing import TypeVar, Optional
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Vazaob(SectionFile):
+class Vazaof(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes às séries sintéticas
-    de vazão para a etapa backward geradas pelo modelo.
+    de vazão para a etapa forward geradas pelo modelo.
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [SecaoDadosVazaob]
+    SECTIONS = [SecaoDadosVazaof]
     STORAGE = "BINARY"
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls,
         diretorio: str,
-        nome_arquivo="vazaob.dat",
+        nome_arquivo="vazaof.dat",
         numero_forwards: int = 200,
-        numero_aberturas: int = 20,
         numero_uhes: int = 164,
         numero_estagios: int = 60,
-    ) -> "Vazaob":
+        numero_estagios_th: int = 12,
+    ) -> "Vazaof":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(
             join(diretorio, nome_arquivo),
             numero_forwards=numero_forwards,
-            numero_aberturas=numero_aberturas,
             numero_uhes=numero_uhes,
             numero_estagios=numero_estagios,
+            numero_estagios_th=numero_estagios_th,
         )
 
     @property
     def series(self) -> Optional[pd.DataFrame]:
         """
         Obtém a tabela com os dados das séries de vazão
-        afluente por UHE, por estágio, série forward e abertura.
+        afluente por UHE e por estágio.
 
         - estagio (`int`): estágio do cenário gerado
         - uhe (`int`): UHE para a qual foi gerado
         - serie (`int`): índice da série forward
-        - abertura (`int`): índice da abertura
-        - valor (`float`): energia em MWmes
+        - valor (`float`): vazão em hm3
 
         :return: A tabela com os dados das séries
         :rtype: pd.DataFrame | None
         """
-        sections = [r for r in self.data.of_type(SecaoDadosVazaob)]
+        sections = [r for r in self.data.of_type(SecaoDadosVazaof)]
         if len(sections) > 0:
             return sections[0].data
         else:
             return None
 
     @series.setter
     def series(self, df: pd.DataFrame):
-        sections = [r for r in self.data.of_type(SecaoDadosVazaob)]
+        sections = [r for r in self.data.of_type(SecaoDadosVazaof)]
         if len(sections) > 0:
             sections[0].data = df
```

### Comparing `inewave-0.0.97/inewave/newave/vazaof.py` & `inewave-0.0.98/inewave/newave/vazaos.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 from cfinterface.files.sectionfile import SectionFile
-from inewave.newave.modelos.vazaof import SecaoDadosVazaof
+from inewave.newave.modelos.vazaos import SecaoDadosVazaos
 import pandas as pd  # type: ignore
 
 from typing import TypeVar, Optional
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Vazaof(SectionFile):
+class Vazaos(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes às séries sintéticas
-    de vazão para a etapa forward geradas pelo modelo.
+    de vazão para a simulação final geradas pelo modelo.
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [SecaoDadosVazaof]
+    SECTIONS = [SecaoDadosVazaos]
     STORAGE = "BINARY"
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls,
         diretorio: str,
-        nome_arquivo="vazaof.dat",
-        numero_forwards: int = 200,
+        nome_arquivo="vazaos.dat",
+        numero_series: int = 2000,
         numero_uhes: int = 164,
         numero_estagios: int = 60,
         numero_estagios_th: int = 12,
-    ) -> "Vazaof":
+    ) -> "Vazaos":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(
             join(diretorio, nome_arquivo),
-            numero_forwards=numero_forwards,
+            numero_series=numero_series,
             numero_uhes=numero_uhes,
             numero_estagios=numero_estagios,
             numero_estagios_th=numero_estagios_th,
         )
 
     @property
     def series(self) -> Optional[pd.DataFrame]:
         """
         Obtém a tabela com os dados das séries de vazão
         afluente por UHE e por estágio.
 
         - estagio (`int`): estágio do cenário gerado
         - uhe (`int`): UHE para a qual foi gerado
-        - serie (`int`): índice da série forward
+        - serie (`int`): índice da série sintética
         - valor (`float`): vazão em hm3
 
         :return: A tabela com os dados das séries
         :rtype: pd.DataFrame | None
         """
-        sections = [r for r in self.data.of_type(SecaoDadosVazaof)]
+        sections = [r for r in self.data.of_type(SecaoDadosVazaos)]
         if len(sections) > 0:
             return sections[0].data
         else:
             return None
 
     @series.setter
     def series(self, df: pd.DataFrame):
-        sections = [r for r in self.data.of_type(SecaoDadosVazaof)]
+        sections = [r for r in self.data.of_type(SecaoDadosVazaos)]
         if len(sections) > 0:
             sections[0].data = df
```

### Comparing `inewave-0.0.97/inewave/newave/vazoes.py` & `inewave-0.0.98/inewave/newave/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/newave/vazpast.py` & `inewave-0.0.98/inewave/newave/agrint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,101 @@
-from inewave.newave.modelos.vazpast import BlocoVazPast
+from inewave.newave.modelos.agrint import (
+    BlocoGruposAgrint,
+    BlocoLimitesPorGrupoAgrint,
+)
 
 from cfinterface.files.sectionfile import SectionFile
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class VazPast(SectionFile):
+class Agrint(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às
-    vazões anteriores ao período de planejamento.
-
-    Esta classe lida com informações de entrada fornecidas ao NEWAVE e
-    que são usadas juntos das contidas no arquivo `vazoes.dat`.
+    Armazena os dados de entrada do NEWAVE referentes aos agrupamentos
+    de intercâmbio.
 
     """
 
     T = TypeVar("T")
 
-    SECTIONS = [BlocoVazPast]
+    SECTIONS = [
+        BlocoGruposAgrint,
+        BlocoLimitesPorGrupoAgrint,
+    ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vazpast.dat"
-    ) -> "VazPast":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="agrint.dat") -> "Agrint":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="vazpast.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="agrint.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
+    @property
+    def agrupamentos(self) -> Optional[pd.DataFrame]:
         """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
+        Tabela com os intercâmbios em cada agrupamento.
 
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
+        - agrupamento (`int`)
+        - submercado_de (`int`)
+        - submercado_para (`int`)
+        - coeficiente (`float`)
+
+        :return: A tabela como um DataFrame.
+        :rtype: pd.DataFrame | None
         """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
+        b = self.data.get_sections_of_type(BlocoGruposAgrint)
+        if isinstance(b, BlocoGruposAgrint):
+            return b.data
+        return None
+
+    @agrupamentos.setter
+    def agrupamentos(self, df: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoGruposAgrint)
+        if isinstance(b, BlocoGruposAgrint):
+            b.data = df
 
     @property
-    def tendencia(self) -> Optional[pd.DataFrame]:
+    def limites_agrupamentos(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com a tendência hidrológica por REE.
+        Tabela com os limites dos agrupamentos de intercâmbio
+        durante o período de estudo.
 
-        - Índice (`int`)
-        - Usina (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - agrupamento (`int`)
+        - mes_inicio (`int`)
+        - ano_inicio (`int`)
+        - mes_fim (`int`)
+        - ano_fim (`int`)
+        - limite_p1 (`float`)
+        - limite_p2 (`float`)
+        - limite_p3 (`float`)
 
-        :return: A tabela como um DataFrame
+        :return: A tabela como um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.__bloco_por_tipo(BlocoVazPast, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoLimitesPorGrupoAgrint)
+        if isinstance(b, BlocoLimitesPorGrupoAgrint):
             return b.data
         return None
 
-    @tendencia.setter
-    def tendencia(self, df: pd.DataFrame):
-        b = self.__bloco_por_tipo(BlocoVazPast, 0)
-        if b is not None:
+    @limites_agrupamentos.setter
+    def limites_agrupamentos(self, df: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoLimitesPorGrupoAgrint)
+        if isinstance(b, BlocoLimitesPorGrupoAgrint):
             b.data = df
```

### Comparing `inewave-0.0.97/inewave/nwlistcf/arquivos.py` & `inewave-0.0.98/inewave/nwlistcf/arquivos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from inewave.nwlistcf.modelos.arquivos import BlocoNomesArquivos
 
 from cfinterface.files.sectionfile import SectionFile
 
-from typing import List, TypeVar, Type, Optional
+from typing import List, TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
@@ -41,46 +41,26 @@
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     def __le_nome_por_indice(self, indice: int) -> Optional[str]:
-        b = self.__bloco_por_tipo(BlocoNomesArquivos, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoNomesArquivos)
+        if isinstance(b, BlocoNomesArquivos):
             if indice in b.data.index:
                 dado = b.data.iloc[indice, 1]
                 if isinstance(dado, str):
                     return dado
         return None
 
     def __atualiza_nome_por_indice(self, indice: int, nome: str):
-        b = self.__bloco_por_tipo(BlocoNomesArquivos, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoNomesArquivos)
+        if isinstance(b, BlocoNomesArquivos):
             dif = indice - b.data.shape[0] + 1
             if dif > 0:
                 col_vazia = [None] * dif
                 b.data = pd.concat(
                     [
                         b.data,
                         pd.DataFrame(
@@ -98,16 +78,18 @@
     def arquivos(self) -> List[str]:
         """
         Os nomes dos arquivos utilizados.
 
         :return: Os arquivos na mesma ordem em que são declarados
         :rtype: List[str]
         """
-        b = self.__bloco_por_tipo(BlocoNomesArquivos, 0)
-        return [] if b is None else b.data.iloc[:, 1]
+        b = self.data.get_sections_of_type(BlocoNomesArquivos)
+        return (
+            [] if not isinstance(b, BlocoNomesArquivos) else b.data.iloc[:, 1]
+        )
 
     @property
     def nwlistcf(self) -> Optional[str]:
         """
         Nome do arquivo de dados gerais utilizado pelo NWLISTCF.
         """
         return self.__le_nome_por_indice(0)
```

### Comparing `inewave-0.0.97/inewave/nwlistcf/estados.py` & `inewave-0.0.98/inewave/nwlistcf/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistcf/modelos/arquivos.py` & `inewave-0.0.98/inewave/nwlistcf/modelos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistcf/modelos/caso.py` & `inewave-0.0.98/inewave/nwlistcf/modelos/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistcf/modelos/estados.py` & `inewave-0.0.98/inewave/nwlistcf/modelos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistcf/modelos/nwlistcfdat.py` & `inewave-0.0.98/inewave/nwlistcf/modelos/nwlistcfdat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistcf/modelos/nwlistcfrel.py` & `inewave-0.0.98/inewave/nwlistcf/modelos/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistcf/nwlistcfdat.py` & `inewave-0.0.98/inewave/nwlistcf/nwlistcfdat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from inewave.nwlistcf.modelos.nwlistcfdat import (
     PeriodoImpressaoCortesEstados,
     OpcoesImpressao,
 )
 
 from cfinterface.files.sectionfile import SectionFile
-from typing import TypeVar, Optional, Type, List
+from typing import TypeVar, Optional, List
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
 class Nwlistcfdat(SectionFile):
@@ -32,102 +32,82 @@
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def mes_inicio(self) -> Optional[int]:
         """
         O mês (calendário) de início para impressão dos cortes
 
         :return: O mês calendário de início
         :rtype: Optional[int] | None
         """
-        b = self.__bloco_por_tipo(PeriodoImpressaoCortesEstados, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(PeriodoImpressaoCortesEstados)
+        if isinstance(b, PeriodoImpressaoCortesEstados):
             return b.data[0]
         return None
 
     @mes_inicio.setter
     def mes_inicio(self, v: int):
-        b = self.__bloco_por_tipo(PeriodoImpressaoCortesEstados, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(PeriodoImpressaoCortesEstados)
+        if isinstance(b, PeriodoImpressaoCortesEstados):
             b.data[0] = v
 
     @property
     def mes_fim(self) -> Optional[int]:
         """
         O mês de fim para impressão dos cortes
 
         :return: O mês calendário de fim
         :rtype: Optional[int] | None
         """
-        b = self.__bloco_por_tipo(PeriodoImpressaoCortesEstados, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(PeriodoImpressaoCortesEstados)
+        if isinstance(b, PeriodoImpressaoCortesEstados):
             return b.data[1]
         return None
 
     @mes_fim.setter
     def mes_fim(self, v: int):
-        b = self.__bloco_por_tipo(PeriodoImpressaoCortesEstados, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(PeriodoImpressaoCortesEstados)
+        if isinstance(b, PeriodoImpressaoCortesEstados):
             b.data[1] = v
 
     @property
     def imprime_cortes_ativos(self) -> Optional[int]:
         """
         O flag para impressão somente dos cortes ativos.
 
         :return: O valor do flag
         :rtype: Optional[int] | None
         """
-        b = self.__bloco_por_tipo(PeriodoImpressaoCortesEstados, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(PeriodoImpressaoCortesEstados)
+        if isinstance(b, PeriodoImpressaoCortesEstados):
             return b.data[2]
         return None
 
     @imprime_cortes_ativos.setter
     def imprime_cortes_ativos(self, v: int):
-        b = self.__bloco_por_tipo(PeriodoImpressaoCortesEstados, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(PeriodoImpressaoCortesEstados)
+        if isinstance(b, PeriodoImpressaoCortesEstados):
             b.data[2] = v
 
     @property
     def opcoes_impressao(self) -> Optional[List[int]]:
         """
         As opções de impressão selecionadas.
 
         :return: As opções de impressão
         :rtype: Optional[List[int]] | None
         """
-        b = self.__bloco_por_tipo(OpcoesImpressao, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(OpcoesImpressao)
+        if isinstance(b, OpcoesImpressao):
             return b.data
         return None
 
     @opcoes_impressao.setter
     def opcoes_impressao(self, v: List[int]):
-        b = self.__bloco_por_tipo(OpcoesImpressao, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(OpcoesImpressao)
+        if isinstance(b, OpcoesImpressao):
             b.data = v
```

### Comparing `inewave-0.0.97/inewave/nwlistcf/nwlistcfrel.py` & `inewave-0.0.98/inewave/nwlistcf/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/cdef.py` & `inewave-0.0.98/inewave/nwlistop/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/cdefsin.py` & `inewave-0.0.98/inewave/nwlistop/cdefsin.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class CdefSIN(ArquivoSIN):
+class Cdefsin(ArquivoSIN):
     """
     Armazena os dados das saídas referentes ao custo de déficit
     de cada estágio em cada série.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `cdefsin.out`.
     """
@@ -21,14 +21,14 @@
     BLOCKS = [
         CdefAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="cdefsin.out"
-    ) -> "CdefSIN":
+    ) -> "Cdefsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/cmarg.py` & `inewave-0.0.98/inewave/nwlistop/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/cmargmed.py` & `inewave-0.0.98/inewave/nwlistop/ghtotm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
-    ArquivoSubmercado,
+from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
+    ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.cmargmed import CmargsAnos
+from inewave.nwlistop.modelos.ghtotm import GHAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class CmargMed(ArquivoSubmercado):
+class Ghtotm(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes aos custos marginais de operação
-    por submercado.
+    Armazena os dados das saídas referentes à geração hidraulica total
+    por patamar, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `cmarg00x-med.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `ghtotm00x.out`, onde x varia conforme o
     submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        CmargsAnos,
+        GHAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="cmarg001-med.out"
-    ) -> "CmargMed":
+        cls, diretorio: str, nome_arquivo="ghtotm001.out"
+    ) -> "Ghtotm":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/coper.py` & `inewave-0.0.98/inewave/nwlistop/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/corteolm.py` & `inewave-0.0.98/inewave/nwlistop/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/cterm.py` & `inewave-0.0.98/inewave/nwlistop/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/ctermsin.py` & `inewave-0.0.98/inewave/nwlistop/evertsin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from inewave.nwlistop.modelos.ctermsin import CtermsAnos
 from inewave.nwlistop.modelos.arquivos.arquivosin import (
     ArquivoSIN,
 )
+from inewave.nwlistop.modelos.evertsin import EvertAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class CtermSIN(ArquivoSIN):
+class Evertsin(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes aos custos de geração térmica
-    para o SIN.
+    Armazena os dados das saídas referentes ao vertimento de reservatórios
+    , para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ctermsin.out`.
+    NWLISTOP e reproduzidas no `evertsin.out`.
 
     """
 
     BLOCKS = [
-        CtermsAnos,
+        EvertAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ctermsin.out"
-    ) -> "CtermSIN":
+        cls, diretorio: str, nome_arquivo="evertsin.out"
+    ) -> "Evertsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/deficit.py` & `inewave-0.0.98/inewave/nwlistop/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/defsin.py` & `inewave-0.0.98/inewave/nwlistop/ghmaxrsin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
     ArquivoSINPatamar,
 )
-from inewave.nwlistop.modelos.defsin import DefAnos
+from inewave.nwlistop.modelos.ghmaxrsin import GHAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class DefSIN(ArquivoSINPatamar):
+class Ghmaxrsin(ArquivoSINPatamar):
     """
-    Armazena os dados das saídas referentes ao déficit
-    por patamar para o SIN.
+    Armazena os dados das saídas referentes à geração hidraulica máxima
+    considerando restrições elétricas por patamar para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `defsinp001.out`.
+    NWLISTOP e reproduzidas nos `ghmaxsin.out`.
     """
 
     BLOCKS = [
-        DefAnos,
+        GHAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="defsinp001.out"
-    ) -> "DefSIN":
+        cls, diretorio: str, nome_arquivo="ghmaxrsin.out"
+    ) -> "Ghmaxrsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/depminuh.py` & `inewave-0.0.98/inewave/nwlistop/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/dfphauh.py` & `inewave-0.0.98/inewave/nwlistop/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/dlppdfmax.py` & `inewave-0.0.98/inewave/nwlistop/rhslppdf.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
     ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.dlppdfmax import DLPPdfmaxAnos
+from inewave.nwlistop.modelos.rhslppdf import RHSLPPdfAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class DLPPdfmax(ArquivoREEPatamar):
+class Rhslppdf(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes à violação das restrições LPP
+    Armazena os dados das saídas referentes ao RHS das restrições LPP
     de defluência máxima por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dlppdfmax00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `rhslppdf00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         REE,
-        DLPPdfmaxAnos,
+        RHSLPPdfAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dlppdfmax001.out"
-    ) -> "DLPPdfmax":
+        cls, diretorio: str, nome_arquivo="rhslppdf001.out"
+    ) -> "Rhslppdf":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/dlppdfmaxm.py` & `inewave-0.0.98/inewave/nwlistop/dlppdfmaxm.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from inewave.nwlistop.modelos.dlppdfmax import DLPPdfmaxAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class DLPPdfmaxm(ArquivoSubmercadoPatamar):
+class Dlppdfmaxm(ArquivoSubmercadoPatamar):
     """
     Armazena os dados das saídas referentes à violação das restrições LPP
     de defluência máxima por patamar, por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `dlppdfmax00x.out`, onde x varia conforme o
     Submercado em questão.
@@ -24,14 +24,14 @@
         Submercado,
         DLPPdfmaxAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="dlppdfmaxm001.out"
-    ) -> "DLPPdfmaxm":
+    ) -> "Dlppdfmaxm":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/dlppdfmaxs.py` & `inewave-0.0.98/inewave/nwlistop/dlppdfmaxs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from inewave.nwlistop.modelos.dlppdfmaxs import DLPPdfmaxAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class DLPPdfmaxs(ArquivoSINPatamar):
+class Dlppdfmaxs(ArquivoSINPatamar):
     """
     Armazena os dados das saídas referentes à violação das restrições
     LPP de defluência máxima por patamar para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `dlppdfmaxs.out`.
     """
@@ -20,14 +20,14 @@
     BLOCKS = [
         DLPPdfmaxAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="dlppdfmaxs.out"
-    ) -> "DLPPdfmaxs":
+    ) -> "Dlppdfmaxs":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/dlpptbmax.py` & `inewave-0.0.98/inewave/nwlistop/ghmax.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
     ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.dlpptbmax import DLPPtbmaxAnos
+from inewave.nwlistop.modelos.ghmax import GHAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class DLPPtbmax(ArquivoREEPatamar):
+class Ghmax(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes à violação das restrições LPP
-    de turbinamento máximo por patamar, por REE.
+    Armazena os dados das saídas referentes à geração hidraulica máxima
+    por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dlpptbmax00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `ghmax00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         REE,
-        DLPPtbmaxAnos,
+        GHAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dlpptbmax001.out"
-    ) -> "DLPPtbmax":
+        cls, diretorio: str, nome_arquivo="ghmax001.out"
+    ) -> "Ghmax":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/dlpptbmaxm.py` & `inewave-0.0.98/inewave/nwlistop/dlpptbmaxm.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from inewave.nwlistop.modelos.dlppdfmax import DLPPdfmaxAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class DLPPtbmaxm(ArquivoSubmercadoPatamar):
+class Dlpptbmaxm(ArquivoSubmercadoPatamar):
     """
     Armazena os dados das saídas referentes à violação das restrições LPP
     de turbinamento máximo por patamar, por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `dlpptbmax00x.out`, onde x varia conforme o
     Submercado em questão.
@@ -24,14 +24,14 @@
         Submercado,
         DLPPdfmaxAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="dlpptbmaxm001.out"
-    ) -> "DLPPtbmaxm":
+    ) -> "Dlpptbmaxm":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/dlpptbmaxs.py` & `inewave-0.0.98/inewave/nwlistop/geol.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
-    ArquivoSINPatamar,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.dlpptbmaxs import DLPPtbmaxAnos
+from inewave.nwlistop.modelos.geol import GEAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class DLPPtbmaxs(ArquivoSINPatamar):
+class Geol(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à violação das restrições
-    LPP de turbinamento máximo por patamar para o SIN.
+    Armazena os dados das saídas referentes à geração eólica total
+    por patamar, por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dlpptbmaxs.out`.
+    NWLISTOP e reproduzidas nos `geol00x.out`, onde x varia conforme o
+    PEE em questão.
+
     """
 
     BLOCKS = [
-        DLPPtbmaxAnos,
+        Usina,
+        GEAnos,
     ]
 
     @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dlpptbmaxs.out"
-    ) -> "DLPPtbmaxs":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="geol001.out") -> "Geol":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/dtbmax.py` & `inewave-0.0.98/inewave/nwlistop/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/dtbmin.py` & `inewave-0.0.98/inewave/nwlistop/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/dvazmax.py` & `inewave-0.0.98/inewave/nwlistop/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/eaf.py` & `inewave-0.0.98/inewave/nwlistop/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/eafb.py` & `inewave-0.0.98/inewave/nwlistop/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/eafbm.py` & `inewave-0.0.98/inewave/nwlistop/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/eafbsin.py` & `inewave-0.0.98/inewave/nwlistop/eafbsin.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class EafbSIN(ArquivoSIN):
+class Eafbsin(ArquivoSIN):
     """
     Armazena os dados das saídas referentes à energia natural
     afluente para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `eafbsin.out`.
     """
@@ -21,14 +21,14 @@
     BLOCKS = [
         EafsAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="eafbsin.out"
-    ) -> "EafbSIN":
+    ) -> "Eafbsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/eafm.py` & `inewave-0.0.98/inewave/nwlistop/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/earmf.py` & `inewave-0.0.98/inewave/nwlistop/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/earmfm.py` & `inewave-0.0.98/inewave/nwlistop/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/earmfp.py` & `inewave-0.0.98/inewave/nwlistop/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/earmfpm.py` & `inewave-0.0.98/inewave/nwlistop/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/earmfpsin.py` & `inewave-0.0.98/inewave/nwlistop/ghtot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-from inewave.nwlistop.modelos.earmfpsin import EarmsAnos
-
-from inewave.nwlistop.modelos.arquivos.arquivosin import (
-    ArquivoSIN,
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
+    ArquivoREEPatamar,
 )
+from inewave.nwlistop.modelos.ghtot import GHAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class EarmfpSIN(ArquivoSIN):
+class Ghtot(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes às energias
-    armazenadas finais para o SIN e em % da energia armazenável máxima.
+    Armazena os dados das saídas referentes à geração hidraulica total
+    por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `earmfpsin.out`, onde x varia conforme o
-    submercado em questão.
+    NWLISTOP e reproduzidas nos `ghtot00x.out`, onde x varia conforme o
+    REE em questão.
+
     """
 
     BLOCKS = [
-        EarmsAnos,
+        REE,
+        GHAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="earmfpsin.out"
-    ) -> "EarmfpSIN":
+        cls, diretorio: str, nome_arquivo="ghtot001.out"
+    ) -> "Ghtot":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/earmfsin.py` & `inewave-0.0.98/inewave/nwlistop/verturbsin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from inewave.nwlistop.modelos.earmfsin import EarmAnos
-
+from inewave.nwlistop.modelos.verturbsin import VertAnos
 from inewave.nwlistop.modelos.arquivos.arquivosin import (
     ArquivoSIN,
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class EarmfSIN(ArquivoSIN):
+class Verturbsin(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes à energia armazenada
-    final em MWmes para o SIN.
+    Armazena os dados das saídas referentes às energias
+    vertidas para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `eafmfsin.out`.
+    NWLISTOP e reproduzidas nos `verturbsin.out`.
+
     """
 
     BLOCKS = [
-        EarmAnos,
+        VertAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="earmfsin.out"
-    ) -> "EarmfSIN":
+        cls, diretorio: str, nome_arquivo="verturbsin.out"
+    ) -> "Verturbsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/evert.py` & `inewave-0.0.98/inewave/nwlistop/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/evertm.py` & `inewave-0.0.98/inewave/nwlistop/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/evertsin.py` & `inewave-0.0.98/inewave/nwlistop/earmfsin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
+from inewave.nwlistop.modelos.earmfsin import EarmAnos
+
 from inewave.nwlistop.modelos.arquivos.arquivosin import (
     ArquivoSIN,
 )
-from inewave.nwlistop.modelos.evertsin import EvertAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class EvertSIN(ArquivoSIN):
+class Earmfsin(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes ao vertimento de reservatórios
-    , para o SIN.
+    Armazena os dados das saídas referentes à energia armazenada
+    final em MWmes para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas no `evertsin.out`.
-
+    NWLISTOP e reproduzidas nos `eafmfsin.out`.
     """
 
     BLOCKS = [
-        EvertAnos,
+        EarmAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="evertsin.out"
-    ) -> "EvertSIN":
+        cls, diretorio: str, nome_arquivo="earmfsin.out"
+    ) -> "Earmfsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/exces.py` & `inewave-0.0.98/inewave/nwlistop/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/excessin.py` & `inewave-0.0.98/inewave/nwlistop/excessin.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from inewave.nwlistop.modelos.exces import ExcesAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class ExcesSIN(ArquivoSINPatamar):
+class Excessin(ArquivoSINPatamar):
     """
     Armazena os dados das saídas referentes ao excesso de energia
     por patamar, para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas no `excessin.out`
 
@@ -21,14 +21,14 @@
     BLOCKS = [
         ExcesAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="excessin.out"
-    ) -> "ExcesSIN":
+    ) -> "Excessin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/fteolm.py` & `inewave-0.0.98/inewave/nwlistop/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/fteolsin.py` & `inewave-0.0.98/inewave/nwlistop/fteolsin.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from inewave.nwlistop.modelos.exces import ExcesAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class FteolSIN(ArquivoSINPatamar):
+class Fteolsin(ArquivoSINPatamar):
     """
     Armazena os dados das saídas referentes à folga da variável de
     geração eólica para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas no `fteolsin.out`
 
@@ -21,14 +21,14 @@
     BLOCKS = [
         ExcesAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="fteolsin.out"
-    ) -> "FteolSIN":
+    ) -> "Fteolsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/geol.py` & `inewave-0.0.98/inewave/nwlistop/qafluh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
-    ArquivoUsinaPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivousina import (
+    ArquivoUsina,
 )
-from inewave.nwlistop.modelos.geol import GEAnos
+from inewave.nwlistop.modelos.qafluh import QaflAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Geol(ArquivoUsinaPatamar):
+class Qafluh(ArquivoUsina):
     """
-    Armazena os dados das saídas referentes à geração eólica total
-    por patamar, por usina.
+    Armazena os dados das saídas referentes às vazões afluentes por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `geol00x.out`, onde x varia conforme o
-    PEE em questão.
+    NWLISTOP e reproduzidas nos `qafluh00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        GEAnos,
+        QaflAnos,
     ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="geol001.out") -> "Geol":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="qafluh001.out"
+    ) -> "Qafluh":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/geolm.py` & `inewave-0.0.98/inewave/nwlistop/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/geolsin.py` & `inewave-0.0.98/inewave/nwlistop/geolsin.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class GeolSIN(ArquivoSINPatamar):
+class Geolsin(ArquivoSINPatamar):
     """
     Armazena os dados das saídas referentes à geração eólica total
     para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `geolsin.out`.
     """
@@ -21,14 +21,14 @@
     BLOCKS = [
         GEAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="geolsin.out"
-    ) -> "GeolSIN":
+    ) -> "Geolsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/ghiduh.py` & `inewave-0.0.98/inewave/nwlistop/ghiduh.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from inewave.nwlistop.modelos.ghiduh import GhidAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class GhidUH(ArquivoUsinaPatamar):
+class Ghiduh(ArquivoUsinaPatamar):
     """
     Armazena os dados das saídas referentes à geração hidráulica por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `ghiduh00x.out`, onde x varia conforme a
     usina em questão.
 
@@ -23,14 +23,14 @@
         Usina,
         GhidAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="ghiduh001.out"
-    ) -> "GhidUH":
+    ) -> "Ghiduh":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/ghmax.py` & `inewave-0.0.98/inewave/nwlistop/vagua.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
-    ArquivoREEPatamar,
-)
-from inewave.nwlistop.modelos.ghmax import GHAnos
+from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
+
+from inewave.nwlistop.modelos.vagua import VAAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Ghmax(ArquivoREEPatamar):
+class Vagua(ArquivoREE):
     """
-    Armazena os dados das saídas referentes à geração hidraulica máxima
-    por patamar, por REE.
+    Armazena os dados das saídas referentes aos valores da água
+    por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghmax00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `vagua00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         REE,
-        GHAnos,
+        VAAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghmax001.out"
-    ) -> "Ghmax":
+        cls, diretorio: str, nome_arquivo="vagua001.out"
+    ) -> "Vagua":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/ghmaxm.py` & `inewave-0.0.98/inewave/nwlistop/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/ghmaxmr.py` & `inewave-0.0.98/inewave/nwlistop/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/ghmaxr.py` & `inewave-0.0.98/inewave/nwlistop/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/ghmaxrsin.py` & `inewave-0.0.98/inewave/nwlistop/ghmaxsin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
     ArquivoSINPatamar,
 )
-from inewave.nwlistop.modelos.ghmaxrsin import GHAnos
+from inewave.nwlistop.modelos.ghmaxsin import GHAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class GhmaxrSIN(ArquivoSINPatamar):
+class Ghmaxsin(ArquivoSINPatamar):
     """
     Armazena os dados das saídas referentes à geração hidraulica máxima
-    considerando restrições elétricas por patamar para o SIN.
+    por patamar para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `ghmaxsin.out`.
     """
 
     BLOCKS = [
         GHAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghmaxrsin.out"
-    ) -> "GhmaxrSIN":
+        cls, diretorio: str, nome_arquivo="ghmaxsin.out"
+    ) -> "Ghmaxsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/ghmaxsin.py` & `inewave-0.0.98/inewave/nwlistop/dlppdfmax.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
-    ArquivoSINPatamar,
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
+    ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.ghmaxsin import GHAnos
+from inewave.nwlistop.modelos.dlppdfmax import DLPPdfmaxAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class GhmaxSIN(ArquivoSINPatamar):
+class Dlppdfmax(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes à geração hidraulica máxima
-    por patamar para o SIN.
+    Armazena os dados das saídas referentes à violação das restrições LPP
+    de defluência máxima por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghmaxsin.out`.
+    NWLISTOP e reproduzidas nos `dlppdfmax00x.out`, onde x varia conforme o
+    REE em questão.
+
     """
 
     BLOCKS = [
-        GHAnos,
+        REE,
+        DLPPdfmaxAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghmaxsin.out"
-    ) -> "GhmaxSIN":
+        cls, diretorio: str, nome_arquivo="dlppdfmax001.out"
+    ) -> "Dlppdfmax":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/ghtot.py` & `inewave-0.0.98/inewave/nwlistop/dlpptbmax.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
     ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.ghtot import GHAnos
+from inewave.nwlistop.modelos.dlpptbmax import DLPPtbmaxAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Ghtot(ArquivoREEPatamar):
+class Dlpptbmax(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes à geração hidraulica total
-    por patamar, por REE.
+    Armazena os dados das saídas referentes à violação das restrições LPP
+    de turbinamento máximo por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghtot00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `dlpptbmax00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         REE,
-        GHAnos,
+        DLPPtbmaxAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghtot001.out"
-    ) -> "Ghtot":
+        cls, diretorio: str, nome_arquivo="dlpptbmax001.out"
+    ) -> "Dlpptbmax":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/ghtotm.py` & `inewave-0.0.98/inewave/nwlistop/verturbm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
-    ArquivoSubmercadoPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.ghtotm import GHAnos
+from inewave.nwlistop.modelos.verturbm import VertAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Ghtotm(ArquivoSubmercadoPatamar):
+class Verturbm(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes à geração hidraulica total
-    por patamar, por submercado.
+    Armazena os dados das saídas referentes às energias
+    vertidas, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghtotm00x.out`, onde x varia conforme o
-    submercado em questão.
+    NWLISTOP e reproduzidas nos `vertub00x.out`, onde x varia conforme o
+    REE em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        GHAnos,
+        VertAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghtotm001.out"
-    ) -> "Ghtotm":
+        cls, diretorio: str, nome_arquivo="verturbm001.out"
+    ) -> "Verturbm":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/ghtotsin.py` & `inewave-0.0.98/inewave/nwlistop/ghtotsin.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from inewave.nwlistop.modelos.ghtotsin import GHAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class GhtotSIN(ArquivoSINPatamar):
+class Ghtotsin(ArquivoSINPatamar):
     """
     Armazena os dados das saídas referentes à geração hidraulica total
     por patamar para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `ghtotsin.out`.
     """
@@ -20,14 +20,14 @@
     BLOCKS = [
         GHAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="ghtotsin.out"
-    ) -> "GhtotSIN":
+    ) -> "Ghtotsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/gtert.py` & `inewave-0.0.98/inewave/nwlistop/gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/gttot.py` & `inewave-0.0.98/inewave/nwlistop/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/gttotsin.py` & `inewave-0.0.98/inewave/nwlistop/gttotsin.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class GttotSIN(ArquivoSINPatamar):
+class Gttotsin(ArquivoSINPatamar):
     """
     Armazena os dados das saídas referentes à geração térmica total
     por patamar, para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `gttotsin.out`.
     """
@@ -20,14 +20,14 @@
     BLOCKS = [
         GTAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="gttotsin.out"
-    ) -> "GttotSIN":
+    ) -> "Gttotsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/intercambio.py` & `inewave-0.0.98/inewave/nwlistop/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/invade.py` & `inewave-0.0.98/inewave/nwlistop/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/invadem.py` & `inewave-0.0.98/inewave/nwlistop/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/mediasmerc.py` & `inewave-0.0.98/inewave/nwlistop/mediasmerc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import pandas as pd  # type: ignore
 
 from inewave.nwlistop.modelos.mediasmerc import LeituraMediasMerc
 
 
-class MediasMerc:
+class Mediasmerc:
     """
     Armazena os dados das saídas referentes às médias de diversas variáveis
     agrupadas por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `MEDIAS-MERC.CSV`.
 
     """
 
     def __init__(self, dados: pd.DataFrame):
         self.__dados = dados
 
     def __eq__(self, o: object) -> bool:
         """
-        A igualdade entre MediasMerc avalia todos os valores da tabela.
+        A igualdade entre Mediasmerc avalia todos os valores da tabela.
         """
-        if not isinstance(o, MediasMerc):
+        if not isinstance(o, Mediasmerc):
             return False
-        m: MediasMerc = o
+        m: Mediasmerc = o
         return self.medias.equals(m.medias)
 
     @property
     def medias(self) -> pd.DataFrame:
         return self.__dados
 
     @medias.setter
```

### Comparing `inewave-0.0.97/inewave/nwlistop/mediassin.py` & `inewave-0.0.98/inewave/nwlistop/mediassin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import pandas as pd  # type: ignore
 
 from inewave.nwlistop.modelos.mediassin import LeituraMediasSIN
 
 
-class MediasSIN:
+class Mediassin:
     """
     Armazena os dados das saídas referentes às médias de diversas variáveis
     para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `MEDIAS-SIN.CSV`.
 
     """
 
     def __init__(self, dados: pd.DataFrame):
         self.__dados = dados
 
     def __eq__(self, o: object) -> bool:
         """
-        A igualdade entre MediasSIN avalia todos os valores da tabela.
+        A igualdade entre Mediassin avalia todos os valores da tabela.
         """
-        if not isinstance(o, MediasSIN):
+        if not isinstance(o, Mediassin):
             return False
-        m: MediasSIN = o
+        m: Mediassin = o
         return self.medias.equals(m.medias)
 
     @property
     def medias(self) -> pd.DataFrame:
         return self.__dados
 
     @medias.setter
```

### Comparing `inewave-0.0.97/inewave/nwlistop/mercl.py` & `inewave-0.0.98/inewave/nwlistop/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/merclsin.py` & `inewave-0.0.98/inewave/nwlistop/merclsin.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class MerclSIN(ArquivoSIN):
+class Merclsin(ArquivoSIN):
     """
     Armazena os dados das saídas referentes ao mercado líquido
     de cada estágio em cada série.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `merclsin.out`.
     """
@@ -21,14 +21,14 @@
     BLOCKS = [
         MerclAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="merclsin.out"
-    ) -> "MerclSIN":
+    ) -> "Merclsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py` & `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,73 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.blocos.valoresclassetermicaseriepatamar import (
-    ValoresClasseTermicaSeriePatamar,
+from inewave.nwlistop.modelos.blocos.valoresserie import (
+    ValoresSerie,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 
 
-class ArquivoClasseTermicaSubmercadoPatamar(BlockFile):
+class ArquivoSubmercado(BlockFile):
     """
-    Armazena os dados das saídas por patamar, por submercado e por
-    classe térmica.
+    Armazena os dados das saídas por submercado.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [Submercado, ValoresClasseTermicaSeriePatamar]
+    BLOCKS = [Submercado, ValoresSerie]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoClasseTermicaSubmercadoPatamar":
+    ) -> "ArquivoSubmercado":
         return cls.read(diretorio, nome_arquivo)
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
-        for b in self.data.of_type(ValoresClasseTermicaSeriePatamar):
+        for b in self.data.of_type(ValoresSerie):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
                 df = b.data
             else:
                 df = pd.concat([df, b.data], ignore_index=True)
         return df
 
     @property
     def valores(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com os valores por classe térmica, por patamar, por série e
+        Tabela com os valores, por série e
         por mês/ano de estudo.
 
-        - Ano (`int`)
-        - Classe (`int`)
-        - Série (`int`)
-        - Patamar (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - data (`datetime`)
+        - serie (`str`)
+        - valor (`float`)
 
-        :return: A tabela dos valores por patamar.
+        :return: A tabela dos valores.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
 
     @property
     def submercado(self) -> Optional[str]:
         """
         O submercado associado ao arquivo lido.
 
         :return: Os nome do submercado
         :rtype: str
         """
-        b = self.__bloco_por_tipo(Submercado, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(Submercado)
+        if isinstance(b, Submercado):
             return b.data
         return None
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py` & `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from inewave.nwlistop.modelos.blocos.parsubmercados import ParSubmercados
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 
 
 class ArquivoParSubmercadoPatamar(BlockFile):
     """
     Armazena os dados das saídas por patamar, por par de submercados.
     """
 
@@ -26,34 +26,14 @@
         cls, diretorio: str, nome_arquivo="arq.out"
     ) -> "ArquivoParSubmercadoPatamar":
         return cls.read(diretorio, nome_arquivo)
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresSeriePatamar):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
@@ -64,20 +44,18 @@
 
     @property
     def valores(self) -> Optional[pd.DataFrame]:
         """
         Tabela com os valores por patamar, por série e
         por mês/ano de estudo.
 
-        - Ano (`int`)
-        - Série (`int`)
-        - Patamar (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - data (`datetime`)
+        - patamar (`str`)
+        - serie (`str`)
+        - valor (`float`)
 
         :return: A tabela dos valores por patamar.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
@@ -86,24 +64,24 @@
     def submercado_de(self) -> Optional[str]:
         """
         O submercado de origem associado ao arquivo lido.
 
         :return: Os nome do submercado
         :rtype: str
         """
-        b = self.__bloco_por_tipo(ParSubmercados, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(ParSubmercados)
+        if isinstance(b, ParSubmercados):
             return b.data[0]
         return None
 
     @property
     def submercado_para(self) -> Optional[str]:
         """
         O submercado de destino associado ao arquivo lido.
 
         :return: Os nome do submercado
         :rtype: str
         """
-        b = self.__bloco_por_tipo(ParSubmercados, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(ParSubmercados)
+        if isinstance(b, ParSubmercados):
             return b.data[1]
         return None
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoree.py` & `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivousina.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,39 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.blocos.valoresserie import (
     ValoresSerie,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 
 
-class ArquivoREE(BlockFile):
+class ArquivoUsina(BlockFile):
     """
-    Armazena os dados das saídas por REE.
+    Armazena os dados das saídas por usina.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [REE, ValoresSerie]
+    BLOCKS = [Usina, ValoresSerie]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoREE":
+    ) -> "ArquivoUsina":
         return cls.read(diretorio, nome_arquivo)
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresSerie):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
@@ -64,33 +44,30 @@
 
     @property
     def valores(self) -> Optional[pd.DataFrame]:
         """
         Tabela com os valores, por série e
         por mês/ano de estudo.
 
-        - Ano (`int`)
-        - Série (`int`)
-        - Patamar (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - data (`datetime`)
+        - serie (`str`)
+        - valor (`float`)
 
         :return: A tabela dos valores.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
 
     @property
-    def ree(self) -> Optional[str]:
+    def usina(self) -> Optional[str]:
         """
-        O REE associado ao arquivo lido.
+        A usina associada ao arquivo lido.
 
-        :return: O nome do ree
+        :return: O nome da usina
         :rtype: str
         """
-        b = self.__bloco_por_tipo(REE, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(Usina)
+        if isinstance(b, Usina):
             return b.data
         return None
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py` & `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 
 
 class ArquivoREEPatamar(BlockFile):
     """
     Armazena os dados das saídas por patamar, por REE.
     """
 
@@ -26,34 +26,14 @@
         cls, diretorio: str, nome_arquivo="arq.out"
     ) -> "ArquivoREEPatamar":
         return cls.read(diretorio, nome_arquivo)
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresSeriePatamar):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
@@ -64,20 +44,18 @@
 
     @property
     def valores(self) -> Optional[pd.DataFrame]:
         """
         Tabela com os valores por patamar, por série e
         por mês/ano de estudo.
 
-        - Ano (`int`)
-        - Série (`int`)
-        - Patamar (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - data (`datetime`)
+        - patamar (`str`)
+        - serie (`str`)
+        - valor (`float`)
 
         :return: A tabela dos valores por patamar.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
@@ -86,11 +64,11 @@
     def ree(self) -> Optional[str]:
         """
         O REE associado ao arquivo lido.
 
         :return: O nome do REE
         :rtype: str
         """
-        b = self.__bloco_por_tipo(REE, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(REE)
+        if isinstance(b, REE):
             return b.data
         return None
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from inewave.nwlistop.modelos.blocos.valoresserie import (
-    ValoresSerie,
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
 from typing import TypeVar, Optional
 
 
-class ArquivoSIN(BlockFile):
+class ArquivoSINPatamar(BlockFile):
     """
     Armazena os dados das saídas por submercado.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [ValoresSerie]
+    BLOCKS = [ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoSIN":
+    ) -> "ArquivoSINPatamar":
         return cls.read(diretorio, nome_arquivo)
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
-        for b in self.data.of_type(ValoresSerie):
+        for b in self.data.of_type(ValoresSeriePatamar):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
                 df = b.data
             else:
                 df = pd.concat([df, b.data], ignore_index=True)
@@ -43,20 +43,18 @@
 
     @property
     def valores(self) -> Optional[pd.DataFrame]:
         """
         Tabela com os valores por patamar, por série e
         por mês/ano de estudo.
 
-        - Ano (`int`)
-        - Série (`int`)
-        - Patamar (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - data (`datetime`)
+        - patamar (`str`)
+        - serie (`str`)
+        - valor (`float`)
 
         :return: A tabela dos valores por patamar.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py` & `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
-    ValoresSeriePatamar,
+from inewave.nwlistop.modelos.blocos.valoresserie import (
+    ValoresSerie,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
 from typing import TypeVar, Optional
 
 
-class ArquivoSINPatamar(BlockFile):
+class ArquivoSIN(BlockFile):
     """
     Armazena os dados das saídas por submercado.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [ValoresSeriePatamar]
+    BLOCKS = [ValoresSerie]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoSINPatamar":
+    ) -> "ArquivoSIN":
         return cls.read(diretorio, nome_arquivo)
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
-        for b in self.data.of_type(ValoresSeriePatamar):
+        for b in self.data.of_type(ValoresSerie):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
                 df = b.data
             else:
                 df = pd.concat([df, b.data], ignore_index=True)
@@ -43,20 +43,17 @@
 
     @property
     def valores(self) -> Optional[pd.DataFrame]:
         """
         Tabela com os valores por patamar, por série e
         por mês/ano de estudo.
 
-        - Ano (`int`)
-        - Série (`int`)
-        - Patamar (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - data (`datetime`)
+        - serie (`str`)
+        - valor (`float`)
 
         :return: A tabela dos valores por patamar.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py` & `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoree.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,39 @@
-from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.blocos.valoresserie import (
     ValoresSerie,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 
 
-class ArquivoSubmercado(BlockFile):
+class ArquivoREE(BlockFile):
     """
-    Armazena os dados das saídas por submercado.
+    Armazena os dados das saídas por REE.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [Submercado, ValoresSerie]
+    BLOCKS = [REE, ValoresSerie]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoSubmercado":
+    ) -> "ArquivoREE":
         return cls.read(diretorio, nome_arquivo)
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresSerie):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
@@ -64,33 +44,30 @@
 
     @property
     def valores(self) -> Optional[pd.DataFrame]:
         """
         Tabela com os valores, por série e
         por mês/ano de estudo.
 
-        - Ano (`int`)
-        - Série (`int`)
-        - Patamar (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - data (`datetime`)
+        - serie (`str`)
+        - valor (`float`)
 
         :return: A tabela dos valores.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
 
     @property
-    def submercado(self) -> Optional[str]:
+    def ree(self) -> Optional[str]:
         """
-        O submercado associado ao arquivo lido.
+        O REE associado ao arquivo lido.
 
-        :return: Os nome do submercado
+        :return: O nome do ree
         :rtype: str
         """
-        b = self.__bloco_por_tipo(Submercado, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(REE)
+        if isinstance(b, REE):
             return b.data
         return None
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py` & `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,39 @@
-from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 
 
-class ArquivoSubmercadoPatamar(BlockFile):
+class ArquivoUsinaPatamar(BlockFile):
     """
-    Armazena os dados das saídas por patamar, por submercado.
+    Armazena os dados das saídas por patamar, por Usina.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [Submercado, ValoresSeriePatamar]
+    BLOCKS = [Usina, ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoSubmercadoPatamar":
+    ) -> "ArquivoUsinaPatamar":
         return cls.read(diretorio, nome_arquivo)
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresSeriePatamar):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
@@ -64,33 +44,31 @@
 
     @property
     def valores(self) -> Optional[pd.DataFrame]:
         """
         Tabela com os valores por patamar, por série e
         por mês/ano de estudo.
 
-        - Ano (`int`)
-        - Série (`int`)
-        - Patamar (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - data (`datetime`)
+        - patamar (`str`)
+        - serie (`str`)
+        - valor (`float`)
 
         :return: A tabela dos valores por patamar.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
 
     @property
-    def submercado(self) -> Optional[str]:
+    def usina(self) -> Optional[str]:
         """
-        O submercado associado ao arquivo lido.
+        A usina associada ao arquivo lido.
 
-        :return: Os nome do submercado
+        :return: O nome da usina
         :rtype: str
         """
-        b = self.__bloco_por_tipo(Submercado, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(Usina)
+        if isinstance(b, Usina):
             return b.data
         return None
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivousina.py` & `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,96 +1,74 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.blocos.valoresserie import (
-    ValoresSerie,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 
 
-class ArquivoUsina(BlockFile):
+class ArquivoSubmercadoPatamar(BlockFile):
     """
-    Armazena os dados das saídas por usina.
+    Armazena os dados das saídas por patamar, por submercado.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [Usina, ValoresSerie]
+    BLOCKS = [Submercado, ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoUsina":
+    ) -> "ArquivoSubmercadoPatamar":
         return cls.read(diretorio, nome_arquivo)
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
-        for b in self.data.of_type(ValoresSerie):
+        for b in self.data.of_type(ValoresSeriePatamar):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
                 df = b.data
             else:
                 df = pd.concat([df, b.data], ignore_index=True)
         return df
 
     @property
     def valores(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com os valores, por série e
+        Tabela com os valores por patamar, por série e
         por mês/ano de estudo.
 
-        - Ano (`int`)
-        - Série (`int`)
-        - Patamar (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - data (`datetime`)
+        - patamar (`str`)
+        - serie (`str`)
+        - valor (`float`)
 
-        :return: A tabela dos valores.
+        :return: A tabela dos valores por patamar.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
 
     @property
-    def usina(self) -> Optional[str]:
+    def submercado(self) -> Optional[str]:
         """
-        A usina associada ao arquivo lido.
+        O submercado associado ao arquivo lido.
 
-        :return: O nome da usina
+        :return: Os nome do submercado
         :rtype: str
         """
-        b = self.__bloco_por_tipo(Usina, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(Submercado)
+        if isinstance(b, Submercado):
             return b.data
         return None
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py` & `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,96 +1,76 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
-    ValoresSeriePatamar,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.blocos.valoresclassetermicaseriepatamar import (
+    ValoresClasseTermicaSeriePatamar,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
-from typing import Type, TypeVar, Optional
+from typing import TypeVar, Optional
 
 
-class ArquivoUsinaPatamar(BlockFile):
+class ArquivoClasseTermicaSubmercadoPatamar(BlockFile):
     """
-    Armazena os dados das saídas por patamar, por Usina.
+    Armazena os dados das saídas por patamar, por submercado e por
+    classe térmica.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [Usina, ValoresSeriePatamar]
+    BLOCKS = [Submercado, ValoresClasseTermicaSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoUsinaPatamar":
+    ) -> "ArquivoClasseTermicaSubmercadoPatamar":
         return cls.read(diretorio, nome_arquivo)
 
     def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
         self.write(diretorio, nome_arquivo)
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
-        for b in self.data.of_type(ValoresSeriePatamar):
+        for b in self.data.of_type(ValoresClasseTermicaSeriePatamar):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
                 df = b.data
             else:
                 df = pd.concat([df, b.data], ignore_index=True)
         return df
 
     @property
     def valores(self) -> Optional[pd.DataFrame]:
         """
-        Tabela com os valores por patamar, por série e
+        Tabela com os valores por classe térmica, por patamar, por série e
         por mês/ano de estudo.
 
-        - Ano (`int`)
-        - Série (`int`)
-        - Patamar (`str`)
-        - Janeiro (`float`)
-        - ...
-        - Dezembro (`float`)
+        - classe (`str`)
+        - data (`datetime`)
+        - patamar (`str`)
+        - serie (`str`)
+        - valor (`float`)
 
         :return: A tabela dos valores por patamar.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
 
     @property
-    def usina(self) -> Optional[str]:
+    def submercado(self) -> Optional[str]:
         """
-        A usina associada ao arquivo lido.
+        O submercado associado ao arquivo lido.
 
-        :return: O nome da usina
+        :return: Os nome do submercado
         :rtype: str
         """
-        b = self.__bloco_por_tipo(Usina, 0)
-        if b is not None:
+        b = self.data.get_blocks_of_type(Submercado)
+        if isinstance(b, Submercado):
             return b.data
         return None
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/blocos/parsubmercados.py` & `inewave-0.0.98/inewave/nwlistop/modelos/blocos/parsubmercados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/blocos/ree.py` & `inewave-0.0.98/inewave/nwlistop/modelos/blocos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/blocos/submercado.py` & `inewave-0.0.98/inewave/nwlistop/modelos/blocos/submercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/blocos/usina.py` & `inewave-0.0.98/inewave/nwlistop/modelos/blocos/usina.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py` & `inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from inewave.config import (
     MESES_DF,
     MAX_PATAMARES,
     MAX_SERIES_SINTETICAS,
     MAX_UTES,
 )
+from inewave._utils.formatacao import formata_df_meses_para_datas_nwlistop
 
 from typing import IO, List
 import pandas as pd  # type: ignore
 import numpy as np  # type: ignore
 
 
 class ValoresClasseTermicaSeriePatamar(Block):
@@ -42,34 +43,34 @@
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            cols = MESES_DF + ["Média"]
-            df = pd.DataFrame(tabela, columns=["Classe", "Série"] + cols)
-            df["Ano"] = self.__ano
-            df["Patamar"] = patamares
-            df = df[["Ano", "Classe", "Série", "Patamar"] + cols]
+            cols = MESES_DF
+            df = pd.DataFrame(tabela, columns=["classe", "serie"] + cols)
+            df["ano"] = self.__ano
+            df["patamar"] = patamares
+            df = df[["ano", "classe", "serie", "patamar"] + cols]
             df = df.astype(
-                {"Classe": "int64", "Série": "int64", "Ano": "int64"}
+                {"classe": "int64", "serie": "int64", "ano": "int64"}
             )
-            return df
+            return formata_df_meses_para_datas_nwlistop(df)
 
         self.__ano = self.__linha_ano.read(file.readline())[0]
         file.readline()
 
         # Variáveis auxiliares
         self.__classe_atual = 0
         self.__serie_atual = 0
         tabela = np.zeros(
             (
                 MAX_PATAMARES * MAX_SERIES_SINTETICAS * MAX_UTES,
-                len(MESES_DF) + 3,
+                len(MESES_DF) + 2,
             )
         )
         patamares: List[str] = []
         i = 0
         intervalo_classes = False
         while True:
             linha = file.readline()
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/blocos/valoresserie.py` & `inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,76 @@
 from cfinterface.components.block import Block
 from cfinterface.components.line import Line
 
-from inewave.config import MESES_DF, MAX_SERIES_SINTETICAS
+from inewave.config import MESES_DF, MAX_PATAMARES, MAX_SERIES_SINTETICAS
+from inewave._utils.formatacao import formata_df_meses_para_datas_nwlistop
 
-from typing import IO
+from typing import IO, List
 import pandas as pd  # type: ignore
 import numpy as np  # type: ignore
 
 
-class ValoresSerie(Block):
+class ValoresSeriePatamar(Block):
     """
-    Bloco com a informaçao de uma tabela para o SIN, com
-    entradas por série.
+    Bloco com a informaçao de uma tabela por submercado, com
+    entradas por série e patamar.
     """
 
     BEGIN_PATTERN = "     ANO: "
-    END_PATTERN = "MEDIA  "
+    END_PATTERN = " MEDIA"
     HEADER_LINE = Line([])
     DATA_LINE = Line([])
 
     def __init__(self, previous=None, next=None, data=None) -> None:
         super().__init__(previous, next, data)
         self.__linha_ano = self.__class__.HEADER_LINE
         self.__linha = self.__class__.DATA_LINE
 
     def __eq__(self, o: object) -> bool:
-        if not isinstance(o, ValoresSerie):
+        if not isinstance(o, ValoresSeriePatamar):
             return False
-        bloco: ValoresSerie = o
+        bloco: ValoresSeriePatamar = o
         if not all(
             [
                 isinstance(self.data, pd.DataFrame),
                 isinstance(o.data, pd.DataFrame),
             ]
         ):
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            cols = ["Série"] + MESES_DF + ["Média"]
-            df = pd.DataFrame(tabela, columns=cols)
-            df["Ano"] = self.__ano
-            df.loc[df["Série"].isna(), "Série"] = 1
-            df = df[["Ano"] + cols]
-            df = df.astype({"Série": "int64", "Ano": "int64"})
-            return df
+            cols = MESES_DF
+            df = pd.DataFrame(tabela, columns=["serie"] + cols)
+            df["ano"] = self.__ano
+            df.loc[df["serie"].isna(), "serie"] = 1
+            df["patamar"] = patamares
+            df = df[["ano", "serie", "patamar"] + cols]
+            df = df.astype({"serie": "int64", "ano": "int64"})
+            return formata_df_meses_para_datas_nwlistop(df)
 
         self.__ano = self.__linha_ano.read(file.readline())[0]
         file.readline()
 
         # Variáveis auxiliares
-        tabela = np.zeros((MAX_SERIES_SINTETICAS, len(MESES_DF) + 2))
+        self.__serie_atual = 0
+        tabela = np.zeros(
+            (MAX_PATAMARES * MAX_SERIES_SINTETICAS, len(MESES_DF) + 1)
+        )
+        patamares: List[str] = []
         i = 0
         while True:
             linha = file.readline()
             if self.ends(linha) or len(linha) <= 1:
                 tabela = tabela[:i, :]
                 self.data = converte_tabela_em_df()
                 break
-            tabela[i, :] = self.__linha.read(linha)
+            dados = self.__linha.read(linha)
+            if dados[0] is not None:
+                self.__serie_atual = dados[0]
+            tabela[i, 0] = self.__serie_atual
+            patamares.append(dados[1])
+            tabela[i, 1:] = dados[2:]
             i += 1
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py` & `inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresserie.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,66 @@
 from cfinterface.components.block import Block
 from cfinterface.components.line import Line
 
-from inewave.config import MESES_DF, MAX_PATAMARES, MAX_SERIES_SINTETICAS
+from inewave.config import MESES_DF, MAX_SERIES_SINTETICAS
+from inewave._utils.formatacao import formata_df_meses_para_datas_nwlistop
 
-from typing import IO, List
+from typing import IO
 import pandas as pd  # type: ignore
 import numpy as np  # type: ignore
 
 
-class ValoresSeriePatamar(Block):
+class ValoresSerie(Block):
     """
-    Bloco com a informaçao de uma tabela por submercado, com
-    entradas por série e patamar.
+    Bloco com a informaçao de uma tabela para o SIN, com
+    entradas por série.
     """
 
     BEGIN_PATTERN = "     ANO: "
-    END_PATTERN = " MEDIA"
+    END_PATTERN = "MEDIA  "
     HEADER_LINE = Line([])
     DATA_LINE = Line([])
 
     def __init__(self, previous=None, next=None, data=None) -> None:
         super().__init__(previous, next, data)
         self.__linha_ano = self.__class__.HEADER_LINE
         self.__linha = self.__class__.DATA_LINE
 
     def __eq__(self, o: object) -> bool:
-        if not isinstance(o, ValoresSeriePatamar):
+        if not isinstance(o, ValoresSerie):
             return False
-        bloco: ValoresSeriePatamar = o
+        bloco: ValoresSerie = o
         if not all(
             [
                 isinstance(self.data, pd.DataFrame),
                 isinstance(o.data, pd.DataFrame),
             ]
         ):
             return False
         else:
             return self.data.equals(bloco.data)
 
     # Override
     def read(self, file: IO, *args, **kwargs):
         def converte_tabela_em_df():
-            cols = MESES_DF + ["Média"]
-            df = pd.DataFrame(tabela, columns=["Série"] + cols)
-            df["Ano"] = self.__ano
-            df.loc[df["Série"].isna(), "Série"] = 1
-            df["Patamar"] = patamares
-            df = df[["Ano", "Série", "Patamar"] + cols]
-            df = df.astype({"Série": "int64", "Ano": "int64"})
-            return df
+            cols = ["serie"] + MESES_DF
+            df = pd.DataFrame(tabela, columns=cols)
+            df["ano"] = self.__ano
+            df.loc[df["serie"].isna(), "serie"] = 1
+            df = df[["ano"] + cols]
+            df = df.astype({"serie": "int64", "ano": "int64"})
+            return formata_df_meses_para_datas_nwlistop(df)
 
         self.__ano = self.__linha_ano.read(file.readline())[0]
         file.readline()
 
         # Variáveis auxiliares
-        self.__serie_atual = 0
-        tabela = np.zeros(
-            (MAX_PATAMARES * MAX_SERIES_SINTETICAS, len(MESES_DF) + 2)
-        )
-        patamares: List[str] = []
+        tabela = np.zeros((MAX_SERIES_SINTETICAS, len(MESES_DF) + 1))
         i = 0
         while True:
             linha = file.readline()
             if self.ends(linha) or len(linha) <= 1:
                 tabela = tabela[:i, :]
                 self.data = converte_tabela_em_df()
                 break
-            dados = self.__linha.read(linha)
-            if dados[0] is not None:
-                self.__serie_atual = dados[0]
-            tabela[i, 0] = self.__serie_atual
-            patamares.append(dados[1])
-            tabela[i, 1:] = dados[2:]
+            tabela[i, :] = self.__linha.read(linha)
             i += 1
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/cdef.py` & `inewave-0.0.98/inewave/nwlistop/modelos/cdef.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(10, 7 + 10 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(10, 7 + 10 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/cdefsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/cdefsin.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(10, 7 + 10 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(10, 7 + 10 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/cmarg.py` & `inewave-0.0.98/inewave/nwlistop/modelos/cmarg.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             IntegerField(2, 9),
         ]
-        + [FloatField(8, 15 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 15 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/cmargmed.py` & `inewave-0.0.98/inewave/nwlistop/modelos/cterm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
-from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
+from inewave.nwlistop.modelos.blocos.valoresserie import (
+    ValoresSerie,
+)
 
 
-class CmargsAnos(ValoresSerie):
+class CtermsAnos(ValoresSerie):
     """
-    Bloco com a informaçao do submercado associado aos valores de Custo
-    Marginal de Operação.
+    Bloco com a informaçao do submercado associado aos valores de custo
+    de geração térmica.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(8, 9 + 10 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 8 + 10 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/coper.py` & `inewave-0.0.98/inewave/nwlistop/modelos/coper.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(10, 7 + 10 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(10, 7 + 10 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/corteolm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/dfphauh.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from cfinterface.components.floatfield import FloatField
 
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class CorteolmAnos(ValoresSeriePatamar):
+class DfphauhAnos(ValoresSeriePatamar):
     """
     Bloco com as informações das tabelas de corte de geração eólica
     da usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(9, 11 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/cterm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/qafluh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
+
 from inewave.nwlistop.modelos.blocos.valoresserie import (
     ValoresSerie,
 )
 
 
-class CtermsAnos(ValoresSerie):
+class QaflAnos(ValoresSerie):
     """
-    Bloco com a informaçao do submercado associado aos valores de custo
-    de geração térmica.
+    Bloco com as informações das tabelas de vazão afluente por
+    usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 8 + 10 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/ctermsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/ctermsin.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 8 + 10 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 8 + 10 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/def.py` & `inewave-0.0.98/inewave/nwlistop/modelos/ghtot.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,20 @@
 
 
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class DefAnos(ValoresSeriePatamar):
+class GHAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de déficit.
+    Bloco com as informações das tabelas de geração hidráulica.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
-        [
+        [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
-        ]  # type: ignore
-        + [
-            FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)  # type: ignore
         ]
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/defsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/geol.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
-
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class DefAnos(ValoresSeriePatamar):
+class GEAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de déficit.
+    Bloco com as informações das tabelas de geração eólica.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
-        [
+        [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
-        ]  # type: ignore
-        + [
-            FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)  # type: ignore
         ]
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/depminuh.py` & `inewave-0.0.98/inewave/nwlistop/modelos/depminuh.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/dflppdfmaxm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/dflppdfmaxm.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/dflpptbmaxm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/dflpptbmaxm.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/dfphauh.py` & `inewave-0.0.98/inewave/nwlistop/modelos/dvazmax.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from cfinterface.components.floatfield import FloatField
 
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class DfphauhAnos(ValoresSeriePatamar):
+class DvazmaxAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de corte de geração eólica
+    Bloco com as informações das tabelas de violação de vazão máxima
     da usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/dlppdfmax.py` & `inewave-0.0.98/inewave/nwlistop/modelos/corteolm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
-from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
+from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
 
-
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class DLPPdfmaxAnos(ValoresSeriePatamar):
+class CorteolmAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de violação das restrições LPP
-    de defluência máxima.
+    Bloco com as informações das tabelas de corte de geração eólica
+    da usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 11 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/dlppdfmaxs.py` & `inewave-0.0.98/inewave/nwlistop/modelos/dlppdfmaxs.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/dlpptbmax.py` & `inewave-0.0.98/inewave/nwlistop/modelos/rhslppdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class DLPPtbmaxAnos(ValoresSeriePatamar):
+class RHSLPPdfAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de violação das restrições LPP
-    de turbinamento máximo.
+    Bloco com as informações das tabelas de RHS das restrições LPP
+    de defluência máxima.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/dlpptbmaxs.py` & `inewave-0.0.98/inewave/nwlistop/modelos/ghmax.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 
 
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class DLPPtbmaxAnos(ValoresSeriePatamar):
+class GHAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de violação das restrições LPP
-    de turbinamento máximo.
+    Bloco com as informações das tabelas de geração hidráulica máxima.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/dtbmax.py` & `inewave-0.0.98/inewave/nwlistop/modelos/vghminuh.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from cfinterface.components.floatfield import FloatField
 
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class DtbmaxAnos(ValoresSeriePatamar):
+class VGhminuhAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de violação de turbinamento máximo
-    da usina por mês/ano de estudo.
+    Bloco com as informações das tabelas de violação da meta de
+    geração hidráulica mínima por usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/dtbmin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/dtbmax.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from cfinterface.components.floatfield import FloatField
 
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class DtbminAnos(ValoresSeriePatamar):
+class DtbmaxAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de violação de turbinamento mínimo
+    Bloco com as informações das tabelas de violação de turbinamento máximo
     da usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/dvazmax.py` & `inewave-0.0.98/inewave/nwlistop/modelos/ghmaxm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
-from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.integerfield import IntegerField
+from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
+
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class DvazmaxAnos(ValoresSeriePatamar):
+class GHAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de violação de vazão máxima
-    da usina por mês/ano de estudo.
+    Bloco com as informações das tabelas de geração hidráulica máxima.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/eaf.py` & `inewave-0.0.98/inewave/nwlistop/modelos/eaf.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(8, 6 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 6 + 9 * i, 0) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/eafb.py` & `inewave-0.0.98/inewave/nwlistop/modelos/eafb.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(8, 7 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 7 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/eafbm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/eafm.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,10 +14,10 @@
     por série e por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [IntegerField(4, 2)]  # type: ignore
         + [
-            FloatField(8, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)  # type: ignore
+            FloatField(8, 6 + 9 * i, 0) for i in range(len(MESES_DF))  # type: ignore
         ]
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/eafbsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/eafbsin.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     por série e por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [IntegerField(4, 2)]  # type: ignore
         + [
-            FloatField(9, 6 + 9 * i, 0) for i in range(len(MESES_DF) + 1)  # type: ignore
+            FloatField(9, 6 + 9 * i, 0) for i in range(len(MESES_DF))  # type: ignore
         ]
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/eafm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/eafbm.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,10 +14,10 @@
     por série e por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [IntegerField(4, 2)]  # type: ignore
         + [
-            FloatField(8, 6 + 9 * i, 0) for i in range(len(MESES_DF) + 1)  # type: ignore
+            FloatField(8, 7 + 9 * i, 0) for i in range(len(MESES_DF))  # type: ignore
         ]
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/earmf.py` & `inewave-0.0.98/inewave/nwlistop/modelos/earmf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(8, 8 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 8 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/earmfm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/earmfm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     por série e por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [IntegerField(4, 2)]  # type: ignore
         + [
-            FloatField(8, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)  # type: ignore
+            FloatField(8, 7 + 9 * i, 0) for i in range(len(MESES_DF))  # type: ignore
         ]
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/earmfp.py` & `inewave-0.0.98/inewave/nwlistop/modelos/earmfp.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,9 +15,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
         ]
-        + [FloatField(8, 7 + 10 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 7 + 10 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/earmfpm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/earmfpm.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     por série e por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [IntegerField(4, 1)]  # type: ignore
         + [
-            FloatField(8, 7 + 10 * i, 1) for i in range(len(MESES_DF) + 1)  # type: ignore
+            FloatField(8, 7 + 10 * i, 1) for i in range(len(MESES_DF))  # type: ignore
         ]
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/earmfpsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/earmfpsin.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,10 +14,10 @@
     por série e por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [IntegerField(4, 1)]  # type: ignore
         + [
-            FloatField(8, 7 + 10 * i, 1) for i in range(len(MESES_DF) + 1)  # type: ignore
+            FloatField(8, 7 + 10 * i, 1) for i in range(len(MESES_DF))  # type: ignore
         ]
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/earmfsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/earmfsin.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     final em MWmes para o SIN.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [IntegerField(4, 2)]  # type: ignore
         + [
-            FloatField(9, 6 + 9 * i, 0) for i in range(len(MESES_DF) + 1)  # type: ignore
+            FloatField(9, 6 + 9 * i, 0) for i in range(len(MESES_DF))  # type: ignore
         ]
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/evert.py` & `inewave-0.0.98/inewave/nwlistop/modelos/evert.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/evertm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/evertm.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/evertsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/evertsin.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/exces.py` & `inewave-0.0.98/inewave/nwlistop/modelos/exces.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/excessin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/excessin.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/fteolm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/fteolm.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/fteolsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/fteolsin.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/geol.py` & `inewave-0.0.98/inewave/nwlistop/modelos/ghmaxmr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
+
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class GEAnos(ValoresSeriePatamar):
+class GHAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração eólica.
+    Bloco com as informações das tabelas de geração hidráulica máxima.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/geolm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/ghmaxr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
+
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class GEAnos(ValoresSeriePatamar):
+class GHAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração eólica.
+    Bloco com as informações das tabelas de geração hidráulica máxima.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/geolsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/ghmaxrsin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
+
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class GEAnos(ValoresSeriePatamar):
+class GHAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração eólica.
+    Bloco com as informações das tabelas de geração hidráulica máxima.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/ghiduh.py` & `inewave-0.0.98/inewave/nwlistop/modelos/dtbmin.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from cfinterface.components.floatfield import FloatField
 
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class GhidAnos(ValoresSeriePatamar):
+class DtbminAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração hidráulica
-    usina por mês/ano de estudo.
+    Bloco com as informações das tabelas de violação de turbinamento mínimo
+    da usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/ghmax.py` & `inewave-0.0.98/inewave/nwlistop/modelos/ghmaxsin.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/ghmaxm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/ghtotsin.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
 class GHAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração hidráulica máxima.
+    Bloco com as informações das tabelas de geração hidráulica.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
-        [  # type: ignore
+        [
             IntegerField(4, 1),
             LiteralField(5, 6),
+        ]  # type: ignore
+        + [
+            FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))  # type: ignore
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/ghmaxmr.py` & `inewave-0.0.98/inewave/nwlistop/modelos/ghtotm.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
 
-from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
-    ValoresSeriePatamar,
-)
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import ValoresSeriePatamar  # type: ignore
 
 
 class GHAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração hidráulica máxima.
+    Bloco com as informações das tabelas de geração hidráulica.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/ghmaxr.py` & `inewave-0.0.98/inewave/nwlistop/modelos/gttotsin.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
 
-from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
-    ValoresSeriePatamar,
-)
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import ValoresSeriePatamar  # type: ignore
 
 
-class GHAnos(ValoresSeriePatamar):
+class GTAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração hidráulica máxima.
+    Bloco com as informações das tabelas de geração térmica.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/ghmaxrsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/intercambio.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
 
-from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
-    ValoresSeriePatamar,
-)
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import ValoresSeriePatamar  # type: ignore
 
 
-class GHAnos(ValoresSeriePatamar):
+class IntercambioAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração hidráulica máxima.
+    Bloco com as informações das tabelas de intercâmbio.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 1),
+            IntegerField(4, 2),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/ghmaxsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/gtert.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
-
-from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
-    ValoresSeriePatamar,
+from inewave.nwlistop.modelos.blocos.valoresclassetermicaseriepatamar import (
+    ValoresClasseTermicaSeriePatamar,  # type: ignore
 )
 
 
-class GHAnos(ValoresSeriePatamar):
+class GTAnos(ValoresClasseTermicaSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração hidráulica máxima.
+    Bloco com as informações das tabelas de geração térmica por classe.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 1),
-            LiteralField(5, 6),
+            IntegerField(3, 2),
+            IntegerField(4, 7),
+            LiteralField(1, 15),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 16 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/ghtot.py` & `inewave-0.0.98/inewave/nwlistop/modelos/geolm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
-
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class GHAnos(ValoresSeriePatamar):
+class GEAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração hidráulica.
+    Bloco com as informações das tabelas de geração eólica.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/ghtotm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/verturb.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
-from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
 
-from inewave.nwlistop.modelos.blocos.valoresseriepatamar import ValoresSeriePatamar  # type: ignore
+from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
 
 
-class GHAnos(ValoresSeriePatamar):
+class VertAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de geração hidráulica.
+    Bloco com as informações das tabelas de energia vertida
+    por série e por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 1),
-            LiteralField(5, 6),
+            IntegerField(4, 2),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 7 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/ghtotsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/dlppdfmax.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 
 
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class GHAnos(ValoresSeriePatamar):
+class DLPPdfmaxAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração hidráulica.
+    Bloco com as informações das tabelas de violação das restrições LPP
+    de defluência máxima.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
-        [
+        [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
-        ]  # type: ignore
-        + [
-            FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)  # type: ignore
         ]
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/gtert.py` & `inewave-0.0.98/inewave/nwlistop/modelos/rhslpptb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
-from inewave.nwlistop.modelos.blocos.valoresclassetermicaseriepatamar import (
-    ValoresClasseTermicaSeriePatamar,  # type: ignore
+
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
 )
 
 
-class GTAnos(ValoresClasseTermicaSeriePatamar):
+class RHSLPPtbAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de geração térmica por classe.
+    Bloco com as informações das tabelas de RHS das restrições LPP
+    de turbinamento máximo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(3, 2),
-            IntegerField(4, 7),
-            LiteralField(1, 15),
+            IntegerField(4, 1),
+            LiteralField(5, 6),
         ]
-        + [FloatField(9, 16 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/gttot.py` & `inewave-0.0.98/inewave/nwlistop/modelos/gttot.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/gttotsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/verturbm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
-from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
 
-from inewave.nwlistop.modelos.blocos.valoresseriepatamar import ValoresSeriePatamar  # type: ignore
+from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
 
 
-class GTAnos(ValoresSeriePatamar):
+class VertAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de geração térmica.
+    Bloco com as informações das tabelas de energia vertida
+    por série e por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 1),
-            LiteralField(5, 6),
+            IntegerField(4, 2),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 7 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/intercambio.py` & `inewave-0.0.98/inewave/nwlistop/modelos/verturbsin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
-from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
 
-from inewave.nwlistop.modelos.blocos.valoresseriepatamar import ValoresSeriePatamar  # type: ignore
+from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
 
 
-class IntercambioAnos(ValoresSeriePatamar):
+class VertAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de intercâmbio.
+    Bloco com as informações das tabelas de energia vertida
+    por série e por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
-            LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 7 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/invade.py` & `inewave-0.0.98/inewave/nwlistop/modelos/invade.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/invadem.py` & `inewave-0.0.98/inewave/nwlistop/modelos/invadem.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/mediasmerc.py` & `inewave-0.0.98/inewave/nwlistop/modelos/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/mediassin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/mercl.py` & `inewave-0.0.98/inewave/nwlistop/modelos/mercl.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(8, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 7 + 9 * i, 0) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/merclsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/merclsin.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(8, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 7 + 9 * i, 0) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/nwlistopdat.py` & `inewave-0.0.98/inewave/nwlistop/modelos/nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/perdf.py` & `inewave-0.0.98/inewave/nwlistop/modelos/cmargmed.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
 from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
 
 
-class PerdfAnos(ValoresSerie):
+class CmargsAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de vertimento fio d'água.
+    Bloco com a informaçao do submercado associado aos valores de Custo
+    Marginal de Operação.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 9 + 10 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/perdfm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/qincruh.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
-from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
 
+from inewave.nwlistop.modelos.blocos.valoresserie import (
+    ValoresSerie,
+)
 
-class PerdfAnos(ValoresSerie):
+
+class QincrAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de vertimento fio d'água.
+    Bloco com as informações das tabelas de vazão incremental por
+    usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/perdfsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/varmpuh.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
-from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
 
+from inewave.nwlistop.modelos.blocos.valoresserie import (
+    ValoresSerie,
+)
 
-class PerdfAnos(ValoresSerie):
+
+class VarmAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de vertimento fio d'água.
+    Bloco com as informações das tabelas de volume armazenado por
+    usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/qafluh.py` & `inewave-0.0.98/inewave/nwlistop/modelos/varmuh.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from cfinterface.components.floatfield import FloatField
 
 from inewave.nwlistop.modelos.blocos.valoresserie import (
     ValoresSerie,
 )
 
 
-class QaflAnos(ValoresSerie):
+class VarmAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de vazão afluente por
+    Bloco com as informações das tabelas de volume armazenado por
     usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/qincruh.py` & `inewave-0.0.98/inewave/nwlistop/modelos/vevmin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
+from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
 
-from inewave.nwlistop.modelos.blocos.valoresserie import (
-    ValoresSerie,
-)
 
-
-class QincrAnos(ValoresSerie):
+class VevminAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de vazão incremental por
-    usina por mês/ano de estudo.
+    Bloco com as informações das tabelas de violação da meta
+    de energia de vazão mínima em MWmes.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/rhslppdf.py` & `inewave-0.0.98/inewave/nwlistop/modelos/vevminm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
-from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
+from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
 
 
-from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
-    ValoresSeriePatamar,
-)
-
-
-class RHSLPPdfAnos(ValoresSeriePatamar):
+class VevminAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de RHS das restrições LPP
-    de defluência máxima.
+    Bloco com as informações das tabelas de violação da meta
+    de energia de vazão mínima em MWmes.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 1),
-            LiteralField(5, 6),
+            IntegerField(4, 2),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/vagua.py` & `inewave-0.0.98/inewave/nwlistop/modelos/ghiduh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
+from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
 
-from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
+)
 
 
-class VAAnos(ValoresSerie):
+class GhidAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de valor da água por
-    REE por mês/ano de estudo.
+    Bloco com as informações das tabelas de geração hidráulica
+    usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 2),
+            IntegerField(4, 1),
+            LiteralField(5, 6),
         ]
-        + [FloatField(8, 9 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/varmpuh.py` & `inewave-0.0.98/inewave/nwlistop/modelos/vturuh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
+from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
 
-from inewave.nwlistop.modelos.blocos.valoresserie import (
-    ValoresSerie,
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
 )
 
 
-class VarmAnos(ValoresSerie):
+class VturAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de volume armazenado por
+    Bloco com as informações das tabelas de volume turbinado por
     usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 2),
+            IntegerField(4, 1),
+            LiteralField(5, 6),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/varmuh.py` & `inewave-0.0.98/inewave/nwlistop/modelos/vertuh.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
+from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
 
-from inewave.nwlistop.modelos.blocos.valoresserie import (
-    ValoresSerie,
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
 )
 
 
-class VarmAnos(ValoresSerie):
+class VertAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de volume armazenado por
+    Bloco com as informações das tabelas de volume vertido por
     usina por mês/ano de estudo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 2),
+            IntegerField(4, 1),
+            LiteralField(5, 6),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/vento.py` & `inewave-0.0.98/inewave/nwlistop/modelos/vevminsin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.floatfield import FloatField
+from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
 
-from inewave.nwlistop.modelos.blocos.valoresserie import (
-    ValoresSerie,
-)
 
-
-class VentoAnos(ValoresSerie):
+class VevminAnos(ValoresSerie):
     """
-    Bloco com as informações das tabelas de vento por
-    usina por mês/ano de estudo.
+    Bloco com as informações das tabelas de violação da meta
+    de energia de vazão mínima em MWmes.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 2),
         ]
-        + [FloatField(9, 6 + 9 * i, 4) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/vertuh.py` & `inewave-0.0.98/inewave/nwlistop/modelos/dlpptbmax.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
-from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.integerfield import IntegerField
+from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
+
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class VertAnos(ValoresSeriePatamar):
+class DLPPtbmaxAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de volume vertido por
-    usina por mês/ano de estudo.
+    Bloco com as informações das tabelas de violação das restrições LPP
+    de turbinamento máximo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/verturb.py` & `inewave-0.0.98/inewave/nwlistop/modelos/dlpptbmaxs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
+from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
 
-from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
+)
 
 
-class VertAnos(ValoresSerie):
+class DLPPtbmaxAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de energia vertida
-    por série e por mês/ano de estudo.
+    Bloco com as informações das tabelas de violação das restrições LPP
+    de turbinamento máximo.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 2),
+            IntegerField(4, 1),
+            LiteralField(5, 6),
         ]
-        + [FloatField(8, 7 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/verturbm.py` & `inewave-0.0.98/inewave/nwlistop/modelos/vghmin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
+from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
 
-from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
+)
 
 
-class VertAnos(ValoresSerie):
+class VghminAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de energia vertida
-    por série e por mês/ano de estudo.
+    Bloco com as informações das tabelas de violação da meta de
+    geração hidráulica mínima.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 2),
+            IntegerField(4, 1),
+            LiteralField(5, 6),
         ]
-        + [FloatField(8, 7 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/verturbsin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/vghminm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
+from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
 
-from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
+)
 
 
-class VertAnos(ValoresSerie):
+class VghminAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de energia vertida
-    por série e por mês/ano de estudo.
+    Bloco com as informações das tabelas de violação da meta de
+    geração hidráulica mínima.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 2),
+            IntegerField(4, 1),
+            LiteralField(5, 6),
         ]
-        + [FloatField(8, 7 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/vevmin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/vghminsin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
+from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
-from inewave.nwlistop.modelos.blocos.valoresserie import ValoresSerie
 
 
-class VevminAnos(ValoresSerie):
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
+)
+
+
+class VghminAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de violação da meta
-    de energia de vazão mínima em MWmes.
+    Bloco com as informações das tabelas de violação da meta de
+    geração hidráulica mínima.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
-            IntegerField(4, 2),
+            IntegerField(4, 1),
+            LiteralField(5, 6),
         ]
-        + [FloatField(9, 7 + 9 * i, 0) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/vghmin.py` & `inewave-0.0.98/inewave/nwlistop/modelos/geolsin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
-
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class VghminAnos(ValoresSeriePatamar):
+class GEAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de violação da meta de
-    geração hidráulica mínima.
+    Bloco com as informações das tabelas de geração eólica.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
         [  # type: ignore
             IntegerField(4, 1),
             LiteralField(5, 6),
         ]
-        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF) + 1)]  # type: ignore
+        + [FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/modelos/vturuh.py` & `inewave-0.0.98/inewave/nwlistop/modelos/def.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from inewave.config import MESES_DF
 
 from cfinterface.components.line import Line
-from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.integerfield import IntegerField
+from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
 
+
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 
-class VturAnos(ValoresSeriePatamar):
+class DefAnos(ValoresSeriePatamar):
     """
-    Bloco com as informações das tabelas de volume turbinado por
-    usina por mês/ano de estudo.
+    Bloco com as informações das tabelas de déficit.
     """
 
     HEADER_LINE = Line([IntegerField(4, 10)])
     DATA_LINE = Line(
-        [  # type: ignore
+        [
             IntegerField(4, 1),
             LiteralField(5, 6),
+        ]  # type: ignore
+        + [
+            FloatField(8, 12 + 9 * i, 1) for i in range(len(MESES_DF))  # type: ignore
         ]
-        + [FloatField(9, 14 + 9 * i, 2) for i in range(len(MESES_DF) + 1)]  # type: ignore
     )
```

### Comparing `inewave-0.0.97/inewave/nwlistop/nwlistopdat.py` & `inewave-0.0.98/inewave/nwlistop/nwlistopdat.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from inewave.nwlistop.modelos.nwlistopdat import (
     BlocoDadosNwlistop,
 )
 
 from cfinterface.files.sectionfile import SectionFile
-from typing import TypeVar, Optional, Type, List
+from typing import TypeVar, Optional, List
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
 class Nwlistopdat(SectionFile):
@@ -31,175 +31,155 @@
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def __bloco_por_tipo(self, bloco: Type[T], indice: int) -> Optional[T]:
-        """
-        Obtém um gerador de blocos de um tipo, se houver algum no arquivo.
-
-        :param bloco: Um tipo de bloco para ser lido
-        :type bloco: T
-        :param indice: O índice do bloco a ser acessado, dentre os do tipo
-        :type indice: int
-        :return: O gerador de blocos, se houver
-        :rtype: Optional[Generator[T], None, None]
-        """
-        try:
-            return next(
-                b
-                for i, b in enumerate(self.data.of_type(bloco))
-                if i == indice
-            )
-        except StopIteration:
-            return None
-
     @property
     def opcao(self) -> Optional[int]:
         """
         A opção de execução do programa nwlistop.
 
         :return: O flag de opção
         :rtype: Optional[int] | None
         """
-        b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+        if isinstance(b, BlocoDadosNwlistop):
             return b.data.get("opcao")
         return None
 
     @opcao.setter
     def opcao(self, v: int):
-        b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-        if b is not None:
+        b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+        if isinstance(b, BlocoDadosNwlistop):
             b.data["opcao"] = v
 
     @property
     def periodo_inicial_impressao(self) -> Optional[int]:
         """
         O período inicial para impressão dos dados de saída.
 
         :return: O índice do período
         :rtype: Optional[int] | None
         """
         if self.opcao in [1, 2, 4]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 return b.data["periodos"][0]
             return None
         else:
             raise ValueError("Períodos só são suportados nas opções [1, 2, 4]")
 
     @periodo_inicial_impressao.setter
     def periodo_inicial_impressao(self, v: int):
         if self.opcao in [1, 2, 4]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 b.data["periodos"][0] = v
         else:
             raise ValueError("Períodos só são suportados nas opções [1, 2, 4]")
 
     @property
     def periodo_final_impressao(self) -> Optional[int]:
         """
         O período final para impressão dos dados de saída.
 
         :return: O índice do período
         :rtype: Optional[int] | None
         """
         if self.opcao in [1, 2, 4]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 return b.data["periodos"][1]
             return None
         else:
             raise ValueError("Períodos só são suportados nas opções [1, 2, 4]")
 
     @periodo_final_impressao.setter
     def periodo_final_impressao(self, v: int):
         if self.opcao in [1, 2, 4]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 b.data["periodos"][1] = v
         else:
             raise ValueError("Períodos só são suportados nas opções [1, 2, 4]")
 
     @property
     def serie_inicial_impressao(self) -> Optional[int]:
         """
         A série inicial para impressão dos dados de saída.
 
         :return: O índice da série
         :rtype: Optional[int] | None
         """
         if self.opcao in [1]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 return b.data["series"][0]
             return None
         else:
             raise ValueError("Séries só são suportadas na opção [1]")
 
     @serie_inicial_impressao.setter
     def serie_inicial_impressao(self, v: int):
         if self.opcao in [1]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 b.data["series"][0] = v
         else:
             raise ValueError("Séries só são suportadas na opção [1]")
 
     @property
     def serie_final_impressao(self) -> Optional[int]:
         """
         A série final para impressão dos dados de saída.
 
         :return: O índice da série
         :rtype: Optional[int] | None
         """
         if self.opcao in [1]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 return b.data["series"][1]
             return None
         else:
             raise ValueError("Séries só são suportadas na opção [1]")
 
     @serie_final_impressao.setter
     def serie_final_impressao(self, v: int):
         if self.opcao in [1]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 b.data["series"][1] = v
         else:
             raise ValueError("Séries só são suportadas na opção [1]")
 
     @property
     def variaveis_impressao_estagios_agregados(self) -> Optional[List[int]]:
         """
         As variáveis dos períodos agregados a serem impressas na
         opção 2.
 
         :return: A lista dos códigos das variáveis.
         :rtype: Optional[List[int]] | None
         """
         if self.opcao in [2]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 return b.data["variaveis_ree"]
             return None
         else:
             raise ValueError("Variáveis só são suportadas na opção [2]")
 
     @variaveis_impressao_estagios_agregados.setter
     def variaveis_impressao_estagios_agregados(self, v: List[int]):
         if self.opcao in [2]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 b.data["variaveis_ree"] = v
         else:
             raise ValueError("Variáveis só são suportadas na opção [2]")
 
     @property
     def variaveis_impressao_estagios_individualizados(
         self,
@@ -208,26 +188,26 @@
         As variáveis dos períodos individualizados a serem impressas na
         opção 2.
 
         :return: A lista dos códigos das variáveis.
         :rtype: Optional[List[int]] | None
         """
         if self.opcao in [2]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 return b.data["variaveis_uhe"]
             return None
         else:
             raise ValueError("Variáveis só são suportadas na opção [2]")
 
     @variaveis_impressao_estagios_individualizados.setter
     def variaveis_impressao_estagios_individualizados(self, v: List[int]):
         if self.opcao in [2]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 b.data["variaveis_uhe"] = v
         else:
             raise ValueError("Variáveis só são suportadas na opção [2]")
 
     @property
     def uhes_impressao_estagios_individualizados(
         self,
@@ -235,22 +215,22 @@
         """
         As UHEs que terão as variáveis impressas na opção 2.
 
         :return: A lista dos códigos das UHEs.
         :rtype: Optional[List[int]] | None
         """
         if self.opcao in [2]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 return b.data["uhes"]
             return None
         else:
             raise ValueError("UHEs só são suportadas na opção [2]")
 
     @uhes_impressao_estagios_individualizados.setter
     def uhes_impressao_estagios_individualizados(self, v: List[int]):
         if self.opcao in [2]:
-            b = self.__bloco_por_tipo(BlocoDadosNwlistop, 0)
-            if b is not None:
+            b = self.data.get_sections_of_type(BlocoDadosNwlistop)
+            if isinstance(b, BlocoDadosNwlistop):
                 b.data["uhes"] = v
         else:
             raise ValueError("UHEs só são suportadas na opção [2]")
```

### Comparing `inewave-0.0.97/inewave/nwlistop/perdf.py` & `inewave-0.0.98/inewave/nwlistop/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/perdfm.py` & `inewave-0.0.98/inewave/nwlistop/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/perdfsin.py` & `inewave-0.0.98/inewave/nwlistop/vertuh.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.modelos.arquivos.arquivosin import (
-    ArquivoSIN,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.perdfsin import PerdfAnos
+from inewave.nwlistop.modelos.vertuh import VertAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class PerdfSIN(ArquivoSIN):
+class Vertuh(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes ao vertimento fio d'água
-    , para o SIN.
+    Armazena os dados das saídas referentes aos vertimentos por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas no `perdfsin.out`.
+    NWLISTOP e reproduzidas nos `vertuh00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
-        PerdfAnos,
+        Usina,
+        VertAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="perdfsin.out"
-    ) -> "PerdfSIN":
+        cls, diretorio: str, nome_arquivo="vertuh001.out"
+    ) -> "Vertuh":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/qafluh.py` & `inewave-0.0.98/inewave/nwlistop/vturuh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousina import (
-    ArquivoUsina,
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.qafluh import QaflAnos
+from inewave.nwlistop.modelos.vturuh import VturAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class QaflUH(ArquivoUsina):
+class Vturuh(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes às vazões afluentes por usina.
+    Armazena os dados das saídas referentes às vazões turbinadas por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `qafluh00x.out`, onde x varia conforme a
+    NWLISTOP e reproduzidas nos `vturuh00x.out`, onde x varia conforme a
     usina em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        QaflAnos,
+        VturAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="qafluh001.out"
-    ) -> "QaflUH":
+        cls, diretorio: str, nome_arquivo="vturuh001.out"
+    ) -> "Vturuh":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/qincruh.py` & `inewave-0.0.98/inewave/nwlistop/qincruh.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from inewave.nwlistop.modelos.qincruh import QincrAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class QincrUH(ArquivoUsina):
+class Qincruh(ArquivoUsina):
     """
     Armazena os dados das saídas referentes às vazões incrementais por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `qincruh00x.out`, onde x varia conforme a
     usina em questão.
 
@@ -23,14 +23,14 @@
         Usina,
         QincrAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="qincruh001.out"
-    ) -> "QincrUH":
+    ) -> "Qincruh":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/rhslppdf.py` & `inewave-0.0.98/inewave/nwlistop/rhslpptb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
     ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.rhslppdf import RHSLPPdfAnos
+from inewave.nwlistop.modelos.rhslpptb import RHSLPPtbAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class RHSLPPdf(ArquivoREEPatamar):
+class Rhslpptb(ArquivoREEPatamar):
     """
     Armazena os dados das saídas referentes ao RHS das restrições LPP
-    de defluência máxima por patamar, por REE.
+    de turbinamento máximo por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `rhslppdf00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `rhslpptb00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         REE,
-        RHSLPPdfAnos,
+        RHSLPPtbAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="rhslppdf001.out"
-    ) -> "RHSLPPdf":
+        cls, diretorio: str, nome_arquivo="rhslpptb001.out"
+    ) -> "Rhslpptb":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/rhslpptb.py` & `inewave-0.0.98/inewave/nwlistop/dlpptbmaxs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
-    ArquivoREEPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
+    ArquivoSINPatamar,
 )
-from inewave.nwlistop.modelos.rhslpptb import RHSLPPtbAnos
+from inewave.nwlistop.modelos.dlpptbmaxs import DLPPtbmaxAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class RHSLPPtb(ArquivoREEPatamar):
+class Dlpptbmaxs(ArquivoSINPatamar):
     """
-    Armazena os dados das saídas referentes ao RHS das restrições LPP
-    de turbinamento máximo por patamar, por REE.
+    Armazena os dados das saídas referentes à violação das restrições
+    LPP de turbinamento máximo por patamar para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `rhslpptb00x.out`, onde x varia conforme o
-    REE em questão.
-
+    NWLISTOP e reproduzidas nos `dlpptbmaxs.out`.
     """
 
     BLOCKS = [
-        REE,
-        RHSLPPtbAnos,
+        DLPPtbmaxAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="rhslpptb001.out"
-    ) -> "RHSLPPtb":
+        cls, diretorio: str, nome_arquivo="dlpptbmaxs.out"
+    ) -> "Dlpptbmaxs":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/vagua.py` & `inewave-0.0.98/inewave/nwlistop/ctermsin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
-
-from inewave.nwlistop.modelos.vagua import VAAnos
+from inewave.nwlistop.modelos.ctermsin import CtermsAnos
+from inewave.nwlistop.modelos.arquivos.arquivosin import (
+    ArquivoSIN,
+)
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Vagua(ArquivoREE):
+class Ctermsin(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes aos valores da água
-    por REE.
+    Armazena os dados das saídas referentes aos custos de geração térmica
+    para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vagua00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas nos `ctermsin.out`.
 
     """
 
     BLOCKS = [
-        REE,
-        VAAnos,
+        CtermsAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vagua001.out"
-    ) -> "Vagua":
+        cls, diretorio: str, nome_arquivo="ctermsin.out"
+    ) -> "Ctermsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/varmpuh.py` & `inewave-0.0.98/inewave/nwlistop/varmpuh.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from inewave.nwlistop.modelos.varmpuh import VarmAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class VarmpUH(ArquivoUsina):
+class Varmpuh(ArquivoUsina):
     """
     Armazena os dados das saídas referentes aos armazenamentos em
     percentual por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `varmpuh00x.out`, onde x varia conforme a
     usina em questão.
@@ -24,14 +24,14 @@
         Usina,
         VarmAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="varmpuh001.out"
-    ) -> "VarmpUH":
+    ) -> "Varmpuh":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/varmuh.py` & `inewave-0.0.98/inewave/nwlistop/varmuh.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from inewave.nwlistop.modelos.varmuh import VarmAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class VarmUH(ArquivoUsina):
+class Varmuh(ArquivoUsina):
     """
     Armazena os dados das saídas referentes aos armazenamentos por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `varmuh00x.out`, onde x varia conforme a
     usina em questão.
 
@@ -23,14 +23,14 @@
         Usina,
         VarmAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="varmuh001.out"
-    ) -> "VarmUH":
+    ) -> "Varmuh":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/vento.py` & `inewave-0.0.98/inewave/nwlistop/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/vertuh.py` & `inewave-0.0.98/inewave/nwlistop/vevminm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
-    ArquivoUsinaPatamar,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.vertuh import VertAnos
+from inewave.nwlistop.modelos.vevminm import VevminAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class VertUH(ArquivoUsinaPatamar):
+class Vevminm(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes aos vertimentos por usina.
+    Armazena os dados das saídas referentes às violações da meta
+    de energia da vazão mínima, por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vertuh00x.out`, onde x varia conforme a
-    usina em questão.
+    NWLISTOP e reproduzidas nos `vevminm00x.out`, onde x varia conforme o
+    Submercado em questão.
 
     """
 
     BLOCKS = [
-        Usina,
-        VertAnos,
+        Submercado,
+        VevminAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vertuh001.out"
-    ) -> "VertUH":
+        cls, diretorio: str, nome_arquivo="vevminm001.out"
+    ) -> "Vevminm":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/verturb.py` & `inewave-0.0.98/inewave/nwlistop/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/verturbm.py` & `inewave-0.0.98/inewave/nwlistop/perdfsin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
-    ArquivoSubmercado,
+from inewave.nwlistop.modelos.arquivos.arquivosin import (
+    ArquivoSIN,
 )
-from inewave.nwlistop.modelos.verturbm import VertAnos
+from inewave.nwlistop.modelos.perdfsin import PerdfAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Verturbm(ArquivoSubmercado):
+class Perdfsin(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes às energias
-    vertidas, por submercado.
+    Armazena os dados das saídas referentes ao vertimento fio d'água
+    , para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vertub00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas no `perdfsin.out`.
 
     """
 
     BLOCKS = [
-        Submercado,
-        VertAnos,
+        PerdfAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="verturbm001.out"
-    ) -> "Verturbm":
+        cls, diretorio: str, nome_arquivo="perdfsin.out"
+    ) -> "Perdfsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/verturbsin.py` & `inewave-0.0.98/inewave/nwlistop/vghminsin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from inewave.nwlistop.modelos.verturbsin import VertAnos
-from inewave.nwlistop.modelos.arquivos.arquivosin import (
-    ArquivoSIN,
+from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
+    ArquivoSINPatamar,
 )
+from inewave.nwlistop.modelos.vghmin import VghminAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class VerturbSIN(ArquivoSIN):
+class Vghminsin(ArquivoSINPatamar):
     """
-    Armazena os dados das saídas referentes às energias
-    vertidas para o SIN.
+    Armazena os dados das saídas referentes à violação da meta de geração
+    hidraulica mínima por patamar, para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `verturbsin.out`.
+    NWLISTOP e reproduzidas no `vghminsin.out`.
 
     """
 
     BLOCKS = [
-        VertAnos,
+        VghminAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="verturbsin.out"
-    ) -> "VerturbSIN":
+        cls, diretorio: str, nome_arquivo="vghminsin.out"
+    ) -> "Vghminsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/vevmin.py` & `inewave-0.0.98/inewave/nwlistop/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/vevminm.py` & `inewave-0.0.98/inewave/nwlistop/earmfpsin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
-    ArquivoSubmercado,
+from inewave.nwlistop.modelos.earmfpsin import EarmsAnos
+
+from inewave.nwlistop.modelos.arquivos.arquivosin import (
+    ArquivoSIN,
 )
-from inewave.nwlistop.modelos.vevminm import VevminAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Vevminm(ArquivoSubmercado):
+class Earmfpsin(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes às violações da meta
-    de energia da vazão mínima, por Submercado.
+    Armazena os dados das saídas referentes às energias
+    armazenadas finais para o SIN e em % da energia armazenável máxima.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vevminm00x.out`, onde x varia conforme o
-    Submercado em questão.
-
+    NWLISTOP e reproduzidas nos `earmfpsin.out`, onde x varia conforme o
+    submercado em questão.
     """
 
     BLOCKS = [
-        Submercado,
-        VevminAnos,
+        EarmsAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vevminm001.out"
-    ) -> "Vevminm":
+        cls, diretorio: str, nome_arquivo="earmfpsin.out"
+    ) -> "Earmfpsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/vevminsin.py` & `inewave-0.0.98/inewave/nwlistop/vevminsin.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from inewave.nwlistop.modelos.vevminsin import VevminAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class VevminSIN(ArquivoSIN):
+class Vevminsin(ArquivoSIN):
     """
     Armazena os dados das saídas referentes às violações da meta
     de energia da vazão mínima para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
     NWLISTOP e reproduzidas nos `vevminsin.out`
 
@@ -21,14 +21,14 @@
     BLOCKS = [
         VevminAnos,
     ]
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="vevminsin.out"
-    ) -> "VevminSIN":
+    ) -> "Vevminsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/vghmin.py` & `inewave-0.0.98/inewave/nwlistop/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/vghminm.py` & `inewave-0.0.98/inewave/nwlistop/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/inewave/nwlistop/vghminsin.py` & `inewave-0.0.98/inewave/nwlistop/vghminuh.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
-    ArquivoSINPatamar,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.vghmin import VghminAnos
+from inewave.nwlistop.modelos.vghminuh import VGhminuhAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class VghminSIN(ArquivoSINPatamar):
+class Vghminuh(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à violação da meta de geração
-    hidraulica mínima por patamar, para o SIN.
+    Armazena os dados das saídas referentes à violação da meta de
+    geração hidráulica mínima por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas no `vghminsin.out`.
+    NWLISTOP e reproduzidas nos `vghminuh00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
-        VghminAnos,
+        Usina,
+        VGhminuhAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vghminsin.out"
-    ) -> "VghminSIN":
+        cls, diretorio: str, nome_arquivo="vghminuh001.out"
+    ) -> "Vghminuh":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/vghminuh.py` & `inewave-0.0.98/inewave/nwlistop/cmargmed.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
-    ArquivoUsinaPatamar,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.vghminuh import VGhminuhAnos
+from inewave.nwlistop.modelos.cmargmed import CmargsAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class VghminUH(ArquivoUsinaPatamar):
+class Cmargmed(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes à violação da meta de
-    geração hidráulica mínima por usina.
+    Armazena os dados das saídas referentes aos custos marginais de operação
+    por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vghminuh00x.out`, onde x varia conforme a
-    usina em questão.
+    NWLISTOP e reproduzidas nos `cmarg00x-med.out`, onde x varia conforme o
+    submercado em questão.
 
     """
 
     BLOCKS = [
-        Usina,
-        VGhminuhAnos,
+        Submercado,
+        CmargsAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vghminuh001.out"
-    ) -> "VghminUH":
+        cls, diretorio: str, nome_arquivo="cmarg001-med.out"
+    ) -> "Cmargmed":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave/nwlistop/vturuh.py` & `inewave-0.0.98/inewave/nwlistop/defsin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
-    ArquivoUsinaPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
+    ArquivoSINPatamar,
 )
-from inewave.nwlistop.modelos.vturuh import VturAnos
+from inewave.nwlistop.modelos.defsin import DefAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class VturUH(ArquivoUsinaPatamar):
+class Defsin(ArquivoSINPatamar):
     """
-    Armazena os dados das saídas referentes às vazões turbinadas por usina.
+    Armazena os dados das saídas referentes ao déficit
+    por patamar para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vturuh00x.out`, onde x varia conforme a
-    usina em questão.
-
+    NWLISTOP e reproduzidas nos `defsinp001.out`.
     """
 
     BLOCKS = [
-        Usina,
-        VturAnos,
+        DefAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vturuh001.out"
-    ) -> "VturUH":
+        cls, diretorio: str, nome_arquivo="defsinp001.out"
+    ) -> "Defsin":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.97/inewave.egg-info/PKG-INFO` & `inewave-0.0.98/inewave.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 0.0.97
+Version: 0.0.98
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,28 +20,31 @@
 
 O `inewave` é um pacote Python para manipulação dos arquivos de entrada e saída do programa [NEWAVE](http://www.cepel.br/pt_br/produtos/newave-modelo-de-planejamento-da-operacao-de-sistemas-hidrotermicos-interligados-de-longo-e-medio-prazo.htm). O NEWAVE é desenvolvido pelo [CEPEL](http://www.cepel.br) e utilizado para os estudos de planejamento e operação do Sistema Interligado Nacional (SIN).
 
 O inewave oferece:
 
 - Meios para leitura dos arquivos de entrada e saída do NEWAVE e programas associados: NWLISTCF e NWLISTOP
 
-- Armazenamento e processamento de dados otimizados com o uso de NumPy e Pandas
+- Facilidades para estudo e análise dos dados utilizando DataFrames do pandas
 
 - Dados estruturados em modelos com o uso do paradigma de orientação a objetos (OOP)
 
-- Utilidades de escritas dos arquivos de entrada do NEWAVE para elaboração automatizada de estudos
-
-Com inewave é possível ler os arquivos de texto, característicos do NEWAVE, para poupar processamento futuro e reduzir o tempo de execução.
 
 ## Instalação
 
-O inewave é compatível com versões de Python >= 3.8 e é construído com base no framework [cfinterface](https://github.com/rjmalves/cfi), que deve sempre ser mantido na versão mais atualizada para a distribuição de Python instalada.
+O inewave é compatível com versões de Python >= 3.8.
 
-Em posse de uma instalação local de Python, é recomendado que se use um ambiente virtual para instalação de módulos de terceiros, sendo que o inewave não é uma exceção. Para mais detalhes sobre o uso de ambientes virtuais, recomenda-se a leitura do recurso oficial de Python para ambientes virtuais: [venv](https://docs.python.org/3/library/venv.html).
+É possível instalar a versão distribuída oficialmente com pip:
 
 ```
 python -m pip install inewave
 ```
 
+É possível realizar a instalação da versão de desenvolvimento fazendo o uso do Git.
+
+```
+pip install git+https://github.com/rjmalves/inewave
+```
+
 ## Documentação
 
 Guias, tutoriais e as referências podem ser encontrados no site oficial do pacote: https://rjmalves.github.io/inewave
```

### Comparing `inewave-0.0.97/inewave.egg-info/SOURCES.txt` & `inewave-0.0.98/inewave.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 LICENSE.md
 README.md
 setup.py
+examples/__init__.py
+examples/plot_dger.py
+examples/plot_modif.py
+examples/plot_pmo.py
+examples/plot_sistema.py
 inewave/__init__.py
 inewave/config.py
 inewave/py.typed
 inewave.egg-info/PKG-INFO
 inewave.egg-info/SOURCES.txt
 inewave.egg-info/dependency_links.txt
 inewave.egg-info/requires.txt
 inewave.egg-info/top_level.txt
 inewave/_utils/__init__.py
+inewave/_utils/formatacao.py
 inewave/_utils/leituracsv.py
 inewave/newave/__init__.py
 inewave/newave/abertura.py
 inewave/newave/adterm.py
 inewave/newave/agrint.py
 inewave/newave/arquivos.py
 inewave/newave/avl_cortesfpha_nwv.py
```

### Comparing `inewave-0.0.97/setup.py` & `inewave-0.0.98/setup.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/adterm.py` & `inewave-0.0.98/tests/mocks/arquivos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/agrint.py` & `inewave-0.0.98/tests/mocks/arquivos/agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/arquivos.py` & `inewave-0.0.98/tests/mocks/arquivos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/arquivos_nwlistcf.py` & `inewave-0.0.98/tests/mocks/arquivos/arquivos_nwlistcf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/avl_cortesfpha_nwv.py` & `inewave-0.0.98/tests/mocks/arquivos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/avl_desvfpha_s.py` & `inewave-0.0.98/tests/mocks/arquivos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/avl_desvfpha_v_q.py` & `inewave-0.0.98/tests/mocks/arquivos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/cadic.py` & `inewave-0.0.98/tests/mocks/arquivos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/cdef.py` & `inewave-0.0.98/tests/mocks/arquivos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/cdefsin.py` & `inewave-0.0.98/tests/mocks/arquivos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/clast.py` & `inewave-0.0.98/tests/mocks/arquivos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/cmarg.py` & `inewave-0.0.98/tests/mocks/arquivos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/cmargmed.py` & `inewave-0.0.98/tests/mocks/arquivos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/confhd.py` & `inewave-0.0.98/tests/mocks/arquivos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/conft.py` & `inewave-0.0.98/tests/mocks/arquivos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/coper.py` & `inewave-0.0.98/tests/mocks/arquivos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/corteolm.py` & `inewave-0.0.98/tests/mocks/arquivos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/cterm.py` & `inewave-0.0.98/tests/mocks/arquivos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ctermsin.py` & `inewave-0.0.98/tests/mocks/arquivos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/curva.py` & `inewave-0.0.98/tests/mocks/arquivos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/cvar.py` & `inewave-0.0.98/tests/mocks/arquivos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/deficit.py` & `inewave-0.0.98/tests/mocks/arquivos/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/defsin.py` & `inewave-0.0.98/tests/mocks/arquivos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/depminuh.py` & `inewave-0.0.98/tests/mocks/arquivos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dfphauh.py` & `inewave-0.0.98/tests/mocks/arquivos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dger.py` & `inewave-0.0.98/tests/mocks/arquivos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dlppdfmax.py` & `inewave-0.0.98/tests/mocks/arquivos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dlppdfmaxm.py` & `inewave-0.0.98/tests/mocks/arquivos/dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dlppdfmaxs.py` & `inewave-0.0.98/tests/mocks/arquivos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dlpptbmax.py` & `inewave-0.0.98/tests/mocks/arquivos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dlpptbmaxm.py` & `inewave-0.0.98/tests/mocks/arquivos/dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dlpptbmaxs.py` & `inewave-0.0.98/tests/mocks/arquivos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dsvagua.py` & `inewave-0.0.98/tests/mocks/arquivos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dtbmax.py` & `inewave-0.0.98/tests/mocks/arquivos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dtbmin.py` & `inewave-0.0.98/tests/mocks/arquivos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/dvazmax.py` & `inewave-0.0.98/tests/mocks/arquivos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eaf.py` & `inewave-0.0.98/tests/mocks/arquivos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eafb.py` & `inewave-0.0.98/tests/mocks/arquivos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eafbm.py` & `inewave-0.0.98/tests/mocks/arquivos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eafbsin.py` & `inewave-0.0.98/tests/mocks/arquivos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eafm.py` & `inewave-0.0.98/tests/mocks/arquivos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eafpast.py` & `inewave-0.0.98/tests/mocks/arquivos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/earmf.py` & `inewave-0.0.98/tests/mocks/arquivos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/earmfm.py` & `inewave-0.0.98/tests/mocks/arquivos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/earmfp.py` & `inewave-0.0.98/tests/mocks/arquivos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/earmfpm.py` & `inewave-0.0.98/tests/mocks/arquivos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/earmfpsin.py` & `inewave-0.0.98/tests/mocks/arquivos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/earmfsin.py` & `inewave-0.0.98/tests/mocks/arquivos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eolicacadastro.py` & `inewave-0.0.98/tests/mocks/arquivos/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eolicaconfig.py` & `inewave-0.0.98/tests/mocks/arquivos/eolicaconfig.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eolicafte.py` & `inewave-0.0.98/tests/mocks/arquivos/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eolicageracao.py` & `inewave-0.0.98/tests/mocks/arquivos/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eolicahistorico.py` & `inewave-0.0.98/tests/mocks/arquivos/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/eolicaposto.py` & `inewave-0.0.98/tests/mocks/arquivos/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/estados.py` & `inewave-0.0.98/tests/mocks/arquivos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/evert.py` & `inewave-0.0.98/tests/mocks/arquivos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/evertm.py` & `inewave-0.0.98/tests/mocks/arquivos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/evertsin.py` & `inewave-0.0.98/tests/mocks/arquivos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/exces.py` & `inewave-0.0.98/tests/mocks/arquivos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/excessin.py` & `inewave-0.0.98/tests/mocks/arquivos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/exph.py` & `inewave-0.0.98/tests/mocks/arquivos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/expt.py` & `inewave-0.0.98/tests/mocks/arquivos/expt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/fteolm.py` & `inewave-0.0.98/tests/mocks/arquivos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/fteolsin.py` & `inewave-0.0.98/tests/mocks/arquivos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/geol.py` & `inewave-0.0.98/tests/mocks/arquivos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/geolm.py` & `inewave-0.0.98/tests/mocks/arquivos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/geolsin.py` & `inewave-0.0.98/tests/mocks/arquivos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ghiduh.py` & `inewave-0.0.98/tests/mocks/arquivos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ghmax.py` & `inewave-0.0.98/tests/mocks/arquivos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ghmaxm.py` & `inewave-0.0.98/tests/mocks/arquivos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ghmaxmr.py` & `inewave-0.0.98/tests/mocks/arquivos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ghmaxr.py` & `inewave-0.0.98/tests/mocks/arquivos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ghmaxrsin.py` & `inewave-0.0.98/tests/mocks/arquivos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ghmaxsin.py` & `inewave-0.0.98/tests/mocks/arquivos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ghmin.py` & `inewave-0.0.98/tests/mocks/arquivos/ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ghtot.py` & `inewave-0.0.98/tests/mocks/arquivos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ghtotm.py` & `inewave-0.0.98/tests/mocks/arquivos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ghtotsin.py` & `inewave-0.0.98/tests/mocks/arquivos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/gtert.py` & `inewave-0.0.98/tests/mocks/arquivos/gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/gttot.py` & `inewave-0.0.98/tests/mocks/arquivos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/gttotsin.py` & `inewave-0.0.98/tests/mocks/arquivos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/intercambio.py` & `inewave-0.0.98/tests/mocks/arquivos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/invade.py` & `inewave-0.0.98/tests/mocks/arquivos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/invadem.py` & `inewave-0.0.98/tests/mocks/arquivos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/manutt.py` & `inewave-0.0.98/tests/mocks/arquivos/manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/mercl.py` & `inewave-0.0.98/tests/mocks/arquivos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/merclsin.py` & `inewave-0.0.98/tests/mocks/arquivos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/modif.py` & `inewave-0.0.98/tests/mocks/arquivos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/newavetim.py` & `inewave-0.0.98/tests/mocks/arquivos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/nwlistcfrel.py` & `inewave-0.0.98/tests/mocks/arquivos/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/nwlistopdat.py` & `inewave-0.0.98/tests/mocks/arquivos/nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/nwv_avl_evap.py` & `inewave-0.0.98/tests/mocks/arquivos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/nwv_cortes_evap.py` & `inewave-0.0.98/tests/mocks/arquivos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/nwv_eco_evap.py` & `inewave-0.0.98/tests/mocks/arquivos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/parp.py` & `inewave-0.0.98/tests/mocks/arquivos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/parpeol.py` & `inewave-0.0.98/tests/mocks/arquivos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/parpvaz.py` & `inewave-0.0.98/tests/mocks/arquivos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/patamar.py` & `inewave-0.0.98/tests/mocks/arquivos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/penalid.py` & `inewave-0.0.98/tests/mocks/arquivos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/perdf.py` & `inewave-0.0.98/tests/mocks/arquivos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/perdfm.py` & `inewave-0.0.98/tests/mocks/arquivos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/perdfsin.py` & `inewave-0.0.98/tests/mocks/arquivos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/pmo.py` & `inewave-0.0.98/tests/mocks/arquivos/pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/qafluh.py` & `inewave-0.0.98/tests/mocks/arquivos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/qincruh.py` & `inewave-0.0.98/tests/mocks/arquivos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/re.py` & `inewave-0.0.98/tests/mocks/arquivos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/ree.py` & `inewave-0.0.98/tests/mocks/arquivos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/restricaoeletrica.py` & `inewave-0.0.98/tests/mocks/arquivos/restricaoeletrica.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/restricaoenergia.py` & `inewave-0.0.98/tests/mocks/arquivos/restricaoenergia.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/restricaovazao.py` & `inewave-0.0.98/tests/mocks/arquivos/restricaovazao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/rhslppdf.py` & `inewave-0.0.98/tests/mocks/arquivos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/rhslpptb.py` & `inewave-0.0.98/tests/mocks/arquivos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/selcor.py` & `inewave-0.0.98/tests/mocks/arquivos/selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/sistema.py` & `inewave-0.0.98/tests/mocks/arquivos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/term.py` & `inewave-0.0.98/tests/mocks/arquivos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vagua.py` & `inewave-0.0.98/tests/mocks/arquivos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/varmpuh.py` & `inewave-0.0.98/tests/mocks/arquivos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/varmuh.py` & `inewave-0.0.98/tests/mocks/arquivos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vazpast.py` & `inewave-0.0.98/tests/mocks/arquivos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vento.py` & `inewave-0.0.98/tests/mocks/arquivos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vertuh.py` & `inewave-0.0.98/tests/mocks/arquivos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/verturb.py` & `inewave-0.0.98/tests/mocks/arquivos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/verturbm.py` & `inewave-0.0.98/tests/mocks/arquivos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/verturbsin.py` & `inewave-0.0.98/tests/mocks/arquivos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vevmin.py` & `inewave-0.0.98/tests/mocks/arquivos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vevminm.py` & `inewave-0.0.98/tests/mocks/arquivos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vevminsin.py` & `inewave-0.0.98/tests/mocks/arquivos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vghmin.py` & `inewave-0.0.98/tests/mocks/arquivos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vghminm.py` & `inewave-0.0.98/tests/mocks/arquivos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vghminsin.py` & `inewave-0.0.98/tests/mocks/arquivos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vghminuh.py` & `inewave-0.0.98/tests/mocks/arquivos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/arquivos/vturuh.py` & `inewave-0.0.98/tests/mocks/arquivos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/mocks/mock_open.py` & `inewave-0.0.98/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_adterm.py` & `inewave-0.0.98/tests/newave/test_adterm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from inewave.newave.modelos.adterm import BlocoUTEAdTerm
-from inewave.newave import AdTerm
+from inewave.newave import Adterm
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.adterm import MockBlocoUTEAdTerm
 
 
@@ -22,51 +22,51 @@
     assert b.data.iloc[0, 3] == 230.70
     assert b.data.iloc[-1, -1] == 0.00
 
 
 def test_atributos_encontrados_adterm():
     m: MagicMock = mock_open(read_data="".join(MockBlocoUTEAdTerm))
     with patch("builtins.open", m):
-        ad = AdTerm.read(ARQ_TESTE)
+        ad = Adterm.read(ARQ_TESTE)
         assert ad.despachos is not None
 
 
 def test_atributos_nao_encontrados_adterm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = AdTerm.read(ARQ_TESTE)
+        ad = Adterm.read(ARQ_TESTE)
         assert ad.despachos is None
 
 
 def test_eq_adterm():
     m: MagicMock = mock_open(read_data="".join(MockBlocoUTEAdTerm))
     with patch("builtins.open", m):
-        ad1 = AdTerm.read(ARQ_TESTE)
-        ad2 = AdTerm.read(ARQ_TESTE)
+        ad1 = Adterm.read(ARQ_TESTE)
+        ad2 = Adterm.read(ARQ_TESTE)
         assert ad1 == ad2
 
 
 def test_neq_adterm():
     m: MagicMock = mock_open(read_data="".join(MockBlocoUTEAdTerm))
     with patch("builtins.open", m):
-        ad1 = AdTerm.read(ARQ_TESTE)
-        ad2 = AdTerm.read(ARQ_TESTE)
+        ad1 = Adterm.read(ARQ_TESTE)
+        ad2 = Adterm.read(ARQ_TESTE)
         ad2.despachos.iloc[0, 0] = -1
         assert ad1 != ad2
 
 
 def test_leitura_escrita_adterm():
     m_leitura: MagicMock = mock_open(read_data="".join(MockBlocoUTEAdTerm))
     with patch("builtins.open", m_leitura):
-        ad1 = AdTerm.read(ARQ_TESTE)
+        ad1 = Adterm.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         ad1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        ad2 = AdTerm.read(ARQ_TESTE)
+        ad2 = Adterm.read(ARQ_TESTE)
         assert ad1 == ad2
```

### Comparing `inewave-0.0.97/tests/newave/test_agrint.py` & `inewave-0.0.98/tests/newave/test_agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_arquivos.py` & `inewave-0.0.98/tests/newave/test_arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_avl_cortesfpha_nwv.py` & `inewave-0.0.98/tests/newave/test_avl_cortesfpha_nwv.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def test_atributos_encontrados_avl_nwv_cortesfpha_nwv():
     m: MagicMock = mock_open(read_data="".join(MockAvlCortesFphaNwv))
     with patch("builtins.open", m):
         rel = AvlCortesFpha.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
-        assert rel.tabela.at[0, "indice_usina"] == 4
+        assert rel.tabela.at[0, "codigo_usina"] == 4
         assert rel.tabela.at[0, "periodo"] == 1
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert rel.tabela.at[0, "indice_corte"] == 1
         assert rel.tabela.at[0, "fator_correcao"] == 1.0
         assert rel.tabela.at[0, "rhs_energia"] == 0.0
         assert rel.tabela.at[0, "coeficiente_volume_util_MW_hm3"] == 0.0
         assert (
```

### Comparing `inewave-0.0.97/tests/newave/test_avl_desvfpha_s.py` & `inewave-0.0.98/tests/newave/test_avl_desvfpha_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def test_atributos_encontrados_avl_desvfpha_s():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvFphaS))
     with patch("builtins.open", m):
         rel = AvlDesvFphaS.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
-        assert rel.tabela.at[0, "indice_usina"] == 4
+        assert rel.tabela.at[0, "codigo_usina"] == 4
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert rel.tabela.at[0, "volume_armazenado_percentual"] == 100.0
         assert rel.tabela.at[0, "vazao_turbinada_m3s"] == 0.0
         assert rel.tabela.at[0, "vazao_vertida_m3s"] == 0.0
         assert rel.tabela.at[0, "desvio_percentual"] == 0.0
```

### Comparing `inewave-0.0.97/tests/newave/test_avl_desvfpha_v_q.py` & `inewave-0.0.98/tests/newave/test_avl_desvfpha_v_q.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def test_atributos_encontrados_avl_desvfpha_v_q():
     m: MagicMock = mock_open(read_data="".join(MockAvlDesvFphaVQ))
     with patch("builtins.open", m):
         rel = AvlDesvFphaVQ.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
-        assert rel.tabela.at[0, "indice_usina"] == 4
+        assert rel.tabela.at[0, "codigo_usina"] == 4
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert pd.isna(rel.tabela.at[0, "volume_armazenado_percentual"])
         assert rel.tabela.at[0, "vazao_turbinada_m3s"] == 0.0
         assert rel.tabela.at[0, "desvio_percentual"] == 0.0
 
 
 def test_eq_avl_desvfpha_v_q():
```

### Comparing `inewave-0.0.97/tests/newave/test_cadic.py` & `inewave-0.0.98/tests/newave/test_cadic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from inewave.newave.modelos.cadic import BlocoCargasAdicionais
 
-from inewave.newave import CAdic
+from inewave.newave import Cadic
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.cadic import MockBlocoCargasAdicionais
 
@@ -23,53 +23,53 @@
     assert b.data.iloc[0, 2] == "CONS.ITAIPU"
     assert b.data.iloc[-1, -1] == 2246
 
 
 def test_atributos_encontrados_cadic():
     m: MagicMock = mock_open(read_data="".join(MockBlocoCargasAdicionais))
     with patch("builtins.open", m):
-        ad = CAdic.read(ARQ_TESTE)
+        ad = Cadic.read(ARQ_TESTE)
         assert ad.cargas is not None
 
 
 def test_atributos_nao_encontrados_cadic():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = CAdic.read(ARQ_TESTE)
+        ad = Cadic.read(ARQ_TESTE)
         assert ad.cargas is None
 
 
 def test_eq_cadic():
     m: MagicMock = mock_open(read_data="".join(MockBlocoCargasAdicionais))
     with patch("builtins.open", m):
-        ad1 = CAdic.read(ARQ_TESTE)
-        ad2 = CAdic.read(ARQ_TESTE)
+        ad1 = Cadic.read(ARQ_TESTE)
+        ad2 = Cadic.read(ARQ_TESTE)
         assert ad1 == ad2
 
 
 def test_neq_cadic():
     m: MagicMock = mock_open(read_data="".join(MockBlocoCargasAdicionais))
     with patch("builtins.open", m):
-        ad1 = CAdic.read(ARQ_TESTE)
-        ad2 = CAdic.read(ARQ_TESTE)
+        ad1 = Cadic.read(ARQ_TESTE)
+        ad2 = Cadic.read(ARQ_TESTE)
         ad2.cargas.iloc[0, 0] = -1
         assert ad1 != ad2
 
 
 def test_leitura_escrita_cadic():
     m_leitura: MagicMock = mock_open(
         read_data="".join(MockBlocoCargasAdicionais)
     )
     with patch("builtins.open", m_leitura):
-        ad1 = CAdic.read(ARQ_TESTE)
+        ad1 = Cadic.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         ad1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        ad2 = CAdic.read(ARQ_TESTE)
+        ad2 = Cadic.read(ARQ_TESTE)
         assert ad1 == ad2
```

### Comparing `inewave-0.0.97/tests/newave/test_caso.py` & `inewave-0.0.98/tests/newave/test_caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_clast.py` & `inewave-0.0.98/tests/newave/test_clast.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Rotinas de testes associadas ao arquivo clast.dat do NEWAVE
 from inewave.newave.modelos.clast import BlocoUTEClasT
 from inewave.newave.modelos.clast import BlocoModificacaoUTEClasT
 
-from inewave.newave import ClasT
+from inewave.newave import Clast
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.clast import MockBlocoUTEClasT
 from tests.mocks.arquivos.clast import MockBlocoModificacaoClasT
@@ -25,22 +25,22 @@
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 0.0
 
 
 def test_atributos_encontrados_ute_clast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoUTEClasT))
     with patch("builtins.open", m):
-        ct = ClasT.read(ARQ_TESTE)
+        ct = Clast.read(ARQ_TESTE)
         assert ct.usinas is not None
 
 
 def test_atributos_nao_encontrados_ute_clast():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ct = ClasT.read(ARQ_TESTE)
+        ct = Clast.read(ARQ_TESTE)
         assert ct.usinas is None
 
 
 def test_bloco_modificacao_clast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoModificacaoClasT))
     b = BlocoModificacaoUTEClasT()
     with patch("builtins.open", m):
@@ -50,51 +50,51 @@
     assert b.data.iloc[0, 0] == 211
     assert b.data.iloc[-1, -1] == "PORTO ITAQUI"
 
 
 def test_atributos_encontrados_modificacao_clast():
     m: MagicMock = mock_open(read_data="".join(MockClasT))
     with patch("builtins.open", m):
-        ct = ClasT.read(ARQ_TESTE)
+        ct = Clast.read(ARQ_TESTE)
         assert ct.modificacoes is not None
 
 
 def test_atributos_nao_encontrados_modificacao_clast():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ct = ClasT.read(ARQ_TESTE)
+        ct = Clast.read(ARQ_TESTE)
         assert ct.modificacoes is None
 
 
 def test_eq_clast():
     m: MagicMock = mock_open(read_data="".join(MockClasT))
     with patch("builtins.open", m):
-        ct1 = ClasT.read(ARQ_TESTE)
-        ct2 = ClasT.read(ARQ_TESTE)
+        ct1 = Clast.read(ARQ_TESTE)
+        ct2 = Clast.read(ARQ_TESTE)
         assert ct1 == ct2
 
 
 def test_neq_cadic():
     m: MagicMock = mock_open(read_data="".join(MockClasT))
     with patch("builtins.open", m):
-        ct1 = ClasT.read(ARQ_TESTE)
-        ct2 = ClasT.read(ARQ_TESTE)
+        ct1 = Clast.read(ARQ_TESTE)
+        ct2 = Clast.read(ARQ_TESTE)
         ct2.usinas.iloc[0, 0] = -1
         assert ct1 != ct2
 
 
 def test_leitura_escrita_clast():
     m_leitura: MagicMock = mock_open(read_data="".join(MockClasT))
     with patch("builtins.open", m_leitura):
-        ct1 = ClasT.read(ARQ_TESTE)
+        ct1 = Clast.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         ct1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        ct2 = ClasT.read(ARQ_TESTE)
+        ct2 = Clast.read(ARQ_TESTE)
         assert ct1 == ct2
```

### Comparing `inewave-0.0.97/tests/newave/test_confhd.py` & `inewave-0.0.98/tests/newave/test_confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_conft.py` & `inewave-0.0.98/tests/newave/test_conft.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Rotinas de testes associadas ao arquivo conft.dat do NEWAVE
 from inewave.newave.modelos.conft import BlocoConfUTE
 
-from inewave.newave import ConfT
-
+from inewave.newave import Conft
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.conft import MockBlocoConfUTE
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
@@ -23,51 +22,51 @@
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 209
 
 
 def test_atributos_encontrados_conft():
     m: MagicMock = mock_open(read_data="".join(MockBlocoConfUTE))
     with patch("builtins.open", m):
-        ad = ConfT.read(ARQ_TESTE)
+        ad = Conft.read(ARQ_TESTE)
         assert ad.usinas is not None
 
 
 def test_atributos_nao_encontrados_conft():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = ConfT.read(ARQ_TESTE)
+        ad = Conft.read(ARQ_TESTE)
         assert ad.usinas is None
 
 
 def test_eq_conft():
     m: MagicMock = mock_open(read_data="".join(MockBlocoConfUTE))
     with patch("builtins.open", m):
-        cf1 = ConfT.read(ARQ_TESTE)
-        cf2 = ConfT.read(ARQ_TESTE)
+        cf1 = Conft.read(ARQ_TESTE)
+        cf2 = Conft.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_conft():
     m: MagicMock = mock_open(read_data="".join(MockBlocoConfUTE))
     with patch("builtins.open", m):
-        cf1 = ConfT.read(ARQ_TESTE)
-        cf2 = ConfT.read(ARQ_TESTE)
+        cf1 = Conft.read(ARQ_TESTE)
+        cf2 = Conft.read(ARQ_TESTE)
         cf2.usinas.iloc[0, 0] = -1
         assert cf1 != cf2
 
 
 def test_leitura_escrita_conft():
     m_leitura: MagicMock = mock_open(read_data="".join(MockBlocoConfUTE))
     with patch("builtins.open", m_leitura):
-        cf1 = ConfT.read(ARQ_TESTE)
+        cf1 = Conft.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = ConfT.read(ARQ_TESTE)
+        cf2 = Conft.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.97/tests/newave/test_cortes.py` & `inewave-0.0.98/tests/newave/test_cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_cortesh.py` & `inewave-0.0.98/tests/newave/test_cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_curva.py` & `inewave-0.0.98/tests/newave/test_curva.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Rotinas de testes associadas ao arquivo curva.dat do NEWAVE
 from inewave.newave.modelos.curva import (
     BlocoConfiguracoesPenalizacaoCurva,
     BlocoPenalidadesViolacaoREECurva,
-    BlocoCurvaSegurancaSubsistema,
+    BlocoCurvaSegurancaREE,
     BlocoMaximoIteracoesProcessoIterativoEtapa2,
     BlocoIteracaoAPartirProcessoIterativoEtapa2,
     BlocoToleranciaProcessoIterativoEtapa2,
     BlocoImpressaoRelatorioProcessoIterativoEtapa2,
 )
 
 from inewave.newave import Curva
@@ -48,15 +48,15 @@
 
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 1745.08
 
 
 def test_bloco_curva_seguranca():
     m: MagicMock = mock_open(read_data="".join(MockBlocoCurvaSeguranca))
-    b = BlocoCurvaSegurancaSubsistema()
+    b = BlocoCurvaSegurancaREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 10.0
```

### Comparing `inewave-0.0.97/tests/newave/test_cvar.py` & `inewave-0.0.98/tests/newave/test_cvar.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Rotinas de testes associadas ao arquivo cvar.dat do NEWAVE
 from inewave.newave.modelos.cvar import (
     BlocoValoresConstantesCVAR,
     BlocoAlfaVariavelNoTempo,
     BlocoLambdaVariavelNoTempo,
 )
 
-from inewave.newave import CVAR
+from inewave.newave import Cvar
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.cvar import (
     MockBlocoValoresConstantes,
@@ -54,55 +54,55 @@
     assert b.data.iloc[0, 0] == "2017"
     assert b.data.iloc[-1, -1] == 10.0
 
 
 def test_atributos_encontrados_cvar():
     m: MagicMock = mock_open(read_data="".join(MockCVAR))
     with patch("builtins.open", m):
-        ad = CVAR.read(ARQ_TESTE)
+        ad = Cvar.read(ARQ_TESTE)
         assert ad.valores_constantes != [None, None]
         assert ad.alfa_variavel is not None
         assert ad.lambda_variavel is not None
 
 
 def test_atributos_nao_encontrados_cvar():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = CVAR.read(ARQ_TESTE)
+        ad = Cvar.read(ARQ_TESTE)
         assert ad.valores_constantes is None
         assert ad.alfa_variavel is None
         assert ad.lambda_variavel is None
 
 
 def test_eq_cvar():
     m: MagicMock = mock_open(read_data="".join(MockCVAR))
     with patch("builtins.open", m):
-        cf1 = CVAR.read(ARQ_TESTE)
-        cf2 = CVAR.read(ARQ_TESTE)
+        cf1 = Cvar.read(ARQ_TESTE)
+        cf2 = Cvar.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_cvar():
     m: MagicMock = mock_open(read_data="".join(MockCVAR))
     with patch("builtins.open", m):
-        cf1 = CVAR.read(ARQ_TESTE)
-        cf2 = CVAR.read(ARQ_TESTE)
+        cf1 = Cvar.read(ARQ_TESTE)
+        cf2 = Cvar.read(ARQ_TESTE)
         cf2.valores_constantes = [0, 0]
         assert cf1 != cf2
 
 
 def test_leitura_escrita_cvar():
     m_leitura: MagicMock = mock_open(read_data="".join(MockCVAR))
     with patch("builtins.open", m_leitura):
-        cf1 = CVAR.read(ARQ_TESTE)
+        cf1 = Cvar.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = CVAR.read(ARQ_TESTE)
+        cf2 = Cvar.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.97/tests/newave/test_dger.py` & `inewave-0.0.98/tests/newave/test_dger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Rotinas de testes associadas ao arquivo dger.dat do NEWAVE
-from inewave.newave.dger import DGer
+from inewave.newave.dger import Dger
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.dger import MockDger
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_nao_encontrados_dger():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.nome_caso == ""
         assert d.tipo_execucao is None
         assert d.duracao_periodo is None
         assert d.num_anos_estudo is None
         assert d.mes_inicio_pre_estudo is None
         assert d.mes_inicio_estudo is None
         assert d.ano_inicio_estudo is None
@@ -134,15 +134,15 @@
         assert d.estacoes_bombeamento is None
         assert d.canal_desvio is None
 
 
 def test_atributos_encontrados_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.nome_caso is not None
         assert d.tipo_execucao is not None
         assert d.duracao_periodo is not None
         assert d.num_anos_estudo is not None
         assert d.mes_inicio_pre_estudo is not None
         assert d.mes_inicio_estudo is not None
         assert d.ano_inicio_estudo is not None
@@ -260,614 +260,614 @@
         assert d.estacoes_bombeamento is not None
         assert d.canal_desvio is not None
 
 
 def test_nome_caso_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.nome_caso == (
             "PMO JANEIRO - 2021  22/12/2020 12:43:55  Niveis"
             + " para 26/12 NW Versao 27.5_CPAMP"
         )
         novo_valor = "Teste"
         d.nome_caso = novo_valor
         assert d.nome_caso == novo_valor
 
 
 def test_tipo_execucao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.tipo_execucao == 1
         novo_valor = 0
         d.tipo_execucao = novo_valor
         assert d.tipo_execucao == novo_valor
 
 
 def test_duracao_periodo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.duracao_periodo == 1
         novo_valor = 0
         d.duracao_periodo = novo_valor
         assert d.duracao_periodo == novo_valor
 
 
 def test_num_anos_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.num_anos_estudo == 5
         novo_valor = 0
         d.num_anos_estudo = novo_valor
         assert d.num_anos_estudo == novo_valor
 
 
 def test_mes_inicio_pre_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.mes_inicio_pre_estudo == 1
         novo_valor = 0
         d.mes_inicio_pre_estudo = novo_valor
         assert d.mes_inicio_pre_estudo == novo_valor
 
 
 def test_mes_inicio_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.mes_inicio_estudo == 1
         novo_valor = 0
         d.mes_inicio_estudo = novo_valor
         assert d.mes_inicio_estudo == novo_valor
 
 
 def test_ano_inicio_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.ano_inicio_estudo == 2021
         novo_valor = 0
         d.ano_inicio_estudo = novo_valor
         assert d.ano_inicio_estudo == novo_valor
 
 
 def test_num_anos_pre_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.num_anos_pre_estudo == 0
         novo_valor = 5
         d.num_anos_pre_estudo = novo_valor
         assert d.num_anos_pre_estudo == novo_valor
 
 
 def test_num_anos_pos_estudo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.num_anos_pos_estudo == 5
         novo_valor = 0
         d.num_anos_pos_estudo = novo_valor
         assert d.num_anos_pos_estudo == novo_valor
 
 
 def test_num_anos_pos_sim_final_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.num_anos_pos_sim_final == 0
         novo_valor = 1
         d.num_anos_pos_sim_final = novo_valor
         assert d.num_anos_pos_sim_final == novo_valor
 
 
 def test_imprime_dados_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.imprime_dados == 1
         novo_valor = 0
         d.imprime_dados = novo_valor
         assert d.imprime_dados == novo_valor
 
 
 def test_imprime_mercados_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.imprime_mercados == 1
         novo_valor = 0
         d.imprime_mercados = novo_valor
         assert d.imprime_mercados == novo_valor
 
 
 def test_imprime_energias_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.imprime_energias == 1
         novo_valor = 0
         d.imprime_energias = novo_valor
         assert d.imprime_energias == novo_valor
 
 
 def test_imprime_modelo_estocastico_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.imprime_modelo_estocastico == 1
         novo_valor = 0
         d.imprime_modelo_estocastico = novo_valor
         assert d.imprime_modelo_estocastico == novo_valor
 
 
 def test_imprime_subsistema_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.imprime_subsistema == 1
         novo_valor = 0
         d.imprime_subsistema = novo_valor
         assert d.imprime_subsistema == novo_valor
 
 
 def test_num_max_iteracoes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.num_max_iteracoes == 45
         novo_valor = 0
         d.num_max_iteracoes = novo_valor
         assert d.num_max_iteracoes == novo_valor
 
 
 def test_num_forwards_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.num_forwards == 200
         novo_valor = 0
         d.num_forwards = novo_valor
         assert d.num_forwards == novo_valor
 
 
 def test_num_aberturas_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.num_aberturas == 20
         novo_valor = 0
         d.num_aberturas = novo_valor
         assert d.num_aberturas == novo_valor
 
 
 def test_num_series_sinteticas_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.num_series_sinteticas == 2000
         novo_valor = 0
         d.num_series_sinteticas = novo_valor
         assert d.num_series_sinteticas == novo_valor
 
 
 def test_ordem_maxima_parp_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.ordem_maxima_parp == 6
         novo_valor = 0
         d.ordem_maxima_parp = novo_valor
         assert d.ordem_maxima_parp == novo_valor
 
 
 def test_ano_inicial_historico_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.ano_inicial_historico == 1931
         novo_valor = 0
         d.ano_inicial_historico = novo_valor
         assert d.ano_inicial_historico == novo_valor
 
 
 def test_tamanho_registro_arquivo_historico_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.tamanho_registro_arquivo_historico == 0
         novo_valor = 1
         d.tamanho_registro_arquivo_historico = novo_valor
         assert d.tamanho_registro_arquivo_historico == novo_valor
 
 
 def test_calcula_volume_inicial_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.calcula_volume_inicial == 1
         novo_valor = 0
         d.calcula_volume_inicial = novo_valor
         assert d.calcula_volume_inicial == novo_valor
 
 
 def test_volume_inicial_subsistema_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.volume_inicial_subsistema == [0.0, 0.0, 0.0, 0.0, 0.0]
         novo_valor = [1.0, 1.0, 1.0, 1.0, 1.0]
         d.volume_inicial_subsistema = novo_valor
         assert d.volume_inicial_subsistema == novo_valor
 
 
 def test_tolerancia_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.tolerancia == 95.0
         novo_valor = 0.0
         d.tolerancia = novo_valor
         assert d.tolerancia == novo_valor
 
 
 def test_taxa_de_desconto_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.taxa_de_desconto == 12.0
         novo_valor = 0.0
         d.taxa_de_desconto = novo_valor
         assert d.taxa_de_desconto == novo_valor
 
 
 def test_tipo_simulacao_final_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.tipo_simulacao_final == 1
         novo_valor = 0
         d.tipo_simulacao_final = novo_valor
         assert d.tipo_simulacao_final == novo_valor
 
 
 def test_agregacao_simulacao_final_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.agregacao_simulacao_final == 1
         novo_valor = 0
         d.agregacao_simulacao_final = novo_valor
         assert d.agregacao_simulacao_final == novo_valor
 
 
 def test_impressao_operacao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.impressao_operacao == 1
         novo_valor = 0
         d.impressao_operacao = novo_valor
         assert d.impressao_operacao == novo_valor
 
 
 def test_impressao_convergencia_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.impressao_convergencia == 1
         novo_valor = 0
         d.impressao_convergencia = novo_valor
         assert d.impressao_convergencia == novo_valor
 
 
 def test_intervalo_para_gravar_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.intervalo_para_gravar == 1
         novo_valor = 0
         d.intervalo_para_gravar = novo_valor
         assert d.intervalo_para_gravar == novo_valor
 
 
 def test_num_minimo_iteracoes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.num_minimo_iteracoes == 30
         novo_valor = 0
         d.num_minimo_iteracoes = novo_valor
         assert d.num_minimo_iteracoes == novo_valor
 
 
 def test_racionamento_preventivo_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.racionamento_preventivo == 0
         novo_valor = 1
         d.racionamento_preventivo = novo_valor
         assert d.racionamento_preventivo == novo_valor
 
 
 def test_num_anos_manutencao_utes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.num_anos_manutencao_utes == 1
         novo_valor = 0
         d.num_anos_manutencao_utes = novo_valor
         assert d.num_anos_manutencao_utes == novo_valor
 
 
 def test_tendencia_hidrologica_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.considera_tendencia_hidrologica_calculo_politica == 2
         assert d.considera_tendencia_hidrologica_sim_final == 2
         novo_valor = 0
         d.considera_tendencia_hidrologica_calculo_politica = novo_valor
         assert d.considera_tendencia_hidrologica_calculo_politica == novo_valor
         d.considera_tendencia_hidrologica_sim_final = novo_valor
         assert d.considera_tendencia_hidrologica_sim_final == novo_valor
 
 
 def test_restricao_itaipu_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.restricao_itaipu == 0
         novo_valor = 1
         d.restricao_itaipu = novo_valor
         assert d.restricao_itaipu == novo_valor
 
 
 def test_bid_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.bid == 0
         novo_valor = 1
         d.bid = novo_valor
         assert d.bid == novo_valor
 
 
 def test_perdas_rede_transmissao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.perdas_rede_transmissao == 0
         novo_valor = 1
         d.perdas_rede_transmissao = novo_valor
         assert d.perdas_rede_transmissao == novo_valor
 
 
 def test_el_nino_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.el_nino == 0
         novo_valor = 1
         d.el_nino = novo_valor
         assert d.el_nino == novo_valor
 
 
 def test_enso_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.enso == 0
         novo_valor = 1
         d.enso = novo_valor
         assert d.enso == novo_valor
 
 
 def test_duracao_por_patamar_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.duracao_por_patamar == 1
         novo_valor = 0
         d.duracao_por_patamar = novo_valor
         assert d.duracao_por_patamar == novo_valor
 
 
 def test_outros_usos_da_agua_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.outros_usos_da_agua == 1
         novo_valor = 0
         d.outros_usos_da_agua = novo_valor
         assert d.outros_usos_da_agua == novo_valor
 
 
 def test_correcao_desvio_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.correcao_desvio == 1
         novo_valor = 0
         d.correcao_desvio = novo_valor
         assert d.correcao_desvio == novo_valor
 
 
 def test_curva_aversao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.curva_aversao == 1
         novo_valor = 0
         d.curva_aversao = novo_valor
         assert d.curva_aversao == novo_valor
 
 
 def test_tipo_geracao_enas_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.tipo_geracao_enas == 0
         novo_valor = 1
         d.tipo_geracao_enas = novo_valor
         assert d.tipo_geracao_enas == novo_valor
 
 
 def test_risco_deficit_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.primeira_profundidade_risco_deficit == 1.0
         assert d.segunda_profundidade_risco_deficit == 2.5
         novo_valor = 0.0
         d.primeira_profundidade_risco_deficit = novo_valor
         assert d.primeira_profundidade_risco_deficit == novo_valor
         d.segunda_profundidade_risco_deficit = novo_valor
         assert d.segunda_profundidade_risco_deficit == novo_valor
 
 
 def test_iteracao_para_simulacao_final_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.iteracao_para_simulacao_final == 0
         novo_valor = 1
         d.iteracao_para_simulacao_final = novo_valor
         assert d.iteracao_para_simulacao_final == novo_valor
 
 
 def test_agrupamento_livre_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.agrupamento_livre == 1
         novo_valor = 0
         d.agrupamento_livre = novo_valor
         assert d.agrupamento_livre == novo_valor
 
 
 def test_equalizacao_penal_intercambio_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.equalizacao_penal_intercambio == 1
         novo_valor = 0
         d.equalizacao_penal_intercambio = novo_valor
         assert d.equalizacao_penal_intercambio == novo_valor
 
 
 def test_representacao_submotorizacao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.representacao_submotorizacao == 2
         novo_valor = 0
         d.representacao_submotorizacao = novo_valor
         assert d.representacao_submotorizacao == novo_valor
 
 
 def test_ordenacao_automatica_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.ordenacao_automatica == 0
         novo_valor = 1
         d.ordenacao_automatica = novo_valor
         assert d.ordenacao_automatica == novo_valor
 
 
 def test_considera_carga_adicional_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.considera_carga_adicional == 1
         novo_valor = 0
         d.considera_carga_adicional = novo_valor
         assert d.considera_carga_adicional == novo_valor
 
 
 def test_delta_zsup_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.delta_zsup == 10
         novo_valor = 0.0
         d.delta_zsup = novo_valor
         assert d.delta_zsup == novo_valor
 
 
 def test_delta_zinf_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.delta_zinf == 0.2
         novo_valor = 0.0
         d.delta_zinf = novo_valor
         assert d.delta_zinf == novo_valor
 
 
 def test_deltas_consecutivos_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.deltas_consecutivos == 3
         novo_valor = 0
         d.deltas_consecutivos = novo_valor
         assert d.deltas_consecutivos == novo_valor
 
 
 def test_despacho_antecipado_gnl_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.despacho_antecipado_gnl == 1
         novo_valor = 0
         d.despacho_antecipado_gnl = novo_valor
         assert d.despacho_antecipado_gnl == novo_valor
 
 
 def test_modif_automatica_adterm_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.modif_automatica_adterm == 1
         novo_valor = 0
         d.modif_automatica_adterm = novo_valor
         assert d.modif_automatica_adterm == novo_valor
 
 
 def test_considera_ghmin_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.considera_ghmin == 1
         novo_valor = 0
         d.considera_ghmin = novo_valor
         assert d.considera_ghmin == novo_valor
 
 
 def test_simulacao_final_com_data_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.simulacao_final_com_data == 0
         novo_valor = 1
         d.simulacao_final_com_data = novo_valor
         assert d.simulacao_final_com_data == novo_valor
 
 
 def test_gerenciamento_pls_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.utiliza_gerenciamento_pls == 0
         assert d.comunicacao_dois_niveis == 0
         assert d.armazenamento_local_arquivos_temporarios == 0
         assert d.alocacao_memoria_ena == 0
         assert d.alocacao_memoria_cortes == 0
         novo_valor = 1
         d.utiliza_gerenciamento_pls = novo_valor
@@ -881,95 +881,95 @@
         d.alocacao_memoria_cortes = novo_valor
         assert d.alocacao_memoria_cortes == novo_valor
 
 
 def test_sar_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.sar == 0
         novo_valor = 1
         d.sar = novo_valor
         assert d.sar == novo_valor
 
 
 def test_cvar_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.cvar == 1
         novo_valor = 0
         d.cvar = novo_valor
         assert d.cvar == novo_valor
 
 
 def test_considera_zsup_min_convergencia_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.considera_zsup_min_convergencia == 0
         novo_valor = 0
         d.considera_zsup_min_convergencia = novo_valor
         assert d.considera_zsup_min_convergencia == novo_valor
 
 
 def test_desconsidera_vazao_minima_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.desconsidera_vazao_minima == 0
         novo_valor = 1
         d.desconsidera_vazao_minima = novo_valor
         assert d.desconsidera_vazao_minima == novo_valor
 
 
 def test_restricoes_eletricas_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.restricoes_eletricas == 1
         novo_valor = 0
         d.restricoes_eletricas = novo_valor
         assert d.restricoes_eletricas == novo_valor
 
 
 def test_selecao_de_cortes_backward_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.selecao_de_cortes_backward == 1
         novo_valor = 0
         d.selecao_de_cortes_backward = novo_valor
         assert d.selecao_de_cortes_backward == novo_valor
 
 
 def test_selecao_de_cortes_forward_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.selecao_de_cortes_forward == 1
         novo_valor = 0
         d.selecao_de_cortes_forward = novo_valor
         assert d.selecao_de_cortes_forward == novo_valor
 
 
 def test_janela_de_cortes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.janela_de_cortes == 0
         novo_valor = 1
         d.janela_de_cortes = novo_valor
         assert d.janela_de_cortes == novo_valor
 
 
 def test_reamostragem_cenarios_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.considera_reamostragem_cenarios == 1
         assert d.tipo_reamostragem_cenarios == 1
         assert d.passo_reamostragem_cenarios == 1
         novo_valor = 0
         d.considera_reamostragem_cenarios = novo_valor
         assert d.considera_reamostragem_cenarios == novo_valor
         d.tipo_reamostragem_cenarios = novo_valor
@@ -977,400 +977,400 @@
         d.passo_reamostragem_cenarios = novo_valor
         assert d.passo_reamostragem_cenarios == novo_valor
 
 
 def test_converge_no_zero_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.converge_no_zero == 0
         novo_valor = 1
         d.converge_no_zero = novo_valor
         assert d.converge_no_zero == novo_valor
 
 
 def test_consulta_fcf_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.consulta_fcf == 0
         novo_valor = 1
         d.consulta_fcf = novo_valor
         assert d.consulta_fcf == novo_valor
 
 
 def test_impressao_ena_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.impressao_ena == 1
         novo_valor = 0
         d.impressao_ena = novo_valor
         assert d.impressao_ena == novo_valor
 
 
 def test_impressao_cortes_ativos_sim_final_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.impressao_cortes_ativos_sim_final == 0
         novo_valor = 1
         d.impressao_cortes_ativos_sim_final = novo_valor
         assert d.impressao_cortes_ativos_sim_final == novo_valor
 
 
 def test_representacao_agregacao_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.representacao_agregacao == 1
         novo_valor = 0
         d.representacao_agregacao = novo_valor
         assert d.representacao_agregacao == novo_valor
 
 
 def test_matriz_correlacao_espacial_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.matriz_correlacao_espacial == 1
         novo_valor = 0
         d.matriz_correlacao_espacial = novo_valor
         assert d.matriz_correlacao_espacial == novo_valor
 
 
 def test_desconsidera_convergencia_estatistica_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.desconsidera_convergencia_estatistica == 1
         novo_valor = 0
         d.desconsidera_convergencia_estatistica = novo_valor
         assert d.desconsidera_convergencia_estatistica == novo_valor
 
 
 def test_momento_reamostragem_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.momento_reamostragem == 1
         novo_valor = 0
         d.momento_reamostragem = novo_valor
         assert d.momento_reamostragem == novo_valor
 
 
 def test_mantem_arquivos_energias_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.mantem_arquivos_energias == 0
         novo_valor = 1
         d.mantem_arquivos_energias = novo_valor
         assert d.mantem_arquivos_energias == novo_valor
 
 
 def test_inicio_teste_convergencia_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.inicio_teste_convergencia == 1
         novo_valor = 0
         d.inicio_teste_convergencia = novo_valor
         assert d.inicio_teste_convergencia == novo_valor
 
 
 def test_sazonaliza_vmint_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.sazonaliza_vmint == 0
         novo_valor = 1
         d.sazonaliza_vmint = novo_valor
         assert d.sazonaliza_vmint == novo_valor
 
 
 def test_sazonaliza_vmaxt_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.sazonaliza_vmaxt == 0
         novo_valor = 1
         d.sazonaliza_vmaxt = novo_valor
         assert d.sazonaliza_vmaxt == novo_valor
 
 
 def test_sazonaliza_vminp_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.sazonaliza_vminp == 0
         novo_valor = 1
         d.sazonaliza_vminp = novo_valor
         assert d.sazonaliza_vminp == novo_valor
 
 
 def test_sazonaliza_cfuga_cmont_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.sazonaliza_cfuga_cmont == 0
         novo_valor = 1
         d.sazonaliza_cfuga_cmont = novo_valor
         assert d.sazonaliza_cfuga_cmont == novo_valor
 
 
 def test_restricoes_emissao_gee_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.restricoes_emissao_gee == 0
         novo_valor = 1
         d.restricoes_emissao_gee = novo_valor
         assert d.restricoes_emissao_gee == novo_valor
 
 
 def test_afluencia_anual_parp_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.consideracao_media_anual_afluencias == 3
         assert d.reducao_automatica_ordem == 0
         novo_valor = 1
         d.consideracao_media_anual_afluencias = novo_valor
         assert d.consideracao_media_anual_afluencias == novo_valor
         d.reducao_automatica_ordem = novo_valor
         assert d.reducao_automatica_ordem == novo_valor
 
 
 def test_restricoes_fornecimento_gas_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.restricoes_fornecimento_gas == 0
         novo_valor = 1
         d.restricoes_fornecimento_gas = novo_valor
         assert d.restricoes_fornecimento_gas == novo_valor
 
 
 def test_memoria_calculo_cortes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.memoria_calculo_cortes == 0
         novo_valor = 1
         d.memoria_calculo_cortes = novo_valor
         assert d.memoria_calculo_cortes == novo_valor
 
 
 def test_considera_geracao_eolica_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.considera_geracao_eolica == 1
         novo_valor = 0
         d.considera_geracao_eolica = novo_valor
         assert d.considera_geracao_eolica == novo_valor
 
 
 def test_penalidade_corte_geracao_eolica_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.penalidade_corte_geracao_eolica == 0.0063
         novo_valor = 1.0
         d.penalidade_corte_geracao_eolica = novo_valor
         assert d.penalidade_corte_geracao_eolica == novo_valor
 
 
 def test_compensacao_correlacao_cruzada_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.compensacao_correlacao_cruzada == 1
         novo_valor = 0
         d.compensacao_correlacao_cruzada = novo_valor
         assert d.compensacao_correlacao_cruzada == novo_valor
 
 
 def test_restricao_turbinamento_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.restricao_turbinamento == 1
         novo_valor = 0
         d.restricao_turbinamento = novo_valor
         assert d.restricao_turbinamento == novo_valor
 
 
 def test_restricao_defluencia_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.restricao_defluencia == 1
         novo_valor = 0
         d.restricao_defluencia = novo_valor
         assert d.restricao_defluencia == novo_valor
 
 
 def test_aproveitamento_base_pls_backward_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.aproveitamento_bases_backward == 1
         novo_valor = 0
         d.aproveitamento_bases_backward = novo_valor
         assert d.aproveitamento_bases_backward == novo_valor
 
 
 def test_impressao_estados_geracao_cortes_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.impressao_estados_geracao_cortes == 1
         novo_valor = 0
         d.impressao_estados_geracao_cortes = novo_valor
         assert d.impressao_estados_geracao_cortes == novo_valor
 
 
 def test_semente_forward_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.semente_forward == 0
         novo_valor = 1000
         d.semente_forward = novo_valor
         assert d.semente_forward == novo_valor
 
 
 def test_semente_backward_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.semente_backward == 0
         novo_valor = 1000
         d.semente_backward = novo_valor
         assert d.semente_backward == novo_valor
 
 
 def test_restricao_lpp_turbinamento_maximo_ree_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.restricao_lpp_turbinamento_maximo_ree == 1
         novo_valor = 0
         d.restricao_lpp_turbinamento_maximo_ree = novo_valor
         assert d.restricao_lpp_turbinamento_maximo_ree == novo_valor
 
 
 def test_restricao_lpp_defluencia_maxima_ree_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.restricao_lpp_defluencia_maxima_ree == 1
         novo_valor = 0
         d.restricao_lpp_defluencia_maxima_ree = novo_valor
         assert d.restricao_lpp_defluencia_maxima_ree == novo_valor
 
 
 def test_restricao_lpp_turbinamento_maximo_uhe_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.restricao_lpp_turbinamento_maximo_uhe == 1
         novo_valor = 0
         d.restricao_lpp_turbinamento_maximo_uhe = novo_valor
         assert d.restricao_lpp_turbinamento_maximo_uhe == novo_valor
 
 
 def test_restricao_lpp_defluencia_maxima_uhe_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.restricao_lpp_defluencia_maxima_uhe == 1
         novo_valor = 0
         d.restricao_lpp_defluencia_maxima_uhe = novo_valor
         assert d.restricao_lpp_defluencia_maxima_uhe == novo_valor
 
 
 def test_restricoes_eletricas_especiais():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.restricoes_eletricas_especiais == 0
         novo_valor = 1
         d.restricoes_eletricas_especiais = novo_valor
         assert d.restricoes_eletricas_especiais == novo_valor
 
 
 def test_funcao_producao_uhe():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.funcao_producao_uhe == 0
         novo_valor = 1
         d.funcao_producao_uhe = novo_valor
         assert d.funcao_producao_uhe == novo_valor
 
 
 def test_fcf_pos_estudo():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.fcf_pos_estudo == 0
         novo_valor = 1
         d.fcf_pos_estudo = novo_valor
         assert d.fcf_pos_estudo == novo_valor
 
 
 def test_estacoes_bombeamento():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.estacoes_bombeamento == 1
         novo_valor = 0
         d.estacoes_bombeamento = novo_valor
         assert d.estacoes_bombeamento == novo_valor
 
 
 def test_canal_desvio():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d = DGer.read(ARQ_TESTE)
+        d = Dger.read(ARQ_TESTE)
         assert d.canal_desvio == 1
         novo_valor = 0
         d.canal_desvio = novo_valor
         assert d.canal_desvio == novo_valor
 
 
 def test_eq_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d1 = DGer.read(ARQ_TESTE)
-        d2 = DGer.read(ARQ_TESTE)
+        d1 = Dger.read(ARQ_TESTE)
+        d2 = Dger.read(ARQ_TESTE)
         assert d1 == d2
 
 
 def test_neq_dger():
     m: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m):
-        d1 = DGer.read(ARQ_TESTE)
-        d2 = DGer.read(ARQ_TESTE)
+        d1 = Dger.read(ARQ_TESTE)
+        d2 = Dger.read(ARQ_TESTE)
         d2.nome_caso = "Teste"
         assert d1 != d2
 
 
 def test_leitura_escrita_dger():
     m_leitura: MagicMock = mock_open(read_data="".join(MockDger))
     with patch("builtins.open", m_leitura):
-        d1 = DGer.read(ARQ_TESTE)
+        d1 = Dger.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         d1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        d2 = DGer.read(ARQ_TESTE)
+        d2 = Dger.read(ARQ_TESTE)
         assert d1 == d2
```

### Comparing `inewave-0.0.97/tests/newave/test_dsvagua.py` & `inewave-0.0.98/tests/newave/test_dsvagua.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Rotinas de testes associadas ao arquivo dsvagua.dat do NEWAVE
 from inewave.newave.modelos.dsvagua import BlocoDsvUHE
 
-from inewave.newave import DSVAgua
+from inewave.newave import Dsvagua
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.dsvagua import MockBlocoDesviosAgua
 
@@ -23,51 +23,51 @@
     assert b.data.iloc[0, 0] == 2020
     assert b.data.iloc[-1, 0] == 2024
 
 
 def test_atributos_encontrados_dsvagua():
     m: MagicMock = mock_open(read_data="".join(MockBlocoDesviosAgua))
     with patch("builtins.open", m):
-        ad = DSVAgua.read(ARQ_TESTE)
+        ad = Dsvagua.read(ARQ_TESTE)
         assert ad.desvios is not None
 
 
 def test_atributos_nao_encontrados_dsvagua():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = DSVAgua.read(ARQ_TESTE)
+        ad = Dsvagua.read(ARQ_TESTE)
         assert ad.desvios is None
 
 
 def test_eq_dsvagua():
     m: MagicMock = mock_open(read_data="".join(MockBlocoDesviosAgua))
     with patch("builtins.open", m):
-        cf1 = DSVAgua.read(ARQ_TESTE)
-        cf2 = DSVAgua.read(ARQ_TESTE)
+        cf1 = Dsvagua.read(ARQ_TESTE)
+        cf2 = Dsvagua.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_dsvagua():
     m: MagicMock = mock_open(read_data="".join(MockBlocoDesviosAgua))
     with patch("builtins.open", m):
-        cf1 = DSVAgua.read(ARQ_TESTE)
-        cf2 = DSVAgua.read(ARQ_TESTE)
+        cf1 = Dsvagua.read(ARQ_TESTE)
+        cf2 = Dsvagua.read(ARQ_TESTE)
         cf2.desvios.iloc[0, 0] = -1
         assert cf1 != cf2
 
 
 def test_leitura_escrita_dsvagua():
     m_leitura: MagicMock = mock_open(read_data="".join(MockBlocoDesviosAgua))
     with patch("builtins.open", m_leitura):
-        cf1 = DSVAgua.read(ARQ_TESTE)
+        cf1 = Dsvagua.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = DSVAgua.read(ARQ_TESTE)
+        cf2 = Dsvagua.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.97/tests/newave/test_eafpast.py` & `inewave-0.0.98/tests/newave/test_eafpast.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Rotinas de testes associadas ao arquivo eafpast.dat do NEWAVE
 from inewave.newave.modelos.eafpast import BlocoEafPast
 
-from inewave.newave import EafPast
+from inewave.newave import Eafpast
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.eafpast import MockBlocoAfluenciasPassadas
 
@@ -22,53 +22,53 @@
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 544.91
 
 
 def test_atributos_encontrados_eafpast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoAfluenciasPassadas))
     with patch("builtins.open", m):
-        ad = EafPast.read(ARQ_TESTE)
+        ad = Eafpast.read(ARQ_TESTE)
         assert ad.tendencia is not None
 
 
 def test_atributos_nao_encontrados_eafpast():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = EafPast.read(ARQ_TESTE)
+        ad = Eafpast.read(ARQ_TESTE)
         assert ad.tendencia is None
 
 
 def test_eq_eafpast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoAfluenciasPassadas))
     with patch("builtins.open", m):
-        cf1 = EafPast.read(ARQ_TESTE)
-        cf2 = EafPast.read(ARQ_TESTE)
+        cf1 = Eafpast.read(ARQ_TESTE)
+        cf2 = Eafpast.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_eafpast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoAfluenciasPassadas))
     with patch("builtins.open", m):
-        cf1 = EafPast.read(ARQ_TESTE)
-        cf2 = EafPast.read(ARQ_TESTE)
+        cf1 = Eafpast.read(ARQ_TESTE)
+        cf2 = Eafpast.read(ARQ_TESTE)
         cf2.tendencia.iloc[0, 0] = -1
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eafpast():
     m_leitura: MagicMock = mock_open(
         read_data="".join(MockBlocoAfluenciasPassadas)
     )
     with patch("builtins.open", m_leitura):
-        cf1 = EafPast.read(ARQ_TESTE)
+        cf1 = Eafpast.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = EafPast.read(ARQ_TESTE)
+        cf2 = Eafpast.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.97/tests/newave/test_enavazb.py` & `inewave-0.0.98/tests/newave/test_enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_enavazf.py` & `inewave-0.0.98/tests/newave/test_enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_energiab.py` & `inewave-0.0.98/tests/newave/test_energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_energiaf.py` & `inewave-0.0.98/tests/newave/test_energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_energias.py` & `inewave-0.0.98/tests/newave/test_energias.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_engnat.py` & `inewave-0.0.98/tests/newave/test_engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_eolicacadastro.py` & `inewave-0.0.98/tests/newave/test_eolicacadastro.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 
 
 def test_neq_eolicacadastro():
     m: MagicMock = mock_open(read_data="".join(MockEolicaCadastro))
     with patch("builtins.open", m):
         cf1 = EolicaCadastro.read(ARQ_TESTE)
         cf2 = EolicaCadastro.read(ARQ_TESTE)
-        cf2.deleta_registro(cf1.eolica_cadastro()[0])
+        cf2.data.remove(cf1.eolica_cadastro()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicacadastro():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaCadastro))
     with patch("builtins.open", m_leitura):
         cf1 = EolicaCadastro.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/newave/test_eolicaconfiguracao.py` & `inewave-0.0.98/tests/newave/test_eolicaconfiguracao.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 
 def test_neq_eolicaconfig():
     m: MagicMock = mock_open(read_data="".join(MockEolicaConfig))
     with patch("builtins.open", m):
         cf1 = EolicaConfiguracao.read(ARQ_TESTE)
         cf2 = EolicaConfiguracao.read(ARQ_TESTE)
-        cf2.deleta_registro(cf1.eolica_configuracao()[0])
+        cf2.data.remove(cf1.eolica_configuracao()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicaconfig():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaConfig))
     with patch("builtins.open", m_leitura):
         cf1 = EolicaConfiguracao.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/newave/test_eolicafte.py` & `inewave-0.0.98/tests/newave/test_eolicafte.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 
 def test_neq_eolicafte():
     m: MagicMock = mock_open(read_data="".join(MockEolicaFTE))
     with patch("builtins.open", m):
         cf1 = EolicaFTE.read(ARQ_TESTE)
         cf2 = EolicaFTE.read(ARQ_TESTE)
-        cf2.deleta_registro(cf1.eolica_funcao_producao()[0])
+        cf2.data.remove(cf1.eolica_funcao_producao()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicafte():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaFTE))
     with patch("builtins.open", m_leitura):
         cf1 = EolicaFTE.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/newave/test_eolicageracao.py` & `inewave-0.0.98/tests/newave/test_eolicageracao.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,15 @@
 
 
 def test_neq_eolicageracao():
     m: MagicMock = mock_open(read_data="".join(MockEolicaGeracao))
     with patch("builtins.open", m):
         cf1 = EolicaGeracao.read(ARQ_TESTE)
         cf2 = EolicaGeracao.read(ARQ_TESTE)
-        cf2.deleta_registro(
-            cf1.eolica_geracao_profundidade_periodo_patamar()[0]
-        )
+        cf2.data.remove(cf1.eolica_geracao_profundidade_periodo_patamar()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicageracao():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaGeracao))
     with patch("builtins.open", m_leitura):
         cf1 = EolicaGeracao.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/newave/test_eolicahistorico.py` & `inewave-0.0.98/tests/newave/test_eolicahistorico.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 
 def test_neq_eolicahistorico():
     m: MagicMock = mock_open(read_data="".join(MockEolicaHistorico))
     with patch("builtins.open", m):
         cf1 = EolicaHistorico.read(ARQ_TESTE)
         cf2 = EolicaHistorico.read(ARQ_TESTE)
-        cf2.deleta_registro(cf1.eolica_historico_vento()[0])
+        cf2.data.remove(cf1.eolica_historico_vento()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicahistorico():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaHistorico))
     with patch("builtins.open", m_leitura):
         cf1 = EolicaHistorico.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/newave/test_eolicaposto.py` & `inewave-0.0.98/tests/newave/test_eolicaposto.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 
 def test_neq_eolicaposto():
     m: MagicMock = mock_open(read_data="".join(MockEolicaPosto))
     with patch("builtins.open", m):
         cf1 = EolicaPosto.read(ARQ_TESTE)
         cf2 = EolicaPosto.read(ARQ_TESTE)
-        cf2.deleta_registro(cf1.posto_vento_cad()[0])
+        cf2.data.remove(cf1.posto_vento_cad()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicaposto():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaPosto))
     with patch("builtins.open", m_leitura):
         cf1 = EolicaPosto.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/newave/test_eolicasubmercado.py` & `inewave-0.0.98/tests/newave/test_eolicasubmercado.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 
 def test_neq_eolicasubmercado():
     m: MagicMock = mock_open(read_data="".join(MockEolicaSubmercado))
     with patch("builtins.open", m):
         cf1 = EolicaSubmercado.read(ARQ_TESTE)
         cf2 = EolicaSubmercado.read(ARQ_TESTE)
-        cf2.deleta_registro(cf1.eolica_submercado()[0])
+        cf2.data.remove(cf1.eolica_submercado()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_eolicasubmercado():
     m_leitura: MagicMock = mock_open(read_data="".join(MockEolicaSubmercado))
     with patch("builtins.open", m_leitura):
         cf1 = EolicaSubmercado.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/newave/test_exph.py` & `inewave-0.0.98/tests/newave/test_exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_expt.py` & `inewave-0.0.98/tests/newave/test_expt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_forward.py` & `inewave-0.0.98/tests/newave/test_forward.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_forwarh.py` & `inewave-0.0.98/tests/newave/test_forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_ghmin.py` & `inewave-0.0.98/tests/newave/test_ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_hidr.py` & `inewave-0.0.98/tests/newave/test_hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_manutt.py` & `inewave-0.0.98/tests/newave/test_manutt.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         assert ad.manutencoes is not None
 
 
 def test_atributos_nao_encontrados_manutt():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         ad = Manutt.read(ARQ_TESTE)
-        print(ad.manutencoes)
         assert ad.manutencoes is None
 
 
 def test_eq_manutt():
     m: MagicMock = mock_open(read_data="".join(MockManutt))
     with patch("builtins.open", m):
         cf1 = Manutt.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/newave/test_modif.py` & `inewave-0.0.98/tests/newave/test_modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_newavetim.py` & `inewave-0.0.98/tests/newave/test_newavetim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import timedelta
 from inewave.newave.modelos.newavetim import (
     BlocoTemposEtapasTim,
 )
 
-from inewave.newave.newavetim import NewaveTim
+from inewave.newave.newavetim import Newavetim
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.newavetim import MockBlocoTemposEtapas, MockNewaveTim
 
@@ -26,33 +26,33 @@
     assert b.data.iloc[0, 0] == "Leitura de Dados"
     assert b.data.iloc[-1, -1] == timedelta(hours=3, minutes=26, seconds=7)
 
 
 def test_atributos_encontrados_newavetim():
     m: MagicMock = mock_open(read_data="".join(MockNewaveTim))
     with patch("builtins.open", m):
-        nt = NewaveTim.read(ARQ_TESTE)
+        nt = Newavetim.read(ARQ_TESTE)
         assert nt.tempos_etapas is not None
 
 
 def test_atributos_nao_encontrados_newavetim():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        nt = NewaveTim.read(ARQ_TESTE)
+        nt = Newavetim.read(ARQ_TESTE)
         assert nt.tempos_etapas is None
 
 
 def test_eq_newavetim():
     m: MagicMock = mock_open(read_data="".join(MockNewaveTim))
     with patch("builtins.open", m):
-        nt1 = NewaveTim.read(ARQ_TESTE)
-        nt2 = NewaveTim.read(ARQ_TESTE)
+        nt1 = Newavetim.read(ARQ_TESTE)
+        nt2 = Newavetim.read(ARQ_TESTE)
         assert nt1 == nt2
 
 
 def test_neq_newavetim():
     m: MagicMock = mock_open(read_data="".join(MockNewaveTim))
     with patch("builtins.open", m):
-        nt1 = NewaveTim.read(ARQ_TESTE)
-        nt2 = NewaveTim.read(ARQ_TESTE)
+        nt1 = Newavetim.read(ARQ_TESTE)
+        nt2 = Newavetim.read(ARQ_TESTE)
         nt2.tempos_etapas.iloc[0, 0] = ""
         assert nt1 != nt2
```

### Comparing `inewave-0.0.97/tests/newave/test_nwv_avl_evap.py` & `inewave-0.0.98/tests/newave/test_nwv_avl_evap.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def test_atributos_encontrados_nwv_avl_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvAvlEvap))
     with patch("builtins.open", m):
         rel = NwvAvlEvap.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
         assert rel.tabela.at[0, "periodo"] == 1
-        assert rel.tabela.at[0, "indice_usina"] == 4
+        assert rel.tabela.at[0, "codigo_usina"] == 4
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert rel.tabela.at[0, "volume_armazenado_hm3"] == 265.86
         assert rel.tabela.at[0, "evaporacao_calculada_hm3"] == 0.23
         assert rel.tabela.at[0, "evaporacao_modelo_hm3"] == 0.23
         assert rel.tabela.at[0, "desvio_absoluto_hm3"] == 0.0
         assert rel.tabela.at[0, "desvio_percentual"] == 0.0
```

### Comparing `inewave-0.0.97/tests/newave/test_nwv_cortes_evap.py` & `inewave-0.0.98/tests/newave/test_nwv_cortes_evap.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def test_atributos_encontrados_nwv_cortes_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvCortesEvap))
     with patch("builtins.open", m):
         rel = NwvCortesEvap.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
         assert rel.tabela.at[0, "periodo"] == 1
-        assert rel.tabela.at[0, "indice_usina"] == 4
+        assert rel.tabela.at[0, "codigo_usina"] == 4
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert rel.tabela.at[0, "derivada_cota_area"] == 0.0000000000
         assert rel.tabela.at[0, "derivada_volume_cota"] == 0.0000000000
         assert rel.tabela.at[0, "volume_referencia_hm3"] == 265.86
         assert rel.tabela.at[0, "evaporacao_referencia_hm3"] == 0.23
         assert rel.tabela.at[0, "coeficiente_volume"] == 0.0000000000
         assert rel.tabela.at[0, "rhs_volume"] == 0.2263
```

### Comparing `inewave-0.0.97/tests/newave/test_nwv_eco_evap.py` & `inewave-0.0.98/tests/newave/test_nwv_eco_evap.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def test_atributos_encontrados_nwv_eco_evap():
     m: MagicMock = mock_open(read_data="".join(MockNwvEcoEvap))
     with patch("builtins.open", m):
         rel = NwvEcoEvap.read(ARQ_TESTE)
         assert rel.versao == "FPHA_NEWAVE"
         assert rel.tabela.at[0, "periodo"] == 1
-        assert rel.tabela.at[0, "indice_usina"] == 4
+        assert rel.tabela.at[0, "codigo_usina"] == 4
         assert rel.tabela.at[0, "nome_usina"] == "FUNIL-GRANDE"
         assert rel.tabela.at[0, "volume_referencia_hm3"] == 265.86
         assert rel.tabela.at[0, "evaporacao_referencia_hm3"] == 0.23
         assert rel.tabela.at[0, "coeficiente_evaporacao_mm_mes"] == 6
         assert rel.tabela.at[0, "flag_evaporacao"] == 1
         assert rel.tabela.at[0, "evaporacao_linear"] == 1
         assert rel.tabela.at[0, "tipo_volume_referencia"] == 1
```

### Comparing `inewave-0.0.97/tests/newave/test_parp.py` & `inewave-0.0.98/tests/newave/test_parp.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     BlocoCorrelRuidosREE,
     BlocoSerieMediasREE,
     BlocoCorrelCruzadaMediaREE,
     BlocoCorrelEspacialAnualConfig,
     BlocoCorrelEspacialMensalConfig,
 )
 
-from inewave.newave import PARp
+from inewave.newave import Parp
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.parp import (
     MockSeriesEnergiaPARp,
@@ -97,18 +97,18 @@
     b = BlocoCoeficientesModeloREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
 
     assert b.data.shape[0] == 1
     assert b.data.shape[1] == 24
-    assert b.data.loc[0, "Psi 1"] == 0.207
-    assert b.data.loc[0, "Psi Norm 1"] == 0.263
-    assert b.data.loc[0, "Psi A"] == 0.177
-    assert b.data.loc[0, "Psi Norm A"] == 0.485
+    assert b.data.loc[0, "psi_1"] == 0.207
+    assert b.data.loc[0, "psi_norm_1"] == 0.263
+    assert b.data.loc[0, "psi_A"] == 0.177
+    assert b.data.loc[0, "psi_norm_A"] == 0.485
 
 
 def test_serie_ruidos_ree():
     m: MagicMock = mock_open(read_data="".join(MockSerieRuidosREE))
     b = BlocoSerieRuidosREE()
     with patch("builtins.open", m):
         with open("", "") as fp:
@@ -184,15 +184,15 @@
     assert b.data.iloc[0, 3] == 1.0000
     assert b.data.iloc[-1, -1] == 0.0671
 
 
 def test_atributos_encontrados_parp():
     m: MagicMock = mock_open(read_data="".join(MockPARp))
     with patch("builtins.open", m):
-        parp = PARp.read(ARQ_TESTE)
+        parp = Parp.read(ARQ_TESTE)
         assert parp.series_energia_ree is not None
         assert parp.correlacao_series_energia_ree is not None
         assert parp.correlacao_parcial_series_energia_ree is not None
         assert parp.ordem_original_modelo is not None
         assert parp.ordem_final_modelo is not None
         assert parp.coeficientes is not None
         assert parp.series_media_ree is not None
@@ -202,15 +202,15 @@
         assert parp.correlacao_espacial_anual is not None
         assert parp.correlacao_espacial_mensal is not None
 
 
 def test_atributos_nao_encontrados_parp():
     m: MagicMock = mock_open(read_data="".join(MockSeriesEnergiaPARp))
     with patch("builtins.open", m):
-        parp = PARp.read(ARQ_TESTE)
+        parp = Parp.read(ARQ_TESTE)
         assert parp.series_energia_ree is not None
         assert parp.correlacao_series_energia_ree is None
         assert parp.correlacao_parcial_series_energia_ree is None
         assert parp.ordem_original_modelo is None
         assert parp.ordem_final_modelo is None
         assert parp.coeficientes is None
         assert parp.series_media_ree is None
@@ -220,19 +220,19 @@
         assert parp.correlacao_espacial_anual is None
         assert parp.correlacao_espacial_mensal is None
 
 
 def test_eq_parp():
     m: MagicMock = mock_open(read_data="".join(MockPARp))
     with patch("builtins.open", m):
-        parp1 = PARp.read(ARQ_TESTE)
-        parp2 = PARp.read(ARQ_TESTE)
+        parp1 = Parp.read(ARQ_TESTE)
+        parp2 = Parp.read(ARQ_TESTE)
         assert parp1 == parp2
 
 
 def test_neq_parp():
     m: MagicMock = mock_open(read_data="".join(MockPARp))
     with patch("builtins.open", m):
-        parp1 = PARp.read(ARQ_TESTE)
-        parp2 = PARp.read(ARQ_TESTE)
+        parp1 = Parp.read(ARQ_TESTE)
+        parp2 = Parp.read(ARQ_TESTE)
         parp2.series_energia_ree.iloc[0, 0] = -1
         assert parp1 != parp2
```

### Comparing `inewave-0.0.97/tests/newave/test_parpeol.py` & `inewave-0.0.98/tests/newave/test_parpeol.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     BlocoCorrelVentosUEE,
     BlocoSerieRuidosUEE,
     BlocoCorrelRuidosUEE,
     BlocoCorrelEspacialAnualConfig,
     BlocoCorrelEspacialMensalConfig,
 )
 
-from inewave.newave.parpeol import PARpeol
+from inewave.newave.parpeol import Parpeol
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.parpeol import (
     MockSeriesVentosUEE,
@@ -103,43 +103,43 @@
     assert b.data.iloc[0, 3] == -0.3616
     assert b.data.iloc[-1, -1] == 1.000
 
 
 def test_atributos_encontrados_parpeol():
     m: MagicMock = mock_open(read_data="".join(MockPARpeol))
     with patch("builtins.open", m):
-        parp = PARpeol.read(ARQ_TESTE)
+        parp = Parpeol.read(ARQ_TESTE)
         assert parp.series_ventos_uee is not None
         assert parp.correlacao_series_ventos_uee is not None
         assert parp.series_ruido_uee is not None
         assert parp.correlacao_series_ruidos_uee is not None
         assert parp.correlacao_espacial_anual is not None
         assert parp.correlacao_espacial_mensal is not None
 
 
 def test_atributos_nao_encontrados_parp():
     m: MagicMock = mock_open(read_data="".join(""))
     with patch("builtins.open", m):
-        parp = PARpeol.read(ARQ_TESTE)
+        parp = Parpeol.read(ARQ_TESTE)
         assert parp.series_ventos_uee is None
         assert parp.correlacao_series_ventos_uee is None
         assert parp.series_ruido_uee is None
         assert parp.correlacao_series_ruidos_uee is None
         assert parp.correlacao_espacial_anual is None
         assert parp.correlacao_espacial_mensal is None
 
 
 def test_eq_parpeol():
     m: MagicMock = mock_open(read_data="".join(MockPARpeol))
     with patch("builtins.open", m):
-        parp1 = PARpeol.read(ARQ_TESTE)
-        parp2 = PARpeol.read(ARQ_TESTE)
+        parp1 = Parpeol.read(ARQ_TESTE)
+        parp2 = Parpeol.read(ARQ_TESTE)
         assert parp1 == parp2
 
 
 def test_neq_parpeol():
     m: MagicMock = mock_open(read_data="".join(MockPARpeol))
     with patch("builtins.open", m):
-        parp1 = PARpeol.read(ARQ_TESTE)
-        parp2 = PARpeol.read(ARQ_TESTE)
+        parp1 = Parpeol.read(ARQ_TESTE)
+        parp2 = Parpeol.read(ARQ_TESTE)
         parp2.series_ventos_uee.iloc[0, 0] = -1
         assert parp1 != parp2
```

### Comparing `inewave-0.0.97/tests/newave/test_parpvaz.py` & `inewave-0.0.98/tests/newave/test_parpvaz.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     BlocoOrdemModeloUHE,
     BlocoCoeficientesModeloUHE,
     BlocoSerieRuidosUHE,
     BlocoCorrelRuidosUHE,
     BlocoCorrelEspacialAnualMensalUHE,
 )
 
-from inewave.newave import PARpvaz
+from inewave.newave import Parpvaz
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.parpvaz import (
     MockSeriesVazoesPARpvaz,
@@ -88,21 +88,20 @@
 
 def test_coeficientes_modelo_uhe():
     m: MagicMock = mock_open(read_data="".join(MockCoeficientesModeloPARpvaz))
     b = BlocoCoeficientesModeloUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
             b.read(fp)
-    print(b.data)
     assert b.data.shape[0] == 1
     assert b.data.shape[1] == 24
-    assert b.data.loc[0, "Psi 1"] == 0.450
-    assert b.data.loc[0, "Psi Norm 1"] == 0.727
-    assert b.data.loc[0, "Psi A"] == 0.0
-    assert b.data.loc[0, "Psi Norm A"] == 0.0
+    assert b.data.loc[0, "psi_1"] == 0.450
+    assert b.data.loc[0, "psi_norm_1"] == 0.727
+    assert b.data.loc[0, "psi_A"] == 0.0
+    assert b.data.loc[0, "psi_norm_A"] == 0.0
 
 
 def test_serie_ruidos_uhe():
     m: MagicMock = mock_open(read_data="".join(MockSerieRuidosPARpvaz))
     b = BlocoSerieRuidosUHE()
     with patch("builtins.open", m):
         with open("", "") as fp:
@@ -141,49 +140,49 @@
     assert b.data.iloc[0, 2] == 0.55
     assert b.data.iloc[-1, -1] == 0.52
 
 
 def test_atributos_encontrados_parpvaz():
     m: MagicMock = mock_open(read_data="".join(MockPARpvaz))
     with patch("builtins.open", m):
-        parp = PARpvaz.read(ARQ_TESTE)
+        parp = Parpvaz.read(ARQ_TESTE)
         assert parp.series_vazoes_uhe is not None
         assert parp.correlacao_series_vazoes_uhe is not None
         assert parp.correlacao_parcial_series_vazoes_uhe is not None
         assert parp.ordem_original_modelo is not None
         assert parp.ordem_final_modelo is not None
         assert parp.coeficientes is not None
         assert parp.series_ruido_uhe is not None
         assert parp.correlacao_series_ruidos_uhe is not None
         assert parp.correlacao_espacial_anual_mensal is not None
 
 
 def test_atributos_nao_encontrados_parpvaz():
     m: MagicMock = mock_open(read_data="".join(MockSerieRuidosPARpvaz))
     with patch("builtins.open", m):
-        parp = PARpvaz.read(ARQ_TESTE)
+        parp = Parpvaz.read(ARQ_TESTE)
         assert parp.series_vazoes_uhe is None
         assert parp.correlacao_series_vazoes_uhe is None
         assert parp.correlacao_parcial_series_vazoes_uhe is None
         assert parp.ordem_original_modelo is None
         assert parp.ordem_final_modelo is None
         assert parp.coeficientes is None
         assert parp.series_ruido_uhe is None
         assert parp.correlacao_series_ruidos_uhe is None
         assert parp.correlacao_espacial_anual_mensal is None
 
 
 def test_eq_parpvaz():
     m: MagicMock = mock_open(read_data="".join(MockPARpvaz))
     with patch("builtins.open", m):
-        parp1 = PARpvaz.read(ARQ_TESTE)
-        parp2 = PARpvaz.read(ARQ_TESTE)
+        parp1 = Parpvaz.read(ARQ_TESTE)
+        parp2 = Parpvaz.read(ARQ_TESTE)
         assert parp1 == parp2
 
 
 def test_neq_parpvaz():
     m: MagicMock = mock_open(read_data="".join(MockPARpvaz))
     with patch("builtins.open", m):
-        parp1 = PARpvaz.read(ARQ_TESTE)
-        parp2 = PARpvaz.read(ARQ_TESTE)
+        parp1 = Parpvaz.read(ARQ_TESTE)
+        parp2 = Parpvaz.read(ARQ_TESTE)
         parp2.series_vazoes_uhe.iloc[0, 0] = -1
         assert parp1 != parp2
```

### Comparing `inewave-0.0.97/tests/newave/test_patamar.py` & `inewave-0.0.98/tests/newave/test_patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_penalid.py` & `inewave-0.0.98/tests/newave/test_penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_pmo.py` & `inewave-0.0.98/tests/newave/test_pmo.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     BlocoMARSPMO,
     BlocoRiscoDeficitENSPMO,
     BlocoCustoOperacaoPMO,
     BlocoCustoOperacaoTotalPMO,
     BlocoProdutibilidadesConfiguracaoPMO,
 )
 
-from inewave.newave import PMO
+from inewave.newave import Pmo
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.pmo import MockBlocoEafPastTendenciaHidrolPMO
 from tests.mocks.arquivos.pmo import MockBlocoEafPastCfugaMedioPMO
@@ -165,15 +165,15 @@
     assert b.data.iloc[1, 14] == 2.2292
     assert b.data.iloc[1, 15] == 2.2697
 
 
 def test_atributos_encontrados_pmo():
     m: MagicMock = mock_open(read_data="".join(MockPMO))
     with patch("builtins.open", m):
-        pmo = PMO.read(ARQ_TESTE)
+        pmo = Pmo.read(ARQ_TESTE)
         assert pmo.eafpast_tendencia_hidrologica is not None
         assert pmo.eafpast_cfuga_medio is not None
         assert pmo.convergencia is not None
         assert pmo.configuracoes_alteracao_potencia is not None
         assert pmo.configuracoes_entrada_reservatorio is not None
         assert pmo.configuracoes_qualquer_modificacao is not None
         assert pmo.retas_perdas_engolimento(1) is not None
@@ -186,30 +186,30 @@
         assert pmo.desvio_custo_operacao_total is not None
         assert pmo.produtibilidades_equivalentes is not None
 
 
 def test_atributos_nao_encontrados_pmo():
     m: MagicMock = mock_open(read_data="".join(MockBlocoConvergenciaPMO))
     with patch("builtins.open", m):
-        pmo = PMO.read(ARQ_TESTE)
+        pmo = Pmo.read(ARQ_TESTE)
         assert pmo.convergencia is not None
         assert pmo.custo_operacao_series_simuladas is None
         assert pmo.custo_operacao_total is None
         assert pmo.desvio_custo_operacao_total is None
         assert pmo.produtibilidades_equivalentes is None
 
 
 def test_eq_pmo():
     m: MagicMock = mock_open(read_data="".join(MockPMO))
     with patch("builtins.open", m):
-        pmo1 = PMO.read(ARQ_TESTE)
-        pmo2 = PMO.read(ARQ_TESTE)
+        pmo1 = Pmo.read(ARQ_TESTE)
+        pmo2 = Pmo.read(ARQ_TESTE)
         assert pmo1 == pmo2
 
 
 def test_neq_pmo():
     m: MagicMock = mock_open(read_data="".join(MockPMO))
     with patch("builtins.open", m):
-        pmo1 = PMO.read(ARQ_TESTE)
-        pmo2 = PMO.read(ARQ_TESTE)
+        pmo1 = Pmo.read(ARQ_TESTE)
+        pmo2 = Pmo.read(ARQ_TESTE)
         pmo2.configuracoes_alteracao_potencia
         assert pmo1 == pmo2
```

### Comparing `inewave-0.0.97/tests/newave/test_re.py` & `inewave-0.0.98/tests/newave/test_re.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Rotinas de testes associadas ao arquivo re.dat do NEWAVE
 from inewave.newave.modelos.re import (
     BlocoUsinasConjuntoRE,
     BlocoConfiguracaoRestricoesRE,
 )
 
-from inewave.newave import RE
+from inewave.newave import Re
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.re import (
     MockBlocoUsinasRestricoes,
@@ -42,53 +42,53 @@
     assert b.data.iloc[-1, 0] == 10
     assert b.data.iloc[-1, -1] == "C. CALDEIRAO E F. GOMES"
 
 
 def test_atributos_encontrados_re():
     m: MagicMock = mock_open(read_data="".join(MockRE))
     with patch("builtins.open", m):
-        ad = RE.read(ARQ_TESTE)
+        ad = Re.read(ARQ_TESTE)
         assert ad.usinas_conjuntos is not None
         assert ad.restricoes is not None
 
 
 def test_atributos_nao_encontrados_re():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = RE.read(ARQ_TESTE)
+        ad = Re.read(ARQ_TESTE)
         assert ad.usinas_conjuntos is None
         assert ad.restricoes is None
 
 
 def test_eq_re():
     m: MagicMock = mock_open(read_data="".join(MockRE))
     with patch("builtins.open", m):
-        cf1 = RE.read(ARQ_TESTE)
-        cf2 = RE.read(ARQ_TESTE)
+        cf1 = Re.read(ARQ_TESTE)
+        cf2 = Re.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_re():
     m: MagicMock = mock_open(read_data="".join(MockRE))
     with patch("builtins.open", m):
-        cf1 = RE.read(ARQ_TESTE)
-        cf2 = RE.read(ARQ_TESTE)
+        cf1 = Re.read(ARQ_TESTE)
+        cf2 = Re.read(ARQ_TESTE)
         cf2.usinas_conjuntos.loc[0, 0] = 0
         assert cf1 != cf2
 
 
 def test_leitura_escrita_re():
     m_leitura: MagicMock = mock_open(read_data="".join(MockRE))
     with patch("builtins.open", m_leitura):
-        cf1 = RE.read(ARQ_TESTE)
+        cf1 = Re.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = RE.read(ARQ_TESTE)
+        cf2 = Re.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.97/tests/newave/test_ree.py` & `inewave-0.0.98/tests/newave/test_ree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Rotinas de testes associadas ao arquivo ree.dat do NEWAVE
-from inewave.newave.ree import REE
+from inewave.newave.ree import Ree
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.ree import (
     MockREE,
@@ -11,53 +11,53 @@
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_ree():
     m: MagicMock = mock_open(read_data="".join(MockREE))
     with patch("builtins.open", m):
-        ad = REE.read(ARQ_TESTE)
+        ad = Ree.read(ARQ_TESTE)
         assert ad.rees is not None
         assert ad.remocao_ficticias is not None
 
 
 def test_atributos_nao_encontrados_ree():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = REE.read(ARQ_TESTE)
+        ad = Ree.read(ARQ_TESTE)
         assert ad.rees is None
         assert ad.remocao_ficticias is None
 
 
 def test_eq_ree():
     m: MagicMock = mock_open(read_data="".join(MockREE))
     with patch("builtins.open", m):
-        cf1 = REE.read(ARQ_TESTE)
-        cf2 = REE.read(ARQ_TESTE)
+        cf1 = Ree.read(ARQ_TESTE)
+        cf2 = Ree.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_ree():
     m: MagicMock = mock_open(read_data="".join(MockREE))
     with patch("builtins.open", m):
-        cf1 = REE.read(ARQ_TESTE)
-        cf2 = REE.read(ARQ_TESTE)
+        cf1 = Ree.read(ARQ_TESTE)
+        cf2 = Ree.read(ARQ_TESTE)
         cf2.rees.loc[0, 0] = 0
         assert cf1 != cf2
 
 
 def test_leitura_escrita_ree():
     m_leitura: MagicMock = mock_open(read_data="".join(MockREE))
     with patch("builtins.open", m_leitura):
-        cf1 = REE.read(ARQ_TESTE)
+        cf1 = Ree.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = REE.read(ARQ_TESTE)
+        cf2 = Ree.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.97/tests/newave/test_restricaoeletrica.py` & `inewave-0.0.98/tests/newave/test_restricaoeletrica.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 
 def test_neq_restricaoeletrica():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoEletrica))
     with patch("builtins.open", m):
         cf1 = RestricaoEletrica.read(ARQ_TESTE)
         cf2 = RestricaoEletrica.read(ARQ_TESTE)
-        cf2.deleta_registro(cf1.re()[0])
+        cf2.data.remove(cf1.re()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_restricaoeletrica():
     m_leitura: MagicMock = mock_open(read_data="".join(MockRestricaoEletrica))
     with patch("builtins.open", m_leitura):
         cf1 = RestricaoEletrica.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/newave/test_restricaoenergia.py` & `inewave-0.0.98/tests/newave/test_restricaoenergia.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 def test_neq_restricaoenergia():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoEnergia))
     with patch("builtins.open", m):
         cf1 = RestricaoEnergia.read(ARQ_TESTE)
         cf2 = RestricaoEnergia.read(ARQ_TESTE)
-        cf2.deleta_registro(cf1.rhe()[0])
+        cf2.data.remove(cf1.rhe()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_restricaoenergia():
     m_leitura: MagicMock = mock_open(read_data="".join(MockRestricaoEnergia))
     with patch("builtins.open", m_leitura):
         cf1 = RestricaoEnergia.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/newave/test_restricaovazao.py` & `inewave-0.0.98/tests/newave/test_restricaovazao.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 def test_neq_restricaovazao():
     m: MagicMock = mock_open(read_data="".join(MockRestricaoVazao))
     with patch("builtins.open", m):
         cf1 = RestricaoVazao.read(ARQ_TESTE)
         cf2 = RestricaoVazao.read(ARQ_TESTE)
-        cf2.deleta_registro(cf1.rhq()[0])
+        cf2.data.remove(cf1.rhq()[0])
         assert cf1 != cf2
 
 
 def test_leitura_escrita_restricaovazao():
     m_leitura: MagicMock = mock_open(read_data="".join(MockRestricaoVazao))
     with patch("builtins.open", m_leitura):
         cf1 = RestricaoVazao.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/newave/test_selcor.py` & `inewave-0.0.98/tests/newave/test_selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_shist.py` & `inewave-0.0.98/tests/newave/test_shist.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_sistema.py` & `inewave-0.0.98/tests/newave/test_sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_term.py` & `inewave-0.0.98/tests/newave/test_term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_vazaob.py` & `inewave-0.0.98/tests/newave/test_vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_vazaof.py` & `inewave-0.0.98/tests/newave/test_vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_vazaos.py` & `inewave-0.0.98/tests/newave/test_vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_vazoes.py` & `inewave-0.0.98/tests/newave/test_vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/newave/test_vazpast.py` & `inewave-0.0.98/tests/newave/test_vazpast.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Rotinas de testes associadas ao arquivo vazpast.dat do NEWAVE
 from inewave.newave.modelos.vazpast import BlocoVazPast
 
-from inewave.newave import VazPast
+from inewave.newave import Vazpast
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.vazpast import MockBlocoVazoesPassadas
 
@@ -23,53 +23,53 @@
     assert b.data.iloc[0, 0] == 1
     assert b.data.iloc[-1, -1] == 20.0
 
 
 def test_atributos_encontrados_vazpast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoVazoesPassadas))
     with patch("builtins.open", m):
-        ad = VazPast.read(ARQ_TESTE)
+        ad = Vazpast.read(ARQ_TESTE)
         assert ad.tendencia is not None
 
 
 def test_atributos_nao_encontrados_vazpast():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        ad = VazPast.read(ARQ_TESTE)
+        ad = Vazpast.read(ARQ_TESTE)
         assert ad.tendencia is None
 
 
 def test_eq_vazpast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoVazoesPassadas))
     with patch("builtins.open", m):
-        cf1 = VazPast.read(ARQ_TESTE)
-        cf2 = VazPast.read(ARQ_TESTE)
+        cf1 = Vazpast.read(ARQ_TESTE)
+        cf2 = Vazpast.read(ARQ_TESTE)
         assert cf1 == cf2
 
 
 def test_neq_vazpast():
     m: MagicMock = mock_open(read_data="".join(MockBlocoVazoesPassadas))
     with patch("builtins.open", m):
-        cf1 = VazPast.read(ARQ_TESTE)
-        cf2 = VazPast.read(ARQ_TESTE)
+        cf1 = Vazpast.read(ARQ_TESTE)
+        cf2 = Vazpast.read(ARQ_TESTE)
         cf2.tendencia.iloc[0, 0] = -1
         assert cf1 != cf2
 
 
 def test_leitura_escrita_vazpast():
     m_leitura: MagicMock = mock_open(
         read_data="".join(MockBlocoVazoesPassadas)
     )
     with patch("builtins.open", m_leitura):
-        cf1 = VazPast.read(ARQ_TESTE)
+        cf1 = Vazpast.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
             chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
-        cf2 = VazPast.read(ARQ_TESTE)
+        cf2 = Vazpast.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.97/tests/nwlistcf/test_arquivos.py` & `inewave-0.0.98/tests/nwlistcf/test_arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/nwlistcf/test_caso.py` & `inewave-0.0.98/tests/nwlistcf/test_caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/nwlistcf/test_estados.py` & `inewave-0.0.98/tests/nwlistcf/test_estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/nwlistcf/test_nwlistcfdat.py` & `inewave-0.0.98/tests/nwlistcf/test_nwlistcfdat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/nwlistcf/test_nwlistcfrel.py` & `inewave-0.0.98/tests/nwlistcf/test_nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/nwlistop/test_cdef.py` & `inewave-0.0.98/tests/nwlistop/test_cdef.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from inewave.nwlistop.cdef import Cdef
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.cdef import MockCdef
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_cdef():
     m: MagicMock = mock_open(read_data="".join(MockCdef))
     with patch("builtins.open", m):
         n = Cdef.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_cdef():
     m: MagicMock = mock_open(read_data="")
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_cdefsin.py` & `inewave-0.0.98/tests/nwlistop/test_geol.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from inewave.nwlistop.cdefsin import CdefSIN
+from inewave.nwlistop.geol import Geol
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.cdefsin import MockCdefSIN
+from tests.mocks.arquivos.geol import MockGeol
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_cdefsin():
-    m: MagicMock = mock_open(read_data="".join(MockCdefSIN))
+def test_atributos_encontrados_geol():
+    m: MagicMock = mock_open(read_data="".join(MockGeol))
     with patch("builtins.open", m):
-        n = CdefSIN.read(ARQ_TESTE)
+        n = Geol.read(ARQ_TESTE)
+        assert n.usina is not None
+        # assert n.pee == "cluster_NE_1"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 2875.5
 
 
-def test_atributos_nao_encontrados_cdefsin():
+def test_atributos_nao_encontrados_geol():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = CdefSIN.read(ARQ_TESTE)
+        n = Geol.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_cdefsin():
-    m: MagicMock = mock_open(read_data="".join(MockCdefSIN))
+def test_eq_geol():
+    m: MagicMock = mock_open(read_data="".join(MockGeol))
     with patch("builtins.open", m):
-        n1 = CdefSIN.read(ARQ_TESTE)
-        n2 = CdefSIN.read(ARQ_TESTE)
+        n1 = Geol.read(ARQ_TESTE)
+        n2 = Geol.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_cmarg.py` & `inewave-0.0.98/tests/nwlistop/test_cmarg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from inewave.nwlistop.cmarg import Cmarg
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.cmarg import MockCmarg
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_cmarg():
     m: MagicMock = mock_open(read_data="".join(MockCmarg))
     with patch("builtins.open", m):
         n = Cmarg.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 1995
-        assert n.valores.iloc[-1, -1] == 35.42
+        assert n.valores.iloc[0, 0] == datetime(1995, 1, 1)
+        assert n.valores.iloc[-1, -1] == 16.61
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_cmarg():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_cmargmed.py` & `inewave-0.0.98/tests/nwlistop/test_cmargmed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.cmargmed import CmargMed
+from inewave.nwlistop.cmargmed import Cmargmed
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.cmargmed import MockCmargMed
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_cmargmed():
     m: MagicMock = mock_open(read_data="".join(MockCmargMed))
     with patch("builtins.open", m):
-        n = CmargMed.read(ARQ_TESTE)
+        n = Cmargmed.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 354.22
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 98.5
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_cmargmed():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = CmargMed.read(ARQ_TESTE)
+        n = Cmargmed.read(ARQ_TESTE)
         assert n.valores is None
         assert n.submercado is None
 
 
 def test_eq_cmargmed():
     m: MagicMock = mock_open(read_data="".join(MockCmargMed))
     with patch("builtins.open", m):
-        n1 = CmargMed.read(ARQ_TESTE)
-        n2 = CmargMed.read(ARQ_TESTE)
+        n1 = Cmargmed.read(ARQ_TESTE)
+        n2 = Cmargmed.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_coper.py` & `inewave-0.0.98/tests/nwlistop/test_coper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from inewave.nwlistop.coper import Coper
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.coper import MockCoper
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_coper():
     m: MagicMock = mock_open(read_data="".join(MockCoper))
     with patch("builtins.open", m):
         n = Coper.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 1155.67
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 691.64
 
 
 def test_atributos_nao_encontrados_coper():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         n = Coper.read(ARQ_TESTE)
         assert n.valores is None
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_corteolm.py` & `inewave-0.0.98/tests/nwlistop/test_fteolm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.corteolm import Corteolm
+from inewave.nwlistop.fteolm import Fteolm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.corteolm import MockCorteolm
+from tests.mocks.arquivos.fteolm import MockFteolm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_corteolm():
-    m: MagicMock = mock_open(read_data="".join(MockCorteolm))
+def test_atributos_encontrados_fteolm():
+    m: MagicMock = mock_open(read_data="".join(MockFteolm))
     with patch("builtins.open", m):
-        n = Corteolm.read(ARQ_TESTE)
+        n = Fteolm.read(ARQ_TESTE)
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_corteolm():
+def test_atributos_nao_encontrados_fteolm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Corteolm.read(ARQ_TESTE)
+        n = Fteolm.read(ARQ_TESTE)
         assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_corteolm():
-    m: MagicMock = mock_open(read_data="".join(MockCorteolm))
+def test_eq_fteolm():
+    m: MagicMock = mock_open(read_data="".join(MockFteolm))
     with patch("builtins.open", m):
-        n1 = Corteolm.read(ARQ_TESTE)
-        n2 = Corteolm.read(ARQ_TESTE)
+        n1 = Fteolm.read(ARQ_TESTE)
+        n2 = Fteolm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_cterm.py` & `inewave-0.0.98/tests/nwlistop/test_gtert.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-from inewave.nwlistop.cterm import Cterm
+from inewave.nwlistop.gtert import Gtert
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.cterm import MockCterm
+from tests.mocks.arquivos.gtert import MockGtert
+
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_cterm():
-    m: MagicMock = mock_open(read_data="".join(MockCterm))
+def test_atributos_encontrados_gtert():
+    m: MagicMock = mock_open(read_data="".join(MockGtert))
     with patch("builtins.open", m):
-        n = Cterm.read(ARQ_TESTE)
+        n = Gtert.read(ARQ_TESTE)
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 585.36
+        assert n.valores.iloc[0, 0] == "1"
+        assert n.valores.iloc[1, -1] == 162.9
 
 
-def test_atributos_nao_encontrados_cterm():
+def test_atributos_nao_encontrados_gtert():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Cterm.read(ARQ_TESTE)
+        n = Gtert.read(ARQ_TESTE)
         assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_cterm():
-    m: MagicMock = mock_open(read_data="".join(MockCterm))
+def test_eq_gtert():
+    m: MagicMock = mock_open(read_data="".join(MockGtert))
     with patch("builtins.open", m):
-        n1 = Cterm.read(ARQ_TESTE)
-        n2 = Cterm.read(ARQ_TESTE)
+        n1 = Gtert.read(ARQ_TESTE)
+        n2 = Gtert.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_ctermsin.py` & `inewave-0.0.98/tests/nwlistop/test_gttot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from inewave.nwlistop.ctermsin import CtermSIN
+from inewave.nwlistop.gttot import Gttot
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ctermsin import MockCtermSIN
+from tests.mocks.arquivos.gttot import MockGttot
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_ctermsin():
-    m: MagicMock = mock_open(read_data="".join(MockCtermSIN))
+def test_atributos_encontrados_gttot():
+    m: MagicMock = mock_open(read_data="".join(MockGttot))
     with patch("builtins.open", m):
-        n = CtermSIN.read(ARQ_TESTE)
+        n = Gttot.read(ARQ_TESTE)
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 1230.35
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 2853.5
 
 
-def test_atributos_nao_encontrados_ctermsin():
+def test_atributos_nao_encontrados_gttot():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = CtermSIN.read(ARQ_TESTE)
+        n = Gttot.read(ARQ_TESTE)
+        assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_ctermsin():
-    m: MagicMock = mock_open(read_data="".join(MockCtermSIN))
+def test_eq_gttot():
+    m: MagicMock = mock_open(read_data="".join(MockGttot))
     with patch("builtins.open", m):
-        n1 = CtermSIN.read(ARQ_TESTE)
-        n2 = CtermSIN.read(ARQ_TESTE)
+        n1 = Gttot.read(ARQ_TESTE)
+        n2 = Gttot.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_deficit.py` & `inewave-0.0.98/tests/nwlistop/test_deficit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from inewave.nwlistop.deficit import Def
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.deficit import MockDef
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_def():
     m: MagicMock = mock_open(read_data="".join(MockDef))
     with patch("builtins.open", m):
         n = Def.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_def():
     m: MagicMock = mock_open(read_data="")
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_defsin.py` & `inewave-0.0.98/tests/nwlistop/test_defsin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.defsin import DefSIN
+from inewave.nwlistop.defsin import Defsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.defsin import MockDefSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_defsin():
     m: MagicMock = mock_open(read_data="".join(MockDefSIN))
     with patch("builtins.open", m):
-        n = DefSIN.read(ARQ_TESTE)
+        n = Defsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_defsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DefSIN.read(ARQ_TESTE)
+        n = Defsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_defsin():
     m: MagicMock = mock_open(read_data="".join(MockDefSIN))
     with patch("builtins.open", m):
-        n1 = DefSIN.read(ARQ_TESTE)
-        n2 = DefSIN.read(ARQ_TESTE)
+        n1 = Defsin.read(ARQ_TESTE)
+        n2 = Defsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_depminuh.py` & `inewave-0.0.98/tests/nwlistop/test_depminuh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from inewave.nwlistop.depminuh import Depminuh
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.depminuh import MockDepminUH
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
@@ -11,16 +12,16 @@
 def test_atributos_encontrados_depminuh():
     m: MagicMock = mock_open(read_data="".join(MockDepminUH))
     with patch("builtins.open", m):
         n = Depminuh.read(ARQ_TESTE)
         assert n.usina is not None
         assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 3.57
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 42.79
 
 
 def test_atributos_nao_encontrados_depminuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         n = Depminuh.read(ARQ_TESTE)
         assert n.usina is None
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_dfphauh.py` & `inewave-0.0.98/tests/nwlistop/test_dfphauh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from inewave.nwlistop.dfphauh import Dfphauh
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.dfphauh import MockDfphauh
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
@@ -11,15 +12,15 @@
 def test_atributos_encontrados_fphauh():
     m: MagicMock = mock_open(read_data="".join(MockDfphauh))
     with patch("builtins.open", m):
         n = Dfphauh.read(ARQ_TESTE)
         assert n.usina is not None
         assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_fphauh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         n = Dfphauh.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_dlppdfmax.py` & `inewave-0.0.98/tests/nwlistop/test_dlppdfmax.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.dlppdfmax import DLPPdfmax
+from inewave.nwlistop.dlppdfmax import Dlppdfmax
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.dlppdfmax import MockDLPPdfmax
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_dlppdfmax():
     m: MagicMock = mock_open(read_data="".join(MockDLPPdfmax))
     with patch("builtins.open", m):
-        n = DLPPdfmax.read(ARQ_TESTE)
+        n = Dlppdfmax.read(ARQ_TESTE)
         assert n.ree is not None
         assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_dlppdfmax():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPdfmax.read(ARQ_TESTE)
+        n = Dlppdfmax.read(ARQ_TESTE)
         assert n.ree is None
         assert n.valores is None
 
 
 def test_eq_dlppdfmax():
     m: MagicMock = mock_open(read_data="".join(MockDLPPdfmax))
     with patch("builtins.open", m):
-        n1 = DLPPdfmax.read(ARQ_TESTE)
-        n2 = DLPPdfmax.read(ARQ_TESTE)
+        n1 = Dlppdfmax.read(ARQ_TESTE)
+        n2 = Dlppdfmax.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_dlppdfmaxm.py` & `inewave-0.0.98/tests/nwlistop/test_dlppdfmaxm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.dlppdfmaxm import DLPPdfmaxm
+from inewave.nwlistop.dlppdfmaxm import Dlppdfmaxm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.dlppdfmaxm import MockDLPPdfmaxm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_dlppdfmaxm():
     m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxm))
     with patch("builtins.open", m):
-        n = DLPPdfmaxm.read(ARQ_TESTE)
+        n = Dlppdfmaxm.read(ARQ_TESTE)
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_dlppdfmaxm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPdfmaxm.read(ARQ_TESTE)
+        n = Dlppdfmaxm.read(ARQ_TESTE)
         assert n.submercado is None
         assert n.valores is None
 
 
 def test_eq_dlppdfmaxm():
     m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxm))
     with patch("builtins.open", m):
-        n1 = DLPPdfmaxm.read(ARQ_TESTE)
-        n2 = DLPPdfmaxm.read(ARQ_TESTE)
+        n1 = Dlppdfmaxm.read(ARQ_TESTE)
+        n2 = Dlppdfmaxm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_dlppdfmaxs.py` & `inewave-0.0.98/tests/nwlistop/test_vento.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from inewave.nwlistop.dlppdfmaxs import DLPPdfmaxs
+from inewave.nwlistop.vento import Vento
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dlppdfmaxs import MockDLPPdfmaxs
+from tests.mocks.arquivos.vento import MockVento
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_dlppdfmaxs():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxs))
+def test_atributos_encontrados_vento():
+    m: MagicMock = mock_open(read_data="".join(MockVento))
     with patch("builtins.open", m):
-        n = DLPPdfmaxs.read(ARQ_TESTE)
+        n = Vento.read(ARQ_TESTE)
+        assert n.usina is not None
+        # assert n.usina == "cluster_NE_1"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 7.63
 
 
-def test_atributos_nao_encontrados_dlppdfmaxs():
+def test_atributos_nao_encontrados_vento():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPdfmaxs.read(ARQ_TESTE)
+        n = Vento.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_dlppdfmaxs():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxs))
+def test_eq_vento():
+    m: MagicMock = mock_open(read_data="".join(MockVento))
     with patch("builtins.open", m):
-        n1 = DLPPdfmaxs.read(ARQ_TESTE)
-        n2 = DLPPdfmaxs.read(ARQ_TESTE)
+        n1 = Vento.read(ARQ_TESTE)
+        n2 = Vento.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_dlpptbmax.py` & `inewave-0.0.98/tests/nwlistop/test_dlpptbmaxs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-from inewave.nwlistop.dlpptbmax import DLPPtbmax
+from inewave.nwlistop.dlpptbmaxs import Dlpptbmaxs
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dlpptbmax import MockDLPPtbmax
+from tests.mocks.arquivos.dlpptbmaxs import MockDLPPtbmaxs
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_dlpptbmax():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmax))
+def test_atributos_encontrados_dlpptbmaxs():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxs))
     with patch("builtins.open", m):
-        n = DLPPtbmax.read(ARQ_TESTE)
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        n = Dlpptbmaxs.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_dlpptbmax():
+def test_atributos_nao_encontrados_dlpptbmaxs():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPtbmax.read(ARQ_TESTE)
-        assert n.ree is None
+        n = Dlpptbmaxs.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_dlpptbmax():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmax))
+def test_eq_dlpptbmaxs():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxs))
     with patch("builtins.open", m):
-        n1 = DLPPtbmax.read(ARQ_TESTE)
-        n2 = DLPPtbmax.read(ARQ_TESTE)
+        n1 = Dlpptbmaxs.read(ARQ_TESTE)
+        n2 = Dlpptbmaxs.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_dlpptbmaxm.py` & `inewave-0.0.98/tests/nwlistop/test_dlpptbmaxm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.dlpptbmaxm import DLPPtbmaxm
+from inewave.nwlistop.dlpptbmaxm import Dlpptbmaxm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.dlpptbmaxm import MockDLPPtbmaxm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_dlpptbmaxm():
     m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxm))
     with patch("builtins.open", m):
-        n = DLPPtbmaxm.read(ARQ_TESTE)
+        n = Dlpptbmaxm.read(ARQ_TESTE)
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_dlpptbmaxm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPtbmaxm.read(ARQ_TESTE)
+        n = Dlpptbmaxm.read(ARQ_TESTE)
         assert n.submercado is None
         assert n.valores is None
 
 
 def test_eq_dlpptbmaxm():
     m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxm))
     with patch("builtins.open", m):
-        n1 = DLPPtbmaxm.read(ARQ_TESTE)
-        n2 = DLPPtbmaxm.read(ARQ_TESTE)
+        n1 = Dlpptbmaxm.read(ARQ_TESTE)
+        n2 = Dlpptbmaxm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_dlpptbmaxs.py` & `inewave-0.0.98/tests/nwlistop/test_dlpptbmax.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from inewave.nwlistop.dlpptbmaxs import DLPPtbmaxs
+from inewave.nwlistop.dlpptbmax import Dlpptbmax
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dlpptbmaxs import MockDLPPtbmaxs
+from tests.mocks.arquivos.dlpptbmax import MockDLPPtbmax
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_dlpptbmaxs():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxs))
+def test_atributos_encontrados_dlpptbmax():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmax))
     with patch("builtins.open", m):
-        n = DLPPtbmaxs.read(ARQ_TESTE)
+        n = Dlpptbmax.read(ARQ_TESTE)
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_dlpptbmaxs():
+def test_atributos_nao_encontrados_dlpptbmax():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = DLPPtbmaxs.read(ARQ_TESTE)
+        n = Dlpptbmax.read(ARQ_TESTE)
+        assert n.ree is None
         assert n.valores is None
 
 
-def test_eq_dlpptbmaxs():
-    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmaxs))
+def test_eq_dlpptbmax():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPtbmax))
     with patch("builtins.open", m):
-        n1 = DLPPtbmaxs.read(ARQ_TESTE)
-        n2 = DLPPtbmaxs.read(ARQ_TESTE)
+        n1 = Dlpptbmax.read(ARQ_TESTE)
+        n2 = Dlpptbmax.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_dtbmax.py` & `inewave-0.0.98/tests/nwlistop/test_dtbmax.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from inewave.nwlistop.dtbmax import Dtbmax
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.dtbmax import MockDtbmax
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
@@ -11,15 +12,15 @@
 def test_atributos_encontrados_dtbmax():
     m: MagicMock = mock_open(read_data="".join(MockDtbmax))
     with patch("builtins.open", m):
         n = Dtbmax.read(ARQ_TESTE)
         assert n.usina is not None
         assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_dtbmax():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         n = Dtbmax.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_dtbmin.py` & `inewave-0.0.98/tests/nwlistop/test_vghminuh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.dtbmin import Dtbmin
+from inewave.nwlistop.vghminuh import Vghminuh
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.dtbmin import MockDtbmin
+from tests.mocks.arquivos.vghminuh import MockVghminUH
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_dtbmin():
-    m: MagicMock = mock_open(read_data="".join(MockDtbmin))
+def test_atributos_encontrados_vghminuh():
+    m: MagicMock = mock_open(read_data="".join(MockVghminUH))
     with patch("builtins.open", m):
-        n = Dtbmin.read(ARQ_TESTE)
+        n = Vghminuh.read(ARQ_TESTE)
         assert n.usina is not None
         assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_dtbmin():
+def test_atributos_nao_encontrados_vghminuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Dtbmin.read(ARQ_TESTE)
+        n = Vghminuh.read(ARQ_TESTE)
         assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_dtbmin():
-    m: MagicMock = mock_open(read_data="".join(MockDtbmin))
+def test_eq_vghminuh():
+    m: MagicMock = mock_open(read_data="".join(MockVghminUH))
     with patch("builtins.open", m):
-        n1 = Dtbmin.read(ARQ_TESTE)
-        n2 = Dtbmin.read(ARQ_TESTE)
+        n1 = Vghminuh.read(ARQ_TESTE)
+        n2 = Vghminuh.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_dvazmax.py` & `inewave-0.0.98/tests/nwlistop/test_dvazmax.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from inewave.nwlistop.dvazmax import Dvazmax
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.dvazmax import MockDvazmax
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
@@ -11,15 +12,15 @@
 def test_atributos_encontrados_dvazmax():
     m: MagicMock = mock_open(read_data="".join(MockDvazmax))
     with patch("builtins.open", m):
         n = Dvazmax.read(ARQ_TESTE)
         assert n.usina is not None
         assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_dvazmax():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         n = Dvazmax.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_eaf.py` & `inewave-0.0.98/tests/nwlistop/test_ghiduh.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.eaf import Eaf
+from inewave.nwlistop.ghiduh import Ghiduh
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.eaf import MockEaf
+from tests.mocks.arquivos.ghiduh import MockGhidUH
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_eaf():
-    m: MagicMock = mock_open(read_data="".join(MockEaf))
+def test_atributos_encontrados_ghiduh():
+    m: MagicMock = mock_open(read_data="".join(MockGhidUH))
     with patch("builtins.open", m):
-        n = Eaf.read(ARQ_TESTE)
+        n = Ghiduh.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 2929.0
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_eaf():
+def test_atributos_nao_encontrados_ghiduh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Eaf.read(ARQ_TESTE)
+        n = Ghiduh.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
-        assert n.ree is None
 
 
-def test_eq_eaf():
-    m: MagicMock = mock_open(read_data="".join(MockEaf))
+def test_eq_ghiduh():
+    m: MagicMock = mock_open(read_data="".join(MockGhidUH))
     with patch("builtins.open", m):
-        n1 = Eaf.read(ARQ_TESTE)
-        n2 = Eaf.read(ARQ_TESTE)
+        n1 = Ghiduh.read(ARQ_TESTE)
+        n2 = Ghiduh.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_eafb.py` & `inewave-0.0.98/tests/nwlistop/test_eafb.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from inewave.nwlistop.eafb import Eafb
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.eafb import MockEafb
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_eafb():
     m: MagicMock = mock_open(read_data="".join(MockEafb))
     with patch("builtins.open", m):
         n = Eafb.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 4523.0
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 5067.0
         assert n.ree is not None
         assert n.ree == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_eafb():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_eafbm.py` & `inewave-0.0.98/tests/nwlistop/test_eafbm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from inewave.nwlistop.eafbm import Eafbm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.eafbm import MockEafbm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_eafbm():
     m: MagicMock = mock_open(read_data="".join(MockEafbm))
     with patch("builtins.open", m):
         n = Eafbm.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 1995
-        assert n.valores.iloc[-1, -1] == 38424.0
+        assert n.valores.iloc[0, 0] == datetime(1995, 1, 1)
+        assert n.valores.iloc[-1, -1] == 28024.0
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_eafbm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_eafbsin.py` & `inewave-0.0.98/tests/nwlistop/test_eafbsin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.eafbsin import EafbSIN
+from inewave.nwlistop.eafbsin import Eafbsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.eafbsin import MockEafbSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_eafbsin():
     m: MagicMock = mock_open(read_data="".join(MockEafbSIN))
     with patch("builtins.open", m):
-        n = EafbSIN.read(ARQ_TESTE)
+        n = Eafbsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 64920.0
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 71599.0
 
 
 def test_atributos_nao_encontrados_eafbsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = EafbSIN.read(ARQ_TESTE)
+        n = Eafbsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_eafbsin():
     m: MagicMock = mock_open(read_data="".join(MockEafbSIN))
     with patch("builtins.open", m):
-        n1 = EafbSIN.read(ARQ_TESTE)
-        n2 = EafbSIN.read(ARQ_TESTE)
+        n1 = Eafbsin.read(ARQ_TESTE)
+        n2 = Eafbsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_eafm.py` & `inewave-0.0.98/tests/nwlistop/test_varmuh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.eafm import Eafm
+from inewave.nwlistop.varmuh import Varmuh
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.eafm import MockEafm
+from tests.mocks.arquivos.varmuh import MockVarmUH
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_eafm():
-    m: MagicMock = mock_open(read_data="".join(MockEafm))
+def test_atributos_encontrados_varmuh():
+    m: MagicMock = mock_open(read_data="".join(MockVarmUH))
     with patch("builtins.open", m):
-        n = Eafm.read(ARQ_TESTE)
+        n = Varmuh.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 17577.0
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_eafm():
+def test_atributos_nao_encontrados_varmuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Eafm.read(ARQ_TESTE)
+        n = Varmuh.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
-        assert n.submercado is None
 
 
-def test_eq_eafm():
-    m: MagicMock = mock_open(read_data="".join(MockEafm))
+def test_eq_varmuh():
+    m: MagicMock = mock_open(read_data="".join(MockVarmUH))
     with patch("builtins.open", m):
-        n1 = Eafm.read(ARQ_TESTE)
-        n2 = Eafm.read(ARQ_TESTE)
+        n1 = Varmuh.read(ARQ_TESTE)
+        n2 = Varmuh.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_earmf.py` & `inewave-0.0.98/tests/nwlistop/test_earmf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from inewave.nwlistop.earmf import Earmf
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.earmf import MockEarmf
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_earmf():
     m: MagicMock = mock_open(read_data="".join(MockEarmf))
     with patch("builtins.open", m):
         n = Earmf.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 20770.0
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 7639.0
         assert n.ree is not None
         assert n.ree == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_earmf():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_earmfm.py` & `inewave-0.0.98/tests/nwlistop/test_ghmaxm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.earmfm import Earmfm
+from inewave.nwlistop.ghmaxm import Ghmaxm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.earmfm import MockEarmfm
+from tests.mocks.arquivos.ghmaxm import MockGhmaxm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_earmfm():
-    m: MagicMock = mock_open(read_data="".join(MockEarmfm))
+def test_atributos_encontrados_ghmaxm():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxm))
     with patch("builtins.open", m):
-        n = Earmfm.read(ARQ_TESTE)
-        assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 122223.0
+        n = Ghmaxm.read(ARQ_TESTE)
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
+        assert n.valores is not None
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 54777.0
 
 
-def test_atributos_nao_encontrados_earmfm():
+def test_atributos_nao_encontrados_ghmaxm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Earmfm.read(ARQ_TESTE)
-        assert n.valores is None
+        n = Ghmaxm.read(ARQ_TESTE)
         assert n.submercado is None
+        assert n.valores is None
 
 
-def test_eq_earmfm():
-    m: MagicMock = mock_open(read_data="".join(MockEarmfm))
+def test_eq_ghmaxm():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxm))
     with patch("builtins.open", m):
-        n1 = Earmfm.read(ARQ_TESTE)
-        n2 = Earmfm.read(ARQ_TESTE)
+        n1 = Ghmaxm.read(ARQ_TESTE)
+        n2 = Ghmaxm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_earmfp.py` & `inewave-0.0.98/tests/nwlistop/test_perdfm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from inewave.nwlistop.earmfp import Earmfp
+from inewave.nwlistop.perdfm import Perdfm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.earmfp import MockEarmfp
+from tests.mocks.arquivos.perdfm import MockPerdfm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_earmfp():
-    m: MagicMock = mock_open(read_data="".join(MockEarmfp))
+def test_atributos_encontrados_perdfm():
+    m: MagicMock = mock_open(read_data="".join(MockPerdfm))
     with patch("builtins.open", m):
-        n = Earmfp.read(ARQ_TESTE)
+        n = Perdfm.read(ARQ_TESTE)
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 71.2
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 316.0
 
 
-def test_atributos_nao_encontrados_earmfp():
+def test_atributos_nao_encontrados_perdfm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Earmfp.read(ARQ_TESTE)
+        n = Perdfm.read(ARQ_TESTE)
+        assert n.submercado is None
         assert n.valores is None
-        assert n.ree is None
 
 
-def test_eq_earmfp():
-    m: MagicMock = mock_open(read_data="".join(MockEarmfp))
+def test_eq_perdfm():
+    m: MagicMock = mock_open(read_data="".join(MockPerdfm))
     with patch("builtins.open", m):
-        n1 = Earmfp.read(ARQ_TESTE)
-        n2 = Earmfp.read(ARQ_TESTE)
+        n1 = Perdfm.read(ARQ_TESTE)
+        n2 = Perdfm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_earmfpm.py` & `inewave-0.0.98/tests/nwlistop/test_perdf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from inewave.nwlistop.earmfpm import Earmfpm
+from inewave.nwlistop.perdf import Perdf
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.earmfpm import MockEarmfpm
+from tests.mocks.arquivos.perdf import MockPerdf
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_earmfpm():
-    m: MagicMock = mock_open(read_data="".join(MockEarmfpm))
+def test_atributos_encontrados_perdf():
+    m: MagicMock = mock_open(read_data="".join(MockPerdf))
     with patch("builtins.open", m):
-        n = Earmfpm.read(ARQ_TESTE)
+        n = Perdf.read(ARQ_TESTE)
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 1995
-        assert n.valores.iloc[-1, -1] == 63.0
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 315.0
 
 
-def test_atributos_nao_encontrados_earmfpm():
+def test_atributos_nao_encontrados_perdf():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Earmfpm.read(ARQ_TESTE)
+        n = Perdf.read(ARQ_TESTE)
+        assert n.ree is None
         assert n.valores is None
-        assert n.submercado is None
 
 
-def test_eq_earmfpm():
-    m: MagicMock = mock_open(read_data="".join(MockEarmfpm))
+def test_eq_perdf():
+    m: MagicMock = mock_open(read_data="".join(MockPerdf))
     with patch("builtins.open", m):
-        n1 = Earmfpm.read(ARQ_TESTE)
-        n2 = Earmfpm.read(ARQ_TESTE)
+        n1 = Perdf.read(ARQ_TESTE)
+        n2 = Perdf.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_earmfpsin.py` & `inewave-0.0.98/tests/nwlistop/test_ghmaxr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from inewave.nwlistop.earmfpsin import EarmfpSIN
+from inewave.nwlistop.ghmaxr import Ghmaxr
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.earmfpsin import MockEarmfpsin
+from tests.mocks.arquivos.ghmaxr import MockGhmaxr
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_earmfpsin():
-    m: MagicMock = mock_open(read_data="".join(MockEarmfpsin))
+def test_atributos_encontrados_ghmaxr():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxr))
     with patch("builtins.open", m):
-        n = EarmfpSIN.read(ARQ_TESTE)
+        n = Ghmaxr.read(ARQ_TESTE)
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 42.1
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 7434.9
 
 
-def test_atributos_nao_encontrados_earmfpsin():
+def test_atributos_nao_encontrados_ghmaxr():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = EarmfpSIN.read(ARQ_TESTE)
+        n = Ghmaxr.read(ARQ_TESTE)
+        assert n.ree is None
         assert n.valores is None
 
 
-def test_eq_earmfpsin():
-    m: MagicMock = mock_open(read_data="".join(MockEarmfpsin))
+def test_eq_ghmaxr():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxr))
     with patch("builtins.open", m):
-        n1 = EarmfpSIN.read(ARQ_TESTE)
-        n2 = EarmfpSIN.read(ARQ_TESTE)
+        n1 = Ghmaxr.read(ARQ_TESTE)
+        n2 = Ghmaxr.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_earmfsin.py` & `inewave-0.0.98/tests/nwlistop/test_earmfsin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.earmfsin import EarmfSIN
+from inewave.nwlistop.earmfsin import Earmfsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.earmfsin import MockEarmfSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_earmfsin():
     m: MagicMock = mock_open(read_data="".join(MockEarmfSIN))
     with patch("builtins.open", m):
-        n = EarmfSIN.read(ARQ_TESTE)
+        n = Earmfsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 177927.0
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 152505.0
 
 
 def test_atributos_nao_encontrados_earmfsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = EarmfSIN.read(ARQ_TESTE)
+        n = Earmfsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_earmfsin():
     m: MagicMock = mock_open(read_data="".join(MockEarmfSIN))
     with patch("builtins.open", m):
-        n1 = EarmfSIN.read(ARQ_TESTE)
-        n2 = EarmfSIN.read(ARQ_TESTE)
+        n1 = Earmfsin.read(ARQ_TESTE)
+        n2 = Earmfsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_evert.py` & `inewave-0.0.98/tests/nwlistop/test_evert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from inewave.nwlistop.evert import Evert
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.evert import MockEvert
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_evert():
     m: MagicMock = mock_open(read_data="".join(MockEvert))
     with patch("builtins.open", m):
         n = Evert.read(ARQ_TESTE)
         assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 24.0
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 37.0
 
 
 def test_atributos_nao_encontrados_evert():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         n = Evert.read(ARQ_TESTE)
         assert n.ree is None
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_evertm.py` & `inewave-0.0.98/tests/nwlistop/test_evertm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from inewave.nwlistop.evertm import Evertm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.evertm import MockEvertm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_evertm():
     m: MagicMock = mock_open(read_data="".join(MockEvertm))
     with patch("builtins.open", m):
         n = Evertm.read(ARQ_TESTE)
         assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 146.0
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 233.0
 
 
 def test_atributos_nao_encontrados_evertm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         n = Evertm.read(ARQ_TESTE)
         assert n.submercado is None
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_evertsin.py` & `inewave-0.0.98/tests/nwlistop/test_cterm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from inewave.nwlistop.evertsin import EvertSIN
+from inewave.nwlistop.cterm import Cterm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.evertsin import MockEvertSIN
+from tests.mocks.arquivos.cterm import MockCterm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_evertsin():
-    m: MagicMock = mock_open(read_data="".join(MockEvertSIN))
+def test_atributos_encontrados_cterm():
+    m: MagicMock = mock_open(read_data="".join(MockCterm))
     with patch("builtins.open", m):
-        n = EvertSIN.read(ARQ_TESTE)
+        n = Cterm.read(ARQ_TESTE)
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 146.0
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 872.41
 
 
-def test_atributos_nao_encontrados_evertsin():
+def test_atributos_nao_encontrados_cterm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = EvertSIN.read(ARQ_TESTE)
+        n = Cterm.read(ARQ_TESTE)
+        assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_evertsin():
-    m: MagicMock = mock_open(read_data="".join(MockEvertSIN))
+def test_eq_cterm():
+    m: MagicMock = mock_open(read_data="".join(MockCterm))
     with patch("builtins.open", m):
-        n1 = EvertSIN.read(ARQ_TESTE)
-        n2 = EvertSIN.read(ARQ_TESTE)
+        n1 = Cterm.read(ARQ_TESTE)
+        n2 = Cterm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_exces.py` & `inewave-0.0.98/tests/nwlistop/test_exces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from inewave.nwlistop.exces import Exces
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.exces import MockExces
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
@@ -11,15 +12,15 @@
 def test_atributos_encontrados_exces():
     m: MagicMock = mock_open(read_data="".join(MockExces))
     with patch("builtins.open", m):
         n = Exces.read(ARQ_TESTE)
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_exces():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         n = Exces.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_excessin.py` & `inewave-0.0.98/tests/nwlistop/test_invadem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.excessin import ExcesSIN
+from inewave.nwlistop.invadem import Invadem
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.excessin import MockExcesSIN
+from tests.mocks.arquivos.invadem import MockInvadem
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_excessin():
-    m: MagicMock = mock_open(read_data="".join(MockExcesSIN))
+def test_atributos_encontrados_invadem():
+    m: MagicMock = mock_open(read_data="".join(MockInvadem))
     with patch("builtins.open", m):
-        n = ExcesSIN.read(ARQ_TESTE)
+        n = Invadem.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_excessin():
+def test_atributos_nao_encontrados_invadem():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = ExcesSIN.read(ARQ_TESTE)
+        n = Invadem.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_excessin():
-    m: MagicMock = mock_open(read_data="".join(MockExcesSIN))
+def test_eq_invadem():
+    m: MagicMock = mock_open(read_data="".join(MockInvadem))
     with patch("builtins.open", m):
-        n1 = ExcesSIN.read(ARQ_TESTE)
-        n2 = ExcesSIN.read(ARQ_TESTE)
+        n1 = Invadem.read(ARQ_TESTE)
+        n2 = Invadem.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_fteolm.py` & `inewave-0.0.98/tests/nwlistop/test_fteolsin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-from inewave.nwlistop.fteolm import Fteolm
+from inewave.nwlistop.fteolsin import Fteolsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.fteolm import MockFteolm
+from tests.mocks.arquivos.fteolsin import MockFteolSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_fteolm():
-    m: MagicMock = mock_open(read_data="".join(MockFteolm))
+def test_atributos_encontrados_fteolsin():
+    m: MagicMock = mock_open(read_data="".join(MockFteolSIN))
     with patch("builtins.open", m):
-        n = Fteolm.read(ARQ_TESTE)
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        n = Fteolsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_fteolm():
+def test_atributos_nao_encontrados_fteolsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Fteolm.read(ARQ_TESTE)
-        assert n.submercado is None
+        n = Fteolsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_fteolm():
-    m: MagicMock = mock_open(read_data="".join(MockFteolm))
+def test_eq_fteolsin():
+    m: MagicMock = mock_open(read_data="".join(MockFteolSIN))
     with patch("builtins.open", m):
-        n1 = Fteolm.read(ARQ_TESTE)
-        n2 = Fteolm.read(ARQ_TESTE)
+        n1 = Fteolsin.read(ARQ_TESTE)
+        n2 = Fteolsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_fteolsin.py` & `inewave-0.0.98/tests/nwlistop/test_vevminsin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.fteolsin import FteolSIN
+from inewave.nwlistop.vevminsin import Vevminsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.fteolsin import MockFteolSIN
+from tests.mocks.arquivos.vevminsin import MockVevminSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_fteolsin():
-    m: MagicMock = mock_open(read_data="".join(MockFteolSIN))
+def test_atributos_encontrados_vevminsin():
+    m: MagicMock = mock_open(read_data="".join(MockVevminSIN))
     with patch("builtins.open", m):
-        n = FteolSIN.read(ARQ_TESTE)
+        n = Vevminsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_fteolsin():
+def test_atributos_nao_encontrados_vevminsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = FteolSIN.read(ARQ_TESTE)
+        n = Vevminsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_fteolsin():
-    m: MagicMock = mock_open(read_data="".join(MockFteolSIN))
+def test_eq_vevminsin():
+    m: MagicMock = mock_open(read_data="".join(MockVevminSIN))
     with patch("builtins.open", m):
-        n1 = FteolSIN.read(ARQ_TESTE)
-        n2 = FteolSIN.read(ARQ_TESTE)
+        n1 = Vevminsin.read(ARQ_TESTE)
+        n2 = Vevminsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_geol.py` & `inewave-0.0.98/tests/nwlistop/test_ctermsin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-from inewave.nwlistop.geol import Geol
+from inewave.nwlistop.ctermsin import Ctermsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.geol import MockGeol
+from tests.mocks.arquivos.ctermsin import MockCtermSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_geol():
-    m: MagicMock = mock_open(read_data="".join(MockGeol))
+def test_atributos_encontrados_ctermsin():
+    m: MagicMock = mock_open(read_data="".join(MockCtermSIN))
     with patch("builtins.open", m):
-        n = Geol.read(ARQ_TESTE)
-        assert n.usina is not None
-        # assert n.pee == "cluster_NE_1"
+        n = Ctermsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 2652.7
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 1581.41
 
 
-def test_atributos_nao_encontrados_geol():
+def test_atributos_nao_encontrados_ctermsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Geol.read(ARQ_TESTE)
-        assert n.usina is None
+        n = Ctermsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_geol():
-    m: MagicMock = mock_open(read_data="".join(MockGeol))
+def test_eq_ctermsin():
+    m: MagicMock = mock_open(read_data="".join(MockCtermSIN))
     with patch("builtins.open", m):
-        n1 = Geol.read(ARQ_TESTE)
-        n2 = Geol.read(ARQ_TESTE)
+        n1 = Ctermsin.read(ARQ_TESTE)
+        n2 = Ctermsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_geolm.py` & `inewave-0.0.98/tests/nwlistop/test_vghminm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.geolm import Geolm
+from inewave.nwlistop.vghminm import Vghminm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.geolm import MockGeolm
+from tests.mocks.arquivos.vghminm import MockVghminm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_geolm():
-    m: MagicMock = mock_open(read_data="".join(MockGeolm))
+def test_atributos_encontrados_vghminm():
+    m: MagicMock = mock_open(read_data="".join(MockVghminm))
     with patch("builtins.open", m):
-        n = Geolm.read(ARQ_TESTE)
+        n = Vghminm.read(ARQ_TESTE)
         assert n.submercado is not None
-        assert n.submercado == "NORDESTE"
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 5850.4
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_geolm():
+def test_atributos_nao_encontrados_vghminm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Geolm.read(ARQ_TESTE)
+        n = Vghminm.read(ARQ_TESTE)
         assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_geolm():
-    m: MagicMock = mock_open(read_data="".join(MockGeolm))
+def test_eq_vghminm():
+    m: MagicMock = mock_open(read_data="".join(MockVghminm))
     with patch("builtins.open", m):
-        n1 = Geolm.read(ARQ_TESTE)
-        n2 = Geolm.read(ARQ_TESTE)
+        n1 = Vghminm.read(ARQ_TESTE)
+        n2 = Vghminm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_geolsin.py` & `inewave-0.0.98/tests/nwlistop/test_geolsin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.geolsin import GeolSIN
+from inewave.nwlistop.geolsin import Geolsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.geolsin import MockGeolSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_geolsin():
     m: MagicMock = mock_open(read_data="".join(MockGeolSIN))
     with patch("builtins.open", m):
-        n = GeolSIN.read(ARQ_TESTE)
+        n = Geolsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 6574.3
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 6721.6
 
 
 def test_atributos_nao_encontrados_geolsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GeolSIN.read(ARQ_TESTE)
+        n = Geolsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_geolsin():
     m: MagicMock = mock_open(read_data="".join(MockGeolSIN))
     with patch("builtins.open", m):
-        n1 = GeolSIN.read(ARQ_TESTE)
-        n2 = GeolSIN.read(ARQ_TESTE)
+        n1 = Geolsin.read(ARQ_TESTE)
+        n2 = Geolsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_ghiduh.py` & `inewave-0.0.98/tests/nwlistop/test_vevmin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.ghiduh import GhidUH
+from inewave.nwlistop.vevmin import Vevmin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghiduh import MockGhidUH
+from tests.mocks.arquivos.vevmin import MockVevmin
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_ghiduh():
-    m: MagicMock = mock_open(read_data="".join(MockGhidUH))
+def test_atributos_encontrados_vevmin():
+    m: MagicMock = mock_open(read_data="".join(MockVevmin))
     with patch("builtins.open", m):
-        n = GhidUH.read(ARQ_TESTE)
-        assert n.usina is not None
-        assert n.usina == "CAMARGOS"
+        n = Vevmin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 8.21
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_ghiduh():
+def test_atributos_nao_encontrados_vevmin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GhidUH.read(ARQ_TESTE)
-        assert n.usina is None
+        n = Vevmin.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.ree is None
 
 
-def test_eq_ghiduh():
-    m: MagicMock = mock_open(read_data="".join(MockGhidUH))
+def test_eq_vevmin():
+    m: MagicMock = mock_open(read_data="".join(MockVevmin))
     with patch("builtins.open", m):
-        n1 = GhidUH.read(ARQ_TESTE)
-        n2 = GhidUH.read(ARQ_TESTE)
+        n1 = Vevmin.read(ARQ_TESTE)
+        n2 = Vevmin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_ghmax.py` & `inewave-0.0.98/tests/nwlistop/test_ghmax.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from inewave.nwlistop.ghmax import Ghmax
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.ghmax import MockGhmax
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
@@ -11,16 +12,16 @@
 def test_atributos_encontrados_ghmax():
     m: MagicMock = mock_open(read_data="".join(MockGhmax))
     with patch("builtins.open", m):
         n = Ghmax.read(ARQ_TESTE)
         assert n.ree is not None
         assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 7841.2
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 7562.6
 
 
 def test_atributos_nao_encontrados_ghmax():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         n = Ghmax.read(ARQ_TESTE)
         assert n.ree is None
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_ghmaxm.py` & `inewave-0.0.98/tests/nwlistop/test_dlppdfmaxs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-from inewave.nwlistop.ghmaxm import Ghmaxm
+from inewave.nwlistop.dlppdfmaxs import Dlppdfmaxs
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghmaxm import MockGhmaxm
+from tests.mocks.arquivos.dlppdfmaxs import MockDLPPdfmaxs
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_ghmaxm():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxm))
+def test_atributos_encontrados_dlppdfmaxs():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxs))
     with patch("builtins.open", m):
-        n = Ghmaxm.read(ARQ_TESTE)
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        n = Dlppdfmaxs.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 54602.6
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_ghmaxm():
+def test_atributos_nao_encontrados_dlppdfmaxs():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Ghmaxm.read(ARQ_TESTE)
-        assert n.submercado is None
+        n = Dlppdfmaxs.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_ghmaxm():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxm))
+def test_eq_dlppdfmaxs():
+    m: MagicMock = mock_open(read_data="".join(MockDLPPdfmaxs))
     with patch("builtins.open", m):
-        n1 = Ghmaxm.read(ARQ_TESTE)
-        n2 = Ghmaxm.read(ARQ_TESTE)
+        n1 = Dlppdfmaxs.read(ARQ_TESTE)
+        n2 = Dlppdfmaxs.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_ghmaxmr.py` & `inewave-0.0.98/tests/nwlistop/test_qincruh.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.ghmaxmr import Ghmaxmr
+from inewave.nwlistop.qincruh import Qincruh
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghmaxmr import MockGhmaxmr
+from tests.mocks.arquivos.qincruh import MockQincrUH
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_ghmaxmr():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxmr))
+def test_atributos_encontrados_qincruh():
+    m: MagicMock = mock_open(read_data="".join(MockQincrUH))
     with patch("builtins.open", m):
-        n = Ghmaxmr.read(ARQ_TESTE)
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        n = Qincruh.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 54233.6
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_ghmaxmr():
+def test_atributos_nao_encontrados_qincruh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Ghmaxmr.read(ARQ_TESTE)
-        assert n.submercado is None
+        n = Qincruh.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_ghmaxmr():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxmr))
+def test_eq_qincruh():
+    m: MagicMock = mock_open(read_data="".join(MockQincrUH))
     with patch("builtins.open", m):
-        n1 = Ghmaxmr.read(ARQ_TESTE)
-        n2 = Ghmaxmr.read(ARQ_TESTE)
+        n1 = Qincruh.read(ARQ_TESTE)
+        n2 = Qincruh.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_ghmaxr.py` & `inewave-0.0.98/tests/nwlistop/test_ghtot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.ghmaxr import Ghmaxr
+from inewave.nwlistop.ghtot import Ghtot
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghmaxr import MockGhmaxr
+from tests.mocks.arquivos.ghtot import MockGhtot
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_ghmaxr():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxr))
+def test_atributos_encontrados_ghtot():
+    m: MagicMock = mock_open(read_data="".join(MockGhtot))
     with patch("builtins.open", m):
-        n = Ghmaxr.read(ARQ_TESTE)
+        n = Ghtot.read(ARQ_TESTE)
         assert n.ree is not None
         assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 7686.3
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 2420.5
 
 
-def test_atributos_nao_encontrados_ghmaxr():
+def test_atributos_nao_encontrados_ghtot():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Ghmaxr.read(ARQ_TESTE)
+        n = Ghtot.read(ARQ_TESTE)
         assert n.ree is None
         assert n.valores is None
 
 
-def test_eq_ghmaxr():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxr))
+def test_eq_ghtot():
+    m: MagicMock = mock_open(read_data="".join(MockGhtot))
     with patch("builtins.open", m):
-        n1 = Ghmaxr.read(ARQ_TESTE)
-        n2 = Ghmaxr.read(ARQ_TESTE)
+        n1 = Ghtot.read(ARQ_TESTE)
+        n2 = Ghtot.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_ghmaxrsin.py` & `inewave-0.0.98/tests/nwlistop/test_ghmaxrsin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.ghmaxrsin import GhmaxrSIN
+from inewave.nwlistop.ghmaxrsin import Ghmaxrsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.ghmaxrsin import MockGhmaxrSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_ghmaxrsin():
     m: MagicMock = mock_open(read_data="".join(MockGhmaxrSIN))
     with patch("builtins.open", m):
-        n = GhmaxrSIN.read(ARQ_TESTE)
+        n = Ghmaxrsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 94172.9
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 93660
 
 
 def test_atributos_nao_encontrados_ghmaxrsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GhmaxrSIN.read(ARQ_TESTE)
+        n = Ghmaxrsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_ghmaxrsin():
     m: MagicMock = mock_open(read_data="".join(MockGhmaxrSIN))
     with patch("builtins.open", m):
-        n1 = GhmaxrSIN.read(ARQ_TESTE)
-        n2 = GhmaxrSIN.read(ARQ_TESTE)
+        n1 = Ghmaxrsin.read(ARQ_TESTE)
+        n2 = Ghmaxrsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_ghmaxsin.py` & `inewave-0.0.98/tests/nwlistop/test_ghmaxmr.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from inewave.nwlistop.ghmaxsin import GhmaxSIN
+from inewave.nwlistop.ghmaxmr import Ghmaxmr
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghmaxsin import MockGhmaxSIN
+from tests.mocks.arquivos.ghmaxmr import MockGhmaxmr
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_ghmaxsin():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxSIN))
+def test_atributos_encontrados_ghmaxmr():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxmr))
     with patch("builtins.open", m):
-        n = GhmaxSIN.read(ARQ_TESTE)
+        n = Ghmaxmr.read(ARQ_TESTE)
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 97716.9
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 54649.3
 
 
-def test_atributos_nao_encontrados_ghmaxsin():
+def test_atributos_nao_encontrados_ghmaxmr():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GhmaxSIN.read(ARQ_TESTE)
+        n = Ghmaxmr.read(ARQ_TESTE)
+        assert n.submercado is None
         assert n.valores is None
 
 
-def test_eq_ghmaxsin():
-    m: MagicMock = mock_open(read_data="".join(MockGhmaxSIN))
+def test_eq_ghmaxmr():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxmr))
     with patch("builtins.open", m):
-        n1 = GhmaxSIN.read(ARQ_TESTE)
-        n2 = GhmaxSIN.read(ARQ_TESTE)
+        n1 = Ghmaxmr.read(ARQ_TESTE)
+        n2 = Ghmaxmr.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_ghtot.py` & `inewave-0.0.98/tests/nwlistop/test_vghminsin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-from inewave.nwlistop.ghtot import Ghtot
+from inewave.nwlistop.vghminsin import Vghminsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghtot import MockGhtot
+from tests.mocks.arquivos.vghminsin import MockVghminSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_ghtot():
-    m: MagicMock = mock_open(read_data="".join(MockGhtot))
+def test_atributos_encontrados_vghminsin():
+    m: MagicMock = mock_open(read_data="".join(MockVghminSIN))
     with patch("builtins.open", m):
-        n = Ghtot.read(ARQ_TESTE)
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        n = Vghminsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 2578.7
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_ghtot():
+def test_atributos_nao_encontrados_vghminsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Ghtot.read(ARQ_TESTE)
-        assert n.ree is None
+        n = Vghminsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_ghtot():
-    m: MagicMock = mock_open(read_data="".join(MockGhtot))
+def test_eq_vghminsin():
+    m: MagicMock = mock_open(read_data="".join(MockVghminSIN))
     with patch("builtins.open", m):
-        n1 = Ghtot.read(ARQ_TESTE)
-        n2 = Ghtot.read(ARQ_TESTE)
+        n1 = Vghminsin.read(ARQ_TESTE)
+        n2 = Vghminsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_ghtotm.py` & `inewave-0.0.98/tests/nwlistop/test_ghtotm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from inewave.nwlistop.ghtotm import Ghtotm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.ghtotm import MockGhtotm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
@@ -11,16 +12,16 @@
 def test_atributos_encontrados_ghtotm():
     m: MagicMock = mock_open(read_data="".join(MockGhtotm))
     with patch("builtins.open", m):
         n = Ghtotm.read(ARQ_TESTE)
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 24494.9
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 36951.5
 
 
 def test_atributos_nao_encontrados_ghtotm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         n = Ghtotm.read(ARQ_TESTE)
         assert n.submercado is None
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_ghtotsin.py` & `inewave-0.0.98/tests/nwlistop/test_vagua.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from inewave.nwlistop.ghtotsin import GhtotSIN
+from inewave.nwlistop.vagua import Vagua
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.ghtotsin import MockGhtotsin
+from tests.mocks.arquivos.vagua import MockVagua
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_ghtotsin():
-    m: MagicMock = mock_open(read_data="".join(MockGhtotsin))
+def test_atributos_encontrados_vagua():
+    m: MagicMock = mock_open(read_data="".join(MockVagua))
     with patch("builtins.open", m):
-        n = GhtotSIN.read(ARQ_TESTE)
+        n = Vagua.read(ARQ_TESTE)
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 46994.0
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == -0.09
 
 
-def test_atributos_nao_encontrados_ghtotsin():
+def test_atributos_nao_encontrados_vagua():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GhtotSIN.read(ARQ_TESTE)
+        n = Vagua.read(ARQ_TESTE)
+        assert n.ree is None
         assert n.valores is None
 
 
-def test_eq_ghtotsin():
-    m: MagicMock = mock_open(read_data="".join(MockGhtotsin))
+def test_eq_vagua():
+    m: MagicMock = mock_open(read_data="".join(MockVagua))
     with patch("builtins.open", m):
-        n1 = GhtotSIN.read(ARQ_TESTE)
-        n2 = GhtotSIN.read(ARQ_TESTE)
+        n1 = Vagua.read(ARQ_TESTE)
+        n2 = Vagua.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_gtert.py` & `inewave-0.0.98/tests/nwlistop/test_dtbmin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.gtert import Gtert
+from inewave.nwlistop.dtbmin import Dtbmin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.gtert import MockGtert
+from tests.mocks.arquivos.dtbmin import MockDtbmin
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_gtert():
-    m: MagicMock = mock_open(read_data="".join(MockGtert))
+def test_atributos_encontrados_dtbmin():
+    m: MagicMock = mock_open(read_data="".join(MockDtbmin))
     with patch("builtins.open", m):
-        n = Gtert.read(ARQ_TESTE)
-        assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        n = Dtbmin.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2023
-        assert n.valores.iloc[-1, -1] == 549.2
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_gtert():
+def test_atributos_nao_encontrados_dtbmin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Gtert.read(ARQ_TESTE)
-        assert n.submercado is None
+        n = Dtbmin.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_gtert():
-    m: MagicMock = mock_open(read_data="".join(MockGtert))
+def test_eq_dtbmin():
+    m: MagicMock = mock_open(read_data="".join(MockDtbmin))
     with patch("builtins.open", m):
-        n1 = Gtert.read(ARQ_TESTE)
-        n2 = Gtert.read(ARQ_TESTE)
+        n1 = Dtbmin.read(ARQ_TESTE)
+        n2 = Dtbmin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_gttot.py` & `inewave-0.0.98/tests/nwlistop/test_verturbm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.gttot import Gttot
+from inewave.nwlistop.verturbm import Verturbm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.gttot import MockGttot
+from tests.mocks.arquivos.verturbm import MockVerturbm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_gttot():
-    m: MagicMock = mock_open(read_data="".join(MockGttot))
+def test_atributos_encontrados_verturbm():
+    m: MagicMock = mock_open(read_data="".join(MockVerturbm))
     with patch("builtins.open", m):
-        n = Gttot.read(ARQ_TESTE)
+        n = Verturbm.read(ARQ_TESTE)
+        assert n.valores is not None
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
-        assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 2710.5
 
 
-def test_atributos_nao_encontrados_gttot():
+def test_atributos_nao_encontrados_verturbm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Gttot.read(ARQ_TESTE)
-        assert n.submercado is None
+        n = Verturbm.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.submercado is None
 
 
-def test_eq_gttot():
-    m: MagicMock = mock_open(read_data="".join(MockGttot))
+def test_eq_verturbm():
+    m: MagicMock = mock_open(read_data="".join(MockVerturbm))
     with patch("builtins.open", m):
-        n1 = Gttot.read(ARQ_TESTE)
-        n2 = Gttot.read(ARQ_TESTE)
+        n1 = Verturbm.read(ARQ_TESTE)
+        n2 = Verturbm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_gttotsin.py` & `inewave-0.0.98/tests/nwlistop/test_gttotsin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.gttotsin import GttotSIN
+from inewave.nwlistop.gttotsin import Gttotsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.gttotsin import MockGttotsin
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_gttotsin():
     m: MagicMock = mock_open(read_data="".join(MockGttotsin))
     with patch("builtins.open", m):
-        n = GttotSIN.read(ARQ_TESTE)
+        n = Gttotsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 5106.0
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 4811.2
 
 
 def test_atributos_nao_encontrados_gttotsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = GttotSIN.read(ARQ_TESTE)
+        n = Gttotsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_gttotsin():
     m: MagicMock = mock_open(read_data="".join(MockGttotsin))
     with patch("builtins.open", m):
-        n1 = GttotSIN.read(ARQ_TESTE)
-        n2 = GttotSIN.read(ARQ_TESTE)
+        n1 = Gttotsin.read(ARQ_TESTE)
+        n2 = Gttotsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_intercambio.py` & `inewave-0.0.98/tests/nwlistop/test_cdefsin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-from inewave.nwlistop.intercambio import Intercambio
+from inewave.nwlistop.cdefsin import Cdefsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.intercambio import MockIntercambio
+from tests.mocks.arquivos.cdefsin import MockCdefSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_intercambio():
-    m: MagicMock = mock_open(read_data="".join(MockIntercambio))
+def test_atributos_encontrados_cdefsin():
+    m: MagicMock = mock_open(read_data="".join(MockCdefSIN))
     with patch("builtins.open", m):
-        n = Intercambio.read(ARQ_TESTE)
-        assert n.submercado_de is not None
-        assert n.submercado_de == "SUDESTE"
-        assert n.submercado_para == "SUL"
+        n = Cdefsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -2] == 2835.2
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_intercambio():
+def test_atributos_nao_encontrados_cdefsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Intercambio.read(ARQ_TESTE)
-        assert n.submercado_de is None
-        assert n.submercado_para is None
+        n = Cdefsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_intercambio():
-    m: MagicMock = mock_open(read_data="".join(MockIntercambio))
+def test_eq_cdefsin():
+    m: MagicMock = mock_open(read_data="".join(MockCdefSIN))
     with patch("builtins.open", m):
-        n1 = Intercambio.read(ARQ_TESTE)
-        n2 = Intercambio.read(ARQ_TESTE)
+        n1 = Cdefsin.read(ARQ_TESTE)
+        n2 = Cdefsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_invade.py` & `inewave-0.0.98/tests/nwlistop/test_vghmin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from inewave.nwlistop.invade import Invade
+from inewave.nwlistop.vghmin import Vghmin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.invade import MockInvade
+from tests.mocks.arquivos.vghmin import MockVghmin
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_invade():
-    m: MagicMock = mock_open(read_data="".join(MockInvade))
+def test_atributos_encontrados_vghmin():
+    m: MagicMock = mock_open(read_data="".join(MockVghmin))
     with patch("builtins.open", m):
-        n = Invade.read(ARQ_TESTE)
+        n = Vghmin.read(ARQ_TESTE)
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_invade():
+def test_atributos_nao_encontrados_vghmin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Invade.read(ARQ_TESTE)
+        n = Vghmin.read(ARQ_TESTE)
+        assert n.ree is None
         assert n.valores is None
 
 
-def test_eq_invade():
-    m: MagicMock = mock_open(read_data="".join(MockInvade))
+def test_eq_vghmin():
+    m: MagicMock = mock_open(read_data="".join(MockVghmin))
     with patch("builtins.open", m):
-        n1 = Invade.read(ARQ_TESTE)
-        n2 = Invade.read(ARQ_TESTE)
+        n1 = Vghmin.read(ARQ_TESTE)
+        n2 = Vghmin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_invadem.py` & `inewave-0.0.98/tests/nwlistop/test_invade.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.invadem import Invadem
+from inewave.nwlistop.invade import Invade
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.invadem import MockInvadem
+from tests.mocks.arquivos.invade import MockInvade
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_invadem():
-    m: MagicMock = mock_open(read_data="".join(MockInvadem))
+def test_atributos_encontrados_invade():
+    m: MagicMock = mock_open(read_data="".join(MockInvade))
     with patch("builtins.open", m):
-        n = Invadem.read(ARQ_TESTE)
+        n = Invade.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_invadem():
+def test_atributos_nao_encontrados_invade():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Invadem.read(ARQ_TESTE)
+        n = Invade.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_invadem():
-    m: MagicMock = mock_open(read_data="".join(MockInvadem))
+def test_eq_invade():
+    m: MagicMock = mock_open(read_data="".join(MockInvade))
     with patch("builtins.open", m):
-        n1 = Invadem.read(ARQ_TESTE)
-        n2 = Invadem.read(ARQ_TESTE)
+        n1 = Invade.read(ARQ_TESTE)
+        n2 = Invade.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_mercl.py` & `inewave-0.0.98/tests/nwlistop/test_mercl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from inewave.nwlistop.mercl import Mercl
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.mercl import MockMercl
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_mercl():
     m: MagicMock = mock_open(read_data="".join(MockMercl))
     with patch("builtins.open", m):
         n = Mercl.read(ARQ_TESTE)
         assert n.valores is not None
         print(n.valores)
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -2] == 37783.0
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 37783.0
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
 def test_atributos_nao_encontrados_mercl():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_merclsin.py` & `inewave-0.0.98/tests/nwlistop/test_merclsin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.merclsin import MerclSIN
+from inewave.nwlistop.merclsin import Merclsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.merclsin import MockMerclSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_merclsin():
     m: MagicMock = mock_open(read_data="".join(MockMerclSIN))
     with patch("builtins.open", m):
-        n = MerclSIN.read(ARQ_TESTE)
+        n = Merclsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -2] == 56819.0
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 56819.0
 
 
 def test_atributos_nao_encontrados_merclsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = MerclSIN.read(ARQ_TESTE)
+        n = Merclsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
 def test_eq_merclsin():
     m: MagicMock = mock_open(read_data="".join(MockMerclSIN))
     with patch("builtins.open", m):
-        n1 = MerclSIN.read(ARQ_TESTE)
-        n2 = MerclSIN.read(ARQ_TESTE)
+        n1 = Merclsin.read(ARQ_TESTE)
+        n2 = Merclsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_nwlistopdat.py` & `inewave-0.0.98/tests/nwlistop/test_nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.97/tests/nwlistop/test_perdf.py` & `inewave-0.0.98/tests/nwlistop/test_vertuh.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from inewave.nwlistop.perdf import Perdf
+from inewave.nwlistop.vertuh import Vertuh
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.perdf import MockPerdf
+from tests.mocks.arquivos.vertuh import MockVertuh
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_perdf():
-    m: MagicMock = mock_open(read_data="".join(MockPerdf))
+def test_atributos_encontrados_vertuh():
+    m: MagicMock = mock_open(read_data="".join(MockVertuh))
     with patch("builtins.open", m):
-        n = Perdf.read(ARQ_TESTE)
-        assert n.ree == "SUDESTE"
+        n = Vertuh.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "ESPORA"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 230.0
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_perdf():
+def test_atributos_nao_encontrados_vertuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Perdf.read(ARQ_TESTE)
-        assert n.ree is None
+        n = Vertuh.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_perdf():
-    m: MagicMock = mock_open(read_data="".join(MockPerdf))
+def test_eq_vertuh():
+    m: MagicMock = mock_open(read_data="".join(MockVertuh))
     with patch("builtins.open", m):
-        n1 = Perdf.read(ARQ_TESTE)
-        n2 = Perdf.read(ARQ_TESTE)
+        n1 = Vertuh.read(ARQ_TESTE)
+        n2 = Vertuh.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_perdfm.py` & `inewave-0.0.98/tests/nwlistop/test_perdfsin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-from inewave.nwlistop.perdfm import Perdfm
+from inewave.nwlistop.perdfsin import Perdfsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.perdfm import MockPerdfm
+from tests.mocks.arquivos.perdfsin import MockPerdfSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_perdfm():
-    m: MagicMock = mock_open(read_data="".join(MockPerdfm))
+def test_atributos_encontrados_perdfsin():
+    m: MagicMock = mock_open(read_data="".join(MockPerdfSIN))
     with patch("builtins.open", m):
-        n = Perdfm.read(ARQ_TESTE)
-        assert n.submercado == "SUDESTE"
+        n = Perdfsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 231.0
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 674.0
 
 
-def test_atributos_nao_encontrados_perdfm():
+def test_atributos_nao_encontrados_perdfsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Perdfm.read(ARQ_TESTE)
-        assert n.submercado is None
+        n = Perdfsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_perdfm():
-    m: MagicMock = mock_open(read_data="".join(MockPerdfm))
+def test_eq_perdfsin():
+    m: MagicMock = mock_open(read_data="".join(MockPerdfSIN))
     with patch("builtins.open", m):
-        n1 = Perdfm.read(ARQ_TESTE)
-        n2 = Perdfm.read(ARQ_TESTE)
+        n1 = Perdfsin.read(ARQ_TESTE)
+        n2 = Perdfsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_perdfsin.py` & `inewave-0.0.98/tests/nwlistop/test_verturbsin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.perdfsin import PerdfSIN
+from inewave.nwlistop.verturbsin import Verturbsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.perdfsin import MockPerdfSIN
+from tests.mocks.arquivos.verturbsin import MockVerturbSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_perdfsin():
-    m: MagicMock = mock_open(read_data="".join(MockPerdfSIN))
+def test_atributos_encontrados_verturbsin():
+    m: MagicMock = mock_open(read_data="".join(MockVerturbSIN))
     with patch("builtins.open", m):
-        n = PerdfSIN.read(ARQ_TESTE)
+        n = Verturbsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 438.0
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_perdfsin():
+def test_atributos_nao_encontrados_verturbsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = PerdfSIN.read(ARQ_TESTE)
+        n = Verturbsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_perdfsin():
-    m: MagicMock = mock_open(read_data="".join(MockPerdfSIN))
+def test_eq_verturbsin():
+    m: MagicMock = mock_open(read_data="".join(MockVerturbSIN))
     with patch("builtins.open", m):
-        n1 = PerdfSIN.read(ARQ_TESTE)
-        n2 = PerdfSIN.read(ARQ_TESTE)
+        n1 = Verturbsin.read(ARQ_TESTE)
+        n2 = Verturbsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_qafluh.py` & `inewave-0.0.98/tests/nwlistop/test_qafluh.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.qafluh import QaflUH
+from inewave.nwlistop.qafluh import Qafluh
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.qafluh import MockQaflUH
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_qafluh():
     m: MagicMock = mock_open(read_data="".join(MockQaflUH))
     with patch("builtins.open", m):
-        n = QaflUH.read(ARQ_TESTE)
+        n = Qafluh.read(ARQ_TESTE)
         assert n.usina is not None
         assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 105.02
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_qafluh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = QaflUH.read(ARQ_TESTE)
+        n = Qafluh.read(ARQ_TESTE)
         assert n.usina is None
         assert n.valores is None
 
 
 def test_eq_qafluh():
     m: MagicMock = mock_open(read_data="".join(MockQaflUH))
     with patch("builtins.open", m):
-        n1 = QaflUH.read(ARQ_TESTE)
-        n2 = QaflUH.read(ARQ_TESTE)
+        n1 = Qafluh.read(ARQ_TESTE)
+        n2 = Qafluh.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_qincruh.py` & `inewave-0.0.98/tests/nwlistop/test_rhslppdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.qincruh import QincrUH
+from inewave.nwlistop.rhslppdf import Rhslppdf
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.qincruh import MockQincrUH
+from tests.mocks.arquivos.rhslppdf import MockRHSLPPdf
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_qincruh():
-    m: MagicMock = mock_open(read_data="".join(MockQincrUH))
+def test_atributos_encontrados_rhslppdf():
+    m: MagicMock = mock_open(read_data="".join(MockRHSLPPdf))
     with patch("builtins.open", m):
-        n = QincrUH.read(ARQ_TESTE)
-        assert n.usina is not None
-        assert n.usina == "CAMARGOS"
+        n = Rhslppdf.read(ARQ_TESTE)
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 105.02
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_qincruh():
+def test_atributos_nao_encontrados_rhslppdf():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = QincrUH.read(ARQ_TESTE)
-        assert n.usina is None
+        n = Rhslppdf.read(ARQ_TESTE)
+        assert n.ree is None
         assert n.valores is None
 
 
-def test_eq_qincruh():
-    m: MagicMock = mock_open(read_data="".join(MockQincrUH))
+def test_eq_rhslppdf():
+    m: MagicMock = mock_open(read_data="".join(MockRHSLPPdf))
     with patch("builtins.open", m):
-        n1 = QincrUH.read(ARQ_TESTE)
-        n2 = QincrUH.read(ARQ_TESTE)
+        n1 = Rhslppdf.read(ARQ_TESTE)
+        n2 = Rhslppdf.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_rhslppdf.py` & `inewave-0.0.98/tests/nwlistop/test_excessin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-from inewave.nwlistop.rhslppdf import RHSLPPdf
+from inewave.nwlistop.excessin import Excessin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.rhslppdf import MockRHSLPPdf
+from tests.mocks.arquivos.excessin import MockExcesSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_rhslppdf():
-    m: MagicMock = mock_open(read_data="".join(MockRHSLPPdf))
+def test_atributos_encontrados_excessin():
+    m: MagicMock = mock_open(read_data="".join(MockExcesSIN))
     with patch("builtins.open", m):
-        n = RHSLPPdf.read(ARQ_TESTE)
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        n = Excessin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_rhslppdf():
+def test_atributos_nao_encontrados_excessin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = RHSLPPdf.read(ARQ_TESTE)
-        assert n.ree is None
+        n = Excessin.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_rhslppdf():
-    m: MagicMock = mock_open(read_data="".join(MockRHSLPPdf))
+def test_eq_excessin():
+    m: MagicMock = mock_open(read_data="".join(MockExcesSIN))
     with patch("builtins.open", m):
-        n1 = RHSLPPdf.read(ARQ_TESTE)
-        n2 = RHSLPPdf.read(ARQ_TESTE)
+        n1 = Excessin.read(ARQ_TESTE)
+        n2 = Excessin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_rhslpptb.py` & `inewave-0.0.98/tests/nwlistop/test_rhslpptb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.rhslpptb import RHSLPPtb
+from inewave.nwlistop.rhslpptb import Rhslpptb
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.rhslpptb import MockRHSLPPtb
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_rhslpptb():
     m: MagicMock = mock_open(read_data="".join(MockRHSLPPtb))
     with patch("builtins.open", m):
-        n = RHSLPPtb.read(ARQ_TESTE)
+        n = Rhslpptb.read(ARQ_TESTE)
         assert n.ree is not None
         assert n.ree == "SUDESTE"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_rhslpptb():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = RHSLPPtb.read(ARQ_TESTE)
+        n = Rhslpptb.read(ARQ_TESTE)
         assert n.ree is None
         assert n.valores is None
 
 
 def test_eq_rhslpptb():
     m: MagicMock = mock_open(read_data="".join(MockRHSLPPtb))
     with patch("builtins.open", m):
-        n1 = RHSLPPtb.read(ARQ_TESTE)
-        n2 = RHSLPPtb.read(ARQ_TESTE)
+        n1 = Rhslpptb.read(ARQ_TESTE)
+        n2 = Rhslpptb.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_vagua.py` & `inewave-0.0.98/tests/nwlistop/test_vturuh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.vagua import Vagua
+from inewave.nwlistop.vturuh import Vturuh
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vagua import MockVagua
+from tests.mocks.arquivos.vturuh import MockVturUH
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_vagua():
-    m: MagicMock = mock_open(read_data="".join(MockVagua))
+def test_atributos_encontrados_vturuh():
+    m: MagicMock = mock_open(read_data="".join(MockVturUH))
     with patch("builtins.open", m):
-        n = Vagua.read(ARQ_TESTE)
-        assert n.ree is not None
-        assert n.ree == "SUDESTE"
+        n = Vturuh.read(ARQ_TESTE)
+        assert n.usina is not None
+        assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == -1.90
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
-def test_atributos_nao_encontrados_vagua():
+def test_atributos_nao_encontrados_vturuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Vagua.read(ARQ_TESTE)
-        assert n.ree is None
+        n = Vturuh.read(ARQ_TESTE)
+        assert n.usina is None
         assert n.valores is None
 
 
-def test_eq_vagua():
-    m: MagicMock = mock_open(read_data="".join(MockVagua))
+def test_eq_vturuh():
+    m: MagicMock = mock_open(read_data="".join(MockVturUH))
     with patch("builtins.open", m):
-        n1 = Vagua.read(ARQ_TESTE)
-        n2 = Vagua.read(ARQ_TESTE)
+        n1 = Vturuh.read(ARQ_TESTE)
+        n2 = Vturuh.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_varmpuh.py` & `inewave-0.0.98/tests/nwlistop/test_verturb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.varmuh import VarmUH
+from inewave.nwlistop.verturb import Verturb
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.varmuh import MockVarmUH
+from tests.mocks.arquivos.verturb import MockVerturb
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_varmuh():
-    m: MagicMock = mock_open(read_data="".join(MockVarmUH))
+def test_atributos_encontrados_verturb():
+    m: MagicMock = mock_open(read_data="".join(MockVerturb))
     with patch("builtins.open", m):
-        n = VarmUH.read(ARQ_TESTE)
-        assert n.usina is not None
-        assert n.usina == "CAMARGOS"
+        n = Verturb.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2022
-        assert n.valores.iloc[-1, -1] == 662.80
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_varmuh():
+def test_atributos_nao_encontrados_verturb():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = VarmUH.read(ARQ_TESTE)
-        assert n.usina is None
+        n = Verturb.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.ree is None
 
 
-def test_eq_varmuh():
-    m: MagicMock = mock_open(read_data="".join(MockVarmUH))
+def test_eq_verturb():
+    m: MagicMock = mock_open(read_data="".join(MockVerturb))
     with patch("builtins.open", m):
-        n1 = VarmUH.read(ARQ_TESTE)
-        n2 = VarmUH.read(ARQ_TESTE)
+        n1 = Verturb.read(ARQ_TESTE)
+        n2 = Verturb.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_varmuh.py` & `inewave-0.0.98/tests/nwlistop/test_varmpuh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.varmpuh import VarmpUH
+from inewave.nwlistop.varmpuh import Varmpuh
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 from tests.mocks.arquivos.varmpuh import MockVarmpUH
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_varmpuh():
     m: MagicMock = mock_open(read_data="".join(MockVarmpUH))
     with patch("builtins.open", m):
-        n = VarmpUH.read(ARQ_TESTE)
+        n = Varmpuh.read(ARQ_TESTE)
         assert n.usina is not None
         assert n.usina == "CAMARGOS"
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 95.35
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 0.0
 
 
 def test_atributos_nao_encontrados_varmpuh():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = VarmpUH.read(ARQ_TESTE)
+        n = Varmpuh.read(ARQ_TESTE)
         assert n.usina is None
         assert n.valores is None
 
 
 def test_eq_varmpuh():
     m: MagicMock = mock_open(read_data="".join(MockVarmpUH))
     with patch("builtins.open", m):
-        n1 = VarmpUH.read(ARQ_TESTE)
-        n2 = VarmpUH.read(ARQ_TESTE)
+        n1 = Varmpuh.read(ARQ_TESTE)
+        n2 = Varmpuh.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_vento.py` & `inewave-0.0.98/tests/nwlistop/test_evertsin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-from inewave.nwlistop.vento import Vento
+from inewave.nwlistop.evertsin import Evertsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vento import MockVento
+from tests.mocks.arquivos.evertsin import MockEvertSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_vento():
-    m: MagicMock = mock_open(read_data="".join(MockVento))
+def test_atributos_encontrados_evertsin():
+    m: MagicMock = mock_open(read_data="".join(MockEvertSIN))
     with patch("builtins.open", m):
-        n = Vento.read(ARQ_TESTE)
-        assert n.usina is not None
-        # assert n.usina == "cluster_NE_1"
+        n = Evertsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2021
-        assert n.valores.iloc[-1, -1] == 7.8825
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
+        assert n.valores.iloc[-1, -1] == 233.0
 
 
-def test_atributos_nao_encontrados_vento():
+def test_atributos_nao_encontrados_evertsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Vento.read(ARQ_TESTE)
-        assert n.usina is None
+        n = Evertsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_vento():
-    m: MagicMock = mock_open(read_data="".join(MockVento))
+def test_eq_evertsin():
+    m: MagicMock = mock_open(read_data="".join(MockEvertSIN))
     with patch("builtins.open", m):
-        n1 = Vento.read(ARQ_TESTE)
-        n2 = Vento.read(ARQ_TESTE)
+        n1 = Evertsin.read(ARQ_TESTE)
+        n2 = Evertsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_vertuh.py` & `inewave-0.0.98/tests/nwlistop/test_earmfp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.vertuh import VertUH
+from inewave.nwlistop.earmfp import Earmfp
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vertuh import MockVertuh
+from tests.mocks.arquivos.earmfp import MockEarmfp
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_vertuh():
-    m: MagicMock = mock_open(read_data="".join(MockVertuh))
+def test_atributos_encontrados_earmfp():
+    m: MagicMock = mock_open(read_data="".join(MockEarmfp))
     with patch("builtins.open", m):
-        n = VertUH.read(ARQ_TESTE)
-        assert n.usina is not None
-        assert n.usina == "ESPORA"
+        n = Earmfp.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 30.74
+        assert n.valores.iloc[0, 0] == datetime(2022, 1, 1)
+        assert n.valores.iloc[-1, -1] == 83.6
+        assert n.ree is not None
+        assert n.ree == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_vertuh():
+def test_atributos_nao_encontrados_earmfp():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = VertUH.read(ARQ_TESTE)
-        assert n.usina is None
+        n = Earmfp.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.ree is None
 
 
-def test_eq_vertuh():
-    m: MagicMock = mock_open(read_data="".join(MockVertuh))
+def test_eq_earmfp():
+    m: MagicMock = mock_open(read_data="".join(MockEarmfp))
     with patch("builtins.open", m):
-        n1 = VertUH.read(ARQ_TESTE)
-        n2 = VertUH.read(ARQ_TESTE)
+        n1 = Earmfp.read(ARQ_TESTE)
+        n2 = Earmfp.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_verturb.py` & `inewave-0.0.98/tests/nwlistop/test_eaf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.verturb import Verturb
+from inewave.nwlistop.eaf import Eaf
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.verturb import MockVerturb
+from tests.mocks.arquivos.eaf import MockEaf
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_verturb():
-    m: MagicMock = mock_open(read_data="".join(MockVerturb))
+def test_atributos_encontrados_eaf():
+    m: MagicMock = mock_open(read_data="".join(MockEaf))
     with patch("builtins.open", m):
-        n = Verturb.read(ARQ_TESTE)
+        n = Eaf.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == -2347.0
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 1401.0
         assert n.ree is not None
         assert n.ree == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_verturb():
+def test_atributos_nao_encontrados_eaf():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Verturb.read(ARQ_TESTE)
+        n = Eaf.read(ARQ_TESTE)
         assert n.valores is None
         assert n.ree is None
 
 
-def test_eq_verturb():
-    m: MagicMock = mock_open(read_data="".join(MockVerturb))
+def test_eq_eaf():
+    m: MagicMock = mock_open(read_data="".join(MockEaf))
     with patch("builtins.open", m):
-        n1 = Verturb.read(ARQ_TESTE)
-        n2 = Verturb.read(ARQ_TESTE)
+        n1 = Eaf.read(ARQ_TESTE)
+        n2 = Eaf.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_verturbm.py` & `inewave-0.0.98/tests/nwlistop/test_vevminm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.verturbm import Verturbm
+from inewave.nwlistop.vevminm import Vevminm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.verturbm import MockVerturbm
+from tests.mocks.arquivos.vevminm import MockVevminm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_verturbm():
-    m: MagicMock = mock_open(read_data="".join(MockVerturbm))
+def test_atributos_encontrados_vevminm():
+    m: MagicMock = mock_open(read_data="".join(MockVevminm))
     with patch("builtins.open", m):
-        n = Verturbm.read(ARQ_TESTE)
+        n = Vevminm.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
+        assert n.valores.iloc[0, 0] == datetime(2020, 1, 1)
         assert n.valores.iloc[-1, -1] == 0.0
         assert n.submercado is not None
         assert n.submercado == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_verturbm():
+def test_atributos_nao_encontrados_vevminm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Verturbm.read(ARQ_TESTE)
+        n = Vevminm.read(ARQ_TESTE)
         assert n.valores is None
         assert n.submercado is None
 
 
-def test_eq_verturbm():
-    m: MagicMock = mock_open(read_data="".join(MockVerturbm))
+def test_eq_vevminm():
+    m: MagicMock = mock_open(read_data="".join(MockVevminm))
     with patch("builtins.open", m):
-        n1 = Verturbm.read(ARQ_TESTE)
-        n2 = Verturbm.read(ARQ_TESTE)
+        n1 = Vevminm.read(ARQ_TESTE)
+        n2 = Vevminm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_verturbsin.py` & `inewave-0.0.98/tests/nwlistop/test_ghmaxsin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.verturbsin import VerturbSIN
+from inewave.nwlistop.ghmaxsin import Ghmaxsin
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.verturbsin import MockVerturbSIN
+from tests.mocks.arquivos.ghmaxsin import MockGhmaxSIN
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_verturbsin():
-    m: MagicMock = mock_open(read_data="".join(MockVerturbSIN))
+def test_atributos_encontrados_ghmaxsin():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxSIN))
     with patch("builtins.open", m):
-        n = VerturbSIN.read(ARQ_TESTE)
+        n = Ghmaxsin.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == -29007.0
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 96465.3
 
 
-def test_atributos_nao_encontrados_verturbsin():
+def test_atributos_nao_encontrados_ghmaxsin():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = VerturbSIN.read(ARQ_TESTE)
+        n = Ghmaxsin.read(ARQ_TESTE)
         assert n.valores is None
 
 
-def test_eq_verturbsin():
-    m: MagicMock = mock_open(read_data="".join(MockVerturbSIN))
+def test_eq_ghmaxsin():
+    m: MagicMock = mock_open(read_data="".join(MockGhmaxSIN))
     with patch("builtins.open", m):
-        n1 = VerturbSIN.read(ARQ_TESTE)
-        n2 = VerturbSIN.read(ARQ_TESTE)
+        n1 = Ghmaxsin.read(ARQ_TESTE)
+        n2 = Ghmaxsin.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_vevminm.py` & `inewave-0.0.98/tests/nwlistop/test_geolm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from inewave.nwlistop.vevminm import Vevminm
+from inewave.nwlistop.geolm import Geolm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vevminm import MockVevminm
+from tests.mocks.arquivos.geolm import MockGeolm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_vevminm():
-    m: MagicMock = mock_open(read_data="".join(MockVevminm))
+def test_atributos_encontrados_geolm():
+    m: MagicMock = mock_open(read_data="".join(MockGeolm))
     with patch("builtins.open", m):
-        n = Vevminm.read(ARQ_TESTE)
-        assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 0.0
+        n = Geolm.read(ARQ_TESTE)
         assert n.submercado is not None
-        assert n.submercado == "SUDESTE"
+        assert n.submercado == "NORDESTE"
+        assert n.valores is not None
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 5964.8
 
 
-def test_atributos_nao_encontrados_vevminm():
+def test_atributos_nao_encontrados_geolm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Vevminm.read(ARQ_TESTE)
-        assert n.valores is None
+        n = Geolm.read(ARQ_TESTE)
         assert n.submercado is None
+        assert n.valores is None
 
 
-def test_eq_vevminm():
-    m: MagicMock = mock_open(read_data="".join(MockVevminm))
+def test_eq_geolm():
+    m: MagicMock = mock_open(read_data="".join(MockGeolm))
     with patch("builtins.open", m):
-        n1 = Vevminm.read(ARQ_TESTE)
-        n2 = Vevminm.read(ARQ_TESTE)
+        n1 = Geolm.read(ARQ_TESTE)
+        n2 = Geolm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.97/tests/nwlistop/test_vevminsin.py` & `inewave-0.0.98/tests/nwlistop/test_eafm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,40 @@
-from inewave.nwlistop.vevminsin import VevminSIN
+from inewave.nwlistop.eafm import Eafm
 
+from datetime import datetime
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.vevminsin import MockVevminSIN
+from tests.mocks.arquivos.eafm import MockEafm
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_vevminsin():
-    m: MagicMock = mock_open(read_data="".join(MockVevminSIN))
+def test_atributos_encontrados_eafm():
+    m: MagicMock = mock_open(read_data="".join(MockEafm))
     with patch("builtins.open", m):
-        n = VevminSIN.read(ARQ_TESTE)
+        n = Eafm.read(ARQ_TESTE)
         assert n.valores is not None
-        assert n.valores.iloc[0, 0] == 2020
-        assert n.valores.iloc[-1, -1] == 0.0
+        assert n.valores.iloc[0, 0] == datetime(2021, 1, 1)
+        assert n.valores.iloc[-1, -1] == 12836.0
+        assert n.submercado is not None
+        assert n.submercado == "SUDESTE"
 
 
-def test_atributos_nao_encontrados_vevminsin():
+def test_atributos_nao_encontrados_eafm():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = VevminSIN.read(ARQ_TESTE)
+        n = Eafm.read(ARQ_TESTE)
         assert n.valores is None
+        assert n.submercado is None
 
 
-def test_eq_vevminsin():
-    m: MagicMock = mock_open(read_data="".join(MockVevminSIN))
+def test_eq_eafm():
+    m: MagicMock = mock_open(read_data="".join(MockEafm))
     with patch("builtins.open", m):
-        n1 = VevminSIN.read(ARQ_TESTE)
-        n2 = VevminSIN.read(ARQ_TESTE)
+        n1 = Eafm.read(ARQ_TESTE)
+        n2 = Eafm.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

