# Comparing `tmp/inewave-0.0.98.tar.gz` & `tmp/inewave-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inewave-0.0.98.tar", last modified: Wed Aug  2 01:19:17 2023, max compression
+gzip compressed data, was "inewave-1.0.0.tar", last modified: Wed Aug  2 14:45:56 2023, max compression
```

## Comparing `inewave-0.0.98.tar` & `inewave-1.0.0.tar`

### file list

```diff
@@ -1,702 +1,702 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.484546 inewave-0.0.98/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 01:14:29.000000 inewave-0.0.98/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-02 01:19:17.484546 inewave-0.0.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-02 01:14:29.000000 inewave-0.0.98/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.348545 inewave-0.0.98/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-02 01:14:29.000000 inewave-0.0.98/examples/plot_dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-02 01:14:29.000000 inewave-0.0.98/examples/plot_modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-02 01:14:29.000000 inewave-0.0.98/examples/plot_pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-08-02 01:14:29.000000 inewave-0.0.98/examples/plot_sistema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.352545 inewave-0.0.98/inewave/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.352545 inewave-0.0.98/inewave/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/_utils/formatacao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/_utils/leituracsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.360545 inewave-0.0.98/inewave/newave/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/abertura.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/bid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/cortes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    81481 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/elnino.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)    42179 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/forwarh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/gee.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/manutt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.368545 inewave-0.0.98/inewave/newave/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/abertura.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/arquivos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.368545 inewave-0.0.98/inewave/newave/modelos/arquivoscsv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/arquivoscsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/arquivoscsv/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/bid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.368545 inewave-0.0.98/inewave/newave/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/blocos/versaomodelo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/cortes.py
--rw-r--r--   0 runner    (1001) docker     (123)    30466 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)   135879 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/elnino.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)    87572 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/forwarh.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/gee.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/manutt.py
--rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30603 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/perda.py
--rw-r--r--   0 runner    (1001) docker     (123)    24463 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/selcor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)    20585 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/tecno.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modelos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/perda.py
--rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/selcor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/tecno.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/newave/vazpast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.368545 inewave-0.0.98/inewave/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/estados.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.372546 inewave-0.0.98/inewave/nwlistcf/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/estados.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/modelos/nwlistcfrel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistcf/nwlistcfrel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.380545 inewave-0.0.98/inewave/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/gtert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/merclsin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/inewave/nwlistop/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivousina.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/inewave/nwlistop/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/parsubmercados.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/submercado.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/usina.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresserie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/def.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dflppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dflpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/gtert.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/modelos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/nwlistop/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/inewave/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.352545 inewave-0.0.98/inewave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-02 01:19:17.000000 inewave-0.0.98/inewave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-08-02 01:19:17.000000 inewave-0.0.98/inewave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 01:19:17.000000 inewave-0.0.98/inewave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 01:19:17.000000 inewave-0.0.98/inewave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 01:19:17.000000 inewave-0.0.98/inewave.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 01:19:17.484546 inewave-0.0.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 01:14:29.000000 inewave-0.0.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/tests/_arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/_arquivos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.392546 inewave-0.0.98/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.464546 inewave-0.0.98/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/arquivos_nwlistcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)    46951 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/caso_nwlistcf_nwlistop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    30063 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)   847210 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)   295249 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)   295245 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105146 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)   295190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)   295196 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   847164 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)   120243 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)   267099 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267152 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)   267153 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267144 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)   291239 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)   291240 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14002 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicaconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)    56476 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/estados.py
--rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)   267138 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104654 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)   120990 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104650 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105178 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105179 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105181 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   847144 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105136 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105141 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105140 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105189 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)    49768 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/gtert.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105188 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105191 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1087195 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)    49720 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/manutt.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    57012 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (123)    76521 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwlistcfrel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)   378349 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    50087 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)   267136 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   380918 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/selcor.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/term.py
--rw-r--r--   0 runner    (1001) docker     (123)   271157 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)   283139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   283209 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)    32259 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)   847200 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267158 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267117 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105173 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105174 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105176 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   847195 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   847135 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/arquivos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.476546 inewave-0.0.98/tests/newave/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_cortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    49743 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_exph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_expt.py
--rw-r--r--   0 runner    (1001) docker     (123)    36320 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_forwarh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_manutt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_parp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_selcor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_shist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/newave/test_vazpast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.476546 inewave-0.0.98/tests/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/test_arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/test_caso.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/test_estados.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/test_nwlistcfdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistcf/test_nwlistcfrel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:19:17.484546 inewave-0.0.98/tests/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_coper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_evert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_exces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_geol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_gtert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_invade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_nwlistopdat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vento.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 01:14:29.000000 inewave-0.0.98/tests/nwlistop/test_vturuh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.442547 inewave-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:02.000000 inewave-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-02 14:45:56.442547 inewave-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-02 14:41:02.000000 inewave-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.238549 inewave-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-02 14:41:02.000000 inewave-1.0.0/examples/plot_dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-02 14:41:02.000000 inewave-1.0.0/examples/plot_modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-02 14:41:02.000000 inewave-1.0.0/examples/plot_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-08-02 14:41:02.000000 inewave-1.0.0/examples/plot_sistema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.242549 inewave-1.0.0/inewave/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.242549 inewave-1.0.0/inewave/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/_utils/formatacao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/_utils/leituracsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.250548 inewave-1.0.0/inewave/newave/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80568 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38978 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/gee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/manutt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.266548 inewave-1.0.0/inewave/newave/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/arquivos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.266548 inewave-1.0.0/inewave/newave/modelos/arquivoscsv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/arquivoscsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/arquivoscsv/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/bid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.266548 inewave-1.0.0/inewave/newave/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/blocos/versaomodelo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30466 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135879 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87572 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/gee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30603 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23381 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/perda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24463 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20585 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modelos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18006 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/perda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/newave/vazpast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.270548 inewave-1.0.0/inewave/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/estados.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.270548 inewave-1.0.0/inewave/nwlistcf/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/modelos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/modelos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/modelos/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/modelos/nwlistcfrel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistcf/nwlistcfrel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.306548 inewave-1.0.0/inewave/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/merclsin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.326548 inewave-1.0.0/inewave/nwlistop/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.330548 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivoree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivosin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivousina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.330548 inewave-1.0.0/inewave/nwlistop/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/blocos/parsubmercados.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/blocos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/blocos/submercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/blocos/usina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/blocos/valoresserie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/dflppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/dflpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/modelos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/nwlistop/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/inewave/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.242549 inewave-1.0.0/inewave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-02 14:45:56.000000 inewave-1.0.0/inewave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21586 2023-08-02 14:45:56.000000 inewave-1.0.0/inewave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:45:56.000000 inewave-1.0.0/inewave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:45:56.000000 inewave-1.0.0/inewave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:45:56.000000 inewave-1.0.0/inewave.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:45:56.442547 inewave-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:41:02.000000 inewave-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.330548 inewave-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.330548 inewave-1.0.0/tests/_arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/_arquivos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.330548 inewave-1.0.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.410547 inewave-1.0.0/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/arquivos_nwlistcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46951 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/caso_nwlistcf_nwlistop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30063 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847210 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295249 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295245 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105146 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295190 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295196 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847164 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120243 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267099 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267152 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267153 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267144 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   291239 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   291240 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14002 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eolicaconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56476 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267138 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104654 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120990 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104650 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105178 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105179 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105181 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847144 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105136 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105139 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105141 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105140 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105189 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105190 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49768 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105188 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105191 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1087195 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49720 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57012 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76521 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/nwlistcfrel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)   378349 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50087 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267136 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   380918 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)   271157 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283139 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283209 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32259 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847200 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267158 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267117 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105173 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105174 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105176 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847195 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847135 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/arquivos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.422547 inewave-1.0.0/tests/newave/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49743 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36320 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_manutt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/newave/test_vazpast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.426547 inewave-1.0.0/tests/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistcf/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistcf/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistcf/test_estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistcf/test_nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistcf/test_nwlistcfrel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:56.442547 inewave-1.0.0/tests/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-08-02 14:41:02.000000 inewave-1.0.0/tests/nwlistop/test_vturuh.py
```

### Comparing `inewave-0.0.98/LICENSE.md` & `inewave-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/PKG-INFO` & `inewave-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 0.0.98
+Version: 1.0.0
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-0.0.98/README.md` & `inewave-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/examples/plot_dger.py` & `inewave-1.0.0/examples/plot_dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/examples/plot_modif.py` & `inewave-1.0.0/examples/plot_modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/examples/plot_pmo.py` & `inewave-1.0.0/examples/plot_pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/examples/plot_sistema.py` & `inewave-1.0.0/examples/plot_sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/_utils/formatacao.py` & `inewave-1.0.0/inewave/_utils/formatacao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/_utils/leituracsv.py` & `inewave-1.0.0/inewave/_utils/leituracsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/config.py` & `inewave-1.0.0/inewave/config.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/__init__.py` & `inewave-1.0.0/inewave/newave/__init__.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/arquivos.py` & `inewave-1.0.0/inewave/newave/arquivos.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from inewave.newave.modelos.arquivos import BlocoNomesArquivos
 
 from cfinterface.files.sectionfile import SectionFile
 
 from typing import List, TypeVar, Optional
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Arquivos(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao arquivo
     `arquivos.dat`.
 
     Esta classe lida com informações de entrada do NEWAVE e
@@ -21,34 +17,14 @@
 
     """
 
     T = TypeVar("T")
 
     SECTIONS = [BlocoNomesArquivos]
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="arquivos.dat"
-    ) -> "Arquivos":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="arquivos.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     def __le_nome_por_indice(self, indice: int) -> Optional[str]:
         b = self.data.get_sections_of_type(BlocoNomesArquivos)
         if isinstance(b, BlocoNomesArquivos):
             if indice in b.data.index:
                 dado = b.data.iloc[indice, 1]
                 if isinstance(dado, str):
                     return dado
```

### Comparing `inewave-0.0.98/inewave/newave/avl_desvfpha_s.py` & `inewave-1.0.0/inewave/newave/avl_desvfpha_s.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from inewave.newave.modelos.blocos.versaomodelo import VersaoModelo
 from inewave.newave.modelos.avl_desvfpha_s import TabelaAvlDesvFphaS
 
 from cfinterface.files.blockfile import BlockFile
 from typing import Optional, TypeVar
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class AvlDesvFphaS(BlockFile):
     """
     Arquivo com os desvios da função de produção no plano de
     vazão vertida (S).
     """
 
@@ -21,25 +17,14 @@
 
     T = TypeVar("T")
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__df_completo: Optional[pd.DataFrame] = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, arquivo: str = "avl_desvfpha_s_001.dat"
-    ) -> "AvlDesvFphaS":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, arquivo))
-
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
         - codigo_usina (`int`)
         - nome_usina (`str`)
```

### Comparing `inewave-0.0.98/inewave/newave/avl_desvfpha_v_q.py` & `inewave-1.0.0/inewave/newave/avl_desvfpha_v_q.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from inewave.newave.modelos.blocos.versaomodelo import VersaoModelo
 from inewave.newave.modelos.avl_desvfpha_v_q import TabelaAvlDesvFphaVQ
 
 from cfinterface.files.blockfile import BlockFile
 from typing import Optional, TypeVar
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class AvlDesvFphaVQ(BlockFile):
     """
     Arquivo com os desvios da função de produção nos planos de
     volume armazenado e vazão turbinada (V-Q).
     """
 
@@ -21,25 +17,14 @@
 
     T = TypeVar("T")
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__df_completo: Optional[pd.DataFrame] = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, arquivo: str = "avl_desvfpha_v_q_001.dat"
-    ) -> "AvlDesvFphaVQ":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, arquivo))
-
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
         - codigo_usina (`int`)
         - nome_usina (`str`)
```

### Comparing `inewave-0.0.98/inewave/newave/clast.py` & `inewave-1.0.0/inewave/newave/clast.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,51 +3,26 @@
     BlocoModificacaoUTEClasT,
 )
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Clast(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às classes de
     usinas térmicas.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS = [BlocoUTEClasT, BlocoModificacaoUTEClasT]
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="clast.dat") -> "Clast":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="clast.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     @property
     def usinas(self) -> Optional[pd.DataFrame]:
         """
         Tabela com as usinas e seus custos.
 
         - codigo (`int`)
         - nome (`str`)
```

### Comparing `inewave-0.0.98/inewave/newave/cortesh.py` & `inewave-1.0.0/inewave/newave/cortesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,25 @@
 from cfinterface.files.sectionfile import SectionFile
 from inewave.newave.modelos.cortesh import SecaoDadosCortesh
 
 import pandas as pd  # type: ignore
 from typing import TypeVar
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Cortesh(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes ao
     cabeçalho dos cortes de Benders.
     """
 
     T = TypeVar("T")
 
     SECTIONS = [SecaoDadosCortesh]
     STORAGE = "BINARY"
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="cortesh.dat"
-    ) -> "Cortesh":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="cortesh.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     def __obtem_dados(self) -> SecaoDadosCortesh:
         dados = [r for r in self.data.of_type(SecaoDadosCortesh)]
         return dados[0]
 
     @property
     def versao_newave(self) -> int:
         """
```

### Comparing `inewave-0.0.98/inewave/newave/curva.py` & `inewave-1.0.0/inewave/newave/curva.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,14 @@
     BlocoImpressaoRelatorioProcessoIterativoEtapa2,
 )
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Curva(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes à curva para
     penalização por volume mínimo dos reservatórios.
     """
 
@@ -31,35 +27,14 @@
         BlocoCurvaSegurancaREE,
         BlocoMaximoIteracoesProcessoIterativoEtapa2,
         BlocoIteracaoAPartirProcessoIterativoEtapa2,
         BlocoToleranciaProcessoIterativoEtapa2,
         BlocoImpressaoRelatorioProcessoIterativoEtapa2,
     ]
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="curva.dat") -> "Curva":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="curva.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     @property
     def configuracoes_penalizacao(self) -> Optional[list]:
         """
         Linha de configuração das opções de penalização do
         arquivo curva.dat.
 
         :return: Os valores dos campos da linha como uma lista.
```

### Comparing `inewave-0.0.98/inewave/newave/dger.py` & `inewave-1.0.0/inewave/newave/dger.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,18 +101,14 @@
 from inewave.newave.modelos.dger import BlocoRestricaoLPPDefluenciaMaximaUHE
 from inewave.newave.modelos.dger import BlocoRestricoesEletricasEspeciais
 from inewave.newave.modelos.dger import BlocoFuncaoProducaoUHE
 from inewave.newave.modelos.dger import BlocoFCFPosEstudo
 from inewave.newave.modelos.dger import BlocoEstacoesBombeamento
 from inewave.newave.modelos.dger import BlocoCanalDesvio
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Dger(SectionFile):
     """
     Classe para armazenar dados gerais de uma execução do NEWAVE.
 
     """
 
@@ -218,35 +214,14 @@
         BlocoRestricoesEletricasEspeciais,
         BlocoFuncaoProducaoUHE,
         BlocoFCFPosEstudo,
         BlocoEstacoesBombeamento,
         BlocoCanalDesvio,
     ]
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="dger.dat") -> "Dger":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="dger.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     @property
     def nome_caso(self) -> Optional[str]:
         """
         Configuração da linha número 1 do arquivo `dger.dat`.
 
         :return: O valor do campo
         :rtype: str
```

### Comparing `inewave-0.0.98/inewave/newave/energias.py` & `inewave-1.0.0/inewave/newave/modelos/energiab.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,95 @@
-from cfinterface.files.sectionfile import SectionFile
-from inewave.newave.modelos.energias import SecaoDadosEnergias
+from cfinterface.components.section import Section
+from cfinterface.components.line import Line
+from cfinterface.components.floatfield import FloatField
+from typing import IO
 import pandas as pd  # type: ignore
+import numpy as np  # type: ignore
 
-from typing import TypeVar, Optional
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
-
-class Energias(SectionFile):
+class SecaoDadosEnergiab(Section):
     """
