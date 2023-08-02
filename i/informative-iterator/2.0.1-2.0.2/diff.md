# Comparing `tmp/informative_iterator-2.0.1.tar.gz` & `tmp/informative_iterator-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "informative_iterator-2.0.1.tar", last modified: Wed Aug  2 16:59:35 2023, max compression
+gzip compressed data, was "informative_iterator-2.0.2.tar", last modified: Wed Aug  2 17:01:48 2023, max compression
```

## Comparing `informative_iterator-2.0.1.tar` & `informative_iterator-2.0.2.tar`

### file list

```diff
@@ -1,377 +1,377 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.985076 informative_iterator-2.0.1/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3241 2023-08-02 16:59:35.984880 informative_iterator-2.0.1/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.806513 informative_iterator-2.0.1/informative_iterator/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.807317 informative_iterator-2.0.1/informative_iterator/__dependencies__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6452 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.807622 informative_iterator-2.0.1/informative_iterator/__dependencies__/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4177 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.800663 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.811281 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/.gitignore
--rw-r--r--   0 jeffhykin   (501) staff       (20)      428 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/.gitrepo
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/README.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.814772 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/pip
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.816304 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/clean
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/commands
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/local_install
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/publish
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/purge
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/shell
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/start
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/subrepo
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.816775 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.822169 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/
--rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif
--rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/setup.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.822975 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/logs/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      315 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/logs/main.py.log
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.825858 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.826017 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    12380 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.826325 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    10649 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/license.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/setup.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/poetry.lock
--rw-r--r--   0 jeffhykin   (501) staff       (20)      483 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/pyproject.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.826905 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/run/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/run/tests
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/run/tests.ps1
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.827448 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.827844 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/.cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/.cache/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.828678 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_clean/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_clean/450_nix.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_clean/600_cache_folder.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_clean/801_python.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.829516 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_manual_start/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.830002 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_purge/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_purge/580_mac_library_caches.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.853974 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/001_010_enable_globbing.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/004_000_add_system_bin.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/090_000_run_project_commands.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_doit_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_resume_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/099_050_finish_spaceship_setup_.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.860657 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.800380 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.860832 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.799096 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.799290 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.863113 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.869205 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.876947 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.877521 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.881339 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin
--rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_cleaning.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.800084 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.881758 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.883642 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.884094 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.884222 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.889513 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.889732 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.889825 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.893211 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.893379 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.893483 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.902456 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.906941 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/long_eval
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/raw_find
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_start.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.908116 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/settings.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.912674 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.915562 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.918652 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/refresh_ignores
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/fornix_core
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.919094 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/home/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/home/.zshenv
--rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/home/.zshrc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.921588 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/requirements/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.922137 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/tests/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1044 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/tests/main.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.924861 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/.gitignore
--rw-r--r--   0 jeffhykin   (501) staff       (20)      419 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/.gitrepo
--rw-r--r--   0 jeffhykin   (501) staff       (20)      733 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/README.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.926065 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/pip
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.927439 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/project/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/project/clean
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/project/commands
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/project/local_install
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      143 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/project/publish
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/project/purge
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/shell
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/start
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/subrepo
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.927883 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/fornix_framework.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.933964 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/
--rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/cd_tutorial.gif
--rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_from_example.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_name.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_versions.png
--rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/setup.md
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.935021 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/.keep
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/license.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1141 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/setup.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.935625 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    14527 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/__init__.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.935984 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/__pycache__/
--rw-r--r--   0 jeffhykin   (501) staff       (20)    12846 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 jeffhykin   (501) staff       (20)    16088 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/neo_map.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)    27953 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/poetry.lock
--rw-r--r--   0 jeffhykin   (501) staff       (20)      489 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/pyproject.toml
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.936195 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.936488 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/.cache/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/.cache/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.937173 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_clean/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_clean/450_nix.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_clean/600_cache_folder.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_clean/801_python.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.942052 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_manual_start/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_manual_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_manual_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.946382 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_purge/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_purge/580_mac_library_caches.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_purge/802_remove_venv.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.957858 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/000_009__add_path_injections__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/001_000__setup_zsh__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/001_010__setup_nix_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/001_010_enable_globbing.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/004_000_add_system_bin.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/005_000__setup_ld_path__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/010_000__ssl_fix__.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/019_000_setup_python_venv.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/021_000_ensure_pip_modules.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/022_000_setup_pythonpath.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/024_000_python_ignores.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/081_000__ensure_all_commands_executable__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/082_000_add_commands_to_path.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/090_000_run_project_commands.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/091_000_commands_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/092_000_doit_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/092_000_resume_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/093_000_customize_ll_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13245 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/094_000_jeffs_git_shortcuts.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/095_000_customize_tree_function.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/099_050_finish_spaceship_setup_.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.962858 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/010_000_setting_up_env_message.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/049_000_link_keychain.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/051_000_copy_git_config.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_deno_store.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_nix_channel.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_tealdeer.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/089_000__sudo_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/091_000__logger_injection__.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/095_000_vim_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/096_000_vscode_injection.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/097_000_atom_injection.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.803881 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.963004 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.802787 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.802945 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.965434 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/copy
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/relative_link
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/remove
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/storage
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.967969 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/basic_init_example
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/inject_into_path
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      750 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/trigger
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.970076 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/escape_grep_regex
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/escape_shell_argument
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/indent
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/remove_doublequotes
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/unindent
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.970941 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.971934 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/commands/ignore
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/commands/mixin
--rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/during_cleaning.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.803665 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.972212 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/fsmonitor-watchman/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/fsmonitor-watchman/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.972419 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-merge/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-merge/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-merge/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.972633 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-update/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-update/901_check_pip_modules
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.972748 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-applypatch/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-applypatch/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.972927 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-commit/.keep
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.973092 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-merge-commit/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-merge-commit/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.973177 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-push/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-push/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.973256 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-receive/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-receive/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.973343 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/prepare-commit-msg/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/prepare-commit-msg/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.973428 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/update/
--rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/update/.keep
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.979569 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/cacert.pem
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.981183 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/ensure_nix_installed
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/fix_ssl
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/lib_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/long_eval
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/package_path_for
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/raw_find
--rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/during_start.sh
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)    27936 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/installer_helper
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/nix.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/parse_dependencies.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/settings.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/shell.nix
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2470 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/uninstaller_helper
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.982340 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/os_mac/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/os_mac/#establish_extension.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/os_mac/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/os_mac/during_start_prep.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.983034 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/#establish_extension.sh
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.983499 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/add_project_to_pythonpath
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/ensure_pip_modules
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/refresh_ignores
--rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/setup_venv
--rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/during_clean.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/during_purge.sh
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/fornix_core
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.984035 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/home/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/home/.zshenv
--rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/home/.zshrc
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.984606 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/requirements/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/requirements/advanced_system_tools.nix
--rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-08-02 16:38:04.000000 informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/requirements/system_tools.toml
--rw-r--r--   0 jeffhykin   (501) staff       (20)    21890 2023-08-02 16:59:02.000000 informative_iterator-2.0.1/informative_iterator/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)      198 2023-08-02 16:40:16.000000 informative_iterator-2.0.1/informative_iterator/settings.json
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:59:35.807206 informative_iterator-2.0.1/informative_iterator.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)     3241 2023-08-02 16:59:35.000000 informative_iterator-2.0.1/informative_iterator.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)    29812 2023-08-02 16:59:35.000000 informative_iterator-2.0.1/informative_iterator.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-08-02 16:59:35.000000 informative_iterator-2.0.1/informative_iterator.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       21 2023-08-02 16:59:35.000000 informative_iterator-2.0.1/informative_iterator.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-08-02 16:59:35.985128 informative_iterator-2.0.1/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1551 2023-08-02 16:43:57.000000 informative_iterator-2.0.1/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.245828 informative_iterator-2.0.2/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3241 2023-08-02 17:01:48.245099 informative_iterator-2.0.2/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.119413 informative_iterator-2.0.2/informative_iterator/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.120236 informative_iterator-2.0.2/informative_iterator/__dependencies__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6452 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.120406 informative_iterator-2.0.2/informative_iterator/__dependencies__/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4177 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.115445 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.121295 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      428 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1850 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.121907 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.122786 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      477 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.123019 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.124547 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.124835 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/logs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      315 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/logs/main.py.log
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.126689 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.126811 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12380 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.126940 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    10649 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1202 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/setup.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    29546 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      483 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.128510 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/run/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/run/tests
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4637 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/run/tests.ps1
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.128734 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.130165 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.130614 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.133183 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.133576 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.137125 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13674 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.139112 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.115131 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.139236 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.113388 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.113544 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.140811 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.143532 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      795 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.148193 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.149056 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.151466 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.114839 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.152161 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.153128 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.155194 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.155444 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.155640 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.158202 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.158535 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.158670 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.158790 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.158913 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.167789 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.171051 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    28669 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.171171 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      604 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5862 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.173271 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.173624 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.179325 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     6083 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.179731 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.179967 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.180875 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/tests/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1044 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/tests/main.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.181595 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8884 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/.gitignore
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      419 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/.gitrepo
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      733 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/README.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.182066 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      156 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/pip
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.182984 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/project/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      461 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/project/clean
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1328 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/project/commands
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       39 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/project/local_install
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      143 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/project/publish
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      860 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/project/purge
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4038 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/shell
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     8865 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/start
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      416 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/subrepo
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.183282 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8842 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/fornix_framework.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.189048 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   706321 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/cd_tutorial.gif
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   141455 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_from_example.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    67463 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_name.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   234123 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_versions.png
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     4209 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/setup.md
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.190239 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/.keep
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1069 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/license.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1141 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.191181 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    14527 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/__init__.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.191557 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/__pycache__/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    12846 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    16088 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/neo_map.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    27953 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/poetry.lock
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      489 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/pyproject.toml
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.191714 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.192417 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/.cache/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/.cache/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.192966 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_clean/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_clean/450_nix.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      464 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_clean/600_cache_folder.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_clean/801_python.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.193557 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_manual_start/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_manual_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_manual_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.193887 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_purge/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_purge/580_mac_library_caches.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_purge/802_remove_venv.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.203938 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/000_009__add_path_injections__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1826 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/001_000__setup_zsh__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       75 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/001_010__setup_nix_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      190 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/001_010_enable_globbing.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      123 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/004_000_add_system_bin.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      368 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/005_000__setup_ld_path__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/010_000__ssl_fix__.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/019_000_setup_python_venv.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/021_000_ensure_pip_modules.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/022_000_setup_pythonpath.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/024_000_python_ignores.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/081_000__ensure_all_commands_executable__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      225 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/082_000_add_commands_to_path.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      154 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/090_000_run_project_commands.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2043 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/091_000_commands_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       93 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/092_000_doit_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      252 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/092_000_resume_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    22180 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/093_000_customize_ll_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13245 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/094_000_jeffs_git_shortcuts.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      120 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/095_000_customize_tree_function.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      186 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/099_050_finish_spaceship_setup_.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.209708 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      204 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/010_000_setting_up_env_message.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/049_000_link_keychain.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/051_000_copy_git_config.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1567 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_deno_store.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      772 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_nix_channel.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1071 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_tealdeer.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       92 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/089_000__sudo_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       94 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/091_000__logger_injection__.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      116 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/095_000_vim_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/096_000_vscode_injection.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      118 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/097_000_atom_injection.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.118511 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.210032 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6087 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.116807 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.116974 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.213224 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      555 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/add_execute_permission
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      650 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/copy
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2280 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/relative_link
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      348 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/remove
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      280 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/storage
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.217605 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1192 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/basic_init_example
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     4392 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5804 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1319 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/inject_into_path
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      750 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/merge_all_templates
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1553 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/trigger
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.219576 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       59 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/escape_grep_regex
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       91 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/escape_shell_argument
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/indent
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       58 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/remove_doublequotes
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1789 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      181 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/unindent
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.221072 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     5930 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.222415 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2782 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/commands/ignore
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2254 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/commands/mixin
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      244 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/during_cleaning.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      347 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.118075 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.222657 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/fsmonitor-watchman/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/fsmonitor-watchman/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.222882 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-merge/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-merge/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-merge/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.226836 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-update/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-update/901_check_pip_modules
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.227109 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-applypatch/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-applypatch/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.227328 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-commit/.keep
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     1447 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.228973 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-merge-commit/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-merge-commit/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.229131 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-push/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-push/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.229225 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-receive/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-receive/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.229311 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/prepare-commit-msg/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/prepare-commit-msg/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.229401 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/update/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        0 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/update/.keep
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.236183 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1376 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)   201623 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/cacert.pem
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.238763 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     7988 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/ensure_nix_installed
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2246 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/fix_ssl
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      742 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/lib_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      164 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/long_eval
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      746 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/package_path_for
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       62 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/raw_find
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      161 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       69 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/during_start.sh
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)    27936 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/installer_helper
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/nix.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    13466 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/parse_dependencies.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      228 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/settings.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/shell.nix
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     2470 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/uninstaller_helper
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.239826 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/os_mac/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      500 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/os_mac/#establish_extension.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      173 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/os_mac/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      437 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/os_mac/during_start_prep.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.240479 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     2072 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/#establish_extension.sh
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.243880 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)       89 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/add_project_to_pythonpath
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)     5976 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/ensure_pip_modules
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      191 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/refresh_ignores
+-rwxr-xr-x   0 jeffhykin   (501) staff       (20)      565 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/setup_venv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      494 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/during_clean.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1949 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/during_purge.sh
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6180 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/fornix_core
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.244431 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/home/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1471 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/home/.zshenv
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       76 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/home/.zshrc
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.244862 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/requirements/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6031 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/requirements/advanced_system_tools.nix
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     8590 2023-08-02 16:38:04.000000 informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/requirements/system_tools.toml
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    21891 2023-08-02 17:01:14.000000 informative_iterator-2.0.2/informative_iterator/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      198 2023-08-02 16:40:16.000000 informative_iterator-2.0.2/informative_iterator/settings.json
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-08-02 17:01:48.120097 informative_iterator-2.0.2/informative_iterator.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     3241 2023-08-02 17:01:47.000000 informative_iterator-2.0.2/informative_iterator.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)    29812 2023-08-02 17:01:48.000000 informative_iterator-2.0.2/informative_iterator.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-08-02 17:01:47.000000 informative_iterator-2.0.2/informative_iterator.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       21 2023-08-02 17:01:47.000000 informative_iterator-2.0.2/informative_iterator.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-08-02 17:01:48.245899 informative_iterator-2.0.2/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1551 2023-08-02 16:43:57.000000 informative_iterator-2.0.2/setup.py
```

### Comparing `informative_iterator-2.0.1/PKG-INFO` & `informative_iterator-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: informative_iterator
-Version: 2.0.1
+Version: 2.0.2
 Summary: A replacement for tqdm
 Home-page: https://github.com/jeff-hykin/informative-iterator.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__init__.py` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__init__.py`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__pycache__/__init__.cpython-38.pyc` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/.gitignore` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/.gitignore`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/README.md` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/README.md`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/commands` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/commands`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/purge` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/project/purge`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/shell` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/shell`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/commands/start` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/commands/start`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/fornix_framework.md`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/cd_tutorial.gif`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_from_example.png`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_name.png`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/images/package_versions.png`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/setup.md` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/documentation/setup.md`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/__init__.py`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/file_system_py/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/license.txt` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/license.txt`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/main/setup.py` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/main/setup.py`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/poetry.lock` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/poetry.lock`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/run/tests` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/run/tests`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/run/tests.ps1` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/run/tests.ps1`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_purge/802_remove_venv.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/001_000__setup_zsh__.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/019_000_setup_python_venv.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/021_000_ensure_pip_modules.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/091_000_commands_function.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/093_000_customize_ll_function.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start/094_000_jeffs_git_shortcuts.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_deno_store.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_nix_channel.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/during_start_prep/060_010_link_tealdeer.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/add_execute_permission`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/copy`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/file_system/relative_link`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/basic_init_example`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/inject_into_path`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/merge_all_templates`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/fornix/trigger`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/ignore`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/commands/mixin`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-merge/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/post-update/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/cacert.pem`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/ensure_nix_installed`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/fix_ssl`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/lib_path_for`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/commands/package_path_for`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/installer_helper`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nix.toml`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/nixpkgs/salt.nix`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/parse_dependencies.nix`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/shell.nix`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/nix/uninstaller_helper`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/ensure_pip_modules`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/commands/setup_venv`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/extensions/python/during_purge.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/fornix_core` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/fornix_core`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/home/.zshenv` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/home/.zshenv`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/requirements/advanced_system_tools.nix`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/settings/requirements/system_tools.toml`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/file_system_py/tests/main.py` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/file_system_py/tests/main.py`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/.gitignore` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/.gitignore`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/README.md` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/README.md`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/project/commands` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/project/commands`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/project/purge` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/project/purge`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/shell` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/shell`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/commands/start` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/commands/start`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/fornix_framework.md` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/fornix_framework.md`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/cd_tutorial.gif` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/cd_tutorial.gif`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_from_example.png` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_from_example.png`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_name.png` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_name.png`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_versions.png` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/images/package_versions.png`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/documentation/setup.md` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/documentation/setup.md`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/license.txt` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/license.txt`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/setup.py` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/setup.py`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/__init__.py` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/__init__.py`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/__pycache__/__init__.cpython-38.pyc` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/neo_map.py` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/main/super_map/neo_map.py`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/poetry.lock` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/poetry.lock`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_manual_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_purge/802_remove_venv.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_purge/802_remove_venv.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/001_000__setup_zsh__.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/001_000__setup_zsh__.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/019_000_setup_python_venv.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/019_000_setup_python_venv.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/021_000_ensure_pip_modules.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/021_000_ensure_pip_modules.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/081_000__ensure_all_commands_executable__.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/081_000__ensure_all_commands_executable__.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/091_000_commands_function.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/091_000_commands_function.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/093_000_customize_ll_function.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/093_000_customize_ll_function.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/094_000_jeffs_git_shortcuts.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start/094_000_jeffs_git_shortcuts.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_deno_store.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_deno_store.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_nix_channel.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_nix_channel.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_tealdeer.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/during_start_prep/060_010_link_tealdeer.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/#establish_extension.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/add_execute_permission` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/add_execute_permission`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/copy` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/copy`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/relative_link` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/file_system/relative_link`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/basic_init_example` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/basic_init_example`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/create_wrapped_command`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/ensure_all_commands_executable`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/inject_into_path` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/inject_into_path`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/merge_all_templates` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/merge_all_templates`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/trigger` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/fornix/trigger`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/#standard/commands/tools/string/remove_spaces_from_names`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/#establish_extension.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/commands/ignore` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/commands/ignore`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/commands/mixin` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/commands/mixin`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-merge/901_check_pip_modules` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-merge/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-update/901_check_pip_modules` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/post-update/901_check_pip_modules`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/git/hooks/pre-commit/002_prevent_large_files.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/#establish_extension.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/cacert.pem` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/cacert.pem`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/ensure_nix_installed` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/ensure_nix_installed`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/fix_ssl` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/fix_ssl`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/lib_path_for` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/lib_path_for`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/package_path_for` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/commands/package_path_for`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/installer_helper` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/installer_helper`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/nix.toml` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/nix.toml`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/parse_dependencies.nix` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/parse_dependencies.nix`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/shell.nix` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/shell.nix`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/uninstaller_helper` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/nix/uninstaller_helper`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/#establish_extension.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/#establish_extension.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/ensure_pip_modules` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/ensure_pip_modules`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/setup_venv` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/commands/setup_venv`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/during_purge.sh` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/extensions/python/during_purge.sh`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/fornix_core` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/fornix_core`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/home/.zshenv` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/home/.zshenv`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/requirements/advanced_system_tools.nix` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/requirements/advanced_system_tools.nix`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__dependencies__/__sources__/super_map/settings/requirements/system_tools.toml` & `informative_iterator-2.0.2/informative_iterator/__dependencies__/__sources__/super_map/settings/requirements/system_tools.toml`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/informative_iterator/__init__.py` & `informative_iterator-2.0.2/informative_iterator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # heavily adpted from: https://raw.githubusercontent.com/PaoloLRinaldi/progress_bar_python/master/perc.py
 from datetime import datetime, timedelta
 from statistics import mean, stdev
 import time
 import sys
 import math
 
-from __dependencies__.super_map import LazyDict
+from .__dependencies__.super_map import LazyDict
 
 # nested indentation support
 try:
     from blissful_basics import print as bliss_print
 except Exception as error:
     # create a placeholder/stand-in
     def bliss_print(*args, **kwargs):
```

### Comparing `informative_iterator-2.0.1/informative_iterator.egg-info/PKG-INFO` & `informative_iterator-2.0.2/informative_iterator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: informative-iterator
-Version: 2.0.1
+Version: 2.0.2
 Summary: A replacement for tqdm
 Home-page: https://github.com/jeff-hykin/informative-iterator.git
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `informative_iterator-2.0.1/informative_iterator.egg-info/SOURCES.txt` & `informative_iterator-2.0.2/informative_iterator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `informative_iterator-2.0.1/setup.py` & `informative_iterator-2.0.2/setup.py`

 * *Files identical despite different names*

