# Comparing `tmp/ibott_browser_manager-1.0.5.tar.gz` & `tmp/ibott_browser_manager-1.0.6.tar.gz`

## Comparing `ibott_browser_manager-1.0.5.tar` & `ibott_browser_manager-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/readme.md
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/requirements.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/.gitignore
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/browser_manager.iml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/misc.xml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/vcs.xml
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/browser/__init__.py
--rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/browser/chrome.py
--rw-r--r--   0        0        0    19398 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/browser/driver_utils.py
--rw-r--r--   0        0        0    13677 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/browser/firefox.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/browser/web_elements.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/LICENSE
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/README.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    18110 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/readme.md
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/requirements.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/.idea/.gitignore
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/.idea/browser_manager.iml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/.idea/misc.xml
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/.idea/vcs.xml
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/browser/__init__.py
+-rw-r--r--   0        0        0    11729 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/browser/chrome.py
+-rw-r--r--   0        0        0    24552 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/browser/driver_utils.py
+-rw-r--r--   0        0        0    13677 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/browser/firefox.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/browser/web_elements.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/LICENSE
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    18110 2020-02-02 00:00:00.000000 ibott_browser_manager-1.0.6/PKG-INFO
```

### Comparing `ibott_browser_manager-1.0.5/readme.md` & `ibott_browser_manager-1.0.6/readme.md`

 * *Files identical despite different names*

### Comparing `ibott_browser_manager-1.0.5/.idea/workspace.xml` & `ibott_browser_manager-1.0.6/.idea/workspace.xml`

 * *Files 18% similar despite different names*

#### Comparing `ibott_browser_manager-1.0.5/.idea/workspace.xml` & `ibott_browser_manager-1.0.6/.idea/workspace.xml`

```diff
@@ -4,15 +4,18 @@
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="4185439a-dcf4-4970-b1a5-6ae6388018d2" name="Changes" comment="Corrección de Bug en Scroll_to_element 
 Se cambia la importación de EC de Telnet a Selenium
 
 from telnetlib import EC
-from selenium.webdriver.support import expected_conditions as EC"/>
+from selenium.webdriver.support import expected_conditions as EC">
+      <change beforePath="$PROJECT_DIR$/browser/driver_utils.py" beforeDir="false" afterPath="$PROJECT_DIR$/browser/driver_utils.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="Git.Settings">
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
@@ -21,20 +24,20 @@
     <option name="stateVersion" value="1"/>
   </component>
   <component name="ProjectId" id="2RWF3JNT6zvWsMfDP4WabmGErRq"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent"><![CDATA[{
-  "keyToString": {
-    "RunOnceActivity.OpenProjectViewOnStart": "true",
-    "RunOnceActivity.ShowReadmeOnStart": "true"
+  <component name="PropertiesComponent">{
+  &quot;keyToString&quot;: {
+    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
+    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;
   }
-}]]></component>
+}</component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="4185439a-dcf4-4970-b1a5-6ae6388018d2" name="Changes" comment=""/>
       <created>1687357729405</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
```

### Comparing `ibott_browser_manager-1.0.5/browser/chrome.py` & `ibott_browser_manager-1.0.6/browser/chrome.py`

 * *Files identical despite different names*

### Comparing `ibott_browser_manager-1.0.5/browser/driver_utils.py` & `ibott_browser_manager-1.0.6/browser/driver_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,137 +6,232 @@
 import urllib.error
 import zipfile
 import xml.etree.ElementTree as elemTree
 import tarfile
 import sys
 import re
 from io import BytesIO
+import zipfile
+import platform as pf
+import json
+from typing import AnyStr, Optional
 logger = logging.getLogger(__name__)
 
-
 def get_chromedriver_filename():
     """
     Returns the filename of the binary for the current platform.
     :return: Binary filename
     """
-    if sys.platform.startswith('win'):
-        return 'chromedriver.exe'
-    return 'chromedriver'
+    if sys.platform.startswith("win"):
+        return "chromedriver.exe"
+    return "chromedriver"
 
 
 def get_variable_separator():
     """
     Returns the environment variable separator for the current platform.
     :return: Environment variable separator
     """