-    Armazena os dados de saída do NEWAVE referentes às séries sintéticas
-    de energia para a simulação final geradas pelo modelo.
+    Registro com os dados das séries sintéticas de energia existentes
+    nos arquivos energiabXXX.dat.
     """
 
-    T = TypeVar("T")
+    def __init__(self, previous=None, next=None, data=None) -> None:
+        super().__init__(previous, next, data)
 
-    SECTIONS = [SecaoDadosEnergias]
-    STORAGE = "BINARY"
-
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
+    def __eq__(self, o: object) -> bool:
+        if not isinstance(o, SecaoDadosEnergiab):
+            return False
+        bloco: SecaoDadosEnergiab = o
+        if not all(
+            [
+                isinstance(self.data, pd.DataFrame),
+                isinstance(o.data, pd.DataFrame),
+            ]
+        ):
+            return False
+        else:
+            return self.data.equals(bloco.data)
 
-    @classmethod
-    def le_arquivo(
-        cls,
-        diretorio: str,
-        nome_arquivo="energias.dat",
-        numero_series: int = 2000,
+    def read(
+        self,
+        file: IO,
+        numero_forwards: int = 200,
+        numero_aberturas: int = 20,
         numero_rees: int = 12,
         numero_estagios: int = 60,
-        numero_estagios_th: int = 12,
-    ) -> "Energias":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(
-            join(diretorio, nome_arquivo),
-            numero_rees=numero_rees,
-            numero_series=numero_series,
-            numero_estagios=numero_estagios,
-            numero_estagios_th=numero_estagios_th,
-        )
-
-    @property
-    def series(self) -> Optional[pd.DataFrame]:
-        """
-        Obtém a tabela com os dados das séries de energia
-        afluente por REE e por estágio, para a simulação final.
-
-        - estagio (`int`): estágio do cenário gerado
-        - ree (`int`): REE para o qual foi gerado
-        - serie (`int`): índice da série sintética
-        - valor (`float`): energia em MWmes
-
-        :return: A tabela com os dados das séries
-        :rtype: pd.DataFrame | None
-        """
-        sections = [r for r in self.data.of_type(SecaoDadosEnergias)]
-        if len(sections) > 0:
-            return sections[0].data
-        else:
-            return None
+        *args,
+        **kwargs,
+    ):
+        numero_registros = (
+            (numero_estagios)
+            * numero_rees
+            * numero_forwards
+            * numero_aberturas
+        )
+        self.__linha = Line(
+            [
+                FloatField(size=8, starting_position=8 * i)
+                for i in range(numero_registros)
+            ],
+            storage="BINARY",
+        )
+        dados = self.__linha.read(file.read(self.__linha.size))
+        indices_estagios = np.arange(1, numero_estagios + 1)
+        estagios_df = np.repeat(
+            indices_estagios, numero_forwards * numero_aberturas * numero_rees
+        )
+        rees_df = np.tile(
+            np.repeat(
+                np.arange(1, numero_rees + 1),
+                numero_forwards * numero_aberturas,
+            ),
+            numero_estagios,
+        )
+        forwards_df = np.tile(
+            np.repeat(np.arange(1, numero_forwards + 1), numero_aberturas),
+            numero_rees * numero_estagios,
+        )
+        aberturas_df = np.tile(
+            np.arange(1, numero_aberturas + 1),
+            numero_rees * numero_estagios * numero_forwards,
+        )
+        df = pd.DataFrame(
+            data={
+                "estagio": estagios_df,
+                "ree": rees_df,
+                "serie": forwards_df,
+                "abertura": aberturas_df,
+                "valor": dados,
+            }
+        )
+        self.data = df
 
-    @series.setter
-    def series(self, df: pd.DataFrame):
-        sections = [r for r in self.data.of_type(SecaoDadosEnergias)]
-        if len(sections) > 0:
-            sections[0].data = df
+    def write(self, file: IO, *args, **kwargs):
+        dados = self.data["valor"].to_numpy()
+        linha = Line(
+            [
+                FloatField(size=8, starting_position=8 * i)
+                for i in range(len(dados))
+            ],
+            storage="BINARY",
+        )
+        file.write(linha.write(dados))
```

### Comparing `inewave-0.0.98/inewave/newave/eolicacadastro.py` & `inewave-1.0.0/inewave/newave/eolicacadastro.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,18 +8,14 @@
     RegistroEolicaCadastroAerogerador,
     RegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo,
     RegistroEolicaConjuntoAerogeradoresPotenciaEfetiva,
     RegistroPEECadastro,
     RegistroPEEPotenciaInstaladaPeriodo,
 )
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class EolicaCadastro(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao cadastro
     das usinas eólicas do sistema.
     """
 
@@ -31,39 +27,14 @@
         RegistroEolicaCadastro,
         RegistroEolicaConjuntoAerogeradoresQuantidadeOperandoPeriodo,
         RegistroEolicaConjuntoAerogeradoresPotenciaEfetiva,
         RegistroPEECadastro,
         RegistroPEEPotenciaInstaladaPeriodo,
     ]
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="eolica-cadastro.csv"
-    ) -> "EolicaCadastro":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(
-        self, diretorio: str, nome_arquivo="eolica-cadastro.csv"
-    ):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     def eolica_cadastro(
         self,
         codigo_eolica: Optional[int] = None,
         nome_eolica: Optional[str] = None,
         quantidade_conjuntos: Optional[str] = None,
     ) -> Optional[Union[RegistroEolicaCadastro, List[RegistroEolicaCadastro]]]:
         """
```

### Comparing `inewave-0.0.98/inewave/newave/eolicaconfiguracao.py` & `inewave-1.0.0/inewave/newave/restricaoeletrica.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,120 +1,112 @@
 from typing import TypeVar, List, Optional, Union
 from datetime import datetime
 
 from cfinterface.files.registerfile import RegisterFile
-from inewave.newave.modelos.eolicaconfiguracao import (
-    RegistroEolicaConfiguracao,
-    RegistroPEEConfiguracaoPeriodo,
+from inewave.newave.modelos.restricaoeletrica import (
+    RegistroRE,
+    RegistroREHorizPer,
+    RegistroRELimFormPer,
 )
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
-class EolicaConfiguracao(RegisterFile):
+class RestricaoEletrica(RegisterFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às configurações
-    das usinas eólicas.
+    Armazena os dados de entrada do NEWAVE referentes ao cadastro
+    das restrições lineares por partes no domínio de energia (REE).
     """
 
     T = TypeVar("T")
 
-    REGISTERS = [RegistroEolicaConfiguracao, RegistroPEEConfiguracaoPeriodo]
-
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
+    REGISTERS = [
+        RegistroRELimFormPer,
+        RegistroREHorizPer,
+        RegistroRE,
+    ]
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="eolica-config.csv"
-    ) -> "EolicaConfiguracao":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
+    def re(
+        self,
+        codigo_restricao: Optional[int] = None,
+        formula: Optional[str] = None,
+    ) -> Optional[Union[RegistroRE, List[RegistroRE]]]:
+        """
+        Obtém um registro que cadastra uma usina restrição elétrica (RE).
 
-    def escreve_arquivo(
-        self, diretorio: str, nome_arquivo="eolica-config.csv"
-    ):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
+        :param codigo_restricao: código que especifica a restrição
+        :type codigo_restricao: int | None
+        :param formula: equação da restrição
+        :type formula: str | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`RegistroRE` |
+            list[:class:`RegistroRE`] | None
+        """
+        return self.data.get_registers_of_type(
+            RegistroRE,
+            codigo_restricao=codigo_restricao,
+            formula=formula,
         )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
 
-    def eolica_configuracao(
+    def re_horiz_per(
         self,
-        codigo_eolica: Optional[int] = None,
+        codigo_restricao: Optional[int] = None,
         data_inicial: Optional[datetime] = None,
         data_final: Optional[datetime] = None,
-        estado_operacao: Optional[str] = None,
-    ) -> Optional[
-        Union[
-            RegistroEolicaConfiguracao,
-            List[RegistroEolicaConfiguracao],
-        ]
-    ]:
-        """
-        Obtém um registro que contém a configuração de operação para
-        uma usina eólica em um período.
-
-        :param codigo_eolica: código que especifica a usina
-        :type codigo_eolica: int | None
-        :param data_inicial: período de início da configuração
+    ) -> Optional[Union[RegistroREHorizPer, List[RegistroREHorizPer]]]:
+        """
+        Obtém um registro que cadastra o horizonte de validade de uma
+        restrição elétrica.
+
+        :param codigo_restricao: código que especifica a restrição
+        :type codigo_restricao: int | None
+        :param data_inicial: data inicial de validade da restrição
         :type data_inicial: datetime | None
-        :param data_final: período de fim da configuração
+        :param data_final: data final de validade da restrição
         :type data_final: datetime | None
-        :param estado_operacao: tipo de operação
-        :type estado_operacao: str | None
         :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroEolicaConfiguracao` |
-            list[:class:`RegistroEolicaConfiguracao`] | None
+        :rtype: :class:`RegistroREHorizPer` |
+            list[:class:`RegistroREHorizPer`] | None
         """
         return self.data.get_registers_of_type(
-            RegistroEolicaConfiguracao,
-            codigo_eolica=codigo_eolica,
+            RegistroREHorizPer,
+            codigo_restricao=codigo_restricao,
             data_inicial=data_inicial,
             data_final=data_final,
-            estado_operacao=estado_operacao,
         )
 
-    def pee_config_per(
+    def re_lim_form_per(
         self,
-        codigo_pee: Optional[int] = None,
+        codigo_restricao: Optional[int] = None,
         data_inicial: Optional[datetime] = None,
         data_final: Optional[datetime] = None,
-        estado_operacao: Optional[str] = None,
-    ) -> Optional[
-        Union[
-            RegistroPEEConfiguracaoPeriodo,
-            List[RegistroPEEConfiguracaoPeriodo],
-        ]
-    ]:
-        """
-        Obtém um registro que contém a configuração de operação para
-        um PEE em um período.
-
-        :param codigo_pee: código que especifica o PEE
-        :type codigo_pee: int | None
-        :param data_inicial: período de início da configuração
+        patamar: Optional[int] = None,
+        limite_inferior: Optional[float] = None,
+        limite_superior: Optional[float] = None,
+    ) -> Optional[Union[RegistroRELimFormPer, List[RegistroRELimFormPer]]]:
+        """
+        Obtém um registro que cadastra os limites por horizonte e por
+        patamar para uma restrição elétrica.
+
+        :param codigo_restricao: código que especifica a restrição
+        :type codigo_restricao: int | None
+        :param data_inicial: data inicial de validade dos limites
         :type data_inicial: datetime | None
-        :param data_final: período de fim da configuração
+        :param data_final: data final de validade dos limites
         :type data_final: datetime | None
-        :param estado_operacao: tipo de operação
-        :type estado_operacao: str | None
+        :param patamar: patamar de validade dos limites
+        :type patamar: int | None
+        :param limite_inferior: limite inferior da restrição
+        :type limite_inferior: float | None
+        :param limite_superior: limite superior da restrição
+        :type limite_superior: float | None
         :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RegistroPEEConfiguracaoPeriodo` |
-            list[:class:`RegistroPEEConfiguracaoPeriodo`] | None
+        :rtype: :class:`RegistroRELimFormPer` |
+            list[:class:`RegistroRELimFormPer`] | None
         """
         return self.data.get_registers_of_type(
-            RegistroPEEConfiguracaoPeriodo,
-            codigo_pee=codigo_pee,
+            RegistroRELimFormPer,
+            codigo_restricao=codigo_restricao,
             data_inicial=data_inicial,
             data_final=data_final,
-            estado_operacao=estado_operacao,
+            patamar=patamar,
+            limite_inferior=limite_inferior,
+            limite_superior=limite_superior,
         )
```

### Comparing `inewave-0.0.98/inewave/newave/eolicasubmercado.py` & `inewave-1.0.0/inewave/newave/restricaoenergia.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,105 @@
 from typing import TypeVar, List, Optional, Union
+from datetime import datetime
 
 from cfinterface.files.registerfile import RegisterFile
-from inewave.newave.modelos.eolicasubmercado import (
-    RegistroEolicaSubmercado,
-    RegistroPEESubmercado,
+from inewave.newave.modelos.restricaoenergia import (
+    RegistroRHE,
+    RegistroRHEHorizPer,
+    RegistroRHELsLPPEarmi,
 )
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
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
-
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
+    REGISTERS = [
+        RegistroRHELsLPPEarmi,
+        RegistroRHEHorizPer,
+        RegistroRHE,
+    ]
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="eolica-submercado.csv"
-    ) -> "EolicaSubmercado":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
+    def rhe(
+        self,
+        codigo_restricao: Optional[int] = None,
+        formula: Optional[str] = None,
+    ) -> Optional[Union[RegistroRHE, List[RegistroRHE]]]:
+        """
+        Obtém um registro que cadastra uma usina restrição linear por
+        partes de energia (REE).
 
-    def escreve_arquivo(
-        self, diretorio: str, nome_arquivo="eolica-submercado.csv"
-    ):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
+        :param codigo_restricao: código que especifica a restrição
+        :type codigo_restricao: int | None
+        :param formula: equação da restrição
+        :type formula: str | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`RegistroRHE` |
+            list[:class:`RegistroRHE`] | None
+        """
+        return self.data.get_registers_of_type(
+            RegistroRHE,
+            codigo_restricao=codigo_restricao,
+            formula=formula,
         )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
 
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
         return self.data.get_registers_of_type(
-            RegistroEolicaSubmercado,
-            codigo_eolica=codigo_eolica,
-            codigo_submercado=codigo_submercado,
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
         return self.data.get_registers_of_type(
-            RegistroPEESubmercado,
-            codigo_pee=codigo_pee,
-            codigo_submercado=codigo_submercado,
+            RegistroRHELsLPPEarmi,
+            codigo_restricao=codigo_restricao,
+            indice_reta=indice_reta,
+            coeficiente_angular=coeficiente_angular,
+            coeficiente_linear=coeficiente_linear,
         )
```

### Comparing `inewave-0.0.98/inewave/newave/forward.py` & `inewave-1.0.0/inewave/newave/forward.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,115 +1,26 @@
 from cfinterface.files.sectionfile import SectionFile
 from inewave.newave.modelos.forward import VariavelOperacao, SecaoDadosForward
 
 
-from typing import TypeVar, Optional, Union, List
+from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Forward(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes às simulações
     forward.
     """
 
     T = TypeVar("T")
 
     SECTIONS = [SecaoDadosForward]
     STORAGE = "BINARY"
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def read(
-        cls,
-        content: Union[str, bytes],
-        tamanho_registro: int = 41264,
-        numero_estagios: int = 60,
-        numero_forwards: int = 200,
-        numero_patamares_carga: int = 3,
-        numero_patamares_deficit: int = 1,
-        numero_agrupamentos_intercambio: int = 1,
-        numero_classes_termicas_submercados: List[int] = [],
-        lag_maximo_usinas_gnl: int = 2,
-        nomes_submercados: List[str] = ["SUDESTE", "SUL", "NORDESTE", "NORTE"],
-        nomes_submercados_totais: List[str] = [
-            "SUDESTE",
-            "SUL",
-            "NORDESTE",
-            "NORTE",
-            "NOFICT1",
-        ],
-        nomes_rees: List[str] = [
-            "SUDESTE",
-            "MADEIRA",
-            "TPIRES",
-            "ITAIPU",
-            "PARANA",
-            "PRNPANEMA",
-            "SUL",
-            "IGUACU",
-            "NORDESTE",
-            "NORTE",
-            "BMONTE",
-            "MAN-AP",
-        ],
-        nomes_classes_termicas: List[str] = [],
-        nomes_usinas_hidreletricas: List[str] = [],
-        nomes_parques_eolicos_equivalentes: List[str] = [],
-        nomes_estacoes_bombeamento: List[str] = [],
-        *args,
-        **kwargs
-    ) -> "Forward":
-        return super().read(
-            content,
-            tamanho_registro=tamanho_registro,
-            numero_estagios=numero_estagios,
-            numero_forwards=numero_forwards,
-            numero_patamares_carga=numero_patamares_carga,
-            numero_patamares_deficit=numero_patamares_deficit,
-            numero_agrupamentos_intercambio=numero_agrupamentos_intercambio,
-            numero_classes_termicas_submercados=numero_classes_termicas_submercados,
-            lag_maximo_usinas_gnl=lag_maximo_usinas_gnl,
-            nomes_submercados=nomes_submercados,
-            nomes_submercados_totais=nomes_submercados_totais,
-            nomes_rees=nomes_rees,
-            nomes_classes_termicas=nomes_classes_termicas,
-            nomes_usinas_hidreletricas=nomes_usinas_hidreletricas,
-            nomes_parques_eolicos_equivalentes=nomes_parques_eolicos_equivalentes,
-            nomes_estacoes_bombeamento=nomes_estacoes_bombeamento,
-            *args,
-            **kwargs
-        )
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="forward.dat"
-    ) -> "Forward":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="forward.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     def __bloco_dados(self) -> Optional[SecaoDadosForward]:
         dados = [r for r in self.data.of_type(SecaoDadosForward)]
         if len(dados) == 1:
             return dados[0]
         else:
             return None
