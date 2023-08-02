# Comparing `tmp/jupyverse-0.2.0.tar.gz` & `tmp/jupyverse-0.2.1.tar.gz`

## Comparing `jupyverse-0.2.0.tar` & `jupyverse-0.2.1.tar`

### file list

```diff
@@ -1,218 +1,231 @@
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    66836 2020-02-02 00:00:00.000000 jupyverse-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.2.0/MANIFEST.in
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.2.0/config.yaml
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jupyverse-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.2.0/pytest.ini
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.devcontainer/requirements.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.2.0/binder/environment.yml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.2.0/binder/jupyter_notebook_config.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.2.0/binder/postBuild
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.2.0/binder/start
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/index.md
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/install.md
--rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/jupyter.svg
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/auth.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/contents.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/frontend.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/jupyterlab.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/kernels.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/lab.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/login.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/nbconvert.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/resource_usage.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/retrolab.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/terminals.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/plugins/yjs.md
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/usage/microservices.md
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/usage/multi_user.md
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.2.0/docs/usage/single_user.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/README.md
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/pyproject.toml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/cli.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.2.0/jupyverse_api/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.2.0/notebooks/admin_users.ipynb
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.2.0/notebooks/admin_users.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/README.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/__init__.py
--rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/config.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/py.typed
--rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth/fps_auth/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/config.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/main.py
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/fps_contents/__init__.py
--rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/fps_contents/fileid.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/fps_contents/py.typed
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/contents/fps_contents/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/MANIFEST.in
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/fps_frontend/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/fps_frontend/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/frontend/fps_frontend/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/MANIFEST.in
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/MANIFEST.in
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/main.py
--rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/MANIFEST.in
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/fps_lab/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/fps_lab/main.py
--rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/fps_lab/routes.py
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/lab/fps_lab/static/favicon.ico
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/COPYING.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/MANIFEST.in
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/routes.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/index.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-file.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-notebook.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-terminal.ico
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon.ico
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/logo/github.svg
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/logo/logo.png
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/login/fps_login/static/style/index.css
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/fps_nbconvert/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/fps_nbconvert/main.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/nbconvert/fps_nbconvert/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/README.md
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/fps_noauth/__init__.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/fps_noauth/backends.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/fps_noauth/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/noauth/fps_noauth/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/COPYING.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/README.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/fps_resource_usage/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/fps_resource_usage/main.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/resource_usage/fps_resource_usage/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/fps_retrolab/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/fps_retrolab/main.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/retrolab/fps_retrolab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/README.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/fps_terminals/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/fps_terminals/main.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/fps_terminals/routes.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/fps_terminals/server.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/terminals/fps_terminals/win_server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/COPYING.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/README.md
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/fps_webdav/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/fps_webdav/config.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/fps_webdav/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/fps_webdav/py.typed
--rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/fps_webdav/routes.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/webdav/tests/test_webdav.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/MANIFEST.in
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/README.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/fps_yjs/__init__.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/fps_yjs/py.typed
--rw-r--r--   0        0        0    15108 2020-02-02 00:00:00.000000 jupyverse-0.2.0/plugins/yjs/fps_yjs/routes.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/test_auth.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/test_contents.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/test_kernels.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/test_server.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/test_settings.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/utils.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.2.0/tests/data/notebook0.ipynb
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.2.0/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.0/COPYING.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.2.0/README.md
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 jupyverse-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 jupyverse-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyverse-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    68064 2020-02-02 00:00:00.000000 jupyverse-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.2.1/MANIFEST.in
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.2.1/config.yaml
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 jupyverse-0.2.1/mkdocs.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.2.1/pytest.ini
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.2.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.2.1/.devcontainer/requirements.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.2.1/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.2.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.2.1/binder/environment.yml
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.2.1/binder/jupyter_notebook_config.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.2.1/binder/postBuild
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.2.1/binder/start
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/index.md
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/install.md
+-rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/jupyter.svg
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/auth.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/contents.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/frontend.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/jupyterlab.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/kernels.md
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/lab.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/login.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/nbconvert.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/resource_usage.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/retrolab.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/terminals.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/plugins/yjs.md
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/tutorials/jupyterhub_jupyverse_deployment.md
+-rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/tutorials/standalone_jupyverse_deployment.md
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/usage/microservices.md
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/usage/multi_user.md
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.2.1/docs/usage/single_user.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/README.md
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/pyproject.toml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.2.1/jupyverse_api/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.2.1/notebooks/admin_users.ipynb
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.2.1/notebooks/admin_users.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/fps_auth/config.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/fps_auth/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/fps_auth/py.typed
+-rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth/fps_auth/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_fief/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_fief/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_fief/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_fief/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_fief/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_fief/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_fief/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_fief/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_fief/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_jupyterhub/COPYING.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_jupyterhub/README.md
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_jupyterhub/pyproject.toml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/__init__.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/config.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/launch.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/models.py
+-rw-r--r--   0        0        0     7509 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/contents/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/contents/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/contents/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/contents/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/contents/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/contents/fps_contents/fileid.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/contents/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/contents/fps_contents/py.typed
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/contents/fps_contents/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/frontend/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/frontend/MANIFEST.in
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/frontend/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/frontend/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/frontend/fps_frontend/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/frontend/fps_frontend/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/frontend/fps_frontend/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/jupyterlab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/jupyterlab/MANIFEST.in
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/jupyterlab/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/jupyterlab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/jupyterlab/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/jupyterlab/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/jupyterlab/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/jupyterlab/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/jupyterlab/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/MANIFEST.in
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/main.py
+-rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/lab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/lab/MANIFEST.in
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/lab/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/lab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/lab/fps_lab/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/lab/fps_lab/main.py
+-rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/lab/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/lab/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/COPYING.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/MANIFEST.in
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/routes.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/static/index.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-file.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-notebook.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-terminal.ico
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon.ico
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/static/logo/github.svg
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/static/logo/logo.png
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/login/fps_login/static/style/index.css
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/nbconvert/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/nbconvert/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/nbconvert/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/nbconvert/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/nbconvert/fps_nbconvert/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/nbconvert/fps_nbconvert/main.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/nbconvert/fps_nbconvert/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/noauth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/noauth/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/noauth/README.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/noauth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/noauth/fps_noauth/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/noauth/fps_noauth/backends.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/noauth/fps_noauth/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/noauth/fps_noauth/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/resource_usage/COPYING.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/resource_usage/README.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/resource_usage/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/resource_usage/fps_resource_usage/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/resource_usage/fps_resource_usage/main.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/resource_usage/fps_resource_usage/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/retrolab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/retrolab/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/retrolab/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/retrolab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/retrolab/fps_retrolab/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/retrolab/fps_retrolab/main.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/retrolab/fps_retrolab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/terminals/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/terminals/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/terminals/README.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/terminals/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/terminals/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/terminals/fps_terminals/main.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/terminals/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/terminals/fps_terminals/server.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/terminals/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/webdav/COPYING.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/webdav/README.md
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/webdav/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/webdav/fps_webdav/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/webdav/fps_webdav/config.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/webdav/fps_webdav/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/webdav/fps_webdav/py.typed
+-rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/webdav/fps_webdav/routes.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/webdav/tests/test_webdav.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/yjs/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/yjs/MANIFEST.in
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/yjs/README.md
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/yjs/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/yjs/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/yjs/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/yjs/fps_yjs/py.typed
+-rw-r--r--   0        0        0    15108 2020-02-02 00:00:00.000000 jupyverse-0.2.1/plugins/yjs/fps_yjs/routes.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jupyverse-0.2.1/tests/test_app.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.2.1/tests/test_auth.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.2.1/tests/test_contents.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.2.1/tests/test_kernels.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 jupyverse-0.2.1/tests/test_server.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.2.1/tests/test_settings.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.2.1/tests/utils.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.2.1/tests/data/notebook0.ipynb
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.2.1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/COPYING.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.2.1/README.md
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 jupyverse-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.2.1/PKG-INFO
```

