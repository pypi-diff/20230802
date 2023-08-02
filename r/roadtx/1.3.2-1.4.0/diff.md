# Comparing `tmp/roadtx-1.3.2.tar.gz` & `tmp/roadtx-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roadtx-1.3.2.tar", last modified: Tue Jun 13 13:32:20 2023, max compression
+gzip compressed data, was "roadtx-1.4.0.tar", last modified: Wed Aug  2 13:30:57 2023, max compression
```

## Comparing `roadtx-1.3.2.tar` & `roadtx-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:32:20.272841 roadtx-1.3.2/
--rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-06-13 13:32:20.272841 roadtx-1.3.2/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:32:20.272841 roadtx-1.3.2/roadtools/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:32:20.272841 roadtx-1.3.2/roadtools/roadtx/
--rw-r--r--   0 vsts      (1001) docker     (123)     7865 2023-06-13 13:30:49.000000 roadtx-1.3.2/roadtools/roadtx/keepass.py
--rw-r--r--   0 vsts      (1001) docker     (123)    52771 2023-06-13 13:30:49.000000 roadtx-1.3.2/roadtools/roadtx/main.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14364 2023-06-13 13:30:49.000000 roadtx-1.3.2/roadtools/roadtx/selenium.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:32:20.272841 roadtx-1.3.2/roadtx.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      301 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       54 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 13:32:17.000000 roadtx-1.3.2/roadtx.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       66 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-06-13 13:32:20.000000 roadtx-1.3.2/roadtx.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-13 13:32:20.272841 roadtx-1.3.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1041 2023-06-13 13:30:49.000000 roadtx-1.3.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 13:30:57.651793 roadtx-1.4.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-08-02 13:30:57.651793 roadtx-1.4.0/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 13:30:57.647793 roadtx-1.4.0/roadtools/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 13:30:57.647793 roadtx-1.4.0/roadtools/roadtx/
+-rw-r--r--   0 vsts      (1001) docker     (123)    17290 2023-08-02 13:29:28.000000 roadtx-1.4.0/roadtools/roadtx/federation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7865 2023-08-02 13:29:28.000000 roadtx-1.4.0/roadtools/roadtx/keepass.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    58273 2023-08-02 13:29:28.000000 roadtx-1.4.0/roadtools/roadtx/main.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14851 2023-08-02 13:29:28.000000 roadtx-1.4.0/roadtools/roadtx/selenium.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-02 13:30:57.647793 roadtx-1.4.0/roadtx.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      570 2023-08-02 13:30:57.000000 roadtx-1.4.0/roadtx.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      332 2023-08-02 13:30:57.000000 roadtx-1.4.0/roadtx.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-02 13:30:57.000000 roadtx-1.4.0/roadtx.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       54 2023-08-02 13:30:57.000000 roadtx-1.4.0/roadtx.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-02 13:30:54.000000 roadtx-1.4.0/roadtx.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       74 2023-08-02 13:30:57.000000 roadtx-1.4.0/roadtx.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-08-02 13:30:57.000000 roadtx-1.4.0/roadtx.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-02 13:30:57.651793 roadtx-1.4.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1062 2023-08-02 13:29:28.000000 roadtx-1.4.0/setup.py
```

### Comparing `roadtx-1.3.2/PKG-INFO` & `roadtx-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.3.2
+Version: 1.4.0
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadtx-1.3.2/roadtools/roadtx/keepass.py` & `roadtx-1.4.0/roadtools/roadtx/keepass.py`

 * *Files identical despite different names*

### Comparing `roadtx-1.3.2/roadtools/roadtx/main.py` & `roadtx-1.4.0/roadtools/roadtx/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 import codecs
 import binascii
 import base64
 from urllib.parse import quote_plus
 from roadtools.roadlib.auth import Authentication, get_data, WELLKNOWN_CLIENTS, WELLKNOWN_RESOURCES
 from roadtools.roadlib.deviceauth import DeviceAuthentication
 from roadtools.roadtx.selenium import SeleniumAuthentication
+from roadtools.roadtx.federation import EncryptedPFX, SAMLSigner, encode_object_guid
 import pyotp
 
 RR_HELP = 'ROADtools Token eXchange by Dirk-jan Mollema (@_dirkjan) / Outsider Security (outsidersecurity.nl)'
 
 def main():
     # Primary argument parser
     parser = argparse.ArgumentParser(add_help=True, description=RR_HELP, formatter_class=argparse.RawDescriptionHelpFormatter)