```

### Comparing `inewave-0.0.98/inewave/newave/forwarh.py` & `inewave-1.0.0/inewave/newave/forwarh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,25 @@
 from cfinterface.files.sectionfile import SectionFile
 from inewave.newave.modelos.forwarh import SecaoDadosForwarh
 
 
 from typing import TypeVar, Optional, List
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Forwarh(SectionFile):
     """
     Armazena os dados de saída do NEWAVE referentes ao
     cabeçalho dos dados das simulações forward.
     """
 
     T = TypeVar("T")
 
     SECTIONS = [SecaoDadosForwarh]
     STORAGE = "BINARY"
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="forwarh.dat"
-    ) -> "Forwarh":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="forwarh.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     def __bloco_dados(self) -> Optional[SecaoDadosForwarh]:
         dados = [r for r in self.data.of_type(SecaoDadosForwarh)]
         if len(dados) == 1:
             return dados[0]
         else:
             return None
```

### Comparing `inewave-0.0.98/inewave/newave/hidr.py` & `inewave-1.0.0/inewave/newave/hidr.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 from inewave.newave.modelos.hidr import RegistroUHEHidr
 from inewave.config import MESES_ABREV
 import pandas as pd  # type: ignore
 
 
 from typing import TypeVar, List, Optional, Union, IO
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Hidr(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao cadastro das
     usinas hidroelétricas.
     """
 
@@ -22,32 +18,14 @@
     REGISTERS = [RegistroUHEHidr]
     STORAGE = "BINARY"
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__df: Optional[pd.DataFrame] = None
 
-    @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="hidr.dat") -> "Hidr":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="hidr.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     def write(self, to: Union[str, IO], *args, **kwargs):
         self.__atualiza_registros()
         super().write(to, *args, **kwargs)
 
     def __monta_df_de_registros(self) -> Optional[pd.DataFrame]:
         registros: List[RegistroUHEHidr] = [
             r for r in self.data.of_type(RegistroUHEHidr)
```

### Comparing `inewave-0.0.98/inewave/newave/modelos/adterm.py` & `inewave-1.0.0/inewave/newave/modelos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/agrint.py` & `inewave-1.0.0/inewave/newave/modelos/agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/arquivos.py` & `inewave-1.0.0/inewave/newave/modelos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/arquivoscsv/arquivocsv.py` & `inewave-1.0.0/inewave/newave/modelos/arquivoscsv/arquivocsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/avl_cortesfpha_nwv.py` & `inewave-1.0.0/inewave/newave/modelos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/avl_desvfpha_s.py` & `inewave-1.0.0/inewave/newave/modelos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/avl_desvfpha_v_q.py` & `inewave-1.0.0/inewave/newave/modelos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/blocos/tabelacsv.py` & `inewave-1.0.0/inewave/newave/modelos/blocos/tabelacsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/blocos/versaomodelo.py` & `inewave-1.0.0/inewave/newave/modelos/blocos/versaomodelo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/cadic.py` & `inewave-1.0.0/inewave/newave/modelos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/caso.py` & `inewave-1.0.0/inewave/newave/modelos/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/clast.py` & `inewave-1.0.0/inewave/newave/modelos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/confhd.py` & `inewave-1.0.0/inewave/newave/modelos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/conft.py` & `inewave-1.0.0/inewave/newave/modelos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/cortes.py` & `inewave-1.0.0/inewave/newave/modelos/cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/cortesh.py` & `inewave-1.0.0/inewave/newave/modelos/cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/curva.py` & `inewave-1.0.0/inewave/newave/modelos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/cvar.py` & `inewave-1.0.0/inewave/newave/modelos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/dger.py` & `inewave-1.0.0/inewave/newave/modelos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/dsvagua.py` & `inewave-1.0.0/inewave/newave/modelos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/eafpast.py` & `inewave-1.0.0/inewave/newave/modelos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/enavazb.py` & `inewave-1.0.0/inewave/newave/modelos/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/enavazf.py` & `inewave-1.0.0/inewave/newave/modelos/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/energiab.py` & `inewave-1.0.0/inewave/newave/modelos/vazaob.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from cfinterface.components.line import Line
 from cfinterface.components.floatfield import FloatField
 from typing import IO
 import pandas as pd  # type: ignore
 import numpy as np  # type: ignore
 
 
-class SecaoDadosEnergiab(Section):
+class SecaoDadosVazaob(Section):
     """
-    Registro com os dados das séries sintéticas de energia existentes
-    nos arquivos energiabXXX.dat.
+    Registro com os dados das séries sintéticas de vazão existentes
+    nos arquivos vazaobXXX.dat.
     """
 
     def __init__(self, previous=None, next=None, data=None) -> None:
         super().__init__(previous, next, data)
 
     def __eq__(self, o: object) -> bool:
-        if not isinstance(o, SecaoDadosEnergiab):
+        if not isinstance(o, SecaoDadosVazaob):
             return False
-        bloco: SecaoDadosEnergiab = o
+        bloco: SecaoDadosVazaob = o
         if not all(
             [
                 isinstance(self.data, pd.DataFrame),
                 isinstance(o.data, pd.DataFrame),
             ]
         ):
             return False
@@ -30,56 +30,56 @@
             return self.data.equals(bloco.data)
 
     def read(
         self,
         file: IO,
         numero_forwards: int = 200,
         numero_aberturas: int = 20,
-        numero_rees: int = 12,
+        numero_uhes: int = 164,
         numero_estagios: int = 60,
         *args,
         **kwargs,
     ):
         numero_registros = (
             (numero_estagios)
-            * numero_rees
+            * numero_uhes
             * numero_forwards
             * numero_aberturas
         )
         self.__linha = Line(
             [
                 FloatField(size=8, starting_position=8 * i)
                 for i in range(numero_registros)
             ],
             storage="BINARY",
         )
         dados = self.__linha.read(file.read(self.__linha.size))
         indices_estagios = np.arange(1, numero_estagios + 1)
         estagios_df = np.repeat(
-            indices_estagios, numero_forwards * numero_aberturas * numero_rees
+            indices_estagios, numero_forwards * numero_aberturas * numero_uhes
         )
-        rees_df = np.tile(
+        uhes_df = np.tile(
             np.repeat(
-                np.arange(1, numero_rees + 1),
+                np.arange(1, numero_uhes + 1),
                 numero_forwards * numero_aberturas,
             ),
             numero_estagios,
         )
         forwards_df = np.tile(
             np.repeat(np.arange(1, numero_forwards + 1), numero_aberturas),
-            numero_rees * numero_estagios,
+            numero_uhes * numero_estagios,
         )
         aberturas_df = np.tile(
             np.arange(1, numero_aberturas + 1),
-            numero_rees * numero_estagios * numero_forwards,
+            numero_uhes * numero_estagios * numero_forwards,
         )
         df = pd.DataFrame(
             data={
                 "estagio": estagios_df,
-                "ree": rees_df,
+                "uhe": uhes_df,
                 "serie": forwards_df,
                 "abertura": aberturas_df,
                 "valor": dados,
             }
         )
         self.data = df
```

### Comparing `inewave-0.0.98/inewave/newave/modelos/energiaf.py` & `inewave-1.0.0/inewave/newave/modelos/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/energias.py` & `inewave-1.0.0/inewave/newave/modelos/energias.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/engnat.py` & `inewave-1.0.0/inewave/newave/modelos/engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/eolicacadastro.py` & `inewave-1.0.0/inewave/newave/modelos/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/eolicaconfiguracao.py` & `inewave-1.0.0/inewave/newave/modelos/eolicaconfiguracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/eolicafte.py` & `inewave-1.0.0/inewave/newave/modelos/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/eolicageracao.py` & `inewave-1.0.0/inewave/newave/modelos/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/eolicahistorico.py` & `inewave-1.0.0/inewave/newave/modelos/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/eolicaposto.py` & `inewave-1.0.0/inewave/newave/modelos/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/eolicasubmercado.py` & `inewave-1.0.0/inewave/newave/modelos/eolicasubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/exph.py` & `inewave-1.0.0/inewave/newave/modelos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/expt.py` & `inewave-1.0.0/inewave/newave/modelos/expt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/forward.py` & `inewave-1.0.0/inewave/newave/modelos/forward.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/forwarh.py` & `inewave-1.0.0/inewave/newave/modelos/forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/ghmin.py` & `inewave-1.0.0/inewave/newave/modelos/ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/hidr.py` & `inewave-1.0.0/inewave/newave/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/manutt.py` & `inewave-1.0.0/inewave/newave/modelos/manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/modif.py` & `inewave-1.0.0/inewave/newave/modelos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/newavetim.py` & `inewave-1.0.0/inewave/newave/modelos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/nwv_avl_evap.py` & `inewave-1.0.0/inewave/newave/modelos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/nwv_cortes_evap.py` & `inewave-1.0.0/inewave/newave/modelos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/nwv_eco_evap.py` & `inewave-1.0.0/inewave/newave/modelos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/parp.py` & `inewave-1.0.0/inewave/newave/modelos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/parpeol.py` & `inewave-1.0.0/inewave/newave/modelos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/parpvaz.py` & `inewave-1.0.0/inewave/newave/modelos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/patamar.py` & `inewave-1.0.0/inewave/newave/modelos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/penalid.py` & `inewave-1.0.0/inewave/newave/modelos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/pmo.py` & `inewave-1.0.0/inewave/newave/modelos/pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/re.py` & `inewave-1.0.0/inewave/newave/modelos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/ree.py` & `inewave-1.0.0/inewave/newave/modelos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/restricaoeletrica.py` & `inewave-1.0.0/inewave/newave/modelos/restricaoeletrica.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/restricaoenergia.py` & `inewave-1.0.0/inewave/newave/modelos/restricaoenergia.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/restricaovazao.py` & `inewave-1.0.0/inewave/newave/modelos/restricaovazao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/selcor.py` & `inewave-1.0.0/inewave/newave/modelos/selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/shist.py` & `inewave-1.0.0/inewave/newave/modelos/shist.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/sistema.py` & `inewave-1.0.0/inewave/newave/modelos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/term.py` & `inewave-1.0.0/inewave/newave/modelos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/vazaob.py` & `inewave-1.0.0/inewave/newave/modelos/vazaof.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,86 +2,79 @@
 from cfinterface.components.line import Line
 from cfinterface.components.floatfield import FloatField
 from typing import IO
 import pandas as pd  # type: ignore
 import numpy as np  # type: ignore
 
 
-class SecaoDadosVazaob(Section):
+class SecaoDadosVazaof(Section):
     """
     Registro com os dados das séries sintéticas de vazão existentes
-    nos arquivos vazaobXXX.dat.
+    nos arquivos vazaofXXX.dat.
     """
 
     def __init__(self, previous=None, next=None, data=None) -> None:
         super().__init__(previous, next, data)
 
     def __eq__(self, o: object) -> bool:
-        if not isinstance(o, SecaoDadosVazaob):
+        if not isinstance(o, SecaoDadosVazaof):
             return False
-        bloco: SecaoDadosVazaob = o
+        bloco: SecaoDadosVazaof = o
         if not all(
             [
                 isinstance(self.data, pd.DataFrame),
                 isinstance(o.data, pd.DataFrame),
             ]
         ):
             return False
         else:
             return self.data.equals(bloco.data)
 
     def read(
         self,
         file: IO,
         numero_forwards: int = 200,
-        numero_aberturas: int = 20,
         numero_uhes: int = 164,
         numero_estagios: int = 60,
+        numero_estagios_th: int = 12,
         *args,
         **kwargs,
     ):
         numero_registros = (
-            (numero_estagios)
+            (numero_estagios + numero_estagios_th)
             * numero_uhes
             * numero_forwards
-            * numero_aberturas
         )
         self.__linha = Line(
             [
                 FloatField(size=8, starting_position=8 * i)
                 for i in range(numero_registros)
             ],
             storage="BINARY",
         )
         dados = self.__linha.read(file.read(self.__linha.size))
-        indices_estagios = np.arange(1, numero_estagios + 1)
+        indices_estagios = np.arange(
+            1 - numero_estagios_th, numero_estagios + 1
+        )
         estagios_df = np.repeat(
-            indices_estagios, numero_forwards * numero_aberturas * numero_uhes
+            indices_estagios, numero_forwards * numero_uhes
         )
         uhes_df = np.tile(
-            np.repeat(
-                np.arange(1, numero_uhes + 1),
-                numero_forwards * numero_aberturas,
-            ),
-            numero_estagios,
+            np.repeat(np.arange(1, numero_uhes + 1), numero_forwards),
+            numero_estagios + numero_estagios_th,
         )
         forwards_df = np.tile(
-            np.repeat(np.arange(1, numero_forwards + 1), numero_aberturas),
-            numero_uhes * numero_estagios,
-        )
-        aberturas_df = np.tile(
-            np.arange(1, numero_aberturas + 1),
-            numero_uhes * numero_estagios * numero_forwards,
+            np.arange(1, numero_forwards + 1),
+            numero_uhes * (numero_estagios + numero_estagios_th),
         )
         df = pd.DataFrame(
             data={
                 "estagio": estagios_df,
                 "uhe": uhes_df,
                 "serie": forwards_df,
-                "abertura": aberturas_df,
                 "valor": dados,
             }
         )
         self.data = df
 
     def write(self, file: IO, *args, **kwargs):
         dados = self.data["valor"].to_numpy()
```

### Comparing `inewave-0.0.98/inewave/newave/modelos/vazaof.py` & `inewave-1.0.0/inewave/newave/modelos/vazaos.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,79 +2,77 @@
 from cfinterface.components.line import Line
 from cfinterface.components.floatfield import FloatField
 from typing import IO
 import pandas as pd  # type: ignore
 import numpy as np  # type: ignore
 
 
-class SecaoDadosVazaof(Section):
+class SecaoDadosVazaos(Section):
     """
     Registro com os dados das séries sintéticas de vazão existentes
-    nos arquivos vazaofXXX.dat.
+    no arquivo vazaos.dat.
     """
 
     def __init__(self, previous=None, next=None, data=None) -> None:
         super().__init__(previous, next, data)
 
     def __eq__(self, o: object) -> bool:
-        if not isinstance(o, SecaoDadosVazaof):
+        if not isinstance(o, SecaoDadosVazaos):
             return False
-        bloco: SecaoDadosVazaof = o
+        bloco: SecaoDadosVazaos = o
         if not all(
             [
                 isinstance(self.data, pd.DataFrame),
                 isinstance(o.data, pd.DataFrame),
             ]
         ):
             return False
         else:
             return self.data.equals(bloco.data)
 
     def read(
         self,
         file: IO,
-        numero_forwards: int = 200,
+        numero_series: int = 2000,
         numero_uhes: int = 164,
         numero_estagios: int = 60,
         numero_estagios_th: int = 12,
         *args,
         **kwargs,
     ):
         numero_registros = (
             (numero_estagios + numero_estagios_th)
             * numero_uhes
-            * numero_forwards
+            * numero_series
         )
         self.__linha = Line(
             [
                 FloatField(size=8, starting_position=8 * i)
                 for i in range(numero_registros)
             ],
             storage="BINARY",
         )
         dados = self.__linha.read(file.read(self.__linha.size))
         indices_estagios = np.arange(
             1 - numero_estagios_th, numero_estagios + 1
         )
-        estagios_df = np.repeat(
-            indices_estagios, numero_forwards * numero_uhes
-        )
+        estagios_df = np.repeat(indices_estagios, numero_series * numero_uhes)
         uhes_df = np.tile(
-            np.repeat(np.arange(1, numero_uhes + 1), numero_forwards),
+            np.repeat(np.arange(1, numero_uhes + 1), numero_series),
             numero_estagios + numero_estagios_th,
         )
-        forwards_df = np.tile(
-            np.arange(1, numero_forwards + 1),
+        series_df = np.tile(
+            np.arange(1, numero_series + 1),
             numero_uhes * (numero_estagios + numero_estagios_th),
         )
         df = pd.DataFrame(
             data={
                 "estagio": estagios_df,
                 "uhe": uhes_df,
-                "serie": forwards_df,
+                "serie": series_df,
                 "valor": dados,
             }
         )
         self.data = df
 
     def write(self, file: IO, *args, **kwargs):
         dados = self.data["valor"].to_numpy()
```

### Comparing `inewave-0.0.98/inewave/newave/modelos/vazoes.py` & `inewave-1.0.0/inewave/newave/modelos/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modelos/vazpast.py` & `inewave-1.0.0/inewave/newave/modelos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/newave/modif.py` & `inewave-1.0.0/inewave/newave/modif.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,18 +18,14 @@
     TURBMINT,
 )
 
 
 from typing import TypeVar, List, Optional, Union
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Modif(RegisterFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às alterações nas
     configurações das usinas hidroelétricas.
     """
 
@@ -49,35 +45,14 @@
         VMINP,
         VAZMINT,
         VAZMAXT,
         TURBMAXT,
         TURBMINT,
     ]
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="modif.dat") -> "Modif":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="modif.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     def usina(
         self,
         codigo: Optional[int] = None,
         nome: Optional[str] = None,
         df: bool = False,
     ) -> Optional[Union[USINA, List[USINA], pd.DataFrame]]:
         """
```

### Comparing `inewave-0.0.98/inewave/newave/nwv_avl_evap.py` & `inewave-1.0.0/inewave/newave/nwv_cortes_evap.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,34 @@
 from inewave.newave.modelos.blocos.versaomodelo import VersaoModelo
-from inewave.newave.modelos.nwv_avl_evap import TabelaAvlEvap
+from inewave.newave.modelos.nwv_cortes_evap import TabelaCortesEvap
 
 from inewave.newave.modelos.arquivoscsv.arquivocsv import ArquivoCSV
 from typing import Optional
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
-class NwvAvlEvap(ArquivoCSV):
+class NwvCortesEvap(ArquivoCSV):
     """
