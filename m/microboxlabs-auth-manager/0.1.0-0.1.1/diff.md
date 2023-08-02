# Comparing `tmp/microboxlabs_auth_manager-0.1.0.tar.gz` & `tmp/microboxlabs_auth_manager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microboxlabs_auth_manager-0.1.0.tar", max compression
+gzip compressed data, was "microboxlabs_auth_manager-0.1.1.tar", max compression
```

## Comparing `microboxlabs_auth_manager-0.1.0.tar` & `microboxlabs_auth_manager-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1885 2023-08-02 11:33:06.968875 microboxlabs_auth_manager-0.1.0/README.md
--rw-r--r--   0        0        0       58 2023-08-01 12:20:59.155367 microboxlabs_auth_manager-0.1.0/microboxlabs_auth_manager/__init__.py
--rw-r--r--   0        0        0     1899 2023-08-01 12:15:07.485015 microboxlabs_auth_manager-0.1.0/microboxlabs_auth_manager/auth_token.py
--rw-r--r--   0        0        0      431 2023-08-01 12:32:15.519609 microboxlabs_auth_manager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2618 1970-01-01 00:00:00.000000 microboxlabs_auth_manager-0.1.0/setup.py
--rw-r--r--   0        0        0     2369 1970-01-01 00:00:00.000000 microboxlabs_auth_manager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1885 2023-08-02 11:48:33.341147 microboxlabs_auth_manager-0.1.1/README.md
+-rw-r--r--   0        0        0       58 2023-08-01 12:20:59.155367 microboxlabs_auth_manager-0.1.1/microboxlabs_auth_manager/__init__.py
+-rw-r--r--   0        0        0     1899 2023-08-01 12:15:07.485015 microboxlabs_auth_manager-0.1.1/microboxlabs_auth_manager/auth_token.py
+-rw-r--r--   0        0        0      431 2023-08-02 11:50:17.048295 microboxlabs_auth_manager-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2618 1970-01-01 00:00:00.000000 microboxlabs_auth_manager-0.1.1/setup.py
+-rw-r--r--   0        0        0     2369 1970-01-01 00:00:00.000000 microboxlabs_auth_manager-0.1.1/PKG-INFO
```

### Comparing `microboxlabs_auth_manager-0.1.0/README.md` & `microboxlabs_auth_manager-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
 ## Development
 
 For development purposes, you'll want to clone the repository and set up using Poetry:
 
 ```bash
 # Clone the repository
-git clone https://github.com/your_username/microboxlabs-auth-manager-sdk.git
-cd microboxlabs-auth-manager-sdk
+git clone https://github.com/microboxlabs/auth-manager.git
+cd auth-manager
 
 # Install the SDK dependencies for development
 poetry install
 ```
 
 ### Running Tests
 
@@ -65,15 +65,15 @@
 ## Features
 
 - Seamless authentication with Microboxlabs services.
 - Token management: acquire, refresh, and validate tokens.
 
 ## Documentation
 