-    if sys.platform.startswith('win'):
-        return ';'
-    return ':'
-
-
-def get_platform_architecture():
-    if sys.platform.startswith('linux') and sys.maxsize > 2 ** 32:
-        platform = 'linux'
-        architecture = '64'
-    elif sys.platform == 'darwin':
-        platform = 'mac'
-        architecture = '64'
-    elif sys.platform.startswith('win'):
-        platform = 'win'
-        architecture = '32'
+    if sys.platform.startswith("win"):
+        return ";"
+    return ":"
+
+
+def get_platform_architecture(chrome_version=None):
+    if sys.platform.startswith("linux") and sys.maxsize > 2**32:
+        platform = "linux"
+        architecture = "64"
+    elif sys.platform == "darwin":
+        platform = "mac"
+        # At some points, the release naming for Apple arm changed;
+        # Looking in http://chromedriver.storage.googleapis.com/, the changeover happened across these releases:
+        # 106.0.5249.61/chromedriver_mac_arm64.zip
+        # 106.0.5249.21/chromedriver_mac64_m1.zip
+        # Mac architecture naming changed again as of the transition to CfT
+        # 115.0.5763.0/mac-arm64/chromedriver-mac-arm64.zip'
+        # 115.0.5763.0/mac-x64/chromedriver-mac-x64.zip'
+        if pf.processor() == "arm":
+            if chrome_version is not None and chrome_version >= "115.0.5763.0":
+                print("CHROME >= 115.0.5763.0, using mac-arm64 as architecture identifier")
+                architecture = "-arm64"
+            elif chrome_version is not None and chrome_version <= "106.0.5249.21":
+                print("CHROME <= 106.0.5249.21, using mac64_m1 as architecture identifier")
+                architecture = "64_m1"
+            else:
+                architecture = "_arm64"
+        elif pf.processor() == "i386":
+            if chrome_version is not None and chrome_version >= "115.0.5763.0":
+                print("CHROME >= 115.0.5763.0, using mac-x64 as architecture identifier")
+                architecture = "-x64"
+            else:
+                architecture = "mac64"
+        else:
+            raise RuntimeError("Could not determine Mac processor architecture.")
+    elif sys.platform.startswith("win"):
+        platform = "win"
+        architecture = "32"
     else:
-        raise RuntimeError('Could not determine chromedriver download URL for this platform.')
+        raise RuntimeError(
+            "Could not determine chromedriver download URL for this platform."
+        )
     return platform, architecture
 
 