-    Arquivo com a avaliação da evaporação linear do NEWAVE.
+    Arquivo com os cortes da evaporação linear do NEWAVE.
     """
 
-    BLOCKS = [VersaoModelo, TabelaAvlEvap]
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, arquivo: str = "nwv_avl_evap.csv"
-    ) -> "NwvAvlEvap":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, arquivo))
+    BLOCKS = [VersaoModelo, TabelaCortesEvap]
 
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
         - periodo (`int`)
-        - codigo_usina (`int`)
+        - indice_usina (`int`)
         - nome_usina (`str`)
-        - volume_armazenado_hm3 (`float`)
-        - evaporacao_calculada_hm3 (`float`)
-        - evaporacao_modelo_hm3 (`float`)
-        - desvio_absoluto_hm3 (`float`)
-        - desvio_percentual (`float`)
+        - derivada_cota_area (`float`)
+        - derivada_volume_cota (`float`)
+        - volume_referencia_hm3 (`float`)
+        - evaporacao_referencia_hm3 (`float`)
+        - coeficiente_volume (`float`)
+        - rhs_volume (`float`)
 
         :return: A tabela como um dataframe
         :rtype: pd.DataFrame | None
         """
         return self._tabela()
```

### Comparing `inewave-0.0.98/inewave/newave/nwv_eco_evap.py` & `inewave-1.0.0/inewave/newave/nwv_avl_evap.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,33 @@
 from inewave.newave.modelos.blocos.versaomodelo import VersaoModelo
-from inewave.newave.modelos.nwv_eco_evap import TabelaEcoEvap
+from inewave.newave.modelos.nwv_avl_evap import TabelaAvlEvap
 
 from inewave.newave.modelos.arquivoscsv.arquivocsv import ArquivoCSV
 from typing import Optional
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
-class NwvEcoEvap(ArquivoCSV):
+class NwvAvlEvap(ArquivoCSV):
     """
-    Arquivo com o eco dos dados da evaporação linear do NEWAVE.
+    Arquivo com a avaliação da evaporação linear do NEWAVE.
     """
 
-    BLOCKS = [VersaoModelo, TabelaEcoEvap]
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, arquivo: str = "nwv_eco_evap.csv"
-    ) -> "NwvEcoEvap":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, arquivo))
+    BLOCKS = [VersaoModelo, TabelaAvlEvap]
 
     @property
     def tabela(self) -> Optional[pd.DataFrame]:
         """
         A tabela de dados que está contida no arquivo.
 
         - periodo (`int`)
         - codigo_usina (`int`)
         - nome_usina (`str`)
-        - volume_referencia_hm3 (`float`)
-        - evaporacao_referencia_hm3 (`float`)
-        - coeficiente_evaporacao_mm_mes (`int`)
-        - flag_evaporacao (`int`)
-        - evaporacao_linear (`int`)
-        - tipo_volume_referencia (`int`)
+        - volume_armazenado_hm3 (`float`)
+        - evaporacao_calculada_hm3 (`float`)
+        - evaporacao_modelo_hm3 (`float`)
+        - desvio_absoluto_hm3 (`float`)
+        - desvio_percentual (`float`)
 
         :return: A tabela como um dataframe
         :rtype: pd.DataFrame | None
         """
         return self._tabela()
```

### Comparing `inewave-0.0.98/inewave/newave/parp.py` & `inewave-1.0.0/inewave/newave/parp.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 from inewave.newave.modelos.parp import BlocoCorrelEspacialMensalConfig
 
 from cfinterface.components.block import Block
 from cfinterface.files.blockfile import BlockFile
 from typing import Type, TypeVar, Optional, Any, List
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Parp(BlockFile):
     """
     Armazena os dados de saída do NEWAVE referentes aos modelos e às
     séries sintéticas de energia geradas pelo PAR(p).
 
 
@@ -59,23 +55,14 @@
         self.__correl_cruzada_media = None
         self.__ordem_original_modelo = None
         self.__ordem_final_modelo = None
         self.__coeficientes = None
         self.__correl_espacial_anual = None
         self.__correl_espacial_mensal = None
 
-    @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="parp.dat") -> "Parp":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
     def __rees(self) -> Optional[List[str]]:
         """
         Retorna a lista dos REEs lidos do arquivo.
 
         :return: Os nomes dos REEs
         :rtype: List[str]
         """
```

### Comparing `inewave-0.0.98/inewave/newave/parpeol.py` & `inewave-1.0.0/inewave/newave/parpeol.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,14 @@
 from inewave.newave.modelos.parpeol import BlocoCorrelEspacialMensalConfig
 
 from cfinterface.components.block import Block
 from cfinterface.files.blockfile import BlockFile
 from typing import Type, TypeVar, Optional, Any, List
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Parpeol(BlockFile):
     """
     Armazena os dados de saída do NEWAVE referentes às
     séries sintéticas de ventos geradas pelo PAR(p).
 
     Esta classe lida com informações de saída do NEWAVE e
@@ -42,25 +38,14 @@
         self.__series_ventos = None
         self.__correl_series_ventos = None
         self.__series_ruido = None
         self.__correl_series_ruido = None
         self.__correl_espacial_anual = None
         self.__correl_espacial_mensal = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="parpeol.dat"
-    ) -> "Parpeol":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
     def __uees(self) -> Optional[List[str]]:
         """
         Retorna a lista das UEEs lidos do arquivo.
 
         :return: Os nomes das UEEs
         :rtype: List[str]
         """