+    parser.add_argument('-p', '--proxy', action='store', help="Proxy requests through a proxy (format: proxyip:port). Ignores TLS validation if specified, unless --secure is used.")
+    parser.add_argument('-s', '--secure', action='store_true', help="Enforce certificate validation even if using a proxy")
+
     # Add subparsers for modules
     subparsers = parser.add_subparsers(dest='command')
 
     # Construct authentication module options
     auth = Authentication()
     auth_parser = subparsers.add_parser('gettokens', aliases=['auth','gettoken'], help='Authenticate to Azure AD and get access/refresh tokens. Supports various authentication methods.')
     auth.get_sub_argparse(auth_parser, for_rr=False)
@@ -67,14 +71,16 @@
     prt_parser.add_argument('--pfx-pass', action='store', metavar='password', help='PFX file password')
     prt_parser.add_argument('--pfx-base64', action='store', metavar='BASE64', help='PFX file as base64 string')
     prt_parser.add_argument('-tk', '--transport-key-pem', action='store', metavar='file', help='Private key file containing transport key (if different from device key)')
 
     prt_parser.add_argument('-u', '--username', action='store', metavar='USER', help='User to authenticate')
     prt_parser.add_argument('-p', '--password', action='store', metavar='PASSWORD', help='Password')
     prt_parser.add_argument('-r', '--refresh-token', action='store', help='Refresh token')
+    prt_parser.add_argument('--saml-token', action='store', help='SAML token for federated auth (use value stdin to read from input)')
+
 
 
     prt_parser.add_argument('-f', '--prt-file', default="roadtx.prt", action='store', metavar='FILE', help='PRT storage file (to save or load in case of renewal)')
     prt_parser.add_argument('--prt', action='store', metavar='PRT', help='Primary Refresh Token (for renewal)')
     prt_parser.add_argument('-s', '--prt-sessionkey', action='store', help='Primary Refresh Token session key (as hex key)')
 
     prt_parser.add_argument('-hk', '--hello-key', action='store', help='Windows Hello PEM file')
@@ -278,14 +284,17 @@
                                 default='geckodriver')
     intauth_parser.add_argument('-k', '--keep-open',
                                 action='store_true',
                                 help='Do not close the browser window after timeout. Useful if you want to browse online apps with the obtained credentials')
     intauth_parser.add_argument('--capture-code',
                                 action='store_true',
                                 help='Do not attempt to redeem any authentication code but print it instead')
+    intauth_parser.add_argument('--federated',
+                                action='store_true',
+                                help='Fill in password on Federation server login page (assumes AD FS)')
 
     # Interactive auth using Selenium - creds from keepass
     kdbauth_parser = subparsers.add_parser('keepassauth', help='Selenium based authentication with credentials from a KeePass database')
     kdbauth_parser.add_argument('-u', '--username', action='store', help='User to authenticate as (must exist as username in KeePass)')
     kdbauth_parser.add_argument('-kp', '--keepass', action='store', metavar='KPFILE', default='roadtx.kdbx', help='KeePass file (default: roadtx.kdbx)')
     kdbauth_parser.add_argument('-kpp', '--keepass-password', action='store', metavar='KPPASS', help='KeePass file password. Can also be provided via KPPASS environment variable.')
     kdbauth_parser.add_argument('-url', '--auth-url', action='store', metavar='URL', help=urlhelp)
@@ -323,14 +332,17 @@
                                 default='geckodriver')
     kdbauth_parser.add_argument('-k', '--keep-open',
                                 action='store_true',
                                 help='Do not close the browser window after timeout. Useful if you want to browse online apps with the obtained credentials')
     kdbauth_parser.add_argument('--capture-code',
                                 action='store_true',
                                 help='Do not attempt to redeem any authentication code but print it instead')
+    kdbauth_parser.add_argument('--federated',
+                                action='store_true',
+                                help='Fill in password on Federation server login page (assumes AD FS)')
 
 
     # Interactive auth using Selenium - inject PRT
     browserprtauth_parser = subparsers.add_parser('browserprtauth', help='Selenium based auth with automatic PRT usage. Emulates Edge browser with PRT')
     browserprtauth_parser.add_argument('-url', '--auth-url', action='store', metavar='URL', help=urlhelp)
     browserprtauth_parser.add_argument('-c',
                                        '--client',
@@ -453,25 +465,59 @@
                                 action='store',
                                 help='File to store the credentials (default: .roadtools_auth)',
                                 default='.roadtools_auth')
     enrauth_parser.add_argument('--tokens-stdout',
                                 action='store_true',
                                 help='Do not store tokens on disk, pipe to stdout instead')
 