-def get_chromedriver_url(version):
+def get_chromedriver_url(chromedriver_version, no_ssl=False):
     """
     Generates the download URL for current platform , architecture and the given version.
     Supports Linux, MacOS and Windows.
-    :param version: chromedriver version string
-    :return: Download URL for chromedriver
-    """
-    base_url = 'https://chromedriver.storage.googleapis.com/'
-    platform, architecture = get_platform_architecture()
-    return base_url + version + '/chromedriver_' + platform + architecture + '.zip'
+
+    :param chromedriver_version: ChromeDriver version string
+    :param no_ssl:               Whether to use the encryption protocol when downloading the chrome driver
+    :return:                     String. Download URL for chromedriver
+    """
+    platform, architecture = get_platform_architecture(chromedriver_version)
+    if chromedriver_version >= "115":  # new CfT ChromeDriver versions have their URLs published
+        versions_url = "googlechromelabs.github.io/chrome-for-testing/known-good-versions-with-downloads.json"
+        versions_url = "http://" + versions_url if no_ssl else "https://" + versions_url
+        download_version_list = json.load(urllib.request.urlopen(versions_url))
+        for good_version in download_version_list["versions"]:
+            if good_version["version"] == chromedriver_version:
+                download_urls = good_version["downloads"]["chromedriver"]
+                for url in download_urls:
+                    if url["platform"] == platform + architecture:
+                        return url['url']
+    else:  # old ChromeDriver versions use the old urls
+        base_url = "chromedriver.storage.googleapis.com/"
+        base_url = "http://" + base_url if no_ssl else "https://" + base_url
+        return base_url + chromedriver_version + "/chromedriver_" + platform + architecture + ".zip"
 
 
 def find_binary_in_path(filename):
     """
     Searches for a binary named `filename` in the current PATH. If an executable is found, its absolute path is returned
     else None.
     :param filename: Filename of the binary
     :return: Absolute path or None
     """
-    if 'PATH' not in os.environ:
+    if "PATH" not in os.environ:
         return None
-    for directory in os.environ['PATH'].split(get_variable_separator()):
+    for directory in os.environ["PATH"].split(get_variable_separator()):
         binary = os.path.abspath(os.path.join(directory, filename))
         if os.path.isfile(binary) and os.access(binary, os.X_OK):
             return binary
     return None
 
 
 def check_version(binary, required_version):
     try:
-        version = subprocess.check_output([binary, '-v'])
-        version = re.match(r'.*?([\d.]+).*?', version.decode('utf-8'))[1]
+        version = subprocess.check_output([binary, "-v"])
+        version = re.match(r".*?([\d.]+).*?", version.decode("utf-8"))[1]
         if version == required_version:
             return True
     except Exception:
         return False
     return False
 
 
 def get_chrome_version():
     """
     :return: the version of chrome installed on client
     """
     platform, _ = get_platform_architecture()
-    if platform == 'linux':
-        executable_name = 'google-chrome'
-        if os.path.isfile('/usr/bin/chromium-browser'):
-            executable_name = 'chromium-browser'
-        if os.path.isfile('/usr/bin/chromium'):
-            executable_name = 'chromium'
-        with subprocess.Popen([executable_name, '--version'], stdout=subprocess.PIPE) as proc:
-            version = proc.stdout.read().decode('utf-8').replace('Chromium', '').replace('Google Chrome', '').strip()
-    elif platform == 'mac':
-        process = subprocess.Popen(['/Applications/Google Chrome.app/Contents/MacOS/Google Chrome', '--version'],
-                                   stdout=subprocess.PIPE)
-        version = process.communicate()[0].decode('UTF-8').replace('Google Chrome', '').strip()
-    elif platform == 'win':
+    if platform == "linux":
+        path = get_linux_executable_path()
+        with subprocess.Popen([path, "--version"], stdout=subprocess.PIPE) as proc:
+            version = (
+                proc.stdout.read()
+                .decode("utf-8")
+                .replace("Chromium", "")
+                .replace("Google Chrome", "")
+                .strip()
+            )
+    elif platform == "mac":
         process = subprocess.Popen(
-            ['reg', 'query', 'HKEY_CURRENT_USER\\Software\\Google\\Chrome\\BLBeacon', '/v', 'version'],
-            stdout=subprocess.PIPE, stderr=subprocess.DEVNULL, stdin=subprocess.DEVNULL
+            [
+                "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
+                "--version",
+            ],
+            stdout=subprocess.PIPE,
         )
-        version = process.communicate()[0].decode('UTF-8').strip().split()[-1]
+        version = (
+            process.communicate()[0]
+            .decode("UTF-8")
+            .replace("Google Chrome", "")
+            .strip()
+        )
+    elif platform == "win":
+        # check both of Program Files and Program Files (x86).
+        # if the version isn't found on both of them, version is an empty string.
+        dirs = [f.name for f in os.scandir("C:\\Program Files\\Google\\Chrome\\Application") if f.is_dir() and re.match("^[0-9.]+$", f.name)]
+        if dirs:
+            version = max(dirs)
+        else:
+            dirs = [f.name for f in os.scandir("C:\\Program Files (x86)\\Google\\Chrome\\Application") if f.is_dir() and re.match("^[0-9.]+$", f.name)]
+            version = max(dirs) if dirs else ''
     else:
         return
     return version
 
 
+def get_linux_executable_path():
+    """
+    Look through a list of candidates for Google Chrome executables that might
+    exist, and return the full path to first one that does. Raise a ValueError
+    if none do.
+
+    :return: the full path to a Chrome executable on the system
+    """
+    for executable in (
+        "google-chrome",
+        "google-chrome-stable",
+        "google-chrome-beta",
+        "google-chrome-dev",
+        "chromium-browser",
+        "chromium",
+    ):
+        path = shutil.which(executable)
+        if path is not None:
+            return path
+    raise ValueError("No chrome executable found on PATH")
+
+
 def get_major_version(version):
     """
     :param version: the version of chrome
     :return: the major version of chrome
     """
-    return version.split('.')[0]
+    return version.split(".")[0]
 
 
-def get_matched_chromedriver_version(version):
+def get_matched_chromedriver_version(chrome_version, no_ssl=False):
     """