```

### Comparing `inewave-0.0.98/inewave/newave/parpvaz.py` & `inewave-1.0.0/inewave/newave/parpvaz.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 from inewave.newave.modelos.parpvaz import BlocoCorrelEspacialAnualMensalUHE
 
 from cfinterface.components.block import Block
 from cfinterface.files.blockfile import BlockFile
 from typing import Type, TypeVar, Optional, Any, List
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Parpvaz(BlockFile):
     """
     Armazena os dados de saída do NEWAVE referentes aos modelos e às
     séries sintéticas de vazões geradas pelo PAR(p).
 
 
@@ -50,25 +46,14 @@
         self.__series_ruido = None
         self.__correl_series_ruido = None
         self.__ordem_original_modelo = None
         self.__ordem_final_modelo = None
         self.__coeficientes = None
         self.__correl_espacial_anual_mensal = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="parpvaz.dat"
-    ) -> "Parpvaz":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
     def __uhes(self) -> Optional[List[str]]:
         """
         Retorna a lista das UHEs lidos do arquivo.
 
         :return: Os nomes das UHEs
         :rtype: List[str]
         """
```

### Comparing `inewave-0.0.98/inewave/newave/patamar.py` & `inewave-1.0.0/inewave/newave/sistema.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,181 +1,160 @@
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
 from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
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
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="patamar.dat"
-    ) -> "Patamar":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="patamar.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
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
-        b = self.data.get_sections_of_type(BlocoNumeroPatamares)
-        if isinstance(b, BlocoNumeroPatamares):
+        b = self.data.get_sections_of_type(BlocoNumeroPatamaresDeficit)
+        if isinstance(b, BlocoNumeroPatamaresDeficit):
             return b.data
         return None
 
-    @numero_patamares.setter
-    def numero_patamares(self, n: int):
-        b = self.data.get_sections_of_type(BlocoNumeroPatamares)
-        if isinstance(b, BlocoNumeroPatamares):
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
 
-        - ano (`int`)
-        - janeiro (`float`)
-        - fevereiro (`float`)
+        - codigo_submercado (`int`)
+        - nome_submercado (`str`)
+        - ficticio (`int`)
+        - custo_deficit_patamar_1 (`float`)
         - ...
-        - dezembro (`float`)
+        - custo_deficit_patamar_5 (`float`)
+        - corte_patamar_1 (`float`)
+        - ...
+        - corte_patamar_5 (`float`)
 
         :return: A duração por mês em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.data.get_sections_of_type(BlocoDuracaoPatamar)
-        if isinstance(b, BlocoDuracaoPatamar):
+        b = self.data.get_sections_of_type(BlocoCustosDeficit)
+        if isinstance(b, BlocoCustosDeficit):
             return b.data
         return None
 
-    @duracao_mensal_patamares.setter
-    def duracao_mensal_patamares(self, df: pd.DataFrame):
-        b = self.data.get_sections_of_type(BlocoDuracaoPatamar)
-        if isinstance(b, BlocoDuracaoPatamar):
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
 
+        - submercado_de (`int`)
+        - submercado_para (`int`)
+        - sentido (`int`)
         - ano (`int`)
         - janeiro (`float`)
-        - fevereiro (`float`)
         - ...
         - dezembro (`float`)
 
-        :return: A carga por mês em um DataFrame.
+        :return: A duração por mês em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.data.get_sections_of_type(BlocoCargaPatamar)
-        if isinstance(b, BlocoCargaPatamar):
+        b = self.data.get_sections_of_type(BlocoIntercambioSubsistema)
+        if isinstance(b, BlocoIntercambioSubsistema):
             return b.data
         return None
 
-    @carga_patamares.setter
-    def carga_patamares(self, df: pd.DataFrame):
-        b = self.data.get_sections_of_type(BlocoCargaPatamar)
-        if isinstance(b, BlocoCargaPatamar):
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
 
-        - submercado_de (`str`)
-        - submercado_para (`str`)
+        - submercado (`int`)
         - ano (`int`)
         - janeiro (`float`)
-        - fevereiro (`float`)
         - ...
         - dezembro (`float`)
 
         :return: A carga por mês em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.data.get_sections_of_type(BlocoIntercambioPatamarSubsistemas)
-        if isinstance(b, BlocoIntercambioPatamarSubsistemas):
+        b = self.data.get_sections_of_type(BlocoMercadoEnergiaSistema)
+        if isinstance(b, BlocoMercadoEnergiaSistema):
             return b.data
         return None
 
-    @intercambio_patamares.setter
-    def intercambio_patamares(self, df: pd.DataFrame):
-        b = self.data.get_sections_of_type(BlocoIntercambioPatamarSubsistemas)
-        if isinstance(b, BlocoIntercambioPatamarSubsistemas):
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
 
         - submercado (`int`)
-        - patamar (`int`)
         - bloco (`int`)
+        - fonte (`str`)
         - ano (`int`)
         - janeiro (`float`)
-        - fevereiro (`float`)
         - ...
         - dezembro (`float`)
 
-        :return: Os valores por mês em um DataFrame.
+        :return: A carga por mês em um DataFrame.
         :rtype: pd.DataFrame | None
         """
-        b = self.data.get_sections_of_type(BlocoUsinasNaoSimuladas)
-        if isinstance(b, BlocoUsinasNaoSimuladas):
+        b = self.data.get_sections_of_type(BlocoGeracaoUsinasNaoSimuladas)
+        if isinstance(b, BlocoGeracaoUsinasNaoSimuladas):
             return b.data
         return None
 
-    @usinas_nao_simuladas.setter
-    def usinas_nao_simuladas(self, df: pd.DataFrame):
-        b = self.data.get_sections_of_type(BlocoUsinasNaoSimuladas)
-        if isinstance(b, BlocoUsinasNaoSimuladas):
+    @geracao_usinas_nao_simuladas.setter
+    def geracao_usinas_nao_simuladas(self, df: pd.DataFrame):
+        b = self.data.get_sections_of_type(BlocoGeracaoUsinasNaoSimuladas)
+        if isinstance(b, BlocoGeracaoUsinasNaoSimuladas):
             b.data = df
```

### Comparing `inewave-0.0.98/inewave/newave/pmo.py` & `inewave-1.0.0/inewave/newave/pmo.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 from inewave.newave.modelos.pmo import BlocoCustoOperacaoTotalPMO
 from inewave.newave.modelos.pmo import BlocoProdutibilidadesConfiguracaoPMO
 
 from cfinterface.files.blockfile import BlockFile
 from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Pmo(BlockFile):
     """
     Armazena os dados de entrada do NEWAVE referentes ao
     acompanhamento do programa.
 
     Esta classe lida com as informações de entrada fornecidas ao
@@ -41,23 +37,14 @@
         BlocoMARSPMO,
         BlocoRiscoDeficitENSPMO,
         BlocoCustoOperacaoPMO,
         BlocoCustoOperacaoTotalPMO,
         BlocoProdutibilidadesConfiguracaoPMO,
     ]
 
-    @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="pmo.dat") -> "Pmo":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
     @property
     def eafpast_tendencia_hidrologica(self) -> Optional[pd.DataFrame]:
         """
         Energias afluentes passadas por REE para análise da tendência
         hidrológica, em relação à primeira configuração do sistema,
         em MWmes.
```

### Comparing `inewave-0.0.98/inewave/newave/ree.py` & `inewave-1.0.0/inewave/newave/ree.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 import pandas as pd  # type: ignore
 
 from inewave.newave.modelos.ree import (
     BlocoReesSubmercados,
     BlocoFicticiasIndividualizado,
 )
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Ree(SectionFile):
     """
     Armazena os dados de entrada do NEWAVE referentes às configurações
     dos REEs.
 
     """
@@ -24,35 +20,14 @@
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = [
         BlocoReesSubmercados,
         BlocoFicticiasIndividualizado,
     ]
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="ree.dat") -> "Ree":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ree.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     @property
     def rees(self) -> Optional[pd.DataFrame]:
         """
         Tabela com os REES e os submercados
 
         - codigo (`int`)
         - nome (`str`)
```

### Comparing `inewave-0.0.98/inewave/nwlistcf/arquivos.py` & `inewave-1.0.0/inewave/nwlistcf/arquivos.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from inewave.nwlistcf.modelos.arquivos import BlocoNomesArquivos
 
 from cfinterface.files.sectionfile import SectionFile
 
 from typing import List, TypeVar, Optional
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Arquivos(SectionFile):
     """
     Armazena os dados de entrada do NWLISTCF referentes ao arquivo
     `arquivos.dat`.
 
     Esta classe lida com informações de entrada do NWLISTCF e
@@ -21,34 +17,14 @@
 
     """
 
     T = TypeVar("T")
 
     SECTIONS = [BlocoNomesArquivos]
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="arquivos.dat"
-    ) -> "Arquivos":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="arquivos.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     def __le_nome_por_indice(self, indice: int) -> Optional[str]:
         b = self.data.get_sections_of_type(BlocoNomesArquivos)
         if isinstance(b, BlocoNomesArquivos):
             if indice in b.data.index:
                 dado = b.data.iloc[indice, 1]
                 if isinstance(dado, str):
                     return dado
```

### Comparing `inewave-0.0.98/inewave/nwlistcf/caso.py` & `inewave-1.0.0/inewave/nwlistcf/caso.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,26 @@
 from inewave.nwlistcf.modelos.caso import NomeCaso
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import TypeVar, Optional
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Caso(SectionFile):
     """
     Armazena os dados de entrada do NWLISTCF referentes ao caso de estudo.
 
     Esta classe lida com informações de entrada fornecidas ao NWLISTCF e
     que podem ser modificadas através do arquivo `caso.dat`.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS = [NomeCaso]
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="caso.dat") -> "Caso":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="caso.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
-
     @property
     def arquivos(self) -> Optional[str]:
         """
         Caminho para o arquivo `arquivos.dat` de entrada do NWLISTCF.
 
         :return: O caminho para o arquivo
         :rtype: str | None
```

### Comparing `inewave-0.0.98/inewave/nwlistcf/estados.py` & `inewave-1.0.0/inewave/nwlistcf/estados.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from inewave.nwlistcf.modelos.estados import EstadosPeriodoNwlistcf
 
 from cfinterface.files.blockfile import BlockFile
 from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Estados(BlockFile):
     """
     Armazena os dados dos estados visitados pelo NEWAVE existentes
     no arquivo `estados.rel` do NWLISTCF.
 
     Esta classe armazena os estados de cada uma das variáveis envolvidas
@@ -24,25 +20,14 @@
 
     BLOCKS = [EstadosPeriodoNwlistcf]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__estados_periodos = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="estados.rel"
-    ) -> "Estados":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
     def __monta_tabela_estados(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(EstadosPeriodoNwlistcf):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
```

### Comparing `inewave-0.0.98/inewave/nwlistcf/modelos/arquivos.py` & `inewave-1.0.0/inewave/nwlistcf/modelos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistcf/modelos/caso.py` & `inewave-1.0.0/inewave/nwlistcf/modelos/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistcf/modelos/estados.py` & `inewave-1.0.0/inewave/nwlistcf/modelos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistcf/modelos/nwlistcfdat.py` & `inewave-1.0.0/inewave/nwlistcf/modelos/nwlistcfdat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistcf/modelos/nwlistcfrel.py` & `inewave-1.0.0/inewave/nwlistcf/modelos/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistcf/nwlistcfdat.py` & `inewave-1.0.0/inewave/nwlistcf/nwlistcfdat.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,44 +2,26 @@
     PeriodoImpressaoCortesEstados,
     OpcoesImpressao,
 )
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import TypeVar, Optional, List
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Nwlistcfdat(SectionFile):
     """
     Armazena os dados de entrada para a execução do programa auxiliar
     NWLISTCF, existentes no arquivo `nwlistcf.dat`.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS = [PeriodoImpressaoCortesEstados, OpcoesImpressao]
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="nwlistcf.dat"
-    ) -> "Nwlistcfdat":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
     @property
     def mes_inicio(self) -> Optional[int]:
         """
         O mês (calendário) de início para impressão dos cortes
 
         :return: O mês calendário de início
         :rtype: Optional[int] | None
```

### Comparing `inewave-0.0.98/inewave/nwlistcf/nwlistcfrel.py` & `inewave-1.0.0/inewave/nwlistcf/nwlistcfrel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from inewave.nwlistcf.modelos.nwlistcfrel import CortesPeriodoNwlistcf
 
 from cfinterface.files.blockfile import BlockFile
 from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Nwlistcfrel(BlockFile):
     """
     Armazena os dados dos cortes construídos pelo NEWAVE existentes
     no arquivo `nwlistcf.rel` do NWLISTCF.
 
     Esta classe armazena os cortes da FCF de cada uma das variáveis,
@@ -23,25 +19,14 @@
 
     BLOCKS = [CortesPeriodoNwlistcf]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__cortes_periodos = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="nwlistcf.rel"
-    ) -> "Nwlistcfrel":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
     def __monta_tabela_cortes(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(CortesPeriodoNwlistcf):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
```

### Comparing `inewave-0.0.98/inewave/nwlistop/__init__.py` & `inewave-1.0.0/inewave/nwlistop/__init__.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/depminuh.py` & `inewave-1.0.0/inewave/nwlistop/geol.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,22 @@
 from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
     ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.depminuh import DepminAnos
+from inewave.nwlistop.modelos.geol import GEAnos
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
-class Depminuh(ArquivoUsinaPatamar):
+class Geol(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes À violação de defluência
-    mínima da usina.
+    Armazena os dados das saídas referentes à geração eólica total
+    por patamar, por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `depminuh00x.out`, onde x varia conforme
-    a usina em questão.
+    NWLISTOP e reproduzidas nos `geol00x.out`, onde x varia conforme o
+    PEE em questão.
 
     """
 
     BLOCKS = [
         Usina,
-        DepminAnos,
+        GEAnos,
     ]
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="depminuh001.out"
-    ) -> "Depminuh":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.98/inewave/nwlistop/dlpptbmaxm.py` & `inewave-1.0.0/inewave/nwlistop/cmarg.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,22 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.cmarg import CmargsAnos
 from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
     ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.dlppdfmax import DLPPdfmaxAnos
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
-class Dlpptbmaxm(ArquivoSubmercadoPatamar):
+class Cmarg(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes à violação das restrições LPP
-    de turbinamento máximo por patamar, por Submercado.
+    Armazena os dados das saídas referentes aos custos marginais de operação
+    por patamar, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `dlpptbmax00x.out`, onde x varia conforme o
-    Submercado em questão.
+    NWLISTOP e reproduzidas nos `cmarg00x.out`, onde x varia conforme o
+    submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        DLPPdfmaxAnos,
+        CmargsAnos,
     ]
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="dlpptbmaxm001.out"
-    ) -> "Dlpptbmaxm":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.98/inewave/nwlistop/eafm.py` & `inewave-1.0.0/inewave/nwlistop/earmfm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,22 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
     ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.eafm import EafsAnos