+    # ADFS Encrypted blob decrypt
+    adfsdec_parser = subparsers.add_parser('decryptadfskey', help='Decrypt Encrypted PFX blob from ADFSpoof into PEM or PFX file')
+    adfsdec_parser.add_argument('-c', '--cert-pem', action='store', metavar='file', default='roadtx_adfs.pem', help='Certificate file to save ADFS cert (default: roadtx_adfs.pem)')
+    adfsdec_parser.add_argument('-k', '--key-pem', action='store', metavar='file', default='roadtx_adfs.key', help='Private key file to save ADFS key (default: roadtx_adfs.key)')
+    adfsdec_parser.add_argument('--cert-pfx', action='store', metavar='file', default='roadtx_adfs.pfx', help='File to store the key (default: roadtx_adfs.pfx)')
+    adfsdec_parser.add_argument('-o', '--output-format', action='store', metavar='format', default='pem', choices=['pem', 'pfx'], help='Output format (pem or pfx), default: pem')
+    adfsdec_parser.add_argument('encryptedpfx', action='store', metavar='pfxblob', help='EncryptedPFX data from ADFSpoof')
+    adfsdec_parser.add_argument('key', action='store', metavar='key', help='Decryption key (DKM key)')
+    adfsdec_parser.add_argument('-v', '--verbose', action='store_true', help='Show extra information')
+
+    # ADFS token generation
+    samltoken_parser = subparsers.add_parser('samltoken', help='Create a SAML token using an AD FS key')
+    samltoken_parser.add_argument('-c', '--cert-pem', action='store', metavar='file', help='Certificate file with AD FS cert')
+    samltoken_parser.add_argument('-k', '--key-pem', action='store', metavar='file', help='Private key file with AD FS key')
+    samltoken_parser.add_argument('--cert-pfx', action='store', metavar='file', help='PFX file with AD FS cert/key')
+    samltoken_parser.add_argument('--pfx-pass', action='store', metavar='password', help='PFX file password')
+    samltoken_parser.add_argument('--pfx-base64', action='store', metavar='BASE64', help='PFX file as base64 string')
+    samltoken_parser.add_argument('-i', '--issuer', action='store', required=True, help='Token issuer, must match the federated domain name (without http/https, example: federated.mycompany.com)')
+    samltoken_parser.add_argument('-u', '--unique-id', action='store', help='Unique ID of user to spoof (immutableId in roadrecon)')
+    samltoken_parser.add_argument('-g', '--guid', action='store', help='GUID of user to spoof (from AD), if not specifying the unique id')
+    samltoken_parser.add_argument('-m', '--mfa', action='store_true', help='Include MFA claim in token')
+    samltoken_parser.add_argument('--upn', action='store', required=True, help='userPrincipalName of user to spoof')
+
+
     if len(sys.argv) < 2:
         parser.print_help()
         sys.exit(1)
         return
 
     deviceauth = DeviceAuthentication()
     args = parser.parse_args()
     seleniumproxy = None
 
+    if args.proxy:
+        auth.proxies = deviceauth.proxies = {
+            'https': f'http://{args.proxy}'
+        }
+        seleniumproxy = f'http://{args.proxy}'
+        if not args.secure:
+            auth.verify = deviceauth.verify = False
+
     if args.command in ('auth', 'gettokens', 'gettoken'):
         auth.parse_args(args)
+        if not args.tokens_stdout:
+            print(f'Requesting token for resource {auth.resource_uri}')
         res = auth.get_tokens(args)
         if not res:
             return
         auth.save_tokens(args)
     elif args.command == 'device':
         if args.action in ('register', 'join'):
             if args.access_token:
@@ -508,14 +554,20 @@
             if args.transport_key_pem:
                 # Try loading transport key separately
                 if not deviceauth.loadkey(args.transport_key_pem, transport_only=True):
                     return
             prtdata = None
             if args.username and args.password:
                 prtdata = deviceauth.get_prt_with_password(args.username, args.password)