-    :param version: the version of chrome
-    :return: the version of chromedriver
-    """
-    doc = urllib.request.urlopen('https://chromedriver.storage.googleapis.com').read()
-    root = elemTree.fromstring(doc)
-    for k in root.iter('{http://doc.s3.amazonaws.com/2006-03-01}Key'):
-        if k.text.find(get_major_version(version) + '.') == 0:
-            return k.text.split('/')[0]
+    Try to find a specific version of ChromeDriver to match a version of cCrome
+
+    :param chrome_version: the version of Chrome to match against
+    :param no_ssl:         get version list using unsecured HTTP get
+    :return:               String. The version of chromedriver that matches the Chrome version
+                           None.   if no matching version of chromedriver was discovered
+    """
+    # Newer versions of chrome use the CfT publishing system
+    if chrome_version >= "115":
+        version_url = "googlechromelabs.github.io/chrome-for-testing/known-good-versions.json"
+        version_url = "http://" + version_url if no_ssl else "https://" + version_url
+        good_version_list = json.load(urllib.request.urlopen(version_url))
+        for good_version in good_version_list["versions"]:
+            if good_version["version"] == chrome_version:
+                return chrome_version
+    # check old versions of chrome using the old system
+    else:
+        version_url = "chromedriver.storage.googleapis.com"
+        version_url = "http://" + version_url if no_ssl else "https://" + version_url
+        doc = urllib.request.urlopen(version_url).read()
+        root = elemTree.fromstring(doc)
+        for k in root.iter("{http://doc.s3.amazonaws.com/2006-03-01}Key"):
+            if k.text.find(get_major_version(chrome_version) + ".") == 0:
+                return k.text.split("/")[0]
     return
 
 
 def get_chromedriver_path():
     """
     :return: path of the chromedriver binary
     """
@@ -146,63 +241,74 @@
 def print_chromedriver_path():
     """
     Print the path of the chromedriver binary.
     """
     print(get_chromedriver_path())
 
 
-def download_chromedriver(cwd=None):
+def download_chromedriver(path: Optional[AnyStr] = None, no_ssl: bool = False):
     """
     Downloads, unzips and installs chromedriver.
     If a chromedriver binary is found in PATH it will be copied, otherwise downloaded.
 
-    :param cwd: Flag indicating whether to download to current working directory
+    :param str path: Path of the directory where to save the downloaded chromedriver to.
+    :param bool no_ssl: Determines whether or not to use the encryption protocol when downloading the chrome driver.
     :return: The file path of chromedriver
     """
     chrome_version = get_chrome_version()
     if not chrome_version:
-        logging.debug('Chrome is not installed.')
+        logging.debug("Chrome is not installed.")
         return
-    chromedriver_version = get_matched_chromedriver_version(chrome_version)
+    chromedriver_version = get_matched_chromedriver_version(chrome_version, no_ssl)
     if not chromedriver_version:
-        logging.debug('Can not find chromedriver for currently installed chrome version.')
+        logging.warning(
+            "Can not find chromedriver for currently installed chrome version."
+        )
         return
     major_version = get_major_version(chromedriver_version)
 
-    if cwd:
-        chromedriver_dir = cwd
+    if path:
+        if not os.path.isdir(path):
+            raise ValueError(f"Invalid path: {path}")
+        chromedriver_dir = os.path.join(os.path.abspath(path), major_version)
     else:
         chromedriver_dir = os.path.join(
-            os.path.abspath(os.path.dirname(__file__)),
-            major_version
+            os.path.abspath(os.path.dirname(__file__)), major_version
         )
     chromedriver_filename = get_chromedriver_filename()
     chromedriver_filepath = os.path.join(chromedriver_dir, chromedriver_filename)