+from inewave.nwlistop.modelos.earmfm import EarmsAnos
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
-class Eafm(ArquivoSubmercado):
+class Earmfm(ArquivoSubmercado):
     """
     Armazena os dados das saídas referentes às energias
-    afluentes, por Submercado.
+    armazenadas finais, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `eaf00x.out`, onde x varia conforme o
-    Submercado em questão.
+    NWLISTOP e reproduzidas nos `earmfm00x.out`, onde x varia conforme o
+    submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        EafsAnos,
+        EarmsAnos,
     ]
-
-    @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="eafm001.out") -> "Eafm":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.98/inewave/nwlistop/geolsin.py` & `inewave-1.0.0/inewave/nwlistop/ghiduh.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,21 @@
-from inewave.nwlistop.modelos.geolsin import GEAnos
-
-from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
-    ArquivoSINPatamar,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
+from inewave.nwlistop.modelos.ghiduh import GhidAnos
 
 
-class Geolsin(ArquivoSINPatamar):
+class Ghiduh(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à geração eólica total
-    para o SIN.
+    Armazena os dados das saídas referentes à geração hidráulica por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `geolsin.out`.
+    NWLISTOP e reproduzidas nos `ghiduh00x.out`, onde x varia conforme a
+    usina em questão.
+
     """
 
     BLOCKS = [
-        GEAnos,
+        Usina,
+        GhidAnos,
     ]
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="geolsin.out"
-    ) -> "Geolsin":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.98/inewave/nwlistop/ghtot.py` & `inewave-1.0.0/inewave/nwlistop/deficit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,22 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
-    ArquivoREEPatamar,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
+    ArquivoSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.ghtot import GHAnos
+from inewave.nwlistop.modelos.defsin import DefAnos
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
-class Ghtot(ArquivoREEPatamar):
+class Def(ArquivoSubmercadoPatamar):
     """
     Armazena os dados das saídas referentes à geração hidraulica total
-    por patamar, por REE.
+    por patamar, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghtot00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas nos `ghtotm00x.out`, onde x varia conforme o
+    submercado em questão.
 
     """
 
     BLOCKS = [
-        REE,
-        GHAnos,
+        Submercado,
+        DefAnos,
     ]
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghtot001.out"
-    ) -> "Ghtot":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.98/inewave/nwlistop/gttot.py` & `inewave-1.0.0/inewave/nwlistop/verturbm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,22 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
-    ArquivoSubmercadoPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.gttot import GTAnos
+from inewave.nwlistop.modelos.verturbm import VertAnos
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
-class Gttot(ArquivoSubmercadoPatamar):
+class Verturbm(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes à geração térmica total
-    por patamar, por Submercado.
+    Armazena os dados das saídas referentes às energias
+    vertidas, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `gttot00x.out`, onde x varia conforme o
-    Submercado em questão.
+    NWLISTOP e reproduzidas nos `vertub00x.out`, onde x varia conforme o
+    REE em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        GTAnos,
+        VertAnos,
     ]
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="gttot001.out"
-    ) -> "Gttot":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.98/inewave/nwlistop/invadem.py` & `inewave-1.0.0/inewave/nwlistop/ghmax.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,22 @@
-from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
-    ArquivoSubmercado,
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
+    ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.invade import InvadeAnos
+from inewave.nwlistop.modelos.ghmax import GHAnos
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
-class Invadem(ArquivoSubmercado):
+class Ghmax(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes às violações da CAR
-    , por Submercado.
+    Armazena os dados das saídas referentes à geração hidraulica máxima
+    por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `invadem00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `ghmax00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
-        Submercado,
-        InvadeAnos,
+        REE,
+        GHAnos,
     ]
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="invadem001.out"
-    ) -> "Invadem":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.98/inewave/nwlistop/mediasmerc.py` & `inewave-1.0.0/inewave/nwlistop/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/mediassin.py` & `inewave-1.0.0/inewave/nwlistop/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py` & `inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,14 @@
 
     BLOCKS = [Submercado, ValoresClasseTermicaSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoClasseTermicaSubmercadoPatamar":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
-        self.write(diretorio, nome_arquivo)
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresClasseTermicaSeriePatamar):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
```

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py` & `inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,23 +17,14 @@
 
     BLOCKS = [ParSubmercados, ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoParSubmercadoPatamar":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
-        self.write(diretorio, nome_arquivo)
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresSeriePatamar):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
```

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoree.py` & `inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,30 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.blocos.valoresserie import (
     ValoresSerie,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
 from typing import TypeVar, Optional
 
 
-class ArquivoREE(BlockFile):
+class ArquivoSubmercado(BlockFile):
     """
-    Armazena os dados das saídas por REE.
+    Armazena os dados das saídas por submercado.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [REE, ValoresSerie]
+    BLOCKS = [Submercado, ValoresSerie]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoREE":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
-        self.write(diretorio, nome_arquivo)
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresSerie):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
@@ -56,18 +47,18 @@
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
 
     @property
-    def ree(self) -> Optional[str]:
+    def submercado(self) -> Optional[str]:
         """
-        O REE associado ao arquivo lido.
+        O submercado associado ao arquivo lido.
 
-        :return: O nome do ree
+        :return: Os nome do submercado
         :rtype: str
         """
-        b = self.data.get_blocks_of_type(REE)
-        if isinstance(b, REE):
+        b = self.data.get_blocks_of_type(Submercado)
+        if isinstance(b, Submercado):
             return b.data
         return None
```

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py` & `inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,30 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
 from typing import TypeVar, Optional
 
 
-class ArquivoREEPatamar(BlockFile):
+class ArquivoSubmercadoPatamar(BlockFile):
     """
-    Armazena os dados das saídas por patamar, por REE.
+    Armazena os dados das saídas por patamar, por submercado.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [REE, ValoresSeriePatamar]
+    BLOCKS = [Submercado, ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoREEPatamar":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
-        self.write(diretorio, nome_arquivo)
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresSeriePatamar):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
@@ -57,18 +48,18 @@
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
 
     @property
-    def ree(self) -> Optional[str]:
+    def submercado(self) -> Optional[str]:
         """
-        O REE associado ao arquivo lido.
+        O submercado associado ao arquivo lido.
 
-        :return: O nome do REE
+        :return: Os nome do submercado
         :rtype: str
         """
-        b = self.data.get_blocks_of_type(REE)
-        if isinstance(b, REE):
+        b = self.data.get_blocks_of_type(Submercado)
+        if isinstance(b, Submercado):
             return b.data
         return None
```

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,33 @@
-from inewave.nwlistop.modelos.blocos.valoresserie import (
-    ValoresSerie,
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
+    ValoresSeriePatamar,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
 from typing import TypeVar, Optional
 
 
-class ArquivoSIN(BlockFile):
+class ArquivoREEPatamar(BlockFile):
     """
-    Armazena os dados das saídas por submercado.
+    Armazena os dados das saídas por patamar, por REE.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [ValoresSerie]
+    BLOCKS = [REE, ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoSIN":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
-        self.write(diretorio, nome_arquivo)
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
@@ -44,16 +36,30 @@
     @property
     def valores(self) -> Optional[pd.DataFrame]:
         """
         Tabela com os valores por patamar, por série e
         por mês/ano de estudo.
 
         - data (`datetime`)
+        - patamar (`str`)
         - serie (`str`)
         - valor (`float`)
 
         :return: A tabela dos valores por patamar.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
+
+    @property
+    def ree(self) -> Optional[str]:
+        """
+        O REE associado ao arquivo lido.
+
+        :return: O nome do REE
+        :rtype: str
+        """
+        b = self.data.get_blocks_of_type(REE)
+        if isinstance(b, REE):
+            return b.data
+        return None
```

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py` & `inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,30 @@
+from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
 from typing import TypeVar, Optional
 
 
-class ArquivoSINPatamar(BlockFile):
+class ArquivoUsinaPatamar(BlockFile):
     """
-    Armazena os dados das saídas por submercado.
+    Armazena os dados das saídas por patamar, por Usina.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [ValoresSeriePatamar]
+    BLOCKS = [Usina, ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoSINPatamar":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
-        self.write(diretorio, nome_arquivo)
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresSeriePatamar):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
@@ -54,7 +46,20 @@
 
         :return: A tabela dos valores por patamar.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
+
+    @property
+    def usina(self) -> Optional[str]:
+        """
+        A usina associada ao arquivo lido.
+
+        :return: O nome da usina
+        :rtype: str
+        """
+        b = self.data.get_blocks_of_type(Usina)
+        if isinstance(b, Usina):
+            return b.data
+        return None
```

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivousina.py` & `inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivoree.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,30 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.blocos.valoresserie import (
     ValoresSerie,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
 from typing import TypeVar, Optional
 
 
-class ArquivoUsina(BlockFile):
+class ArquivoREE(BlockFile):
     """
-    Armazena os dados das saídas por usina.
+    Armazena os dados das saídas por REE.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [Usina, ValoresSerie]
+    BLOCKS = [REE, ValoresSerie]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoUsina":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
-        self.write(diretorio, nome_arquivo)
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresSerie):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
@@ -56,18 +47,18 @@
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
 
     @property
-    def usina(self) -> Optional[str]:
+    def ree(self) -> Optional[str]:
         """
-        A usina associada ao arquivo lido.
+        O REE associado ao arquivo lido.
 
-        :return: O nome da usina
+        :return: O nome do ree
         :rtype: str
         """
-        b = self.data.get_blocks_of_type(Usina)
-        if isinstance(b, Usina):
+        b = self.data.get_blocks_of_type(REE)
+        if isinstance(b, REE):
             return b.data
         return None
```

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py` & `inewave-1.0.0/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,29 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
 from inewave.nwlistop.modelos.blocos.valoresseriepatamar import (
     ValoresSeriePatamar,
 )
 
 from cfinterface.files.blockfile import BlockFile
 import pandas as pd  # type: ignore
 from typing import TypeVar, Optional
 
 
-class ArquivoUsinaPatamar(BlockFile):
+class ArquivoSINPatamar(BlockFile):
     """
-    Armazena os dados das saídas por patamar, por Usina.
+    Armazena os dados das saídas por submercado.
     """
 
     T = TypeVar("T")
 
-    BLOCKS = [Usina, ValoresSeriePatamar]
+    BLOCKS = [ValoresSeriePatamar]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__valores = None
 
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="arq.out"
-    ) -> "ArquivoUsinaPatamar":
-        return cls.read(diretorio, nome_arquivo)
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="arq.out"):
-        self.write(diretorio, nome_arquivo)
-
     def __monta_tabela(self) -> pd.DataFrame:
         df = None
         for b in self.data.of_type(ValoresSeriePatamar):
             dados = b.data
             if dados is None:
                 continue
             elif df is None:
@@ -55,20 +45,7 @@
 
         :return: A tabela dos valores por patamar.
         :rtype: pd.DataFrame | None
         """
         if self.__valores is None:
             self.__valores = self.__monta_tabela()
         return self.__valores
-
-    @property
-    def usina(self) -> Optional[str]:
-        """
-        A usina associada ao arquivo lido.
-
-        :return: O nome da usina
-        :rtype: str
-        """
-        b = self.data.get_blocks_of_type(Usina)
-        if isinstance(b, Usina):
-            return b.data
-        return None
```

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/blocos/parsubmercados.py` & `inewave-1.0.0/inewave/nwlistop/modelos/blocos/parsubmercados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/blocos/ree.py` & `inewave-1.0.0/inewave/nwlistop/modelos/blocos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/blocos/submercado.py` & `inewave-1.0.0/inewave/nwlistop/modelos/blocos/submercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/blocos/usina.py` & `inewave-1.0.0/inewave/nwlistop/modelos/blocos/usina.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py` & `inewave-1.0.0/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresserie.py` & `inewave-1.0.0/inewave/nwlistop/modelos/blocos/valoresserie.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py` & `inewave-1.0.0/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/cdef.py` & `inewave-1.0.0/inewave/nwlistop/modelos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/cdefsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/cmarg.py` & `inewave-1.0.0/inewave/nwlistop/modelos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/cmargmed.py` & `inewave-1.0.0/inewave/nwlistop/modelos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/coper.py` & `inewave-1.0.0/inewave/nwlistop/modelos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/corteolm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/cterm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/ctermsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/def.py` & `inewave-1.0.0/inewave/nwlistop/modelos/def.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/defsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/depminuh.py` & `inewave-1.0.0/inewave/nwlistop/modelos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/dflppdfmaxm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/dflppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/dflpptbmaxm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/dflpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/dfphauh.py` & `inewave-1.0.0/inewave/nwlistop/modelos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/dlppdfmax.py` & `inewave-1.0.0/inewave/nwlistop/modelos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/dlppdfmaxs.py` & `inewave-1.0.0/inewave/nwlistop/modelos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/dlpptbmax.py` & `inewave-1.0.0/inewave/nwlistop/modelos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/dlpptbmaxs.py` & `inewave-1.0.0/inewave/nwlistop/modelos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/dtbmax.py` & `inewave-1.0.0/inewave/nwlistop/modelos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/dtbmin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/dvazmax.py` & `inewave-1.0.0/inewave/nwlistop/modelos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/eaf.py` & `inewave-1.0.0/inewave/nwlistop/modelos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/eafb.py` & `inewave-1.0.0/inewave/nwlistop/modelos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/eafbm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/eafbsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/eafm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/earmf.py` & `inewave-1.0.0/inewave/nwlistop/modelos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/earmfm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/earmfp.py` & `inewave-1.0.0/inewave/nwlistop/modelos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/earmfpm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/earmfpsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/earmfsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/evert.py` & `inewave-1.0.0/inewave/nwlistop/modelos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/evertm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/evertsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/exces.py` & `inewave-1.0.0/inewave/nwlistop/modelos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/excessin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/fteolm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/fteolsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/geol.py` & `inewave-1.0.0/inewave/nwlistop/modelos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/geolm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/geolsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/ghiduh.py` & `inewave-1.0.0/inewave/nwlistop/modelos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/ghmax.py` & `inewave-1.0.0/inewave/nwlistop/modelos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/ghmaxm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/ghmaxmr.py` & `inewave-1.0.0/inewave/nwlistop/modelos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/ghmaxr.py` & `inewave-1.0.0/inewave/nwlistop/modelos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/ghmaxrsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/ghmaxsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/ghtot.py` & `inewave-1.0.0/inewave/nwlistop/modelos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/ghtotm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/ghtotsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/gtert.py` & `inewave-1.0.0/inewave/nwlistop/modelos/gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/gttot.py` & `inewave-1.0.0/inewave/nwlistop/modelos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/gttotsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/intercambio.py` & `inewave-1.0.0/inewave/nwlistop/modelos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/invade.py` & `inewave-1.0.0/inewave/nwlistop/modelos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/invadem.py` & `inewave-1.0.0/inewave/nwlistop/modelos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/mediasmerc.py` & `inewave-1.0.0/inewave/nwlistop/modelos/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/mediassin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/mercl.py` & `inewave-1.0.0/inewave/nwlistop/modelos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/merclsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/nwlistopdat.py` & `inewave-1.0.0/inewave/nwlistop/modelos/nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/perdf.py` & `inewave-1.0.0/inewave/nwlistop/modelos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/perdfm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/perdfsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/qafluh.py` & `inewave-1.0.0/inewave/nwlistop/modelos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/qincruh.py` & `inewave-1.0.0/inewave/nwlistop/modelos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/rhslppdf.py` & `inewave-1.0.0/inewave/nwlistop/modelos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/rhslpptb.py` & `inewave-1.0.0/inewave/nwlistop/modelos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/vagua.py` & `inewave-1.0.0/inewave/nwlistop/modelos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/varmpuh.py` & `inewave-1.0.0/inewave/nwlistop/modelos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/varmuh.py` & `inewave-1.0.0/inewave/nwlistop/modelos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/vento.py` & `inewave-1.0.0/inewave/nwlistop/modelos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/vertuh.py` & `inewave-1.0.0/inewave/nwlistop/modelos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/verturb.py` & `inewave-1.0.0/inewave/nwlistop/modelos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/verturbm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/verturbsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/vevmin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/vevminm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/vevminsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/vghmin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/vghminm.py` & `inewave-1.0.0/inewave/nwlistop/modelos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/vghminsin.py` & `inewave-1.0.0/inewave/nwlistop/modelos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/vghminuh.py` & `inewave-1.0.0/inewave/nwlistop/modelos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/modelos/vturuh.py` & `inewave-1.0.0/inewave/nwlistop/modelos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/inewave/nwlistop/nwlistopdat.py` & `inewave-1.0.0/inewave/nwlistop/nwlistopdat.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,26 @@
 from inewave.nwlistop.modelos.nwlistopdat import (
     BlocoDadosNwlistop,
 )
 
 from cfinterface.files.sectionfile import SectionFile
 from typing import TypeVar, Optional, List
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Nwlistopdat(SectionFile):
     """
     Armazena os dados de entrada para a execução do programa auxiliar
     NWLISTOP, existentes no arquivo `nwlistop.dat`.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS = [BlocoDadosNwlistop]
 
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="nwlistop.dat"
-    ) -> "Nwlistopdat":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
-
     @property
     def opcao(self) -> Optional[int]:
         """
         A opção de execução do programa nwlistop.
 
         :return: O flag de opção
         :rtype: Optional[int] | None