-Refer to the [official documentation](URL_TO_YOUR_DOCS) for detailed usage and API references.
+Refer to the [official documentation](https://github.com/microboxlabs/auth-manager#readme) for detailed usage and API references.
 
 ## Contributing
 
 Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.
 
 ## License
```

### Comparing `microboxlabs_auth_manager-0.1.0/microboxlabs_auth_manager/auth_token.py` & `microboxlabs_auth_manager-0.1.1/microboxlabs_auth_manager/auth_token.py`

 * *Files identical despite different names*

### Comparing `microboxlabs_auth_manager-0.1.0/setup.py` & `microboxlabs_auth_manager-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pyjwt>=2.8.0,<3.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'microboxlabs-auth-manager',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
-    'long_description': '# Microboxlabs Auth Manager SDK for Python 3\n\nThis SDK provides a set of tools to interact and manage authentication with Microboxlabs services using Python 3.\n\n## Installation\n\n### Using pip:\n\nYou can install the SDK from PyPI using `pip`:\n\n```bash\npip install microboxlabs-auth-manager-sdk\n```\n\n### Using Poetry:\n\nIf you\'re using Poetry for your project, you can add it as a dependency:\n\n```bash\npoetry add microboxlabs-auth-manager-sdk\n```\n\n## Usage\n\nTo use the SDK in your Python projects:\n\n```python\nfrom microboxlabs_auth_manager import AuthToken\n\n# Initialization with your client details\nauth = AuthToken(client_id="YOUR_CLIENT_ID", \n                           client_secret="YOUR_CLIENT_SECRET", \n                           audience="https://api.microboxlabs.com/v1", \n                           grant_type="client_credentials")\n\n# Get a new access token\naccess_token = auth.get_token()\n```\n\n## Development\n\nFor development purposes, you\'ll want to clone the repository and set up using Poetry:\n\n```bash\n# Clone the repository\ngit clone https://github.com/your_username/microboxlabs-auth-manager-sdk.git\ncd microboxlabs-auth-manager-sdk\n\n# Install the SDK dependencies for development\npoetry install\n```\n\n### Running Tests\n\nEnsure you have the development dependencies installed:\n\n```bash\n# Run tests using unittest (or your preferred testing tool)\npoetry run python -m unittest discover tests\n\n# OR if you\'re using pytest\npoetry run pytest\n```\n\n## Features\n\n- Seamless authentication with Microboxlabs services.\n- Token management: acquire, refresh, and validate tokens.\n\n## Documentation\n\nRefer to the [official documentation](URL_TO_YOUR_DOCS) for detailed usage and API references.\n\n## Contributing\n\nPull requests are welcome! For major changes, please open an issue first to discuss what you\'d like to change.\n\n## License\n\n[MIT](https://choosealicense.com/licenses/mit/)\n',
+    'long_description': '# Microboxlabs Auth Manager SDK for Python 3\n\nThis SDK provides a set of tools to interact and manage authentication with Microboxlabs services using Python 3.\n\n## Installation\n\n### Using pip:\n\nYou can install the SDK from PyPI using `pip`:\n\n```bash\npip install microboxlabs-auth-manager-sdk\n```\n\n### Using Poetry:\n\nIf you\'re using Poetry for your project, you can add it as a dependency:\n\n```bash\npoetry add microboxlabs-auth-manager-sdk\n```\n\n## Usage\n\nTo use the SDK in your Python projects:\n\n```python\nfrom microboxlabs_auth_manager import AuthToken\n\n# Initialization with your client details\nauth = AuthToken(client_id="YOUR_CLIENT_ID", \n                           client_secret="YOUR_CLIENT_SECRET", \n                           audience="https://api.microboxlabs.com/v1", \n                           grant_type="client_credentials")\n\n# Get a new access token\naccess_token = auth.get_token()\n```\n\n## Development\n\nFor development purposes, you\'ll want to clone the repository and set up using Poetry:\n\n```bash\n# Clone the repository\ngit clone https://github.com/microboxlabs/auth-manager.git\ncd auth-manager\n\n# Install the SDK dependencies for development\npoetry install\n```\n\n### Running Tests\n\nEnsure you have the development dependencies installed:\n\n```bash\n# Run tests using unittest (or your preferred testing tool)\npoetry run python -m unittest discover tests\n\n# OR if you\'re using pytest\npoetry run pytest\n```\n\n## Features\n\n- Seamless authentication with Microboxlabs services.\n- Token management: acquire, refresh, and validate tokens.\n\n## Documentation\n\nRefer to the [official documentation](https://github.com/microboxlabs/auth-manager#readme) for detailed usage and API references.\n\n## Contributing\n\nPull requests are welcome! For major changes, please open an issue first to discuss what you\'d like to change.\n\n## License\n\n[MIT](https://choosealicense.com/licenses/mit/)\n',
     'author': 'Michel David',
     'author_email': 'mdavid.cu@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `microboxlabs_auth_manager-0.1.0/PKG-INFO` & `microboxlabs_auth_manager-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microboxlabs-auth-manager
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Michel David
 Author-email: mdavid.cu@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -54,16 +54,16 @@
 
 ## Development
 
 For development purposes, you'll want to clone the repository and set up using Poetry:
 
 ```bash
 # Clone the repository
-git clone https://github.com/your_username/microboxlabs-auth-manager-sdk.git
-cd microboxlabs-auth-manager-sdk
+git clone https://github.com/microboxlabs/auth-manager.git
+cd auth-manager
 
 # Install the SDK dependencies for development
 poetry install
 ```
 
 ### Running Tests
 
@@ -80,15 +80,15 @@
 ## Features
 
 - Seamless authentication with Microboxlabs services.
 - Token management: acquire, refresh, and validate tokens.
 
 ## Documentation
 
-Refer to the [official documentation](URL_TO_YOUR_DOCS) for detailed usage and API references.
+Refer to the [official documentation](https://github.com/microboxlabs/auth-manager#readme) for detailed usage and API references.
 
 ## Contributing
 
 Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.
 
 ## License
```