### Comparing `jupyverse-0.2.0/.pre-commit-config.yaml` & `jupyverse-0.2.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
       - id: check-yaml
       - id: debug-statements
       - id: forbid-new-submodules
       - id: check-builtin-literals
       - id: trailing-whitespace
 
   - repo: https://github.com/psf/black
-    rev: 23.3.0
+    rev: 23.7.0
     hooks:
       - id: black
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.277
+    rev: v0.0.281
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyverse-0.2.0/CHANGELOG.md` & `jupyverse-0.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # Changes in Jupyverse {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.2.1
+
+([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.2.0...dbd047377e6d7f16c235795da578813cf274651f))
+
+### Merged PRs
+
+- Add fps_auth_jupyterhub plugin [#335](https://github.com/jupyter-server/jupyverse/pull/335) ([@davidbrochart](https://github.com/davidbrochart))
+- Add mount_path for mounting app at sub-path [#334](https://github.com/jupyter-server/jupyverse/pull/334) ([@davidbrochart](https://github.com/davidbrochart))
+- Fix external kernels [#333](https://github.com/jupyter-server/jupyverse/pull/333) ([@davidbrochart](https://github.com/davidbrochart))
+- Add documentation on deployment [#327](https://github.com/jupyter-server/jupyverse/pull/327) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-07-13&to=2023-08-02&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-07-13..2023-08-02&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-07-13..2023-08-02&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.2.0
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.10...ebf0e6d40a593eccccaf3ae2753e6ad272135e3b))
 
 ### Merged PRs
 
 - Rerun flaky tests [#331](https://github.com/jupyter-server/jupyverse/pull/331) ([@davidbrochart](https://github.com/davidbrochart))
@@ -14,16 +33,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-07-05&to=2023-07-13&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-07-05..2023-07-13&type=Issues) | [@frankie567](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Afrankie567+updated%3A2023-07-05..2023-07-13&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-07-05..2023-07-13&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.10
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.9...e15a7e4091cfa94dff41b05cf273ed92438ad299))
 
 ### Merged PRs
 
 - Pin ypy-websocket \<0.11 [#325](https://github.com/jupyter-server/jupyverse/pull/325) ([@davidbrochart](https://github.com/davidbrochart))
```

### Comparing `jupyverse-0.2.0/CONTRIBUTING.md` & `jupyverse-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/config.yaml` & `jupyverse-0.2.1/config.yaml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/mkdocs.yml` & `jupyverse-0.2.1/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 nav:
 - Overview: index.md
 - install.md
 - Usage:
   - usage/single_user.md
   - usage/multi_user.md
   - usage/microservices.md
+- Turorials:
+  - tutorials/standalone_jupyverse_deployment.md
+  - tutorials/jupyterhub_jupyverse_deployment.md
 - Plugins:
   - 'auth': plugins/auth.md
   - 'contents': plugins/contents.md
   - 'frontend': plugins/frontend.md
   - 'lab': plugins/lab.md
   - 'jupyterlab': plugins/jupyterlab.md
   - 'retrolab': plugins/retrolab.md
```

### Comparing `jupyverse-0.2.0/.devcontainer/devcontainer.json` & `jupyverse-0.2.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/.github/workflows/check-release.yml` & `jupyverse-0.2.1/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/.github/workflows/main.yml` & `jupyverse-0.2.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/binder/jupyter_notebook_config.py` & `jupyverse-0.2.1/binder/jupyter_notebook_config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/docs/index.md` & `jupyverse-0.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/docs/install.md` & `jupyverse-0.2.1/docs/install.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/docs/jupyter.svg` & `jupyverse-0.2.1/docs/jupyter.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/docs/plugins/auth.md` & `jupyverse-0.2.1/docs/plugins/auth.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/docs/usage/microservices.md` & `jupyverse-0.2.1/docs/usage/microservices.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/docs/usage/multi_user.md` & `jupyverse-0.2.1/docs/usage/multi_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/docs/usage/single_user.md` & `jupyverse-0.2.1/docs/usage/single_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/COPYING.md` & `jupyverse-0.2.1/jupyverse_api/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/pyproject.toml` & `jupyverse-0.2.1/jupyverse_api/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 from pydantic import BaseModel
 
 from .app import App
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/cli.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/app/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/app/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from collections import defaultdict
 from typing import Dict, List
 
 from fastapi import FastAPI
 
 from ..exceptions import RedirectException, _redirect_exception_handler
@@ -12,16 +14,21 @@
 
 class App:
     """A wrapper around FastAPI that checks for endpoint path conflicts."""
 
     _app: FastAPI
     _router_paths: Dict[str, List[str]]
 
-    def __init__(self, app: FastAPI):
-        self._app = app
+    def __init__(self, app: FastAPI, mount_path: str | None = None):
+        if mount_path is None:
+            self._app = app
+        else:
+            subapi = FastAPI()
+            app.mount(mount_path, subapi)
+            self._app = subapi
         app.add_exception_handler(RedirectException, _redirect_exception_handler)
         self._router_paths = defaultdict(list)
 
     @property
     def _paths(self):
         return [path for router, paths in self._router_paths.items() for path in paths]
```

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/auth/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/contents/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/contents/models.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/jupyterlab/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/kernels/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/kernels/models.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/lab/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/main/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/main/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,29 @@
 from fastapi import FastAPI
 from pydantic import BaseModel
 
 from ..app import App
 
 
 class AppComponent(Component):
+    def __init__(
+        self,
+        *,
+        mount_path: str | None = None,
+    ) -> None:
+        super().__init__()
+        self.mount_path = mount_path
+
     async def start(
         self,
         ctx: Context,
     ) -> None:
         app = await ctx.request_resource(FastAPI)
 
-        _app = App(app)
+        _app = App(app, mount_path=self.mount_path)
         ctx.add_resource(_app)
 
 
 class JupyverseComponent(FastAPIComponent):
     def __init__(
         self,
         components: dict[str, dict[str, Any] | None] | None = None,
```

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/nbconvert/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/resource_usage/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/retrolab/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/retrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/terminals/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/jupyverse_api/jupyverse_api/yjs/__init__.py` & `jupyverse-0.2.1/jupyverse_api/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/notebooks/admin_users.ipynb` & `jupyverse-0.2.1/notebooks/admin_users.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/notebooks/admin_users.py` & `jupyverse-0.2.1/notebooks/admin_users.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth/COPYING.md` & `jupyverse-0.2.1/plugins/auth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth/pyproject.toml` & `jupyverse-0.2.1/plugins/auth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth/fps_auth/backends.py` & `jupyverse-0.2.1/plugins/auth/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth/fps_auth/config.py` & `jupyverse-0.2.1/plugins/auth/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth/fps_auth/db.py` & `jupyverse-0.2.1/plugins/auth/fps_auth/db.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth/fps_auth/main.py` & `jupyverse-0.2.1/plugins/auth/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth/fps_auth/routes.py` & `jupyverse-0.2.1/plugins/auth/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth_fief/COPYING.md` & `jupyverse-0.2.1/plugins/auth_fief/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth_fief/pyproject.toml` & `jupyverse-0.2.1/plugins/auth_fief/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/backend.py` & `jupyverse-0.2.1/plugins/auth_fief/fps_auth_fief/backend.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/config.py` & `jupyverse-0.2.1/plugins/auth_fief/fps_auth_fief/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/main.py` & `jupyverse-0.2.1/plugins/auth_fief/fps_auth_fief/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/auth_fief/fps_auth_fief/routes.py` & `jupyverse-0.2.1/plugins/auth_fief/fps_auth_fief/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/contents/COPYING.md` & `jupyverse-0.2.1/plugins/auth_jupyterhub/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/contents/pyproject.toml` & `jupyverse-0.2.1/plugins/contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/contents/fps_contents/fileid.py` & `jupyverse-0.2.1/plugins/contents/fps_contents/fileid.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/contents/fps_contents/routes.py` & `jupyverse-0.2.1/plugins/contents/fps_contents/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/frontend/COPYING.md` & `jupyverse-0.2.1/plugins/contents/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/frontend/pyproject.toml` & `jupyverse-0.2.1/plugins/frontend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/jupyterlab/COPYING.md` & `jupyverse-0.2.1/plugins/frontend/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/jupyterlab/pyproject.toml` & `jupyverse-0.2.1/plugins/jupyterlab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/index.py` & `jupyverse-0.2.1/plugins/jupyterlab/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/main.py` & `jupyverse-0.2.1/plugins/jupyterlab/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/jupyterlab/fps_jupyterlab/routes.py` & `jupyverse-0.2.1/plugins/jupyterlab/fps_jupyterlab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/kernels/COPYING.md` & `jupyverse-0.2.1/plugins/jupyterlab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/kernels/pyproject.toml` & `jupyverse-0.2.1/plugins/kernels/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/kernels/fps_kernels/main.py` & `jupyverse-0.2.1/plugins/kernels/fps_kernels/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/kernels/fps_kernels/routes.py` & `jupyverse-0.2.1/plugins/kernels/fps_kernels/routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,17 +131,18 @@
 
     async def get_sessions(
         self,
         user: User,
     ):
         for session in self.sessions.values():
             kernel_id = session.kernel.id
-            kernel_server = kernels[kernel_id]["server"]
-            session.kernel.last_activity = kernel_server.last_activity["date"]
-            session.kernel.execution_state = kernel_server.last_activity["execution_state"]
+            if kernel_id in kernels:
+                kernel_server = kernels[kernel_id]["server"]
+                session.kernel.last_activity = kernel_server.last_activity["date"]
+                session.kernel.execution_state = kernel_server.last_activity["execution_state"]
         return list(self.sessions.values())
 
     async def create_session(
         self,
         request: Request,
         user: User,
     ):
@@ -303,15 +304,15 @@
         accepted_websocket = AcceptedWebSocket(websocket, subprotocol)
         if kernel_id in kernels:
             kernel_server = kernels[kernel_id]["server"]
             if kernel_server is None:
                 # this is an external kernel
                 # kernel is already launched, just start a kernel server
                 kernel_server = KernelServer(
-                    connection_file=kernel_id,
+                    connection_file=self.kernel_id_to_connection_file[kernel_id],
                     write_connection_file=False,
                 )
                 await kernel_server.start(launch_kernel=False)
                 kernels[kernel_id]["server"] = kernel_server
             await kernel_server.serve(accepted_websocket, session_id, permissions)
 
     async def watch_connection_files(self, path: Path) -> None:
@@ -339,23 +340,24 @@
                     to_delete.append(p)
         for p in to_delete:
             del file_changes[p]
         # process file changes
         for path, cs in file_changes.items():
             for change in cs:
                 if change == Change.deleted:
-                    if path in kernels:
+                    if path in self.kernel_id_to_connection_file.values():
                         kernel_id = list(self.kernel_id_to_connection_file.keys())[
                             list(self.kernel_id_to_connection_file.values()).index(path)
                         ]
+                        del self.kernel_id_to_connection_file[kernel_id]
                         del kernels[kernel_id]
                 elif change == Change.added:
                     try:
                         data = json.loads(Path(path).read_text())
-                    except BaseException:
+                    except Exception:
                         continue
                     if "kernel_name" not in data or "key" not in data:
                         continue
                     # looks like a kernel connection file
                     kernel_id = str(uuid.uuid4())
                     self.kernel_id_to_connection_file[kernel_id] = path
                     kernels[kernel_id] = {
```

### Comparing `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/connect.py` & `jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/driver.py` & `jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py` & `jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/message.py` & `jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_driver/paths.py` & `jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_server/message.py` & `jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/kernels/fps_kernels/kernel_server/server.py` & `jupyverse-0.2.1/plugins/kernels/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/lab/COPYING.md` & `jupyverse-0.2.1/plugins/kernels/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/lab/pyproject.toml` & `jupyverse-0.2.1/plugins/lab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/lab/fps_lab/main.py` & `jupyverse-0.2.1/plugins/lab/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/lab/fps_lab/routes.py` & `jupyverse-0.2.1/plugins/lab/fps_lab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/lab/fps_lab/static/favicon.ico` & `jupyverse-0.2.1/plugins/lab/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/COPYING.md` & `jupyverse-0.2.1/plugins/lab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/pyproject.toml` & `jupyverse-0.2.1/plugins/login/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/routes.py` & `jupyverse-0.2.1/plugins/login/fps_login/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/static/index.html` & `jupyverse-0.2.1/plugins/login/fps_login/static/index.html`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-1.ico` & `jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-2.ico` & `jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-busy-3.ico` & `jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-file.ico` & `jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-notebook.ico` & `jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon-terminal.ico` & `jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/static/favicons/favicon.ico` & `jupyverse-0.2.1/plugins/login/fps_login/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/static/logo/github.svg` & `jupyverse-0.2.1/plugins/login/fps_login/static/logo/github.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/static/logo/logo.png` & `jupyverse-0.2.1/plugins/login/fps_login/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/login/fps_login/static/style/index.css` & `jupyverse-0.2.1/plugins/login/fps_login/static/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/nbconvert/COPYING.md` & `jupyverse-0.2.1/plugins/login/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/nbconvert/pyproject.toml` & `jupyverse-0.2.1/plugins/nbconvert/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/nbconvert/fps_nbconvert/routes.py` & `jupyverse-0.2.1/plugins/nbconvert/fps_nbconvert/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/noauth/COPYING.md` & `jupyverse-0.2.1/plugins/nbconvert/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/noauth/pyproject.toml` & `jupyverse-0.2.1/plugins/noauth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/noauth/fps_noauth/backends.py` & `jupyverse-0.2.1/plugins/noauth/fps_noauth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/resource_usage/COPYING.md` & `jupyverse-0.2.1/plugins/resource_usage/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/resource_usage/pyproject.toml` & `jupyverse-0.2.1/plugins/resource_usage/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/resource_usage/fps_resource_usage/main.py` & `jupyverse-0.2.1/plugins/resource_usage/fps_resource_usage/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/resource_usage/fps_resource_usage/routes.py` & `jupyverse-0.2.1/plugins/resource_usage/fps_resource_usage/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/retrolab/COPYING.md` & `jupyverse-0.2.1/plugins/noauth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/retrolab/pyproject.toml` & `jupyverse-0.2.1/plugins/retrolab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/retrolab/fps_retrolab/main.py` & `jupyverse-0.2.1/plugins/retrolab/fps_retrolab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/retrolab/fps_retrolab/routes.py` & `jupyverse-0.2.1/plugins/retrolab/fps_retrolab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/terminals/COPYING.md` & `jupyverse-0.2.1/plugins/retrolab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/terminals/pyproject.toml` & `jupyverse-0.2.1/plugins/terminals/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/terminals/fps_terminals/main.py` & `jupyverse-0.2.1/plugins/terminals/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/terminals/fps_terminals/routes.py` & `jupyverse-0.2.1/plugins/terminals/fps_terminals/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/terminals/fps_terminals/server.py` & `jupyverse-0.2.1/plugins/terminals/fps_terminals/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/terminals/fps_terminals/win_server.py` & `jupyverse-0.2.1/plugins/terminals/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/webdav/COPYING.md` & `jupyverse-0.2.1/plugins/terminals/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/webdav/pyproject.toml` & `jupyverse-0.2.1/plugins/webdav/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/webdav/fps_webdav/routes.py` & `jupyverse-0.2.1/plugins/webdav/fps_webdav/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/webdav/tests/test_webdav.py` & `jupyverse-0.2.1/plugins/webdav/tests/test_webdav.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/yjs/COPYING.md` & `jupyverse-0.2.1/plugins/webdav/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/yjs/pyproject.toml` & `jupyverse-0.2.1/plugins/yjs/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/yjs/fps_yjs/main.py` & `jupyverse-0.2.1/plugins/yjs/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/plugins/yjs/fps_yjs/routes.py` & `jupyverse-0.2.1/plugins/yjs/fps_yjs/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/tests/conftest.py` & `jupyverse-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/tests/test_auth.py` & `jupyverse-0.2.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/tests/test_contents.py` & `jupyverse-0.2.1/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/tests/test_kernels.py` & `jupyverse-0.2.1/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/tests/test_server.py` & `jupyverse-0.2.1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/tests/test_settings.py` & `jupyverse-0.2.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/tests/utils.py` & `jupyverse-0.2.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/tests/data/notebook0.ipynb` & `jupyverse-0.2.1/tests/data/notebook0.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/.gitignore` & `jupyverse-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/COPYING.md` & `jupyverse-0.2.1/plugins/yjs/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/README.md` & `jupyverse-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.2.0/pyproject.toml` & `jupyverse-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 Homepage = "https://jupyter.org"
 
 [project.optional-dependencies]
 jupyterlab = ["fps-jupyterlab >=0.1.2,<1"]
 retrolab = ["fps-retrolab >=0.1.2,<1"]
 auth = ["fps-auth >=0.1.2,<1", "fps-login >=0.1.2,<1"]
 auth-fief = ["fps-auth-fief >=0.1.2,<1"]
+auth-jupyterhub = ["fps-auth-jupyterhub >=0.1.2,<1"]
 noauth = ["fps-noauth >=0.1.2,<1"]
 test = [
     "mypy",
     "types-setuptools",
     "pytest",
     "pytest-asyncio",
     "pytest-rerunfailures",
@@ -78,30 +79,32 @@
   { value = "pip install -e ./plugins/jupyterlab", if = ["jupyterlab"]},
   { value = "pip install -e ./plugins/retrolab", if = ["retrolab"]},
 ]
 matrix.auth.post-install-commands = [
   { value = "pip install -e ./plugins/noauth", if = ["noauth"] },
   { value = "pip install -e ./plugins/auth -e ./plugins/login", if = ["auth"] },
   { value = "pip install -e ./plugins/auth_fief", if = ["auth_fief"] },
+  { value = "pip install -e ./plugins/auth_jupyterhub", if = ["auth_jupyterhub"] },
 ]
 
 matrix.frontend.scripts = [
   { key = "typecheck1", value = "typecheck0 ./plugins/jupyterlab", if = ["jupyterlab"] },
   { key = "typecheck1", value = "typecheck0 ./plugins/retrolab", if = ["retrolab"] },
 ]
 
 matrix.auth.scripts = [
   { key = "typecheck", value = "typecheck1 ./plugins/noauth", if = ["noauth"] },
   { key = "typecheck", value = "typecheck1 ./plugins/auth ./plugins/login", if = ["auth"] },
   { key = "typecheck", value = "typecheck1 ./plugins/auth_fief", if = ["auth_fief"] },
+  { key = "typecheck", value = "typecheck1 ./plugins/auth_jupyterhub", if = ["auth_jupyterhub"] },
 ]
 
 [[tool.hatch.envs.dev.matrix]]
 frontend = ["jupyterlab", "retrolab"]
-auth = ["noauth", "auth", "auth_fief"]
+auth = ["noauth", "auth", "auth_fief", "auth_jupyterhub"]
 
 [tool.hatch.envs.dev.scripts]
 test = "pytest ./tests plugins/webdav/tests -v --reruns 5 --timeout=60"
 lint = [
   "black --line-length 100 jupyverse ./plugins",
   "isort --profile=black jupyverse ./plugins",
 ]
@@ -140,27 +143,28 @@
 
 [tool.jupyter-releaser.options]
 python_packages = [
     "jupyverse_api:jupyverse_api",
     "plugins/noauth:fps-noauth",
     "plugins/auth:fps-auth",
     "plugins/auth_fief:fps-auth-fief",
+    "plugins/auth_jupyterhub:fps-auth-jupyterhub",
     "plugins/contents:fps-contents",
     "plugins/frontend:fps-frontend",
     "plugins/jupyterlab:fps-jupyterlab",
     "plugins/kernels:fps-kernels",
     "plugins/lab:fps-lab",
     "plugins/nbconvert:fps-nbconvert",
     "plugins/retrolab:fps-retrolab",
     "plugins/terminals:fps-terminals",
     "plugins/yjs:fps-yjs",
     "plugins/resource_usage:fps-resource-usage",
     "plugins/login:fps-login",
     "plugins/webdav:fps-webdav",
-    ".:jupyverse:jupyverse_api,fps-noauth,fps-auth,fps-auth-fief,fps-contents,fps-jupyterlab,fps-kernels,fps-lab,fps-frontend,fps-nbconvert,fps-retrolab,fps-terminals,fps-yjs,fps-resource-usage,fps-webdav"
+    ".:jupyverse:jupyverse_api,fps-noauth,fps-auth,fps-auth-fief,fps-auth-jupyterhub,fps-contents,fps-jupyterlab,fps-kernels,fps-lab,fps-frontend,fps-nbconvert,fps-retrolab,fps-terminals,fps-yjs,fps-resource-usage,fps-webdav"
 ]
 
 [tool.hatch.version]
 path = "jupyverse/__init__.py"
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
```

### Comparing `jupyverse-0.2.0/PKG-INFO` & `jupyverse-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyverse
-Version: 0.2.0
+Version: 0.2.1
 Summary: A set of FPS plugins implementing a Jupyter server
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
@@ -17,14 +17,16 @@
 Requires-Dist: fps-yjs<1,>=0.1.2
 Requires-Dist: jupyverse-api<1,>=0.1.2
 Provides-Extra: auth
 Requires-Dist: fps-auth<1,>=0.1.2; extra == 'auth'
 Requires-Dist: fps-login<1,>=0.1.2; extra == 'auth'
 Provides-Extra: auth-fief
 Requires-Dist: fps-auth-fief<1,>=0.1.2; extra == 'auth-fief'
+Provides-Extra: auth-jupyterhub
+Requires-Dist: fps-auth-jupyterhub<1,>=0.1.2; extra == 'auth-jupyterhub'
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Provides-Extra: jupyterlab
 Requires-Dist: fps-jupyterlab<1,>=0.1.2; extra == 'jupyterlab'
 Provides-Extra: noauth
 Requires-Dist: fps-noauth<1,>=0.1.2; extra == 'noauth'
```