```

### Comparing `inewave-0.0.98/inewave/nwlistop/varmpuh.py` & `inewave-1.0.0/inewave/nwlistop/ghtot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,22 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousina import (
-    ArquivoUsina,
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
+    ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.varmpuh import VarmAnos
+from inewave.nwlistop.modelos.ghtot import GHAnos
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
-class Varmpuh(ArquivoUsina):
+class Ghtot(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes aos armazenamentos em
-    percentual por usina.
+    Armazena os dados das saídas referentes à geração hidraulica total
+    por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `varmpuh00x.out`, onde x varia conforme a
-    usina em questão.
+    NWLISTOP e reproduzidas nos `ghtot00x.out`, onde x varia conforme o
+    REE em questão.
 
     """
 
     BLOCKS = [
-        Usina,
-        VarmAnos,
+        REE,
+        GHAnos,
     ]
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="varmpuh001.out"
-    ) -> "Varmpuh":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.98/inewave/nwlistop/verturbm.py` & `inewave-1.0.0/inewave/nwlistop/ghmaxr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,22 @@
-from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
-    ArquivoSubmercado,
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
+    ArquivoREEPatamar,
 )
-from inewave.nwlistop.modelos.verturbm import VertAnos
+from inewave.nwlistop.modelos.ghmaxr import GHAnos
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
 
-
-class Verturbm(ArquivoSubmercado):
+class Ghmaxr(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes às energias
-    vertidas, por submercado.
+    Armazena os dados das saídas referentes à geração hidraulica máxima
+    considerando restrições elétricas por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vertub00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `ghmax00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
-        Submercado,
-        VertAnos,
+        REE,
+        GHAnos,
     ]
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="verturbm001.out"
-    ) -> "Verturbm":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.98/inewave/nwlistop/vevmin.py` & `inewave-1.0.0/inewave/nwlistop/vevmin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from inewave.nwlistop.modelos.blocos.ree import REE
 from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
 from inewave.nwlistop.modelos.vevmin import VevminAnos
 
-# Para compatibilidade - até versão 1.0.0
-from os.path import join
-import warnings
-
 
 class Vevmin(ArquivoREE):
     """
     Armazena os dados das saídas referentes às violações da meta
     de energia da vazão mínima, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
@@ -18,18 +14,7 @@
 
     """
 
     BLOCKS = [
         REE,
         VevminAnos,
     ]
-
-    @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vevmin001.out"
-    ) -> "Vevmin":
-        msg = (
-            "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
-            + " na versão 1.0.0 - use o método read(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.98/inewave.egg-info/PKG-INFO` & `inewave-1.0.0/inewave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 0.0.98
+Version: 1.0.0
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-0.0.98/inewave.egg-info/SOURCES.txt` & `inewave-1.0.0/inewave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/setup.py` & `inewave-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/adterm.py` & `inewave-1.0.0/tests/mocks/arquivos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/agrint.py` & `inewave-1.0.0/tests/mocks/arquivos/agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/arquivos.py` & `inewave-1.0.0/tests/mocks/arquivos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/arquivos_nwlistcf.py` & `inewave-1.0.0/tests/mocks/arquivos/arquivos_nwlistcf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/avl_cortesfpha_nwv.py` & `inewave-1.0.0/tests/mocks/arquivos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/avl_desvfpha_s.py` & `inewave-1.0.0/tests/mocks/arquivos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/avl_desvfpha_v_q.py` & `inewave-1.0.0/tests/mocks/arquivos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/cadic.py` & `inewave-1.0.0/tests/mocks/arquivos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/cdef.py` & `inewave-1.0.0/tests/mocks/arquivos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/cdefsin.py` & `inewave-1.0.0/tests/mocks/arquivos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/clast.py` & `inewave-1.0.0/tests/mocks/arquivos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/cmarg.py` & `inewave-1.0.0/tests/mocks/arquivos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/cmargmed.py` & `inewave-1.0.0/tests/mocks/arquivos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/confhd.py` & `inewave-1.0.0/tests/mocks/arquivos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/conft.py` & `inewave-1.0.0/tests/mocks/arquivos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/coper.py` & `inewave-1.0.0/tests/mocks/arquivos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/corteolm.py` & `inewave-1.0.0/tests/mocks/arquivos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/cterm.py` & `inewave-1.0.0/tests/mocks/arquivos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ctermsin.py` & `inewave-1.0.0/tests/mocks/arquivos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/curva.py` & `inewave-1.0.0/tests/mocks/arquivos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/cvar.py` & `inewave-1.0.0/tests/mocks/arquivos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/deficit.py` & `inewave-1.0.0/tests/mocks/arquivos/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/defsin.py` & `inewave-1.0.0/tests/mocks/arquivos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/depminuh.py` & `inewave-1.0.0/tests/mocks/arquivos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dfphauh.py` & `inewave-1.0.0/tests/mocks/arquivos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dger.py` & `inewave-1.0.0/tests/mocks/arquivos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dlppdfmax.py` & `inewave-1.0.0/tests/mocks/arquivos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dlppdfmaxm.py` & `inewave-1.0.0/tests/mocks/arquivos/dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dlppdfmaxs.py` & `inewave-1.0.0/tests/mocks/arquivos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dlpptbmax.py` & `inewave-1.0.0/tests/mocks/arquivos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dlpptbmaxm.py` & `inewave-1.0.0/tests/mocks/arquivos/dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dlpptbmaxs.py` & `inewave-1.0.0/tests/mocks/arquivos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dsvagua.py` & `inewave-1.0.0/tests/mocks/arquivos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dtbmax.py` & `inewave-1.0.0/tests/mocks/arquivos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dtbmin.py` & `inewave-1.0.0/tests/mocks/arquivos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/dvazmax.py` & `inewave-1.0.0/tests/mocks/arquivos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eaf.py` & `inewave-1.0.0/tests/mocks/arquivos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eafb.py` & `inewave-1.0.0/tests/mocks/arquivos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eafbm.py` & `inewave-1.0.0/tests/mocks/arquivos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eafbsin.py` & `inewave-1.0.0/tests/mocks/arquivos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eafm.py` & `inewave-1.0.0/tests/mocks/arquivos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eafpast.py` & `inewave-1.0.0/tests/mocks/arquivos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/earmf.py` & `inewave-1.0.0/tests/mocks/arquivos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/earmfm.py` & `inewave-1.0.0/tests/mocks/arquivos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/earmfp.py` & `inewave-1.0.0/tests/mocks/arquivos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/earmfpm.py` & `inewave-1.0.0/tests/mocks/arquivos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/earmfpsin.py` & `inewave-1.0.0/tests/mocks/arquivos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/earmfsin.py` & `inewave-1.0.0/tests/mocks/arquivos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eolicacadastro.py` & `inewave-1.0.0/tests/mocks/arquivos/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eolicaconfig.py` & `inewave-1.0.0/tests/mocks/arquivos/eolicaconfig.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eolicafte.py` & `inewave-1.0.0/tests/mocks/arquivos/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eolicageracao.py` & `inewave-1.0.0/tests/mocks/arquivos/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eolicahistorico.py` & `inewave-1.0.0/tests/mocks/arquivos/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/eolicaposto.py` & `inewave-1.0.0/tests/mocks/arquivos/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/estados.py` & `inewave-1.0.0/tests/mocks/arquivos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/evert.py` & `inewave-1.0.0/tests/mocks/arquivos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/evertm.py` & `inewave-1.0.0/tests/mocks/arquivos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/evertsin.py` & `inewave-1.0.0/tests/mocks/arquivos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/exces.py` & `inewave-1.0.0/tests/mocks/arquivos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/excessin.py` & `inewave-1.0.0/tests/mocks/arquivos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/exph.py` & `inewave-1.0.0/tests/mocks/arquivos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/expt.py` & `inewave-1.0.0/tests/mocks/arquivos/expt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/fteolm.py` & `inewave-1.0.0/tests/mocks/arquivos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/fteolsin.py` & `inewave-1.0.0/tests/mocks/arquivos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/geol.py` & `inewave-1.0.0/tests/mocks/arquivos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/geolm.py` & `inewave-1.0.0/tests/mocks/arquivos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/geolsin.py` & `inewave-1.0.0/tests/mocks/arquivos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ghiduh.py` & `inewave-1.0.0/tests/mocks/arquivos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ghmax.py` & `inewave-1.0.0/tests/mocks/arquivos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ghmaxm.py` & `inewave-1.0.0/tests/mocks/arquivos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ghmaxmr.py` & `inewave-1.0.0/tests/mocks/arquivos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ghmaxr.py` & `inewave-1.0.0/tests/mocks/arquivos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ghmaxrsin.py` & `inewave-1.0.0/tests/mocks/arquivos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ghmaxsin.py` & `inewave-1.0.0/tests/mocks/arquivos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ghmin.py` & `inewave-1.0.0/tests/mocks/arquivos/ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ghtot.py` & `inewave-1.0.0/tests/mocks/arquivos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ghtotm.py` & `inewave-1.0.0/tests/mocks/arquivos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ghtotsin.py` & `inewave-1.0.0/tests/mocks/arquivos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/gtert.py` & `inewave-1.0.0/tests/mocks/arquivos/gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/gttot.py` & `inewave-1.0.0/tests/mocks/arquivos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/gttotsin.py` & `inewave-1.0.0/tests/mocks/arquivos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/intercambio.py` & `inewave-1.0.0/tests/mocks/arquivos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/invade.py` & `inewave-1.0.0/tests/mocks/arquivos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/invadem.py` & `inewave-1.0.0/tests/mocks/arquivos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/manutt.py` & `inewave-1.0.0/tests/mocks/arquivos/manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/mercl.py` & `inewave-1.0.0/tests/mocks/arquivos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/merclsin.py` & `inewave-1.0.0/tests/mocks/arquivos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/modif.py` & `inewave-1.0.0/tests/mocks/arquivos/modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/newavetim.py` & `inewave-1.0.0/tests/mocks/arquivos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/nwlistcfrel.py` & `inewave-1.0.0/tests/mocks/arquivos/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/nwlistopdat.py` & `inewave-1.0.0/tests/mocks/arquivos/nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/nwv_avl_evap.py` & `inewave-1.0.0/tests/mocks/arquivos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/nwv_cortes_evap.py` & `inewave-1.0.0/tests/mocks/arquivos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/nwv_eco_evap.py` & `inewave-1.0.0/tests/mocks/arquivos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/parp.py` & `inewave-1.0.0/tests/mocks/arquivos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/parpeol.py` & `inewave-1.0.0/tests/mocks/arquivos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/parpvaz.py` & `inewave-1.0.0/tests/mocks/arquivos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/patamar.py` & `inewave-1.0.0/tests/mocks/arquivos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/penalid.py` & `inewave-1.0.0/tests/mocks/arquivos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/perdf.py` & `inewave-1.0.0/tests/mocks/arquivos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/perdfm.py` & `inewave-1.0.0/tests/mocks/arquivos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/perdfsin.py` & `inewave-1.0.0/tests/mocks/arquivos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/pmo.py` & `inewave-1.0.0/tests/mocks/arquivos/pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/qafluh.py` & `inewave-1.0.0/tests/mocks/arquivos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/qincruh.py` & `inewave-1.0.0/tests/mocks/arquivos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/re.py` & `inewave-1.0.0/tests/mocks/arquivos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/ree.py` & `inewave-1.0.0/tests/mocks/arquivos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/restricaoeletrica.py` & `inewave-1.0.0/tests/mocks/arquivos/restricaoeletrica.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/restricaoenergia.py` & `inewave-1.0.0/tests/mocks/arquivos/restricaoenergia.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/restricaovazao.py` & `inewave-1.0.0/tests/mocks/arquivos/restricaovazao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/rhslppdf.py` & `inewave-1.0.0/tests/mocks/arquivos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/rhslpptb.py` & `inewave-1.0.0/tests/mocks/arquivos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/selcor.py` & `inewave-1.0.0/tests/mocks/arquivos/selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/sistema.py` & `inewave-1.0.0/tests/mocks/arquivos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/term.py` & `inewave-1.0.0/tests/mocks/arquivos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vagua.py` & `inewave-1.0.0/tests/mocks/arquivos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/varmpuh.py` & `inewave-1.0.0/tests/mocks/arquivos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/varmuh.py` & `inewave-1.0.0/tests/mocks/arquivos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vazpast.py` & `inewave-1.0.0/tests/mocks/arquivos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vento.py` & `inewave-1.0.0/tests/mocks/arquivos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vertuh.py` & `inewave-1.0.0/tests/mocks/arquivos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/verturb.py` & `inewave-1.0.0/tests/mocks/arquivos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/verturbm.py` & `inewave-1.0.0/tests/mocks/arquivos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/verturbsin.py` & `inewave-1.0.0/tests/mocks/arquivos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vevmin.py` & `inewave-1.0.0/tests/mocks/arquivos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vevminm.py` & `inewave-1.0.0/tests/mocks/arquivos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vevminsin.py` & `inewave-1.0.0/tests/mocks/arquivos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vghmin.py` & `inewave-1.0.0/tests/mocks/arquivos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vghminm.py` & `inewave-1.0.0/tests/mocks/arquivos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vghminsin.py` & `inewave-1.0.0/tests/mocks/arquivos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vghminuh.py` & `inewave-1.0.0/tests/mocks/arquivos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/arquivos/vturuh.py` & `inewave-1.0.0/tests/mocks/arquivos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/mocks/mock_open.py` & `inewave-1.0.0/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_adterm.py` & `inewave-1.0.0/tests/newave/test_adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_agrint.py` & `inewave-1.0.0/tests/newave/test_agrint.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_arquivos.py` & `inewave-1.0.0/tests/newave/test_arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_avl_cortesfpha_nwv.py` & `inewave-1.0.0/tests/newave/test_avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_avl_desvfpha_s.py` & `inewave-1.0.0/tests/newave/test_avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_avl_desvfpha_v_q.py` & `inewave-1.0.0/tests/newave/test_avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_cadic.py` & `inewave-1.0.0/tests/newave/test_cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_caso.py` & `inewave-1.0.0/tests/newave/test_caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_clast.py` & `inewave-1.0.0/tests/newave/test_clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_confhd.py` & `inewave-1.0.0/tests/newave/test_confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_conft.py` & `inewave-1.0.0/tests/newave/test_conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_cortes.py` & `inewave-1.0.0/tests/newave/test_cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_cortesh.py` & `inewave-1.0.0/tests/newave/test_cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_curva.py` & `inewave-1.0.0/tests/newave/test_curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_cvar.py` & `inewave-1.0.0/tests/newave/test_cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_dger.py` & `inewave-1.0.0/tests/newave/test_dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_dsvagua.py` & `inewave-1.0.0/tests/newave/test_dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_eafpast.py` & `inewave-1.0.0/tests/newave/test_eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_enavazb.py` & `inewave-1.0.0/tests/newave/test_enavazb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inewave.newave.modelos.enavazb import SecaoDadosEnavazb
 from inewave.newave.enavazb import Enavazb
 
-from os.path import join
+
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/enavazb.dat"
 
 NUM_FORWARDS = 2
```

### Comparing `inewave-0.0.98/tests/newave/test_enavazf.py` & `inewave-1.0.0/tests/newave/test_enavazf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inewave.newave.modelos.enavazf import SecaoDadosEnavazf
 from inewave.newave.enavazf import Enavazf
 
-from os.path import join
+
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/enavazf.dat"
 
 NUM_FORWARDS = 2
```

### Comparing `inewave-0.0.98/tests/newave/test_energiab.py` & `inewave-1.0.0/tests/newave/test_energiab.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inewave.newave.modelos.energiab import SecaoDadosEnergiab
 from inewave.newave.energiab import Energiab
 
-from os.path import join
+
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/energiab.dat"
 
 NUM_FORWARDS = 2
```

### Comparing `inewave-0.0.98/tests/newave/test_energiaf.py` & `inewave-1.0.0/tests/newave/test_energiaf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inewave.newave.modelos.energiaf import SecaoDadosEnergiaf
 from inewave.newave.energiaf import Energiaf
 
-from os.path import join
+
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/energiaf.dat"
 
 NUM_FORWARDS = 2
```

### Comparing `inewave-0.0.98/tests/newave/test_energias.py` & `inewave-1.0.0/tests/newave/test_energias.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inewave.newave.modelos.energias import SecaoDadosEnergias
 from inewave.newave.energias import Energias
 
-from os.path import join
+
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/energias.dat"
 
 NUM_SERIES = 2
```

### Comparing `inewave-0.0.98/tests/newave/test_engnat.py` & `inewave-1.0.0/tests/newave/test_engnat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inewave.newave.modelos.engnat import SecaoDadosEngnat
 from inewave.newave.engnat import Engnat
 from inewave.config import MAX_ANOS_HISTORICO
-from os.path import join
+
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/engnat.dat"
 
 NUM_CONFIGURACOES = 1
```

### Comparing `inewave-0.0.98/tests/newave/test_eolicacadastro.py` & `inewave-1.0.0/tests/newave/test_eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_eolicaconfiguracao.py` & `inewave-1.0.0/tests/newave/test_eolicaconfiguracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_eolicafte.py` & `inewave-1.0.0/tests/newave/test_eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_eolicageracao.py` & `inewave-1.0.0/tests/newave/test_eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_eolicahistorico.py` & `inewave-1.0.0/tests/newave/test_eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_eolicaposto.py` & `inewave-1.0.0/tests/newave/test_eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_eolicasubmercado.py` & `inewave-1.0.0/tests/newave/test_eolicasubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_exph.py` & `inewave-1.0.0/tests/newave/test_exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_expt.py` & `inewave-1.0.0/tests/newave/test_expt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_forward.py` & `inewave-1.0.0/tests/newave/test_forward.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_forwarh.py` & `inewave-1.0.0/tests/newave/test_forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_ghmin.py` & `inewave-1.0.0/tests/newave/test_ghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_hidr.py` & `inewave-1.0.0/tests/newave/test_hidr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inewave.newave.modelos.hidr import RegistroUHEHidr
 from inewave.newave.hidr import Hidr
 
-from os.path import join
+
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/hidr.dat"
```

### Comparing `inewave-0.0.98/tests/newave/test_manutt.py` & `inewave-1.0.0/tests/newave/test_manutt.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_modif.py` & `inewave-1.0.0/tests/newave/test_modif.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_newavetim.py` & `inewave-1.0.0/tests/newave/test_newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_nwv_avl_evap.py` & `inewave-1.0.0/tests/newave/test_nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_nwv_cortes_evap.py` & `inewave-1.0.0/tests/newave/test_nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_nwv_eco_evap.py` & `inewave-1.0.0/tests/newave/test_nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_parp.py` & `inewave-1.0.0/tests/newave/test_parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_parpeol.py` & `inewave-1.0.0/tests/newave/test_parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_parpvaz.py` & `inewave-1.0.0/tests/newave/test_parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_patamar.py` & `inewave-1.0.0/tests/newave/test_patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_penalid.py` & `inewave-1.0.0/tests/newave/test_penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_pmo.py` & `inewave-1.0.0/tests/newave/test_pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_re.py` & `inewave-1.0.0/tests/newave/test_re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_ree.py` & `inewave-1.0.0/tests/newave/test_ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_restricaoeletrica.py` & `inewave-1.0.0/tests/newave/test_restricaoeletrica.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_restricaoenergia.py` & `inewave-1.0.0/tests/newave/test_restricaoenergia.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_restricaovazao.py` & `inewave-1.0.0/tests/newave/test_restricaovazao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_selcor.py` & `inewave-1.0.0/tests/newave/test_selcor.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_shist.py` & `inewave-1.0.0/tests/newave/test_shist.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_sistema.py` & `inewave-1.0.0/tests/newave/test_sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_term.py` & `inewave-1.0.0/tests/newave/test_term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/newave/test_vazaob.py` & `inewave-1.0.0/tests/newave/test_vazaob.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inewave.newave.modelos.vazaob import SecaoDadosVazaob
 from inewave.newave.vazaob import Vazaob
 
-from os.path import join
+
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/vazaob.dat"
 
 NUM_FORWARDS = 2
```

### Comparing `inewave-0.0.98/tests/newave/test_vazaof.py` & `inewave-1.0.0/tests/newave/test_vazaof.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inewave.newave.modelos.vazaof import SecaoDadosVazaof
 from inewave.newave.vazaof import Vazaof
 
-from os.path import join
+
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/vazaof.dat"
 
 NUM_FORWARDS = 2
```

### Comparing `inewave-0.0.98/tests/newave/test_vazaos.py` & `inewave-1.0.0/tests/newave/test_vazaos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inewave.newave.modelos.vazaos import SecaoDadosVazaos
 from inewave.newave.vazaos import Vazaos
 
-from os.path import join
+
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/vazaos.dat"
 
 NUM_SERIES = 2
```

### Comparing `inewave-0.0.98/tests/newave/test_vazoes.py` & `inewave-1.0.0/tests/newave/test_vazoes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from inewave.newave.modelos.vazoes import RegistroVazoesPostos
 from inewave.newave.vazoes import Vazoes
 
-from os.path import join
+
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
 
 ARQ_TESTE = "./tests/mocks/arquivos/vazoes.dat"
```

### Comparing `inewave-0.0.98/tests/newave/test_vazpast.py` & `inewave-1.0.0/tests/newave/test_vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistcf/test_arquivos.py` & `inewave-1.0.0/tests/nwlistcf/test_arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistcf/test_caso.py` & `inewave-1.0.0/tests/nwlistcf/test_caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistcf/test_estados.py` & `inewave-1.0.0/tests/nwlistcf/test_estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistcf/test_nwlistcfdat.py` & `inewave-1.0.0/tests/nwlistcf/test_nwlistcfdat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistcf/test_nwlistcfrel.py` & `inewave-1.0.0/tests/nwlistcf/test_nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_cdef.py` & `inewave-1.0.0/tests/nwlistop/test_cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_cdefsin.py` & `inewave-1.0.0/tests/nwlistop/test_cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_cmarg.py` & `inewave-1.0.0/tests/nwlistop/test_cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_cmargmed.py` & `inewave-1.0.0/tests/nwlistop/test_cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_coper.py` & `inewave-1.0.0/tests/nwlistop/test_coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_corteolm.py` & `inewave-1.0.0/tests/nwlistop/test_corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_cterm.py` & `inewave-1.0.0/tests/nwlistop/test_cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_ctermsin.py` & `inewave-1.0.0/tests/nwlistop/test_ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_deficit.py` & `inewave-1.0.0/tests/nwlistop/test_deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_defsin.py` & `inewave-1.0.0/tests/nwlistop/test_defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_depminuh.py` & `inewave-1.0.0/tests/nwlistop/test_depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_dfphauh.py` & `inewave-1.0.0/tests/nwlistop/test_dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_dlppdfmax.py` & `inewave-1.0.0/tests/nwlistop/test_dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_dlppdfmaxm.py` & `inewave-1.0.0/tests/nwlistop/test_dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_dlppdfmaxs.py` & `inewave-1.0.0/tests/nwlistop/test_dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_dlpptbmax.py` & `inewave-1.0.0/tests/nwlistop/test_dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_dlpptbmaxm.py` & `inewave-1.0.0/tests/nwlistop/test_dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_dlpptbmaxs.py` & `inewave-1.0.0/tests/nwlistop/test_dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_dtbmax.py` & `inewave-1.0.0/tests/nwlistop/test_dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_dtbmin.py` & `inewave-1.0.0/tests/nwlistop/test_dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_dvazmax.py` & `inewave-1.0.0/tests/nwlistop/test_dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_eaf.py` & `inewave-1.0.0/tests/nwlistop/test_eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_eafb.py` & `inewave-1.0.0/tests/nwlistop/test_eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_eafbm.py` & `inewave-1.0.0/tests/nwlistop/test_eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_eafbsin.py` & `inewave-1.0.0/tests/nwlistop/test_eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_eafm.py` & `inewave-1.0.0/tests/nwlistop/test_eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_earmf.py` & `inewave-1.0.0/tests/nwlistop/test_earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_earmfm.py` & `inewave-1.0.0/tests/nwlistop/test_earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_earmfp.py` & `inewave-1.0.0/tests/nwlistop/test_earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_earmfpm.py` & `inewave-1.0.0/tests/nwlistop/test_earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_earmfpsin.py` & `inewave-1.0.0/tests/nwlistop/test_earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_earmfsin.py` & `inewave-1.0.0/tests/nwlistop/test_earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_evert.py` & `inewave-1.0.0/tests/nwlistop/test_evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_evertm.py` & `inewave-1.0.0/tests/nwlistop/test_evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_evertsin.py` & `inewave-1.0.0/tests/nwlistop/test_evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_exces.py` & `inewave-1.0.0/tests/nwlistop/test_exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_excessin.py` & `inewave-1.0.0/tests/nwlistop/test_excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_fteolm.py` & `inewave-1.0.0/tests/nwlistop/test_fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_fteolsin.py` & `inewave-1.0.0/tests/nwlistop/test_fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_geol.py` & `inewave-1.0.0/tests/nwlistop/test_geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_geolm.py` & `inewave-1.0.0/tests/nwlistop/test_geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_geolsin.py` & `inewave-1.0.0/tests/nwlistop/test_geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_ghiduh.py` & `inewave-1.0.0/tests/nwlistop/test_ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_ghmax.py` & `inewave-1.0.0/tests/nwlistop/test_ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_ghmaxm.py` & `inewave-1.0.0/tests/nwlistop/test_ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_ghmaxmr.py` & `inewave-1.0.0/tests/nwlistop/test_ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_ghmaxr.py` & `inewave-1.0.0/tests/nwlistop/test_ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_ghmaxrsin.py` & `inewave-1.0.0/tests/nwlistop/test_ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_ghmaxsin.py` & `inewave-1.0.0/tests/nwlistop/test_ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_ghtot.py` & `inewave-1.0.0/tests/nwlistop/test_ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_ghtotm.py` & `inewave-1.0.0/tests/nwlistop/test_ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_ghtotsin.py` & `inewave-1.0.0/tests/nwlistop/test_ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_gtert.py` & `inewave-1.0.0/tests/nwlistop/test_gtert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_gttot.py` & `inewave-1.0.0/tests/nwlistop/test_gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_gttotsin.py` & `inewave-1.0.0/tests/nwlistop/test_gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_intercambio.py` & `inewave-1.0.0/tests/nwlistop/test_intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_invade.py` & `inewave-1.0.0/tests/nwlistop/test_invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_invadem.py` & `inewave-1.0.0/tests/nwlistop/test_invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_mercl.py` & `inewave-1.0.0/tests/nwlistop/test_mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_merclsin.py` & `inewave-1.0.0/tests/nwlistop/test_merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_nwlistopdat.py` & `inewave-1.0.0/tests/nwlistop/test_nwlistopdat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_perdf.py` & `inewave-1.0.0/tests/nwlistop/test_perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_perdfm.py` & `inewave-1.0.0/tests/nwlistop/test_perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_perdfsin.py` & `inewave-1.0.0/tests/nwlistop/test_perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_qafluh.py` & `inewave-1.0.0/tests/nwlistop/test_qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_qincruh.py` & `inewave-1.0.0/tests/nwlistop/test_qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_rhslppdf.py` & `inewave-1.0.0/tests/nwlistop/test_rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_rhslpptb.py` & `inewave-1.0.0/tests/nwlistop/test_rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_vagua.py` & `inewave-1.0.0/tests/nwlistop/test_vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_varmpuh.py` & `inewave-1.0.0/tests/nwlistop/test_varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_varmuh.py` & `inewave-1.0.0/tests/nwlistop/test_varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_vento.py` & `inewave-1.0.0/tests/nwlistop/test_vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_vertuh.py` & `inewave-1.0.0/tests/nwlistop/test_vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_verturb.py` & `inewave-1.0.0/tests/nwlistop/test_verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_verturbm.py` & `inewave-1.0.0/tests/nwlistop/test_verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_verturbsin.py` & `inewave-1.0.0/tests/nwlistop/test_verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_vevmin.py` & `inewave-1.0.0/tests/nwlistop/test_vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_vevminm.py` & `inewave-1.0.0/tests/nwlistop/test_vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_vevminsin.py` & `inewave-1.0.0/tests/nwlistop/test_vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_vghmin.py` & `inewave-1.0.0/tests/nwlistop/test_vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_vghminm.py` & `inewave-1.0.0/tests/nwlistop/test_vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_vghminsin.py` & `inewave-1.0.0/tests/nwlistop/test_vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_vghminuh.py` & `inewave-1.0.0/tests/nwlistop/test_vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.98/tests/nwlistop/test_vturuh.py` & `inewave-1.0.0/tests/nwlistop/test_vturuh.py`

 * *Files identical despite different names*