+            if args.saml_token:
+                if args.saml_token.lower() == 'stdin':
+                    samltoken = sys.stdin.read()
+                else:
+                    samltoken = args.saml_token
+                prtdata = deviceauth.get_prt_with_samltoken(samltoken)
             if args.refresh_token:
                 prtdata = deviceauth.get_prt_with_refresh_token(args.refresh_token)
 
             if args.username and deviceauth.loadhellokey(args.hello_key):
                 prtdata = deviceauth.get_prt_with_hello_key(args.username)
             if not prtdata:
                 print('You must specify a username + password or refresh token that can be used to request a PRT')
@@ -625,15 +677,15 @@
             return
         selauth.driver = selauth.get_webdriver(service, intercept=True)
         if args.krbtoken:
             result = selauth.selenium_login_with_kerberos(url, args.username, args.password, capture=args.capture_code, krbdata=args.krbtoken)
         elif args.estscookie:
             result = selauth.selenium_login_with_estscookie(url, args.username, args.password, capture=args.capture_code, estscookie=args.estscookie)
         else:
-            result = selauth.selenium_login(url, args.username, args.password, capture=args.capture_code)
+            result = selauth.selenium_login(url, args.username, args.password, capture=args.capture_code, federated=args.federated)
         if args.capture_code:
             if result:
                 print(f'Captured auth code: {result}')
             return
         auth.outfile = args.tokenfile
         auth.save_tokens(args)
     elif args.command == 'keepassauth':
@@ -646,15 +698,15 @@
             url = args.auth_url
         else:
             url = auth.build_auth_url(args.redirect_url, 'code', args.scope)
         service = selauth.get_service(args.driver_path)
         if not service:
             return
         selauth.driver = selauth.get_webdriver(service)
-        result = selauth.selenium_login(url, args.username, password, otpseed, keep=args.keep_open, capture=args.capture_code)
+        result = selauth.selenium_login(url, args.username, password, otpseed, keep=args.keep_open, capture=args.capture_code, federated=args.federated)
         if args.capture_code:
             if result:
                 print(f'Captured auth code: {result}')
             return
         auth.outfile = args.tokenfile
         auth.save_tokens(args)
     elif args.command == 'browserprtauth':
@@ -835,10 +887,37 @@
             "deviceId": deviceid,
             "customKeyInformation": "AQAAAAACAAAAAAAAAAAA",
             "fidoAaGuid": None,
             "fidoAuthenticatorVersion": None,
             "fidoAttestationCertificates": []
         }
         print(json.dumps(data, sort_keys=True, indent=4))