-    if not os.path.isfile(chromedriver_filepath) or \
-            not check_version(chromedriver_filepath, chromedriver_version):
-        logging.debug(f'Downloading chromedriver ({chromedriver_version})...')
+    if not os.path.isfile(chromedriver_filepath) or not check_version(
+        chromedriver_filepath, chromedriver_version
+    ):
+        logging.info(f"Downloading chromedriver ({chromedriver_version})...")
         if not os.path.isdir(chromedriver_dir):
-            os.mkdir(chromedriver_dir)
-        url = get_chromedriver_url(version=chromedriver_version)
+            os.makedirs(chromedriver_dir)
+        url = get_chromedriver_url(chromedriver_version=chromedriver_version, no_ssl=no_ssl)
         try:
             response = urllib.request.urlopen(url)
             if response.getcode() != 200:
-                raise urllib.error.URLError('Not Found')
+                raise urllib.error.URLError("Not Found")
         except urllib.error.URLError:
-            raise RuntimeError(f'Failed to download chromedriver archive: {url}')
+            raise RuntimeError(f"Failed to download chromedriver archive: {url}")
         archive = BytesIO(response.read())
         with zipfile.ZipFile(archive) as zip_file:
-            zip_file.extract(chromedriver_filename, chromedriver_dir)
+            # v115+ have files in subdirectories- need to adjust filename before extracting
+            for zip_info in zip_file.infolist():
+                if os.path.basename(zip_info.filename) == chromedriver_filename:
+                    zip_info.filename = chromedriver_filename
+                    zip_file.extract(zip_info, chromedriver_dir)
+                    break
     else:
-        logging.debug('Chromedriver is already installed.')
+        logging.info("Chromedriver is already installed.")
     if not os.access(chromedriver_filepath, os.X_OK):
         os.chmod(chromedriver_filepath, 0o744)
     return chromedriver_filepath
 
 
+
 def install_chrome(cwd=None):
     """
     Appends the directory of the chromedriver binary file to PATH.
 
     :param cwd: Flag indicating whether to download to current working directory
     :return: The file path of chromedriver
     """
@@ -350,15 +456,15 @@
         :return: version string
         """
         path = (
             "LATEST_RELEASE"
             if not self.target_version
             else f"LATEST_RELEASE_{self.target_version}"
         )
-        return urllib.urlopen(self.__class__.DL_BASE + path).read().decode()
+        return urllib.request.urlopen(self.__class__.DL_BASE + path).read().decode()
 
     def fetch_chromedriver(self):
         """
         Downloads ChromeDriver from source and unpacks the executable
 
         :return: on success, name of the unpacked executable
         """
```

### Comparing `ibott_browser_manager-1.0.5/browser/firefox.py` & `ibott_browser_manager-1.0.6/browser/firefox.py`

 * *Files identical despite different names*

### Comparing `ibott_browser_manager-1.0.5/browser/web_elements.py` & `ibott_browser_manager-1.0.6/browser/web_elements.py`

 * *Files identical despite different names*

### Comparing `ibott_browser_manager-1.0.5/LICENSE` & `ibott_browser_manager-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ibott_browser_manager-1.0.5/README.md` & `ibott_browser_manager-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ibott_browser_manager-1.0.5/pyproject.toml` & `ibott_browser_manager-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "selenium"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ibott_browser_manager"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
     { name="OnameDohe", email="enrique.crespo.debenito@gmail.com" },
 ]
 description = "This packages crates a simple way to work with, Chrome and Firefox Browsers. More info in https://ibott.io/academy/"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `ibott_browser_manager-1.0.5/PKG-INFO` & `ibott_browser_manager-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibott_browser_manager
-Version: 1.0.5
+Version: 1.0.6
 Summary: This packages crates a simple way to work with, Chrome and Firefox Browsers. More info in https://ibott.io/academy/
 Project-URL: Homepage, https://github.com/ecrespo66/browser_manager
 Project-URL: Bug Tracker, https://github.com/ecrespo66/browser_manager/issues
 Author-email: OnameDohe <enrique.crespo.debenito@gmail.com>
 License:                                Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