+    elif args.command == 'decryptadfskey':
+        rawblob = base64.b64decode(args.encryptedpfx)
+        rawkey = binascii.unhexlify(args.key.replace('-',''))
+        pfx = EncryptedPFX(rawblob, rawkey, args.verbose)
+        decrypted_pfx = pfx.decrypt_pfx()
+        if args.output_format == 'pfx':
+            pfx.save_pfx(decrypted_pfx, args.cert_pfx)
+            print(f'Saved decrypted key to {args.cert_pfx}')
+        else:
+            pfx.save_pem(decrypted_pfx, args.cert_pem, args.key_pem)
+            print(f'Saved decrypted certificate to {args.cert_pem} and key to {args.key_pem}')
+    elif args.command == 'samltoken':
+        signer = SAMLSigner()
+        if not signer.loadcert(args.cert_pem, args.key_pem, args.cert_pfx, args.pfx_pass, args.pfx_base64):
+            sys.exit(1)
+        if not args.unique_id and not args.guid:
+            print('Either the unique-id or guid of the user to spoof is required')
+            sys.exit(1)
+        elif args.unique_id:
+            uid = args.unique_id
+        else:
+            uid = encode_object_guid(args.guid)
+        template, assertionid = signer.format_template(uid, args.upn, args.issuer, args.mfa)
+        signed = signer.sign_xml(template, assertionid)
+        print(signed.decode('utf-8'))
+
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `roadtx-1.3.2/roadtools/roadtx/selenium.py` & `roadtx-1.4.0/roadtools/roadtx/selenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,34 +74,43 @@
         userpassword = entry['Password']
         try:
             otpseed = entry['otp']
         except KeyError:
             otpseed = None
         return userpassword, otpseed
 
-    def selenium_login(self, url, identity=None, password=None, otpseed=None, keep=False, capture=False):
+    def selenium_login(self, url, identity=None, password=None, otpseed=None, keep=False, capture=False, federated=False):
         '''
         Selenium based login with optional autofill of whatever is provided
         '''
         driver = self.driver
         driver.get(url)
         if identity and not 'login_hint' in url:
             el = WebDriverWait(driver, 3000).until(lambda d: d.find_element(By.ID, "i0116"))
             el.send_keys(identity + Keys.ENTER)
         if password:
-            els = WebDriverWait(driver, 6000).until(lambda d: d.find_element(By.ID, "i0118"))
-            els.send_keys(password)
-
-            el = WebDriverWait(driver, 6000).until(lambda d: d.find_element(By.ID, "idSIButton9"))
-            try:
-                WebDriverWait(driver, 2).until(lambda d: d.find_element(By.ID, "idonotexist"))
-            except TimeoutException:
-                pass
-            els = WebDriverWait(driver, 6000).until(lambda d: d.find_element(By.ID, "i0118"))
-            els.send_keys(Keys.ENTER)
+            if federated:
+                els = WebDriverWait(driver, 6000).until(lambda d: d.find_element(By.ID, "passwordInput"))
+                els.send_keys(password)
+                try:
+                    WebDriverWait(driver, 1).until(lambda d: d.find_element(By.ID, "idonotexist"))
+                except TimeoutException:
+                    pass
+                els.send_keys(Keys.ENTER)
+            else:
+                els = WebDriverWait(driver, 6000).until(lambda d: d.find_element(By.ID, "i0118"))
+                els.send_keys(password)
+
+                el = WebDriverWait(driver, 6000).until(lambda d: d.find_element(By.ID, "idSIButton9"))
+                try:
+                    WebDriverWait(driver, 2).until(lambda d: d.find_element(By.ID, "idonotexist"))
+                except TimeoutException:
+                    pass
+                els = WebDriverWait(driver, 6000).until(lambda d: d.find_element(By.ID, "i0118"))
+                els.send_keys(Keys.ENTER)
 
         # Quick check of mfa not needed
         try:
             WebDriverWait(driver, 2).until(lambda d: '?code=' in d.current_url)
             res = urlparse(driver.current_url)
             params = parse_qs(res.query)
             code = params['code'][0]
@@ -195,15 +204,15 @@
                     request.headers['Authorization'] = f'Negotiate {krbdata}'
 
         self.driver.request_interceptor = interceptor
         return self.selenium_login(url, identity, password, otpseed, keep=keep, capture=capture)
 
     def selenium_login_with_estscookie(self, url, identity=None, password=None, otpseed=None, keep=False, capture=False, estscookie=None):
         '''
-        Selenium login with Kerberos auth header injection.
+        Selenium login with ESTSAUTH or ESTSAUTHPERSISTENT cookie injection
         '''
         def interceptor(request):
             del request.headers['User-Agent']
             request.headers['User-Agent'] = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/103.0.5060.134 Safari/537.36 Edg/103.0.1264.71'
             request.headers['Sec-Ch-Ua'] = '" Not;A Brand";v="99", "Microsoft Edge";v="103", "Chromium";v="103"'
             request.headers['Sec-Ch-Ua-Mobile'] =  '?0'
             request.headers['Sec-Ch-Ua-Platform'] =  '"Windows"'
```

### Comparing `roadtx-1.3.2/roadtx.egg-info/PKG-INFO` & `roadtx-1.4.0/roadtx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roadtx
-Version: 1.3.2
+Version: 1.4.0
 Summary: ROADtools Token eXchange
 Home-page: https://github.com/dirkjanm/ROADtools/
 Author: Dirk-jan Mollema
 Author-email: dirkjan@outsidersecurity.nl
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `roadtx-1.3.2/setup.py` & `roadtx-1.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 setup(name='roadtx',
-      version='1.3.2',
+      version='1.4.0',
       description='ROADtools Token eXchange',
       author='Dirk-jan Mollema',
       author_email='dirkjan@outsidersecurity.nl',
       url='https://github.com/dirkjanm/ROADtools/',
       license='MIT',
       classifiers=[
           'Intended Audience :: Information Technology',
@@ -13,20 +13,21 @@
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
       ],
       packages=['roadtools.roadtx'],
       install_requires=[
-          'roadlib>=0.18',
+          'roadlib>=0.19',
           'requests',
           'selenium',
           'selenium-wire',
           'pyotp',
-          'pycryptodomex'
+          'pycryptodomex',
+          'signxml'
       ],
       zip_safe=False,
       include_package_data=True,
       entry_points={
           'console_scripts': ['roadtx=roadtools.roadtx.main:main',]
       }
       )
```

