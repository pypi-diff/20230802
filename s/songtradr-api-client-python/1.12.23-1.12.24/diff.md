# Comparing `tmp/songtradr-api-client-python-1.12.23.tar.gz` & `tmp/songtradr-api-client-python-1.12.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songtradr-api-client-python-1.12.23.tar", last modified: Mon Jul 17 09:06:33 2023, max compression
+gzip compressed data, was "songtradr-api-client-python-1.12.24.tar", last modified: Wed Aug  2 12:54:39 2023, max compression
```

## Comparing `songtradr-api-client-python-1.12.23.tar` & `songtradr-api-client-python-1.12.24.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:33.265555 songtradr-api-client-python-1.12.23/
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-17 09:06:33.265555 songtradr-api-client-python-1.12.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-17 09:06:33.269554 songtradr-api-client-python-1.12.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:33.249555 songtradr-api-client-python-1.12.23/songtradr_api_client_python/
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:33.249555 songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21722 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/allowed_values_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/api_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/party_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/playlist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    96081 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/recording_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   255960 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31745 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:33.257555 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/admin_api_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/api_key_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/category_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/category_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/config_access_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/config_identifier_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/contributor_type_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/create_api_key_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/field_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_minimal_with_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_upload_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_w_ith_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/files_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/forgot_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/genre_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/genres_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/init_put_recording_audio_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/jwt_token_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/login_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    41920 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/p_line_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/party_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/party_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/playlist_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/product_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/product_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_for_similarity_search_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_genre_prediction_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    66338 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_file_recording_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_recording_genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_recording_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_recording_tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_referrer_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    24182 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/search_filter_values_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/search_recording_granular_abstraction_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/search_recording_granular_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/sign_up_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/taggram_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/tags_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/tagstrength_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/title_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/track_to_medium_product_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/update_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/usage_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/user_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:33.249555 songtradr-api-client-python-1.12.23/songtradr_api_client_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-17 09:06:33.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-07-17 09:06:33.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:06:33.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-17 09:06:33.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 09:06:33.000000 songtradr-api-client-python-1.12.23/songtradr_api_client_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:33.265555 songtradr-api-client-python-1.12.23/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_admin_api_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_allowed_values_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_api_key_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_api_keys_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_category_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_category_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_config_access_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_config_identifier_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_contributor_type_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_create_api_key_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_field_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_file_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    22975 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_file_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_file_minimal_with_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_file_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_file_upload_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    21599 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_file_w_ith_url_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_files_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_forgot_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_genre_minimal_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-17 09:06:19.000000 songtradr-api-client-python-1.12.23/test/test_genres_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_init_put_recording_audio_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_jwt_token_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_login_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_p_line_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_party_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_party_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_party_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_playlist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_playlist_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_product_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_product_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_for_similarity_search_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_genre_prediction_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_large_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    19341 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_list_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_medium_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_minimal_with_musical_features_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_minimal_with_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_minimal_with_tagstrengths_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_recording_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    14624 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_save_file_recording_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_save_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_save_recording_genre_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_save_recording_party_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_save_recording_playlist_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_save_recording_tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_save_referrer_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_save_taggrams_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_save_user_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_search_filter_values_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_search_recording_granular_abstraction_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_search_recording_granular_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_sign_up_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_tag_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_tag_small_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_taggram_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_tags_summary_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_tagstrength_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_title_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_track_to_medium_product_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_update_password_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_usage_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-17 09:06:20.000000 songtradr-api-client-python-1.12.23/test/test_user_dto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:54:39.963872 songtradr-api-client-python-1.12.24/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-02 12:54:39.963872 songtradr-api-client-python-1.12.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14758 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-02 12:54:39.963872 songtradr-api-client-python-1.12.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:54:39.907871 songtradr-api-client-python-1.12.24/songtradr_api_client_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:54:39.911871 songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22080 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/allowed_values_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/party_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/playlist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96537 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/recording_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   256410 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31745 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:54:39.939871 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/admin_api_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/api_key_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/category_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/category_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/config_access_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/config_identifier_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/contributor_type_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/create_api_key_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/field_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_minimal_with_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_upload_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_w_ith_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/files_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/forgot_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/genre_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/genres_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/init_put_recording_audio_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/jwt_token_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/login_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41921 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/p_line_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/party_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/party_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/playlist_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/product_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/product_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_for_similarity_search_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_genre_prediction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66339 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_file_recording_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_recording_genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_recording_tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_referrer_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24183 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/search_filter_values_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/search_recording_granular_abstraction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/search_recording_granular_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/sign_up_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/taggram_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/tags_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/tagstrength_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/title_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/track_to_medium_product_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/update_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/usage_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:54:39.911871 songtradr-api-client-python-1.12.24/songtradr_api_client_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-02 12:54:39.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-08-02 12:54:39.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:54:39.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 12:54:39.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 12:54:39.000000 songtradr-api-client-python-1.12.24/songtradr_api_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:54:39.963872 songtradr-api-client-python-1.12.24/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_admin_api_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/test/test_allowed_values_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_api_key_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/test/test_api_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_category_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_category_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_config_access_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_config_identifier_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_contributor_type_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_create_api_key_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_field_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_file_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22975 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_file_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_file_minimal_with_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_file_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_file_upload_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21599 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_file_w_ith_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_files_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_forgot_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_genre_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_genres_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_init_put_recording_audio_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_jwt_token_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_login_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_p_line_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/test/test_party_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_party_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_party_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/test/test_playlist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_playlist_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_product_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_product_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/test/test_recording_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_for_similarity_search_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_genre_prediction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19341 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_minimal_with_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_minimal_with_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_minimal_with_tagstrengths_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_recording_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14624 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_save_file_recording_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_save_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_save_recording_genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_save_recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_save_recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_save_recording_tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_save_referrer_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_save_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_save_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_search_filter_values_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_search_recording_granular_abstraction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_search_recording_granular_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_sign_up_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_taggram_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_tags_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_tagstrength_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_title_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_track_to_medium_product_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_update_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_usage_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-08-02 12:54:25.000000 songtradr-api-client-python-1.12.24/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-08-02 12:54:24.000000 songtradr-api-client-python-1.12.24/test/test_user_dto.py
```

### Comparing `songtradr-api-client-python-1.12.23/PKG-INFO` & `songtradr-api-client-python-1.12.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songtradr-api-client-python
-Version: 1.12.23
+Version: 1.12.24
 Summary: Songtradr API
 Home-page: https://github.com/songtradr/songtradr-python-api-client-docs
 Author: Songtradr Inc.
 Author-email: info@songtradr.com
 Keywords: OpenAPI,OpenAPI-Generator,Songtradr API
 Description-Content-Type: text/markdown
```

### Comparing `songtradr-api-client-python-1.12.23/README.md` & `songtradr-api-client-python-1.12.24/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.
 
 1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters.
 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.12.23
-- Package version: 1.12.23
+- API version: 1.12.24
+- Package version: 1.12.24
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://songtradr.com](https://songtradr.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `songtradr-api-client-python-1.12.23/pyproject.toml` & `songtradr-api-client-python-1.12.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "songtradr_api_client_python"
-version = "1.12.23"
+version = "1.12.24"
 description = "Songtradr API"
 authors = ["Songtradr Inc. <info@songtradr.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Songtradr API"]
 include = ["songtradr_api_client_python/py.typed"]
```

### Comparing `songtradr-api-client-python-1.12.23/setup.py` & `songtradr-api-client-python-1.12.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "songtradr-api-client-python"
-VERSION = "1.12.23"
+VERSION = "1.12.24"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/__init__.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "1.12.23"
+__version__ = "1.12.24"
 
 # import apis into sdk package
 from songtradr_api_client_python.api.api_keys_api import APIKeysApi
 from songtradr_api_client_python.api.allowed_values_api import AllowedValuesApi
 from songtradr_api_client_python.api.party_api import PartyApi
 from songtradr_api_client_python.api.playlist_api import PlaylistApi
 from songtradr_api_client_python.api.recording_api import RecordingApi
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/allowed_values_api.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/allowed_values_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -144,15 +144,15 @@
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
         if _params.get('response_size') is not None:  # noqa: E501
-            _query_params.append(('responseSize', _params['response_size'].value))
+            _query_params.append(('responseSize', _params['response_size']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
@@ -185,24 +185,24 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def genres(self, genre_type : Annotated[StrictStr, Field(..., description="Type of the response should have.")], **kwargs) -> List[GenreDTO]:  # noqa: E501
+    def genres(self, genre_type : Annotated[StrictStr, Field(..., description="Type of the response should have.  Deprecated: level1Genre, level2Genre - use musicubeLevel1Genre, musicubeLevel2Genre instead.")], **kwargs) -> List[GenreDTO]:  # noqa: E501
         """Allowed values for genres.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.genres(genre_type, async_req=True)
         >>> result = thread.get()
 
-        :param genre_type: Type of the response should have. (required)
+        :param genre_type: Type of the response should have.  Deprecated: level1Genre, level2Genre - use musicubeLevel1Genre, musicubeLevel2Genre instead. (required)
         :type genre_type: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -213,24 +213,24 @@
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the genres_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.genres_with_http_info(genre_type, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def genres_with_http_info(self, genre_type : Annotated[StrictStr, Field(..., description="Type of the response should have.")], **kwargs) -> ApiResponse:  # noqa: E501
+    def genres_with_http_info(self, genre_type : Annotated[StrictStr, Field(..., description="Type of the response should have.  Deprecated: level1Genre, level2Genre - use musicubeLevel1Genre, musicubeLevel2Genre instead.")], **kwargs) -> ApiResponse:  # noqa: E501
         """Allowed values for genres.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.genres_with_http_info(genre_type, async_req=True)
         >>> result = thread.get()
 
-        :param genre_type: Type of the response should have. (required)
+        :param genre_type: Type of the response should have.  Deprecated: level1Genre, level2Genre - use musicubeLevel1Genre, musicubeLevel2Genre instead. (required)
         :type genre_type: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
@@ -284,15 +284,15 @@
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
         if _params.get('genre_type') is not None:  # noqa: E501
-            _query_params.append(('genreType', _params['genre_type'].value))
+            _query_params.append(('genreType', _params['genre_type']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
@@ -426,15 +426,15 @@
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
         if _params.get('category_name') is not None:  # noqa: E501
-            _query_params.append(('categoryName', _params['category_name'].value))
+            _query_params.append(('categoryName', _params['category_name']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/api_keys_api.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/api_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/party_api.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/party_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/playlist_api.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/playlist_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -164,15 +164,15 @@
         if _params.get('include_recordings') is not None:  # noqa: E501
             _query_params.append(('includeRecordings', _params['include_recordings']))
 
         if _params.get('ignore_usages') is not None:  # noqa: E501
             _query_params.append(('ignoreUsages', _params['ignore_usages']))
 
         if _params.get('usage_filter_mode') is not None:  # noqa: E501
-            _query_params.append(('usageFilterMode', _params['usage_filter_mode'].value))
+            _query_params.append(('usageFilterMode', _params['usage_filter_mode']))
 
         if _params.get('songtradr_playlist_guid') is not None:  # noqa: E501
             _query_params.append(('songtradrPlaylistGuid', _params['songtradr_playlist_guid']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
@@ -333,16 +333,16 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearer-jwt']  # noqa: E501
 
         _response_types_map = {
-            '403': "ErrorResponse",
             '200': "object",
+            '403': "ErrorResponse",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
 
         return self.api_client.call_api(
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/recording_api.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/recording_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -459,15 +459,15 @@
         if _params['ids']:
             _path_params['ids'] = _params['ids']
 
 
         # process the query parameters
         _query_params = []
         if _params.get('category_name') is not None:  # noqa: E501
-            _query_params.append(('categoryName', _params['category_name'].value))
+            _query_params.append(('categoryName', _params['category_name']))
 
         if _params.get('tag_name') is not None:  # noqa: E501
             _query_params.append(('tagName', _params['tag_name']))
 
         if _params.get('genre_name') is not None:  # noqa: E501
             _query_params.append(('genreName', _params['genre_name']))
 
@@ -629,15 +629,15 @@
         if _params['ids']:
             _path_params['ids'] = _params['ids']
 
 
         # process the query parameters
         _query_params = []
         if _params.get('category_name') is not None:  # noqa: E501
-            _query_params.append(('categoryName', _params['category_name'].value))
+            _query_params.append(('categoryName', _params['category_name']))
 
         if _params.get('tag_name') is not None:  # noqa: E501
             _query_params.append(('tagName', _params['tag_name']))
 
         if _params.get('genre_name') is not None:  # noqa: E501
             _query_params.append(('genreName', _params['genre_name']))
 
@@ -1121,33 +1121,35 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def search_recordings(self, similar_to_recording : Annotated[Optional[StrictStr], Field(description="Search for songs similar to a recording.")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre : Annotated[Optional[StrictStr], Field(description="Search for a genre.")] = None, primary_mood_cluster : Annotated[Optional[StrictStr], Field(description="Search for a mood.")] = None, valence : Annotated[Optional[StrictStr], Field(description="Search for valence.")] = None, arousal : Annotated[Optional[StrictStr], Field(description="Search for arousal.")] = None, pleasantness : Annotated[Optional[StrictStr], Field(description="Search for pleasantness.")] = None, engagement : Annotated[Optional[StrictStr], Field(description="Search for an engagement.")] = None, vocals : Annotated[Optional[StrictStr], Field(description="Search for a vocals gender or instrumental songs.")] = None, dominant_instrument : Annotated[Optional[StrictStr], Field(description="Search for a dominant instrument.")] = None, energy : Annotated[Optional[StrictStr], Field(description="Search for energy.")] = None, sound_generation : Annotated[Optional[StrictStr], Field(description="Search for type of sound generation.")] = None, tempo : Annotated[Optional[StrictStr], Field(description="Search for tempo.")] = None, scale : Annotated[Optional[StrictStr], Field(description="Search for tonal scale.")] = None, key : Annotated[Optional[StrictStr], Field(description="Search for harmonic key.")] = None, rhythm : Annotated[Optional[StrictStr], Field(description="Search for rhythm.")] = None, primary_sound_character : Annotated[Optional[StrictStr], Field(description="Search for a sound character.")] = None, timbre : Annotated[Optional[StrictStr], Field(description="Search for timbre.")] = None, roughness : Annotated[Optional[StrictStr], Field(description="Search for roughness.")] = None, tonality : Annotated[Optional[StrictStr], Field(description="Search for tonality.")] = None, harmony : Annotated[Optional[StrictStr], Field(description="Search for a degree of harmoniousness.")] = None, texture : Annotated[Optional[StrictStr], Field(description="Search for texture.")] = None, groovyness : Annotated[Optional[StrictStr], Field(description="Search for groovyness.")] = None, space : Annotated[Optional[StrictStr], Field(description="Search for space.")] = None, origin_decade : Annotated[Optional[StrictStr], Field(description="Search for origin decade.")] = None, curateability : Annotated[Optional[StrictStr], Field(description="Search for curateability.")] = None, use_case : Annotated[Optional[StrictStr], Field(description="Search for use case.")] = None, channel_suitability : Annotated[Optional[StrictStr], Field(description="Search for channel suitability.")] = None, songtradr_track_id : Annotated[Optional[StrictStr], Field(description="Search for Songtradr track id.")] = None, shuffled : Annotated[Optional[StrictStr], Field(description="Sort the results randomly.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort the results.")] = None, page : Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None, **kwargs) -> RecordingListDTO:  # noqa: E501
+    def search_recordings(self, similar_to_recording : Annotated[Optional[StrictStr], Field(description="Search for songs similar to a recording.")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, party_and_title : Annotated[Optional[StrictStr], Field(description="Search for party and title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre : Annotated[Optional[StrictStr], Field(description="Search for a genre.")] = None, primary_mood_cluster : Annotated[Optional[StrictStr], Field(description="Search for a mood.")] = None, valence : Annotated[Optional[StrictStr], Field(description="Search for valence.")] = None, arousal : Annotated[Optional[StrictStr], Field(description="Search for arousal.")] = None, pleasantness : Annotated[Optional[StrictStr], Field(description="Search for pleasantness.")] = None, engagement : Annotated[Optional[StrictStr], Field(description="Search for an engagement.")] = None, vocals : Annotated[Optional[StrictStr], Field(description="Search for a vocals gender or instrumental songs.")] = None, dominant_instrument : Annotated[Optional[StrictStr], Field(description="Search for a dominant instrument.")] = None, energy : Annotated[Optional[StrictStr], Field(description="Search for energy.")] = None, sound_generation : Annotated[Optional[StrictStr], Field(description="Search for type of sound generation.")] = None, tempo : Annotated[Optional[StrictStr], Field(description="Search for tempo.")] = None, scale : Annotated[Optional[StrictStr], Field(description="Search for tonal scale.")] = None, key : Annotated[Optional[StrictStr], Field(description="Search for harmonic key.")] = None, rhythm : Annotated[Optional[StrictStr], Field(description="Search for rhythm.")] = None, primary_sound_character : Annotated[Optional[StrictStr], Field(description="Search for a sound character.")] = None, timbre : Annotated[Optional[StrictStr], Field(description="Search for timbre.")] = None, roughness : Annotated[Optional[StrictStr], Field(description="Search for roughness.")] = None, tonality : Annotated[Optional[StrictStr], Field(description="Search for tonality.")] = None, harmony : Annotated[Optional[StrictStr], Field(description="Search for a degree of harmoniousness.")] = None, texture : Annotated[Optional[StrictStr], Field(description="Search for texture.")] = None, groovyness : Annotated[Optional[StrictStr], Field(description="Search for groovyness.")] = None, space : Annotated[Optional[StrictStr], Field(description="Search for space.")] = None, origin_decade : Annotated[Optional[StrictStr], Field(description="Search for origin decade.")] = None, curateability : Annotated[Optional[StrictStr], Field(description="Search for curateability.")] = None, use_case : Annotated[Optional[StrictStr], Field(description="Search for use case.")] = None, channel_suitability : Annotated[Optional[StrictStr], Field(description="Search for channel suitability.")] = None, songtradr_track_id : Annotated[Optional[StrictStr], Field(description="Search for Songtradr track id.")] = None, shuffled : Annotated[Optional[StrictStr], Field(description="Sort the results randomly.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort the results.")] = None, page : Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None, **kwargs) -> RecordingListDTO:  # noqa: E501
         """Recordings by contributors, moods, musical features and more.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.search_recordings(similar_to_recording, contributor, main_artist, composer, title, language, genre, primary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, energy, sound_generation, tempo, scale, key, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, origin_decade, curateability, use_case, channel_suitability, songtradr_track_id, shuffled, sort, page, size, async_req=True)
+        >>> thread = api.search_recordings(similar_to_recording, contributor, main_artist, composer, title, party_and_title, language, genre, primary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, energy, sound_generation, tempo, scale, key, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, origin_decade, curateability, use_case, channel_suitability, songtradr_track_id, shuffled, sort, page, size, async_req=True)
         >>> result = thread.get()
 
         :param similar_to_recording: Search for songs similar to a recording.
         :type similar_to_recording: str
         :param contributor: Search for a name that was involved as any contributor.
         :type contributor: str
         :param main_artist: Search for a main artist.
         :type main_artist: str
         :param composer: Search for a composer.
         :type composer: str
         :param title: Search for a title.
         :type title: str
+        :param party_and_title: Search for party and title.
+        :type party_and_title: str
         :param language: Search for a language of the lyrics.
         :type language: str
         :param genre: Search for a genre.
         :type genre: str
         :param primary_mood_cluster: Search for a mood.
         :type primary_mood_cluster: str
         :param valence: Search for valence.
@@ -1218,36 +1220,38 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: RecordingListDTO
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the search_recordings_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.search_recordings_with_http_info(similar_to_recording, contributor, main_artist, composer, title, language, genre, primary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, energy, sound_generation, tempo, scale, key, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, origin_decade, curateability, use_case, channel_suitability, songtradr_track_id, shuffled, sort, page, size, **kwargs)  # noqa: E501
+        return self.search_recordings_with_http_info(similar_to_recording, contributor, main_artist, composer, title, party_and_title, language, genre, primary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, energy, sound_generation, tempo, scale, key, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, origin_decade, curateability, use_case, channel_suitability, songtradr_track_id, shuffled, sort, page, size, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def search_recordings_with_http_info(self, similar_to_recording : Annotated[Optional[StrictStr], Field(description="Search for songs similar to a recording.")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre : Annotated[Optional[StrictStr], Field(description="Search for a genre.")] = None, primary_mood_cluster : Annotated[Optional[StrictStr], Field(description="Search for a mood.")] = None, valence : Annotated[Optional[StrictStr], Field(description="Search for valence.")] = None, arousal : Annotated[Optional[StrictStr], Field(description="Search for arousal.")] = None, pleasantness : Annotated[Optional[StrictStr], Field(description="Search for pleasantness.")] = None, engagement : Annotated[Optional[StrictStr], Field(description="Search for an engagement.")] = None, vocals : Annotated[Optional[StrictStr], Field(description="Search for a vocals gender or instrumental songs.")] = None, dominant_instrument : Annotated[Optional[StrictStr], Field(description="Search for a dominant instrument.")] = None, energy : Annotated[Optional[StrictStr], Field(description="Search for energy.")] = None, sound_generation : Annotated[Optional[StrictStr], Field(description="Search for type of sound generation.")] = None, tempo : Annotated[Optional[StrictStr], Field(description="Search for tempo.")] = None, scale : Annotated[Optional[StrictStr], Field(description="Search for tonal scale.")] = None, key : Annotated[Optional[StrictStr], Field(description="Search for harmonic key.")] = None, rhythm : Annotated[Optional[StrictStr], Field(description="Search for rhythm.")] = None, primary_sound_character : Annotated[Optional[StrictStr], Field(description="Search for a sound character.")] = None, timbre : Annotated[Optional[StrictStr], Field(description="Search for timbre.")] = None, roughness : Annotated[Optional[StrictStr], Field(description="Search for roughness.")] = None, tonality : Annotated[Optional[StrictStr], Field(description="Search for tonality.")] = None, harmony : Annotated[Optional[StrictStr], Field(description="Search for a degree of harmoniousness.")] = None, texture : Annotated[Optional[StrictStr], Field(description="Search for texture.")] = None, groovyness : Annotated[Optional[StrictStr], Field(description="Search for groovyness.")] = None, space : Annotated[Optional[StrictStr], Field(description="Search for space.")] = None, origin_decade : Annotated[Optional[StrictStr], Field(description="Search for origin decade.")] = None, curateability : Annotated[Optional[StrictStr], Field(description="Search for curateability.")] = None, use_case : Annotated[Optional[StrictStr], Field(description="Search for use case.")] = None, channel_suitability : Annotated[Optional[StrictStr], Field(description="Search for channel suitability.")] = None, songtradr_track_id : Annotated[Optional[StrictStr], Field(description="Search for Songtradr track id.")] = None, shuffled : Annotated[Optional[StrictStr], Field(description="Sort the results randomly.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort the results.")] = None, page : Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def search_recordings_with_http_info(self, similar_to_recording : Annotated[Optional[StrictStr], Field(description="Search for songs similar to a recording.")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, party_and_title : Annotated[Optional[StrictStr], Field(description="Search for party and title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre : Annotated[Optional[StrictStr], Field(description="Search for a genre.")] = None, primary_mood_cluster : Annotated[Optional[StrictStr], Field(description="Search for a mood.")] = None, valence : Annotated[Optional[StrictStr], Field(description="Search for valence.")] = None, arousal : Annotated[Optional[StrictStr], Field(description="Search for arousal.")] = None, pleasantness : Annotated[Optional[StrictStr], Field(description="Search for pleasantness.")] = None, engagement : Annotated[Optional[StrictStr], Field(description="Search for an engagement.")] = None, vocals : Annotated[Optional[StrictStr], Field(description="Search for a vocals gender or instrumental songs.")] = None, dominant_instrument : Annotated[Optional[StrictStr], Field(description="Search for a dominant instrument.")] = None, energy : Annotated[Optional[StrictStr], Field(description="Search for energy.")] = None, sound_generation : Annotated[Optional[StrictStr], Field(description="Search for type of sound generation.")] = None, tempo : Annotated[Optional[StrictStr], Field(description="Search for tempo.")] = None, scale : Annotated[Optional[StrictStr], Field(description="Search for tonal scale.")] = None, key : Annotated[Optional[StrictStr], Field(description="Search for harmonic key.")] = None, rhythm : Annotated[Optional[StrictStr], Field(description="Search for rhythm.")] = None, primary_sound_character : Annotated[Optional[StrictStr], Field(description="Search for a sound character.")] = None, timbre : Annotated[Optional[StrictStr], Field(description="Search for timbre.")] = None, roughness : Annotated[Optional[StrictStr], Field(description="Search for roughness.")] = None, tonality : Annotated[Optional[StrictStr], Field(description="Search for tonality.")] = None, harmony : Annotated[Optional[StrictStr], Field(description="Search for a degree of harmoniousness.")] = None, texture : Annotated[Optional[StrictStr], Field(description="Search for texture.")] = None, groovyness : Annotated[Optional[StrictStr], Field(description="Search for groovyness.")] = None, space : Annotated[Optional[StrictStr], Field(description="Search for space.")] = None, origin_decade : Annotated[Optional[StrictStr], Field(description="Search for origin decade.")] = None, curateability : Annotated[Optional[StrictStr], Field(description="Search for curateability.")] = None, use_case : Annotated[Optional[StrictStr], Field(description="Search for use case.")] = None, channel_suitability : Annotated[Optional[StrictStr], Field(description="Search for channel suitability.")] = None, songtradr_track_id : Annotated[Optional[StrictStr], Field(description="Search for Songtradr track id.")] = None, shuffled : Annotated[Optional[StrictStr], Field(description="Sort the results randomly.")] = None, sort : Annotated[Optional[StrictStr], Field(description="Sort the results.")] = None, page : Annotated[Optional[StrictInt], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[StrictInt], Field(description="The size of the page to be returned")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """Recordings by contributors, moods, musical features and more.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.search_recordings_with_http_info(similar_to_recording, contributor, main_artist, composer, title, language, genre, primary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, energy, sound_generation, tempo, scale, key, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, origin_decade, curateability, use_case, channel_suitability, songtradr_track_id, shuffled, sort, page, size, async_req=True)
+        >>> thread = api.search_recordings_with_http_info(similar_to_recording, contributor, main_artist, composer, title, party_and_title, language, genre, primary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, energy, sound_generation, tempo, scale, key, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, origin_decade, curateability, use_case, channel_suitability, songtradr_track_id, shuffled, sort, page, size, async_req=True)
         >>> result = thread.get()
 
         :param similar_to_recording: Search for songs similar to a recording.
         :type similar_to_recording: str
         :param contributor: Search for a name that was involved as any contributor.
         :type contributor: str
         :param main_artist: Search for a main artist.
         :type main_artist: str
         :param composer: Search for a composer.
         :type composer: str
         :param title: Search for a title.
         :type title: str
+        :param party_and_title: Search for party and title.
+        :type party_and_title: str
         :param language: Search for a language of the lyrics.
         :type language: str
         :param genre: Search for a genre.
         :type genre: str
         :param primary_mood_cluster: Search for a mood.
         :type primary_mood_cluster: str
         :param valence: Search for valence.
@@ -1337,14 +1341,15 @@
 
         _all_params = [
             'similar_to_recording',
             'contributor',
             'main_artist',
             'composer',
             'title',
+            'party_and_title',
             'language',
             'genre',
             'primary_mood_cluster',
             'valence',
             'arousal',
             'pleasantness',
             'engagement',
@@ -1414,103 +1419,106 @@
 
         if _params.get('composer') is not None:  # noqa: E501
             _query_params.append(('composer', _params['composer']))
 
         if _params.get('title') is not None:  # noqa: E501
             _query_params.append(('title', _params['title']))
 
+        if _params.get('party_and_title') is not None:  # noqa: E501
+            _query_params.append(('partyAndTitle', _params['party_and_title']))
+
         if _params.get('language') is not None:  # noqa: E501
-            _query_params.append(('language', _params['language'].value))
+            _query_params.append(('language', _params['language']))
 
         if _params.get('genre') is not None:  # noqa: E501
             _query_params.append(('genre', _params['genre']))
 
         if _params.get('primary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('primaryMoodCluster', _params['primary_mood_cluster'].value))
+            _query_params.append(('primaryMoodCluster', _params['primary_mood_cluster']))
 
         if _params.get('valence') is not None:  # noqa: E501
-            _query_params.append(('valence', _params['valence'].value))
+            _query_params.append(('valence', _params['valence']))
 
         if _params.get('arousal') is not None:  # noqa: E501
-            _query_params.append(('arousal', _params['arousal'].value))
+            _query_params.append(('arousal', _params['arousal']))
 
         if _params.get('pleasantness') is not None:  # noqa: E501
-            _query_params.append(('pleasantness', _params['pleasantness'].value))
+            _query_params.append(('pleasantness', _params['pleasantness']))
 
         if _params.get('engagement') is not None:  # noqa: E501
-            _query_params.append(('engagement', _params['engagement'].value))
+            _query_params.append(('engagement', _params['engagement']))
 
         if _params.get('vocals') is not None:  # noqa: E501
-            _query_params.append(('vocals', _params['vocals'].value))
+            _query_params.append(('vocals', _params['vocals']))
 
         if _params.get('dominant_instrument') is not None:  # noqa: E501
-            _query_params.append(('dominantInstrument', _params['dominant_instrument'].value))
+            _query_params.append(('dominantInstrument', _params['dominant_instrument']))
 
         if _params.get('energy') is not None:  # noqa: E501
-            _query_params.append(('energy', _params['energy'].value))
+            _query_params.append(('energy', _params['energy']))
 
         if _params.get('sound_generation') is not None:  # noqa: E501
-            _query_params.append(('soundGeneration', _params['sound_generation'].value))
+            _query_params.append(('soundGeneration', _params['sound_generation']))
 
         if _params.get('tempo') is not None:  # noqa: E501
-            _query_params.append(('tempo', _params['tempo'].value))
+            _query_params.append(('tempo', _params['tempo']))
 
         if _params.get('scale') is not None:  # noqa: E501
-            _query_params.append(('scale', _params['scale'].value))
+            _query_params.append(('scale', _params['scale']))
 
         if _params.get('key') is not None:  # noqa: E501
-            _query_params.append(('key', _params['key'].value))
+            _query_params.append(('key', _params['key']))
 
         if _params.get('rhythm') is not None:  # noqa: E501
-            _query_params.append(('rhythm', _params['rhythm'].value))
+            _query_params.append(('rhythm', _params['rhythm']))
 
         if _params.get('primary_sound_character') is not None:  # noqa: E501
-            _query_params.append(('primarySoundCharacter', _params['primary_sound_character'].value))
+            _query_params.append(('primarySoundCharacter', _params['primary_sound_character']))
 
         if _params.get('timbre') is not None:  # noqa: E501
-            _query_params.append(('timbre', _params['timbre'].value))
+            _query_params.append(('timbre', _params['timbre']))
 
         if _params.get('roughness') is not None:  # noqa: E501
-            _query_params.append(('roughness', _params['roughness'].value))
+            _query_params.append(('roughness', _params['roughness']))
 
         if _params.get('tonality') is not None:  # noqa: E501
-            _query_params.append(('tonality', _params['tonality'].value))
+            _query_params.append(('tonality', _params['tonality']))
 
         if _params.get('harmony') is not None:  # noqa: E501
-            _query_params.append(('harmony', _params['harmony'].value))
+            _query_params.append(('harmony', _params['harmony']))
 
         if _params.get('texture') is not None:  # noqa: E501
-            _query_params.append(('texture', _params['texture'].value))
+            _query_params.append(('texture', _params['texture']))
 
         if _params.get('groovyness') is not None:  # noqa: E501
-            _query_params.append(('groovyness', _params['groovyness'].value))
+            _query_params.append(('groovyness', _params['groovyness']))
 
         if _params.get('space') is not None:  # noqa: E501
-            _query_params.append(('space', _params['space'].value))
+            _query_params.append(('space', _params['space']))
 
         if _params.get('origin_decade') is not None:  # noqa: E501
-            _query_params.append(('originDecade', _params['origin_decade'].value))
+            _query_params.append(('originDecade', _params['origin_decade']))
 
         if _params.get('curateability') is not None:  # noqa: E501
-            _query_params.append(('curateability', _params['curateability'].value))
+            _query_params.append(('curateability', _params['curateability']))
 
         if _params.get('use_case') is not None:  # noqa: E501
-            _query_params.append(('useCase', _params['use_case'].value))
+            _query_params.append(('useCase', _params['use_case']))
 
         if _params.get('channel_suitability') is not None:  # noqa: E501
-            _query_params.append(('channelSuitability', _params['channel_suitability'].value))
+            _query_params.append(('channelSuitability', _params['channel_suitability']))
 
         if _params.get('songtradr_track_id') is not None:  # noqa: E501
             _query_params.append(('songtradrTrackId', _params['songtradr_track_id']))
 
         if _params.get('shuffled') is not None:  # noqa: E501
-            _query_params.append(('shuffled', _params['shuffled'].value))
+            _query_params.append(('shuffled', _params['shuffled']))
 
         if _params.get('sort') is not None:  # noqa: E501
-            _query_params.append(('sort', _params['sort'].value))
+            _query_params.append(('sort', _params['sort']))
 
         if _params.get('page') is not None:  # noqa: E501
             _query_params.append(('page', _params['page']))
 
         if _params.get('size') is not None:  # noqa: E501
             _query_params.append(('size', _params['size']))
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/api/user_api.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/api/user_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -1235,15 +1235,15 @@
         if _params['folder_name']:
             _path_params['folderName'] = _params['folder_name']
 
 
         # process the query parameters
         _query_params = []
         if _params.get('category_name') is not None:  # noqa: E501
-            _query_params.append(('categoryName', _params['category_name'].value))
+            _query_params.append(('categoryName', _params['category_name']))
 
         if _params.get('tag_name') is not None:  # noqa: E501
             _query_params.append(('tagName', _params['tag_name']))
 
         if _params.get('genre_name') is not None:  # noqa: E501
             _query_params.append(('genreName', _params['genre_name']))
 
@@ -1430,15 +1430,15 @@
         if _params['folder_name']:
             _path_params['folderName'] = _params['folder_name']
 
 
         # process the query parameters
         _query_params = []
         if _params.get('category_name') is not None:  # noqa: E501
-            _query_params.append(('categoryName', _params['category_name'].value))
+            _query_params.append(('categoryName', _params['category_name']))
 
         if _params.get('tag_name') is not None:  # noqa: E501
             _query_params.append(('tagName', _params['tag_name']))
 
         if _params.get('genre_name') is not None:  # noqa: E501
             _query_params.append(('genreName', _params['genre_name']))
 
@@ -1487,33 +1487,35 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def save_playlist(self, isrc : Annotated[Optional[StrictStr], Field(description="Search for a ISRC")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre_names : Optional[conlist(StrictStr)] = None, tag_names : Optional[conlist(StrictStr)] = None, release_date : Optional[datetime] = None, primary_mood_cluster : Optional[StrictStr] = None, secondary_mood_cluster : Optional[StrictStr] = None, tertiary_mood_cluster : Optional[StrictStr] = None, valence : Optional[StrictStr] = None, arousal : Optional[StrictStr] = None, pleasantness : Optional[StrictStr] = None, engagement : Optional[StrictStr] = None, vocals : Optional[StrictStr] = None, dominant_instrument : Optional[StrictStr] = None, secondary_instrument : Optional[StrictStr] = None, tertiary_instrument : Optional[StrictStr] = None, energy : Optional[StrictStr] = None, sound_generation : Optional[StrictStr] = None, tempo : Optional[StrictStr] = None, scale : Optional[StrictStr] = None, rhythm : Optional[StrictStr] = None, primary_sound_character : Optional[StrictStr] = None, timbre : Optional[StrictStr] = None, roughness : Optional[StrictStr] = None, tonality : Optional[StrictStr] = None, harmony : Optional[StrictStr] = None, texture : Optional[StrictStr] = None, groovyness : Optional[StrictStr] = None, space : Optional[StrictStr] = None, production_rating : Optional[StrictStr] = None, performance_rating : Optional[StrictStr] = None, song_rating : Optional[StrictStr] = None, audience_age : Optional[StrictStr] = None, audience_region : Optional[StrictStr] = None, audience_gender : Optional[StrictStr] = None, origin_decade : Optional[StrictStr] = None, curateability : Optional[StrictStr] = None, use_case : Optional[StrictStr] = None, channel_suitability : Optional[StrictStr] = None, similar_to_recording : Optional[StrictStr] = None, create_playlist_with_name : Optional[StrictStr] = None, songtradr_track_id : Optional[StrictStr] = None, usage_name : Optional[StrictStr] = None, bpm_min : Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None, bpm_max : Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None, name : Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None, folder : Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None, extension : Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None, upload_end_time : Optional[datetime] = None, min_upload_end_time : Optional[datetime] = None, max_upload_end_time : Optional[datetime] = None, fingerprint_status : Annotated[Optional[StrictStr], Field(description="Search for a fingerprint status.")] = None, inference_status : Annotated[Optional[StrictStr], Field(description="Search for a inference status.")] = None, page : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="The size of the page to be returned")] = None, sort : Annotated[Optional[conlist(StrictStr)], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None, **kwargs) -> FileListDTO:  # noqa: E501
+    def save_playlist(self, isrc : Annotated[Optional[StrictStr], Field(description="Search for a ISRC")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, party_and_title : Annotated[Optional[StrictStr], Field(description="Search for party and title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre_names : Optional[conlist(StrictStr)] = None, tag_names : Optional[conlist(StrictStr)] = None, release_date : Optional[datetime] = None, primary_mood_cluster : Optional[StrictStr] = None, secondary_mood_cluster : Optional[StrictStr] = None, tertiary_mood_cluster : Optional[StrictStr] = None, valence : Optional[StrictStr] = None, arousal : Optional[StrictStr] = None, pleasantness : Optional[StrictStr] = None, engagement : Optional[StrictStr] = None, vocals : Optional[StrictStr] = None, dominant_instrument : Optional[StrictStr] = None, secondary_instrument : Optional[StrictStr] = None, tertiary_instrument : Optional[StrictStr] = None, energy : Optional[StrictStr] = None, sound_generation : Optional[StrictStr] = None, tempo : Optional[StrictStr] = None, scale : Optional[StrictStr] = None, rhythm : Optional[StrictStr] = None, primary_sound_character : Optional[StrictStr] = None, timbre : Optional[StrictStr] = None, roughness : Optional[StrictStr] = None, tonality : Optional[StrictStr] = None, harmony : Optional[StrictStr] = None, texture : Optional[StrictStr] = None, groovyness : Optional[StrictStr] = None, space : Optional[StrictStr] = None, production_rating : Optional[StrictStr] = None, performance_rating : Optional[StrictStr] = None, song_rating : Optional[StrictStr] = None, audience_age : Optional[StrictStr] = None, audience_region : Optional[StrictStr] = None, audience_gender : Optional[StrictStr] = None, origin_decade : Optional[StrictStr] = None, curateability : Optional[StrictStr] = None, use_case : Optional[StrictStr] = None, channel_suitability : Optional[StrictStr] = None, similar_to_recording : Optional[StrictStr] = None, create_playlist_with_name : Optional[StrictStr] = None, songtradr_track_id : Optional[StrictStr] = None, usage_name : Optional[StrictStr] = None, bpm_min : Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None, bpm_max : Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None, name : Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None, folder : Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None, extension : Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None, upload_end_time : Optional[datetime] = None, min_upload_end_time : Optional[datetime] = None, max_upload_end_time : Optional[datetime] = None, fingerprint_status : Annotated[Optional[StrictStr], Field(description="Search for a fingerprint status.")] = None, inference_status : Annotated[Optional[StrictStr], Field(description="Search for a inference status.")] = None, page : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="The size of the page to be returned")] = None, sort : Annotated[Optional[conlist(StrictStr)], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None, **kwargs) -> FileListDTO:  # noqa: E501
         """List, search and create playlist of your own files.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.save_playlist(isrc, contributor, main_artist, composer, title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, create_playlist_with_name, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, async_req=True)
+        >>> thread = api.save_playlist(isrc, contributor, main_artist, composer, title, party_and_title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, create_playlist_with_name, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, async_req=True)
         >>> result = thread.get()
 
         :param isrc: Search for a ISRC
         :type isrc: str
         :param contributor: Search for a name that was involved as any contributor.
         :type contributor: str
         :param main_artist: Search for a main artist.
         :type main_artist: str
         :param composer: Search for a composer.
         :type composer: str
         :param title: Search for a title.
         :type title: str
+        :param party_and_title: Search for party and title.
+        :type party_and_title: str
         :param language: Search for a language of the lyrics.
         :type language: str
         :param genre_names:
         :type genre_names: List[str]
         :param tag_names:
         :type tag_names: List[str]
         :param release_date:
@@ -1630,36 +1632,38 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: FileListDTO
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the save_playlist_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.save_playlist_with_http_info(isrc, contributor, main_artist, composer, title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, create_playlist_with_name, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, **kwargs)  # noqa: E501
+        return self.save_playlist_with_http_info(isrc, contributor, main_artist, composer, title, party_and_title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, create_playlist_with_name, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def save_playlist_with_http_info(self, isrc : Annotated[Optional[StrictStr], Field(description="Search for a ISRC")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre_names : Optional[conlist(StrictStr)] = None, tag_names : Optional[conlist(StrictStr)] = None, release_date : Optional[datetime] = None, primary_mood_cluster : Optional[StrictStr] = None, secondary_mood_cluster : Optional[StrictStr] = None, tertiary_mood_cluster : Optional[StrictStr] = None, valence : Optional[StrictStr] = None, arousal : Optional[StrictStr] = None, pleasantness : Optional[StrictStr] = None, engagement : Optional[StrictStr] = None, vocals : Optional[StrictStr] = None, dominant_instrument : Optional[StrictStr] = None, secondary_instrument : Optional[StrictStr] = None, tertiary_instrument : Optional[StrictStr] = None, energy : Optional[StrictStr] = None, sound_generation : Optional[StrictStr] = None, tempo : Optional[StrictStr] = None, scale : Optional[StrictStr] = None, rhythm : Optional[StrictStr] = None, primary_sound_character : Optional[StrictStr] = None, timbre : Optional[StrictStr] = None, roughness : Optional[StrictStr] = None, tonality : Optional[StrictStr] = None, harmony : Optional[StrictStr] = None, texture : Optional[StrictStr] = None, groovyness : Optional[StrictStr] = None, space : Optional[StrictStr] = None, production_rating : Optional[StrictStr] = None, performance_rating : Optional[StrictStr] = None, song_rating : Optional[StrictStr] = None, audience_age : Optional[StrictStr] = None, audience_region : Optional[StrictStr] = None, audience_gender : Optional[StrictStr] = None, origin_decade : Optional[StrictStr] = None, curateability : Optional[StrictStr] = None, use_case : Optional[StrictStr] = None, channel_suitability : Optional[StrictStr] = None, similar_to_recording : Optional[StrictStr] = None, create_playlist_with_name : Optional[StrictStr] = None, songtradr_track_id : Optional[StrictStr] = None, usage_name : Optional[StrictStr] = None, bpm_min : Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None, bpm_max : Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None, name : Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None, folder : Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None, extension : Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None, upload_end_time : Optional[datetime] = None, min_upload_end_time : Optional[datetime] = None, max_upload_end_time : Optional[datetime] = None, fingerprint_status : Annotated[Optional[StrictStr], Field(description="Search for a fingerprint status.")] = None, inference_status : Annotated[Optional[StrictStr], Field(description="Search for a inference status.")] = None, page : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="The size of the page to be returned")] = None, sort : Annotated[Optional[conlist(StrictStr)], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def save_playlist_with_http_info(self, isrc : Annotated[Optional[StrictStr], Field(description="Search for a ISRC")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, party_and_title : Annotated[Optional[StrictStr], Field(description="Search for party and title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre_names : Optional[conlist(StrictStr)] = None, tag_names : Optional[conlist(StrictStr)] = None, release_date : Optional[datetime] = None, primary_mood_cluster : Optional[StrictStr] = None, secondary_mood_cluster : Optional[StrictStr] = None, tertiary_mood_cluster : Optional[StrictStr] = None, valence : Optional[StrictStr] = None, arousal : Optional[StrictStr] = None, pleasantness : Optional[StrictStr] = None, engagement : Optional[StrictStr] = None, vocals : Optional[StrictStr] = None, dominant_instrument : Optional[StrictStr] = None, secondary_instrument : Optional[StrictStr] = None, tertiary_instrument : Optional[StrictStr] = None, energy : Optional[StrictStr] = None, sound_generation : Optional[StrictStr] = None, tempo : Optional[StrictStr] = None, scale : Optional[StrictStr] = None, rhythm : Optional[StrictStr] = None, primary_sound_character : Optional[StrictStr] = None, timbre : Optional[StrictStr] = None, roughness : Optional[StrictStr] = None, tonality : Optional[StrictStr] = None, harmony : Optional[StrictStr] = None, texture : Optional[StrictStr] = None, groovyness : Optional[StrictStr] = None, space : Optional[StrictStr] = None, production_rating : Optional[StrictStr] = None, performance_rating : Optional[StrictStr] = None, song_rating : Optional[StrictStr] = None, audience_age : Optional[StrictStr] = None, audience_region : Optional[StrictStr] = None, audience_gender : Optional[StrictStr] = None, origin_decade : Optional[StrictStr] = None, curateability : Optional[StrictStr] = None, use_case : Optional[StrictStr] = None, channel_suitability : Optional[StrictStr] = None, similar_to_recording : Optional[StrictStr] = None, create_playlist_with_name : Optional[StrictStr] = None, songtradr_track_id : Optional[StrictStr] = None, usage_name : Optional[StrictStr] = None, bpm_min : Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None, bpm_max : Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None, name : Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None, folder : Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None, extension : Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None, upload_end_time : Optional[datetime] = None, min_upload_end_time : Optional[datetime] = None, max_upload_end_time : Optional[datetime] = None, fingerprint_status : Annotated[Optional[StrictStr], Field(description="Search for a fingerprint status.")] = None, inference_status : Annotated[Optional[StrictStr], Field(description="Search for a inference status.")] = None, page : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="The size of the page to be returned")] = None, sort : Annotated[Optional[conlist(StrictStr)], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """List, search and create playlist of your own files.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.save_playlist_with_http_info(isrc, contributor, main_artist, composer, title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, create_playlist_with_name, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, async_req=True)
+        >>> thread = api.save_playlist_with_http_info(isrc, contributor, main_artist, composer, title, party_and_title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, create_playlist_with_name, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, async_req=True)
         >>> result = thread.get()
 
         :param isrc: Search for a ISRC
         :type isrc: str
         :param contributor: Search for a name that was involved as any contributor.
         :type contributor: str
         :param main_artist: Search for a main artist.
         :type main_artist: str
         :param composer: Search for a composer.
         :type composer: str
         :param title: Search for a title.
         :type title: str
+        :param party_and_title: Search for party and title.
+        :type party_and_title: str
         :param language: Search for a language of the lyrics.
         :type language: str
         :param genre_names:
         :type genre_names: List[str]
         :param tag_names:
         :type tag_names: List[str]
         :param release_date:
@@ -1795,14 +1799,15 @@
 
         _all_params = [
             'isrc',
             'contributor',
             'main_artist',
             'composer',
             'title',
+            'party_and_title',
             'language',
             'genre_names',
             'tag_names',
             'release_date',
             'primary_mood_cluster',
             'secondary_mood_cluster',
             'tertiary_mood_cluster',
@@ -1895,16 +1900,19 @@
 
         if _params.get('composer') is not None:  # noqa: E501
             _query_params.append(('composer', _params['composer']))
 
         if _params.get('title') is not None:  # noqa: E501
             _query_params.append(('title', _params['title']))
 
+        if _params.get('party_and_title') is not None:  # noqa: E501
+            _query_params.append(('partyAndTitle', _params['party_and_title']))
+
         if _params.get('language') is not None:  # noqa: E501
-            _query_params.append(('language', _params['language'].value))
+            _query_params.append(('language', _params['language']))
 
         if _params.get('genre_names') is not None:  # noqa: E501
             _query_params.append(('genreNames', _params['genre_names']))
             _collection_formats['genreNames'] = 'multi'
 
         if _params.get('tag_names') is not None:  # noqa: E501
             _query_params.append(('tagNames', _params['tag_names']))
@@ -1913,114 +1921,114 @@
         if _params.get('release_date') is not None:  # noqa: E501
             if isinstance(_params['release_date'], datetime):
                 _query_params.append(('releaseDate', _params['release_date'].strftime(self.api_client.configuration.datetime_format)))
             else:
                 _query_params.append(('releaseDate', _params['release_date']))
 
         if _params.get('primary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('primaryMoodCluster', _params['primary_mood_cluster'].value))
+            _query_params.append(('primaryMoodCluster', _params['primary_mood_cluster']))
 
         if _params.get('secondary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('secondaryMoodCluster', _params['secondary_mood_cluster'].value))
+            _query_params.append(('secondaryMoodCluster', _params['secondary_mood_cluster']))
 
         if _params.get('tertiary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('tertiaryMoodCluster', _params['tertiary_mood_cluster'].value))
+            _query_params.append(('tertiaryMoodCluster', _params['tertiary_mood_cluster']))
 
         if _params.get('valence') is not None:  # noqa: E501
-            _query_params.append(('valence', _params['valence'].value))
+            _query_params.append(('valence', _params['valence']))
 
         if _params.get('arousal') is not None:  # noqa: E501
-            _query_params.append(('arousal', _params['arousal'].value))
+            _query_params.append(('arousal', _params['arousal']))
 
         if _params.get('pleasantness') is not None:  # noqa: E501
-            _query_params.append(('pleasantness', _params['pleasantness'].value))
+            _query_params.append(('pleasantness', _params['pleasantness']))
 
         if _params.get('engagement') is not None:  # noqa: E501
-            _query_params.append(('engagement', _params['engagement'].value))
+            _query_params.append(('engagement', _params['engagement']))
 
         if _params.get('vocals') is not None:  # noqa: E501
-            _query_params.append(('vocals', _params['vocals'].value))
+            _query_params.append(('vocals', _params['vocals']))
 
         if _params.get('dominant_instrument') is not None:  # noqa: E501
-            _query_params.append(('dominantInstrument', _params['dominant_instrument'].value))
+            _query_params.append(('dominantInstrument', _params['dominant_instrument']))
 
         if _params.get('secondary_instrument') is not None:  # noqa: E501
-            _query_params.append(('secondaryInstrument', _params['secondary_instrument'].value))
+            _query_params.append(('secondaryInstrument', _params['secondary_instrument']))
 
         if _params.get('tertiary_instrument') is not None:  # noqa: E501
-            _query_params.append(('tertiaryInstrument', _params['tertiary_instrument'].value))
+            _query_params.append(('tertiaryInstrument', _params['tertiary_instrument']))
 
         if _params.get('energy') is not None:  # noqa: E501
-            _query_params.append(('energy', _params['energy'].value))
+            _query_params.append(('energy', _params['energy']))
 
         if _params.get('sound_generation') is not None:  # noqa: E501
-            _query_params.append(('soundGeneration', _params['sound_generation'].value))
+            _query_params.append(('soundGeneration', _params['sound_generation']))
 
         if _params.get('tempo') is not None:  # noqa: E501
-            _query_params.append(('tempo', _params['tempo'].value))
+            _query_params.append(('tempo', _params['tempo']))
 
         if _params.get('scale') is not None:  # noqa: E501
-            _query_params.append(('scale', _params['scale'].value))
+            _query_params.append(('scale', _params['scale']))
 
         if _params.get('rhythm') is not None:  # noqa: E501
-            _query_params.append(('rhythm', _params['rhythm'].value))
+            _query_params.append(('rhythm', _params['rhythm']))
 
         if _params.get('primary_sound_character') is not None:  # noqa: E501
-            _query_params.append(('primarySoundCharacter', _params['primary_sound_character'].value))
+            _query_params.append(('primarySoundCharacter', _params['primary_sound_character']))
 
         if _params.get('timbre') is not None:  # noqa: E501
-            _query_params.append(('timbre', _params['timbre'].value))
+            _query_params.append(('timbre', _params['timbre']))
 
         if _params.get('roughness') is not None:  # noqa: E501
-            _query_params.append(('roughness', _params['roughness'].value))
+            _query_params.append(('roughness', _params['roughness']))
 
         if _params.get('tonality') is not None:  # noqa: E501
-            _query_params.append(('tonality', _params['tonality'].value))
+            _query_params.append(('tonality', _params['tonality']))
 
         if _params.get('harmony') is not None:  # noqa: E501
-            _query_params.append(('harmony', _params['harmony'].value))
+            _query_params.append(('harmony', _params['harmony']))
 
         if _params.get('texture') is not None:  # noqa: E501
-            _query_params.append(('texture', _params['texture'].value))
+            _query_params.append(('texture', _params['texture']))
 
         if _params.get('groovyness') is not None:  # noqa: E501
-            _query_params.append(('groovyness', _params['groovyness'].value))
+            _query_params.append(('groovyness', _params['groovyness']))
 
         if _params.get('space') is not None:  # noqa: E501
-            _query_params.append(('space', _params['space'].value))
+            _query_params.append(('space', _params['space']))
 
         if _params.get('production_rating') is not None:  # noqa: E501
-            _query_params.append(('productionRating', _params['production_rating'].value))
+            _query_params.append(('productionRating', _params['production_rating']))
 
         if _params.get('performance_rating') is not None:  # noqa: E501
-            _query_params.append(('performanceRating', _params['performance_rating'].value))
+            _query_params.append(('performanceRating', _params['performance_rating']))
 
         if _params.get('song_rating') is not None:  # noqa: E501
-            _query_params.append(('songRating', _params['song_rating'].value))
+            _query_params.append(('songRating', _params['song_rating']))
 
         if _params.get('audience_age') is not None:  # noqa: E501
-            _query_params.append(('audienceAge', _params['audience_age'].value))
+            _query_params.append(('audienceAge', _params['audience_age']))
 
         if _params.get('audience_region') is not None:  # noqa: E501
-            _query_params.append(('audienceRegion', _params['audience_region'].value))
+            _query_params.append(('audienceRegion', _params['audience_region']))
 
         if _params.get('audience_gender') is not None:  # noqa: E501
-            _query_params.append(('audienceGender', _params['audience_gender'].value))
+            _query_params.append(('audienceGender', _params['audience_gender']))
 
         if _params.get('origin_decade') is not None:  # noqa: E501
-            _query_params.append(('originDecade', _params['origin_decade'].value))
+            _query_params.append(('originDecade', _params['origin_decade']))
 
         if _params.get('curateability') is not None:  # noqa: E501
-            _query_params.append(('curateability', _params['curateability'].value))
+            _query_params.append(('curateability', _params['curateability']))
 
         if _params.get('use_case') is not None:  # noqa: E501
-            _query_params.append(('useCase', _params['use_case'].value))
+            _query_params.append(('useCase', _params['use_case']))
 
         if _params.get('channel_suitability') is not None:  # noqa: E501
-            _query_params.append(('channelSuitability', _params['channel_suitability'].value))
+            _query_params.append(('channelSuitability', _params['channel_suitability']))
 
         if _params.get('similar_to_recording') is not None:  # noqa: E501
             _query_params.append(('similarToRecording', _params['similar_to_recording']))
 
         if _params.get('create_playlist_with_name') is not None:  # noqa: E501
             _query_params.append(('createPlaylistWithName', _params['create_playlist_with_name']))
 
@@ -2090,16 +2098,16 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearer-jwt']  # noqa: E501
 
         _response_types_map = {
-            '403': "ErrorResponse",
             '200': "FileListDTO",
+            '403': "ErrorResponse",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
 
         return self.api_client.call_api(
@@ -2239,17 +2247,17 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearer-jwt']  # noqa: E501
 
         _response_types_map = {
+            '409': "ErrorResponse",
             '200': "SignUpDTO",
             '403': "ErrorResponse",
-            '409': "ErrorResponse",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
 
         return self.api_client.call_api(
@@ -2389,16 +2397,16 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['bearer-jwt']  # noqa: E501
 
         _response_types_map = {
-            '401': "ErrorResponse",
             '200': "JwtTokenDTO",
+            '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
             '400': "ErrorResponse",
         }
 
         return self.api_client.call_api(
             '/api/v1/user/token', 'POST',
@@ -2837,16 +2845,16 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['bearer-jwt']  # noqa: E501
 
         _response_types_map = {
-            '404': "ErrorResponse",
             '200': "FileWIthUrlDTO",
+            '404': "ErrorResponse",
             '401': "ErrorResponse",
             '429': "ErrorResponse",
             '500': "ErrorResponse",
         }
 
         return self.api_client.call_api(
             '/api/v1/user/file/{objectKey}', 'GET',
@@ -2862,33 +2870,35 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def user_files(self, isrc : Annotated[Optional[StrictStr], Field(description="Search for a ISRC")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre_names : Optional[conlist(StrictStr)] = None, tag_names : Optional[conlist(StrictStr)] = None, release_date : Optional[datetime] = None, primary_mood_cluster : Optional[StrictStr] = None, secondary_mood_cluster : Optional[StrictStr] = None, tertiary_mood_cluster : Optional[StrictStr] = None, valence : Optional[StrictStr] = None, arousal : Optional[StrictStr] = None, pleasantness : Optional[StrictStr] = None, engagement : Optional[StrictStr] = None, vocals : Optional[StrictStr] = None, dominant_instrument : Optional[StrictStr] = None, secondary_instrument : Optional[StrictStr] = None, tertiary_instrument : Optional[StrictStr] = None, energy : Optional[StrictStr] = None, sound_generation : Optional[StrictStr] = None, tempo : Optional[StrictStr] = None, scale : Optional[StrictStr] = None, rhythm : Optional[StrictStr] = None, primary_sound_character : Optional[StrictStr] = None, timbre : Optional[StrictStr] = None, roughness : Optional[StrictStr] = None, tonality : Optional[StrictStr] = None, harmony : Optional[StrictStr] = None, texture : Optional[StrictStr] = None, groovyness : Optional[StrictStr] = None, space : Optional[StrictStr] = None, production_rating : Optional[StrictStr] = None, performance_rating : Optional[StrictStr] = None, song_rating : Optional[StrictStr] = None, audience_age : Optional[StrictStr] = None, audience_region : Optional[StrictStr] = None, audience_gender : Optional[StrictStr] = None, origin_decade : Optional[StrictStr] = None, curateability : Optional[StrictStr] = None, use_case : Optional[StrictStr] = None, channel_suitability : Optional[StrictStr] = None, similar_to_recording : Optional[StrictStr] = None, songtradr_track_id : Optional[StrictStr] = None, usage_name : Optional[StrictStr] = None, bpm_min : Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None, bpm_max : Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None, name : Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None, folder : Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None, extension : Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None, upload_end_time : Optional[datetime] = None, min_upload_end_time : Optional[datetime] = None, max_upload_end_time : Optional[datetime] = None, fingerprint_status : Annotated[Optional[StrictStr], Field(description="Search for a fingerprint status.")] = None, inference_status : Annotated[Optional[StrictStr], Field(description="Search for a inference status.")] = None, page : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="The size of the page to be returned")] = None, sort : Annotated[Optional[conlist(StrictStr)], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None, **kwargs) -> FileListDTO:  # noqa: E501
+    def user_files(self, isrc : Annotated[Optional[StrictStr], Field(description="Search for a ISRC")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, party_and_title : Annotated[Optional[StrictStr], Field(description="Search for party and title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre_names : Optional[conlist(StrictStr)] = None, tag_names : Optional[conlist(StrictStr)] = None, release_date : Optional[datetime] = None, primary_mood_cluster : Optional[StrictStr] = None, secondary_mood_cluster : Optional[StrictStr] = None, tertiary_mood_cluster : Optional[StrictStr] = None, valence : Optional[StrictStr] = None, arousal : Optional[StrictStr] = None, pleasantness : Optional[StrictStr] = None, engagement : Optional[StrictStr] = None, vocals : Optional[StrictStr] = None, dominant_instrument : Optional[StrictStr] = None, secondary_instrument : Optional[StrictStr] = None, tertiary_instrument : Optional[StrictStr] = None, energy : Optional[StrictStr] = None, sound_generation : Optional[StrictStr] = None, tempo : Optional[StrictStr] = None, scale : Optional[StrictStr] = None, rhythm : Optional[StrictStr] = None, primary_sound_character : Optional[StrictStr] = None, timbre : Optional[StrictStr] = None, roughness : Optional[StrictStr] = None, tonality : Optional[StrictStr] = None, harmony : Optional[StrictStr] = None, texture : Optional[StrictStr] = None, groovyness : Optional[StrictStr] = None, space : Optional[StrictStr] = None, production_rating : Optional[StrictStr] = None, performance_rating : Optional[StrictStr] = None, song_rating : Optional[StrictStr] = None, audience_age : Optional[StrictStr] = None, audience_region : Optional[StrictStr] = None, audience_gender : Optional[StrictStr] = None, origin_decade : Optional[StrictStr] = None, curateability : Optional[StrictStr] = None, use_case : Optional[StrictStr] = None, channel_suitability : Optional[StrictStr] = None, similar_to_recording : Optional[StrictStr] = None, songtradr_track_id : Optional[StrictStr] = None, usage_name : Optional[StrictStr] = None, bpm_min : Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None, bpm_max : Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None, name : Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None, folder : Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None, extension : Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None, upload_end_time : Optional[datetime] = None, min_upload_end_time : Optional[datetime] = None, max_upload_end_time : Optional[datetime] = None, fingerprint_status : Annotated[Optional[StrictStr], Field(description="Search for a fingerprint status.")] = None, inference_status : Annotated[Optional[StrictStr], Field(description="Search for a inference status.")] = None, page : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="The size of the page to be returned")] = None, sort : Annotated[Optional[conlist(StrictStr)], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None, **kwargs) -> FileListDTO:  # noqa: E501
         """List and search your own files.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.user_files(isrc, contributor, main_artist, composer, title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, async_req=True)
+        >>> thread = api.user_files(isrc, contributor, main_artist, composer, title, party_and_title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, async_req=True)
         >>> result = thread.get()
 
         :param isrc: Search for a ISRC
         :type isrc: str
         :param contributor: Search for a name that was involved as any contributor.
         :type contributor: str
         :param main_artist: Search for a main artist.
         :type main_artist: str
         :param composer: Search for a composer.
         :type composer: str
         :param title: Search for a title.
         :type title: str
+        :param party_and_title: Search for party and title.
+        :type party_and_title: str
         :param language: Search for a language of the lyrics.
         :type language: str
         :param genre_names:
         :type genre_names: List[str]
         :param tag_names:
         :type tag_names: List[str]
         :param release_date:
@@ -3003,36 +3013,38 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: FileListDTO
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the user_files_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.user_files_with_http_info(isrc, contributor, main_artist, composer, title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, **kwargs)  # noqa: E501
+        return self.user_files_with_http_info(isrc, contributor, main_artist, composer, title, party_and_title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def user_files_with_http_info(self, isrc : Annotated[Optional[StrictStr], Field(description="Search for a ISRC")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre_names : Optional[conlist(StrictStr)] = None, tag_names : Optional[conlist(StrictStr)] = None, release_date : Optional[datetime] = None, primary_mood_cluster : Optional[StrictStr] = None, secondary_mood_cluster : Optional[StrictStr] = None, tertiary_mood_cluster : Optional[StrictStr] = None, valence : Optional[StrictStr] = None, arousal : Optional[StrictStr] = None, pleasantness : Optional[StrictStr] = None, engagement : Optional[StrictStr] = None, vocals : Optional[StrictStr] = None, dominant_instrument : Optional[StrictStr] = None, secondary_instrument : Optional[StrictStr] = None, tertiary_instrument : Optional[StrictStr] = None, energy : Optional[StrictStr] = None, sound_generation : Optional[StrictStr] = None, tempo : Optional[StrictStr] = None, scale : Optional[StrictStr] = None, rhythm : Optional[StrictStr] = None, primary_sound_character : Optional[StrictStr] = None, timbre : Optional[StrictStr] = None, roughness : Optional[StrictStr] = None, tonality : Optional[StrictStr] = None, harmony : Optional[StrictStr] = None, texture : Optional[StrictStr] = None, groovyness : Optional[StrictStr] = None, space : Optional[StrictStr] = None, production_rating : Optional[StrictStr] = None, performance_rating : Optional[StrictStr] = None, song_rating : Optional[StrictStr] = None, audience_age : Optional[StrictStr] = None, audience_region : Optional[StrictStr] = None, audience_gender : Optional[StrictStr] = None, origin_decade : Optional[StrictStr] = None, curateability : Optional[StrictStr] = None, use_case : Optional[StrictStr] = None, channel_suitability : Optional[StrictStr] = None, similar_to_recording : Optional[StrictStr] = None, songtradr_track_id : Optional[StrictStr] = None, usage_name : Optional[StrictStr] = None, bpm_min : Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None, bpm_max : Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None, name : Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None, folder : Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None, extension : Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None, upload_end_time : Optional[datetime] = None, min_upload_end_time : Optional[datetime] = None, max_upload_end_time : Optional[datetime] = None, fingerprint_status : Annotated[Optional[StrictStr], Field(description="Search for a fingerprint status.")] = None, inference_status : Annotated[Optional[StrictStr], Field(description="Search for a inference status.")] = None, page : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="The size of the page to be returned")] = None, sort : Annotated[Optional[conlist(StrictStr)], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def user_files_with_http_info(self, isrc : Annotated[Optional[StrictStr], Field(description="Search for a ISRC")] = None, contributor : Annotated[Optional[StrictStr], Field(description="Search for a name that was involved as any contributor.")] = None, main_artist : Annotated[Optional[StrictStr], Field(description="Search for a main artist.")] = None, composer : Annotated[Optional[StrictStr], Field(description="Search for a composer.")] = None, title : Annotated[Optional[StrictStr], Field(description="Search for a title.")] = None, party_and_title : Annotated[Optional[StrictStr], Field(description="Search for party and title.")] = None, language : Annotated[Optional[StrictStr], Field(description="Search for a language of the lyrics.")] = None, genre_names : Optional[conlist(StrictStr)] = None, tag_names : Optional[conlist(StrictStr)] = None, release_date : Optional[datetime] = None, primary_mood_cluster : Optional[StrictStr] = None, secondary_mood_cluster : Optional[StrictStr] = None, tertiary_mood_cluster : Optional[StrictStr] = None, valence : Optional[StrictStr] = None, arousal : Optional[StrictStr] = None, pleasantness : Optional[StrictStr] = None, engagement : Optional[StrictStr] = None, vocals : Optional[StrictStr] = None, dominant_instrument : Optional[StrictStr] = None, secondary_instrument : Optional[StrictStr] = None, tertiary_instrument : Optional[StrictStr] = None, energy : Optional[StrictStr] = None, sound_generation : Optional[StrictStr] = None, tempo : Optional[StrictStr] = None, scale : Optional[StrictStr] = None, rhythm : Optional[StrictStr] = None, primary_sound_character : Optional[StrictStr] = None, timbre : Optional[StrictStr] = None, roughness : Optional[StrictStr] = None, tonality : Optional[StrictStr] = None, harmony : Optional[StrictStr] = None, texture : Optional[StrictStr] = None, groovyness : Optional[StrictStr] = None, space : Optional[StrictStr] = None, production_rating : Optional[StrictStr] = None, performance_rating : Optional[StrictStr] = None, song_rating : Optional[StrictStr] = None, audience_age : Optional[StrictStr] = None, audience_region : Optional[StrictStr] = None, audience_gender : Optional[StrictStr] = None, origin_decade : Optional[StrictStr] = None, curateability : Optional[StrictStr] = None, use_case : Optional[StrictStr] = None, channel_suitability : Optional[StrictStr] = None, similar_to_recording : Optional[StrictStr] = None, songtradr_track_id : Optional[StrictStr] = None, usage_name : Optional[StrictStr] = None, bpm_min : Annotated[Optional[StrictInt], Field(description="Search for a minimal bpm.")] = None, bpm_max : Annotated[Optional[StrictInt], Field(description="Search for a maximal bpm.")] = None, name : Annotated[Optional[StrictStr], Field(description="Search for a file name.")] = None, folder : Annotated[Optional[StrictStr], Field(description="Search for a folder.")] = None, extension : Annotated[Optional[StrictStr], Field(description="Search for a file extension.")] = None, upload_end_time : Optional[datetime] = None, min_upload_end_time : Optional[datetime] = None, max_upload_end_time : Optional[datetime] = None, fingerprint_status : Annotated[Optional[StrictStr], Field(description="Search for a fingerprint status.")] = None, inference_status : Annotated[Optional[StrictStr], Field(description="Search for a inference status.")] = None, page : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Zero-based page index (0..N)")] = None, size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="The size of the page to be returned")] = None, sort : Annotated[Optional[conlist(StrictStr)], Field(description="Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """List and search your own files.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.user_files_with_http_info(isrc, contributor, main_artist, composer, title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, async_req=True)
+        >>> thread = api.user_files_with_http_info(isrc, contributor, main_artist, composer, title, party_and_title, language, genre_names, tag_names, release_date, primary_mood_cluster, secondary_mood_cluster, tertiary_mood_cluster, valence, arousal, pleasantness, engagement, vocals, dominant_instrument, secondary_instrument, tertiary_instrument, energy, sound_generation, tempo, scale, rhythm, primary_sound_character, timbre, roughness, tonality, harmony, texture, groovyness, space, production_rating, performance_rating, song_rating, audience_age, audience_region, audience_gender, origin_decade, curateability, use_case, channel_suitability, similar_to_recording, songtradr_track_id, usage_name, bpm_min, bpm_max, name, folder, extension, upload_end_time, min_upload_end_time, max_upload_end_time, fingerprint_status, inference_status, page, size, sort, async_req=True)
         >>> result = thread.get()
 
         :param isrc: Search for a ISRC
         :type isrc: str
         :param contributor: Search for a name that was involved as any contributor.
         :type contributor: str
         :param main_artist: Search for a main artist.
         :type main_artist: str
         :param composer: Search for a composer.
         :type composer: str
         :param title: Search for a title.
         :type title: str
+        :param party_and_title: Search for party and title.
+        :type party_and_title: str
         :param language: Search for a language of the lyrics.
         :type language: str
         :param genre_names:
         :type genre_names: List[str]
         :param tag_names:
         :type tag_names: List[str]
         :param release_date:
@@ -3166,14 +3178,15 @@
 
         _all_params = [
             'isrc',
             'contributor',
             'main_artist',
             'composer',
             'title',
+            'party_and_title',
             'language',
             'genre_names',
             'tag_names',
             'release_date',
             'primary_mood_cluster',
             'secondary_mood_cluster',
             'tertiary_mood_cluster',
@@ -3265,16 +3278,19 @@
 
         if _params.get('composer') is not None:  # noqa: E501
             _query_params.append(('composer', _params['composer']))
 
         if _params.get('title') is not None:  # noqa: E501
             _query_params.append(('title', _params['title']))
 
+        if _params.get('party_and_title') is not None:  # noqa: E501
+            _query_params.append(('partyAndTitle', _params['party_and_title']))
+
         if _params.get('language') is not None:  # noqa: E501
-            _query_params.append(('language', _params['language'].value))
+            _query_params.append(('language', _params['language']))
 
         if _params.get('genre_names') is not None:  # noqa: E501
             _query_params.append(('genreNames', _params['genre_names']))
             _collection_formats['genreNames'] = 'multi'
 
         if _params.get('tag_names') is not None:  # noqa: E501
             _query_params.append(('tagNames', _params['tag_names']))
@@ -3283,114 +3299,114 @@
         if _params.get('release_date') is not None:  # noqa: E501
             if isinstance(_params['release_date'], datetime):
                 _query_params.append(('releaseDate', _params['release_date'].strftime(self.api_client.configuration.datetime_format)))
             else:
                 _query_params.append(('releaseDate', _params['release_date']))
 
         if _params.get('primary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('primaryMoodCluster', _params['primary_mood_cluster'].value))
+            _query_params.append(('primaryMoodCluster', _params['primary_mood_cluster']))
 
         if _params.get('secondary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('secondaryMoodCluster', _params['secondary_mood_cluster'].value))
+            _query_params.append(('secondaryMoodCluster', _params['secondary_mood_cluster']))
 
         if _params.get('tertiary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('tertiaryMoodCluster', _params['tertiary_mood_cluster'].value))
+            _query_params.append(('tertiaryMoodCluster', _params['tertiary_mood_cluster']))
 
         if _params.get('valence') is not None:  # noqa: E501
-            _query_params.append(('valence', _params['valence'].value))
+            _query_params.append(('valence', _params['valence']))
 
         if _params.get('arousal') is not None:  # noqa: E501
-            _query_params.append(('arousal', _params['arousal'].value))
+            _query_params.append(('arousal', _params['arousal']))
 
         if _params.get('pleasantness') is not None:  # noqa: E501
-            _query_params.append(('pleasantness', _params['pleasantness'].value))
+            _query_params.append(('pleasantness', _params['pleasantness']))
 
         if _params.get('engagement') is not None:  # noqa: E501
-            _query_params.append(('engagement', _params['engagement'].value))
+            _query_params.append(('engagement', _params['engagement']))
 
         if _params.get('vocals') is not None:  # noqa: E501
-            _query_params.append(('vocals', _params['vocals'].value))
+            _query_params.append(('vocals', _params['vocals']))
 
         if _params.get('dominant_instrument') is not None:  # noqa: E501
-            _query_params.append(('dominantInstrument', _params['dominant_instrument'].value))
+            _query_params.append(('dominantInstrument', _params['dominant_instrument']))
 
         if _params.get('secondary_instrument') is not None:  # noqa: E501
-            _query_params.append(('secondaryInstrument', _params['secondary_instrument'].value))
+            _query_params.append(('secondaryInstrument', _params['secondary_instrument']))
 
         if _params.get('tertiary_instrument') is not None:  # noqa: E501
-            _query_params.append(('tertiaryInstrument', _params['tertiary_instrument'].value))
+            _query_params.append(('tertiaryInstrument', _params['tertiary_instrument']))
 
         if _params.get('energy') is not None:  # noqa: E501
-            _query_params.append(('energy', _params['energy'].value))
+            _query_params.append(('energy', _params['energy']))
 
         if _params.get('sound_generation') is not None:  # noqa: E501
-            _query_params.append(('soundGeneration', _params['sound_generation'].value))
+            _query_params.append(('soundGeneration', _params['sound_generation']))
 
         if _params.get('tempo') is not None:  # noqa: E501
-            _query_params.append(('tempo', _params['tempo'].value))
+            _query_params.append(('tempo', _params['tempo']))
 
         if _params.get('scale') is not None:  # noqa: E501
-            _query_params.append(('scale', _params['scale'].value))
+            _query_params.append(('scale', _params['scale']))
 
         if _params.get('rhythm') is not None:  # noqa: E501
-            _query_params.append(('rhythm', _params['rhythm'].value))
+            _query_params.append(('rhythm', _params['rhythm']))
 
         if _params.get('primary_sound_character') is not None:  # noqa: E501
-            _query_params.append(('primarySoundCharacter', _params['primary_sound_character'].value))
+            _query_params.append(('primarySoundCharacter', _params['primary_sound_character']))
 
         if _params.get('timbre') is not None:  # noqa: E501
-            _query_params.append(('timbre', _params['timbre'].value))
+            _query_params.append(('timbre', _params['timbre']))
 
         if _params.get('roughness') is not None:  # noqa: E501
-            _query_params.append(('roughness', _params['roughness'].value))
+            _query_params.append(('roughness', _params['roughness']))
 
         if _params.get('tonality') is not None:  # noqa: E501
-            _query_params.append(('tonality', _params['tonality'].value))
+            _query_params.append(('tonality', _params['tonality']))
 
         if _params.get('harmony') is not None:  # noqa: E501
-            _query_params.append(('harmony', _params['harmony'].value))
+            _query_params.append(('harmony', _params['harmony']))
 
         if _params.get('texture') is not None:  # noqa: E501
-            _query_params.append(('texture', _params['texture'].value))
+            _query_params.append(('texture', _params['texture']))
 
         if _params.get('groovyness') is not None:  # noqa: E501
-            _query_params.append(('groovyness', _params['groovyness'].value))
+            _query_params.append(('groovyness', _params['groovyness']))
 
         if _params.get('space') is not None:  # noqa: E501
-            _query_params.append(('space', _params['space'].value))
+            _query_params.append(('space', _params['space']))
 
         if _params.get('production_rating') is not None:  # noqa: E501
-            _query_params.append(('productionRating', _params['production_rating'].value))
+            _query_params.append(('productionRating', _params['production_rating']))
 
         if _params.get('performance_rating') is not None:  # noqa: E501
-            _query_params.append(('performanceRating', _params['performance_rating'].value))
+            _query_params.append(('performanceRating', _params['performance_rating']))
 
         if _params.get('song_rating') is not None:  # noqa: E501
-            _query_params.append(('songRating', _params['song_rating'].value))
+            _query_params.append(('songRating', _params['song_rating']))
 
         if _params.get('audience_age') is not None:  # noqa: E501
-            _query_params.append(('audienceAge', _params['audience_age'].value))
+            _query_params.append(('audienceAge', _params['audience_age']))
 
         if _params.get('audience_region') is not None:  # noqa: E501
-            _query_params.append(('audienceRegion', _params['audience_region'].value))
+            _query_params.append(('audienceRegion', _params['audience_region']))
 
         if _params.get('audience_gender') is not None:  # noqa: E501
-            _query_params.append(('audienceGender', _params['audience_gender'].value))
+            _query_params.append(('audienceGender', _params['audience_gender']))
 
         if _params.get('origin_decade') is not None:  # noqa: E501
-            _query_params.append(('originDecade', _params['origin_decade'].value))
+            _query_params.append(('originDecade', _params['origin_decade']))
 
         if _params.get('curateability') is not None:  # noqa: E501
-            _query_params.append(('curateability', _params['curateability'].value))
+            _query_params.append(('curateability', _params['curateability']))
 
         if _params.get('use_case') is not None:  # noqa: E501
-            _query_params.append(('useCase', _params['use_case'].value))
+            _query_params.append(('useCase', _params['use_case']))
 
         if _params.get('channel_suitability') is not None:  # noqa: E501
-            _query_params.append(('channelSuitability', _params['channel_suitability'].value))
+            _query_params.append(('channelSuitability', _params['channel_suitability']))
 
         if _params.get('similar_to_recording') is not None:  # noqa: E501
             _query_params.append(('similarToRecording', _params['similar_to_recording']))
 
         if _params.get('songtradr_track_id') is not None:  # noqa: E501
             _query_params.append(('songtradrTrackId', _params['songtradr_track_id']))
 
@@ -3879,102 +3895,102 @@
         if _params.get('release_date') is not None:  # noqa: E501
             if isinstance(_params['release_date'], datetime):
                 _query_params.append(('releaseDate', _params['release_date'].strftime(self.api_client.configuration.datetime_format)))
             else:
                 _query_params.append(('releaseDate', _params['release_date']))
 
         if _params.get('primary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('primaryMoodCluster', _params['primary_mood_cluster'].value))
+            _query_params.append(('primaryMoodCluster', _params['primary_mood_cluster']))
 
         if _params.get('secondary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('secondaryMoodCluster', _params['secondary_mood_cluster'].value))
+            _query_params.append(('secondaryMoodCluster', _params['secondary_mood_cluster']))
 
         if _params.get('tertiary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('tertiaryMoodCluster', _params['tertiary_mood_cluster'].value))
+            _query_params.append(('tertiaryMoodCluster', _params['tertiary_mood_cluster']))
 
         if _params.get('valence') is not None:  # noqa: E501
-            _query_params.append(('valence', _params['valence'].value))
+            _query_params.append(('valence', _params['valence']))
 
         if _params.get('arousal') is not None:  # noqa: E501
-            _query_params.append(('arousal', _params['arousal'].value))
+            _query_params.append(('arousal', _params['arousal']))
 
         if _params.get('pleasantness') is not None:  # noqa: E501
-            _query_params.append(('pleasantness', _params['pleasantness'].value))
+            _query_params.append(('pleasantness', _params['pleasantness']))
 
         if _params.get('engagement') is not None:  # noqa: E501
-            _query_params.append(('engagement', _params['engagement'].value))
+            _query_params.append(('engagement', _params['engagement']))
 
         if _params.get('vocals') is not None:  # noqa: E501
-            _query_params.append(('vocals', _params['vocals'].value))
+            _query_params.append(('vocals', _params['vocals']))
 
         if _params.get('dominant_instrument') is not None:  # noqa: E501
-            _query_params.append(('dominantInstrument', _params['dominant_instrument'].value))
+            _query_params.append(('dominantInstrument', _params['dominant_instrument']))
 
         if _params.get('secondary_instrument') is not None:  # noqa: E501
-            _query_params.append(('secondaryInstrument', _params['secondary_instrument'].value))
+            _query_params.append(('secondaryInstrument', _params['secondary_instrument']))
 
         if _params.get('tertiary_instrument') is not None:  # noqa: E501
-            _query_params.append(('tertiaryInstrument', _params['tertiary_instrument'].value))
+            _query_params.append(('tertiaryInstrument', _params['tertiary_instrument']))
 
         if _params.get('energy') is not None:  # noqa: E501
-            _query_params.append(('energy', _params['energy'].value))
+            _query_params.append(('energy', _params['energy']))
 
         if _params.get('sound_generation') is not None:  # noqa: E501
-            _query_params.append(('soundGeneration', _params['sound_generation'].value))
+            _query_params.append(('soundGeneration', _params['sound_generation']))
 
         if _params.get('tempo') is not None:  # noqa: E501
-            _query_params.append(('tempo', _params['tempo'].value))
+            _query_params.append(('tempo', _params['tempo']))
 
         if _params.get('scale') is not None:  # noqa: E501
-            _query_params.append(('scale', _params['scale'].value))
+            _query_params.append(('scale', _params['scale']))
 
         if _params.get('rhythm') is not None:  # noqa: E501
-            _query_params.append(('rhythm', _params['rhythm'].value))
+            _query_params.append(('rhythm', _params['rhythm']))
 
         if _params.get('primary_sound_character') is not None:  # noqa: E501
-            _query_params.append(('primarySoundCharacter', _params['primary_sound_character'].value))
+            _query_params.append(('primarySoundCharacter', _params['primary_sound_character']))
 
         if _params.get('timbre') is not None:  # noqa: E501
-            _query_params.append(('timbre', _params['timbre'].value))
+            _query_params.append(('timbre', _params['timbre']))
 
         if _params.get('roughness') is not None:  # noqa: E501
-            _query_params.append(('roughness', _params['roughness'].value))
+            _query_params.append(('roughness', _params['roughness']))
 
         if _params.get('tonality') is not None:  # noqa: E501
-            _query_params.append(('tonality', _params['tonality'].value))
+            _query_params.append(('tonality', _params['tonality']))
 
         if _params.get('harmony') is not None:  # noqa: E501
-            _query_params.append(('harmony', _params['harmony'].value))
+            _query_params.append(('harmony', _params['harmony']))
 
         if _params.get('texture') is not None:  # noqa: E501
-            _query_params.append(('texture', _params['texture'].value))
+            _query_params.append(('texture', _params['texture']))
 
         if _params.get('groovyness') is not None:  # noqa: E501
-            _query_params.append(('groovyness', _params['groovyness'].value))
+            _query_params.append(('groovyness', _params['groovyness']))
 
         if _params.get('space') is not None:  # noqa: E501
-            _query_params.append(('space', _params['space'].value))
+            _query_params.append(('space', _params['space']))
 
         if _params.get('production_rating') is not None:  # noqa: E501
-            _query_params.append(('productionRating', _params['production_rating'].value))
+            _query_params.append(('productionRating', _params['production_rating']))
 
         if _params.get('performance_rating') is not None:  # noqa: E501
-            _query_params.append(('performanceRating', _params['performance_rating'].value))
+            _query_params.append(('performanceRating', _params['performance_rating']))
 
         if _params.get('song_rating') is not None:  # noqa: E501
-            _query_params.append(('songRating', _params['song_rating'].value))
+            _query_params.append(('songRating', _params['song_rating']))
 
         if _params.get('audience_age') is not None:  # noqa: E501
-            _query_params.append(('audienceAge', _params['audience_age'].value))
+            _query_params.append(('audienceAge', _params['audience_age']))
 
         if _params.get('audience_region') is not None:  # noqa: E501
-            _query_params.append(('audienceRegion', _params['audience_region'].value))
+            _query_params.append(('audienceRegion', _params['audience_region']))
 
         if _params.get('audience_gender') is not None:  # noqa: E501
-            _query_params.append(('audienceGender', _params['audience_gender'].value))
+            _query_params.append(('audienceGender', _params['audience_gender']))
 
         if _params.get('songtradr_track_id') is not None:  # noqa: E501
             _query_params.append(('songtradrTrackId', _params['songtradr_track_id']))
 
         if _params.get('usage_name') is not None:  # noqa: E501
             _query_params.append(('usageName', _params['usage_name']))
 
@@ -4592,15 +4608,15 @@
         if _params.get('composer') is not None:  # noqa: E501
             _query_params.append(('composer', _params['composer']))
 
         if _params.get('title') is not None:  # noqa: E501
             _query_params.append(('title', _params['title']))
 
         if _params.get('language') is not None:  # noqa: E501
-            _query_params.append(('language', _params['language'].value))
+            _query_params.append(('language', _params['language']))
 
         if _params.get('genre_names') is not None:  # noqa: E501
             _query_params.append(('genreNames', _params['genre_names']))
             _collection_formats['genreNames'] = 'multi'
 
         if _params.get('tag_names') is not None:  # noqa: E501
             _query_params.append(('tagNames', _params['tag_names']))
@@ -4609,114 +4625,114 @@
         if _params.get('release_date') is not None:  # noqa: E501
             if isinstance(_params['release_date'], datetime):
                 _query_params.append(('releaseDate', _params['release_date'].strftime(self.api_client.configuration.datetime_format)))
             else:
                 _query_params.append(('releaseDate', _params['release_date']))
 
         if _params.get('primary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('primaryMoodCluster', _params['primary_mood_cluster'].value))
+            _query_params.append(('primaryMoodCluster', _params['primary_mood_cluster']))
 
         if _params.get('secondary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('secondaryMoodCluster', _params['secondary_mood_cluster'].value))
+            _query_params.append(('secondaryMoodCluster', _params['secondary_mood_cluster']))
 
         if _params.get('tertiary_mood_cluster') is not None:  # noqa: E501
-            _query_params.append(('tertiaryMoodCluster', _params['tertiary_mood_cluster'].value))
+            _query_params.append(('tertiaryMoodCluster', _params['tertiary_mood_cluster']))
 
         if _params.get('valence') is not None:  # noqa: E501
-            _query_params.append(('valence', _params['valence'].value))
+            _query_params.append(('valence', _params['valence']))
 
         if _params.get('arousal') is not None:  # noqa: E501
-            _query_params.append(('arousal', _params['arousal'].value))
+            _query_params.append(('arousal', _params['arousal']))
 
         if _params.get('pleasantness') is not None:  # noqa: E501
-            _query_params.append(('pleasantness', _params['pleasantness'].value))
+            _query_params.append(('pleasantness', _params['pleasantness']))
 
         if _params.get('engagement') is not None:  # noqa: E501
-            _query_params.append(('engagement', _params['engagement'].value))
+            _query_params.append(('engagement', _params['engagement']))
 
         if _params.get('vocals') is not None:  # noqa: E501
-            _query_params.append(('vocals', _params['vocals'].value))
+            _query_params.append(('vocals', _params['vocals']))
 
         if _params.get('dominant_instrument') is not None:  # noqa: E501
-            _query_params.append(('dominantInstrument', _params['dominant_instrument'].value))
+            _query_params.append(('dominantInstrument', _params['dominant_instrument']))
 
         if _params.get('secondary_instrument') is not None:  # noqa: E501
-            _query_params.append(('secondaryInstrument', _params['secondary_instrument'].value))
+            _query_params.append(('secondaryInstrument', _params['secondary_instrument']))
 
         if _params.get('tertiary_instrument') is not None:  # noqa: E501
-            _query_params.append(('tertiaryInstrument', _params['tertiary_instrument'].value))
+            _query_params.append(('tertiaryInstrument', _params['tertiary_instrument']))
 
         if _params.get('energy') is not None:  # noqa: E501
-            _query_params.append(('energy', _params['energy'].value))
+            _query_params.append(('energy', _params['energy']))
 
         if _params.get('sound_generation') is not None:  # noqa: E501
-            _query_params.append(('soundGeneration', _params['sound_generation'].value))
+            _query_params.append(('soundGeneration', _params['sound_generation']))
 
         if _params.get('tempo') is not None:  # noqa: E501
-            _query_params.append(('tempo', _params['tempo'].value))
+            _query_params.append(('tempo', _params['tempo']))
 
         if _params.get('scale') is not None:  # noqa: E501
-            _query_params.append(('scale', _params['scale'].value))
+            _query_params.append(('scale', _params['scale']))
 
         if _params.get('rhythm') is not None:  # noqa: E501
-            _query_params.append(('rhythm', _params['rhythm'].value))
+            _query_params.append(('rhythm', _params['rhythm']))
 
         if _params.get('primary_sound_character') is not None:  # noqa: E501
-            _query_params.append(('primarySoundCharacter', _params['primary_sound_character'].value))
+            _query_params.append(('primarySoundCharacter', _params['primary_sound_character']))
 
         if _params.get('timbre') is not None:  # noqa: E501
-            _query_params.append(('timbre', _params['timbre'].value))
+            _query_params.append(('timbre', _params['timbre']))
 
         if _params.get('roughness') is not None:  # noqa: E501
-            _query_params.append(('roughness', _params['roughness'].value))
+            _query_params.append(('roughness', _params['roughness']))
 
         if _params.get('tonality') is not None:  # noqa: E501
-            _query_params.append(('tonality', _params['tonality'].value))
+            _query_params.append(('tonality', _params['tonality']))
 
         if _params.get('harmony') is not None:  # noqa: E501
-            _query_params.append(('harmony', _params['harmony'].value))
+            _query_params.append(('harmony', _params['harmony']))
 
         if _params.get('texture') is not None:  # noqa: E501
-            _query_params.append(('texture', _params['texture'].value))
+            _query_params.append(('texture', _params['texture']))
 
         if _params.get('groovyness') is not None:  # noqa: E501
-            _query_params.append(('groovyness', _params['groovyness'].value))
+            _query_params.append(('groovyness', _params['groovyness']))
 
         if _params.get('space') is not None:  # noqa: E501
-            _query_params.append(('space', _params['space'].value))
+            _query_params.append(('space', _params['space']))
 
         if _params.get('production_rating') is not None:  # noqa: E501
-            _query_params.append(('productionRating', _params['production_rating'].value))
+            _query_params.append(('productionRating', _params['production_rating']))
 
         if _params.get('performance_rating') is not None:  # noqa: E501
-            _query_params.append(('performanceRating', _params['performance_rating'].value))
+            _query_params.append(('performanceRating', _params['performance_rating']))
 
         if _params.get('song_rating') is not None:  # noqa: E501
-            _query_params.append(('songRating', _params['song_rating'].value))
+            _query_params.append(('songRating', _params['song_rating']))
 
         if _params.get('audience_age') is not None:  # noqa: E501
-            _query_params.append(('audienceAge', _params['audience_age'].value))
+            _query_params.append(('audienceAge', _params['audience_age']))
 
         if _params.get('audience_region') is not None:  # noqa: E501
-            _query_params.append(('audienceRegion', _params['audience_region'].value))
+            _query_params.append(('audienceRegion', _params['audience_region']))
 
         if _params.get('audience_gender') is not None:  # noqa: E501
-            _query_params.append(('audienceGender', _params['audience_gender'].value))
+            _query_params.append(('audienceGender', _params['audience_gender']))
 
         if _params.get('origin_decade') is not None:  # noqa: E501
-            _query_params.append(('originDecade', _params['origin_decade'].value))
+            _query_params.append(('originDecade', _params['origin_decade']))
 
         if _params.get('curateability') is not None:  # noqa: E501
-            _query_params.append(('curateability', _params['curateability'].value))
+            _query_params.append(('curateability', _params['curateability']))
 
         if _params.get('use_case') is not None:  # noqa: E501
-            _query_params.append(('useCase', _params['use_case'].value))
+            _query_params.append(('useCase', _params['use_case']))
 
         if _params.get('channel_suitability') is not None:  # noqa: E501
-            _query_params.append(('channelSuitability', _params['channel_suitability'].value))
+            _query_params.append(('channelSuitability', _params['channel_suitability']))
 
         if _params.get('similar_to_recording') is not None:  # noqa: E501
             _query_params.append(('similarToRecording', _params['similar_to_recording']))
 
         if _params.get('songtradr_track_id') is not None:  # noqa: E501
             _query_params.append(('songtradrTrackId', _params['songtradr_track_id']))
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/api_client.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.12.23/python'
+        self.user_agent = 'OpenAPI-Generator/1.12.24/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/api_response.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/api_response.py`

 * *Files identical despite different names*

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/configuration.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -373,16 +373,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.12.23\n"\
-               "SDK Package Version: 1.12.23".\
+               "Version of the API: 1.12.24\n"\
+               "SDK Package Version: 1.12.24".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/exceptions.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/__init__.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/admin_api_user_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/admin_api_user_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -117,7 +117,8 @@
             "total_searches": obj.get("totalSearches"),
             "total_uploads": obj.get("totalUploads"),
             "total_downloads": obj.get("totalDownloads"),
             "total_updates": obj.get("totalUpdates")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/api_key_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/api_key_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -23,18 +23,18 @@
 from pydantic import BaseModel, Field, StrictStr
 
 class ApiKeyDTO(BaseModel):
     """
     ApiKeyDTO
     """
     name: StrictStr = Field(...)
-    created_at: datetime = Field(..., alias="createdAt")
     last_used_at: Optional[datetime] = Field(None, alias="lastUsedAt")
+    created_at: datetime = Field(..., alias="createdAt")
     id: StrictStr = Field(...)
-    __properties = ["name", "createdAt", "lastUsedAt", "id"]
+    __properties = ["name", "lastUsedAt", "createdAt", "id"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -65,13 +65,14 @@
             return None
 
         if not isinstance(obj, dict):
             return ApiKeyDTO.parse_obj(obj)
 
         _obj = ApiKeyDTO.parse_obj({
             "name": obj.get("name"),
-            "created_at": obj.get("createdAt"),
             "last_used_at": obj.get("lastUsedAt"),
+            "created_at": obj.get("createdAt"),
             "id": obj.get("id")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/category_medium_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/category_medium_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -77,7 +77,8 @@
         _obj = CategoryMediumDTO.parse_obj({
             "id": obj.get("id"),
             "name": obj.get("name"),
             "tags": [TagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/category_minimal_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/category_minimal_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -65,7 +65,8 @@
             return CategoryMinimalDTO.parse_obj(obj)
 
         _obj = CategoryMinimalDTO.parse_obj({
             "category_name": obj.get("categoryName")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/config_access_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/config_access_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -81,7 +81,8 @@
 
         _obj = ConfigAccessDTO.parse_obj({
             "accessor_id": obj.get("accessorId"),
             "rights": obj.get("rights")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/config_identifier_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/config_identifier_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -67,7 +67,8 @@
 
         _obj = ConfigIdentifierDTO.parse_obj({
             "identifier_type": obj.get("identifierType"),
             "identifier_value": obj.get("identifierValue")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/contributor_type_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/contributor_type_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -65,7 +65,8 @@
             return ContributorTypeDTO.parse_obj(obj)
 
         _obj = ContributorTypeDTO.parse_obj({
             "type_name": obj.get("typeName")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/create_api_key_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/create_api_key_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -65,7 +65,8 @@
             return CreateApiKeyDTO.parse_obj(obj)
 
         _obj = CreateApiKeyDTO.parse_obj({
             "name": obj.get("name")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/error_response.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,7 +73,8 @@
             "status": obj.get("status"),
             "error": obj.get("error"),
             "message": obj.get("message"),
             "path": obj.get("path")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/field_summary_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/field_summary_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -69,7 +69,8 @@
         _obj = FieldSummaryDTO.parse_obj({
             "field_value": obj.get("fieldValue"),
             "total": obj.get("total"),
             "field_name": obj.get("fieldName")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -128,7 +128,8 @@
             "inference_end_time": obj.get("inferenceEndTime"),
             "recording": RecordingMediumDTO.from_dict(obj.get("recording")) if obj.get("recording") is not None else None,
             "error_time": obj.get("error_time"),
             "error_message": obj.get("error_message")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_list_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_list_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -79,7 +79,8 @@
             "files": [FileDTO.from_dict(_item) for _item in obj.get("files")] if obj.get("files") is not None else None,
             "has_next_page": obj.get("hasNextPage"),
             "current_page_number": obj.get("currentPageNumber"),
             "total_results": obj.get("totalResults")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_minimal_with_url_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_minimal_with_url_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -69,7 +69,8 @@
         _obj = FileMinimalWithUrlDTO.parse_obj({
             "file_name": obj.get("fileName"),
             "url": obj.get("url"),
             "isrc": obj.get("isrc")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_small_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -26,26 +26,26 @@
     """
     Reduced details on a file that has been uploaded for auto-tagging or audio-recognition purposes.
     """
     name: StrictStr = Field(...)
     id: StrictInt = Field(...)
     extension: StrictStr = Field(..., description="extension of the file")
     error_message: Optional[StrictStr] = None
-    folder: StrictStr = Field(...)
     object_key: StrictStr = Field(..., alias="objectKey")
     upload_start_time: Optional[datetime] = Field(None, alias="uploadStartTime")
     upload_end_time: Optional[datetime] = Field(None, alias="uploadEndTime")
     fingerprint_status: Optional[StrictStr] = Field(None, alias="fingerprintStatus", description="status of the audio recognition")
     fingerprint_start_time: Optional[datetime] = Field(None, alias="fingerprintStartTime")
     fingerprint_end_time: Optional[datetime] = Field(None, alias="fingerprintEndTime")
     inference_status: Optional[StrictStr] = Field(None, alias="inferenceStatus", description="status of the auto-tagging")
     inference_start_time: Optional[datetime] = Field(None, alias="inferenceStartTime")
     inference_end_time: Optional[datetime] = Field(None, alias="inferenceEndTime")
     error_time: Optional[datetime] = None
-    __properties = ["name", "id", "extension", "error_message", "folder", "objectKey", "uploadStartTime", "uploadEndTime", "fingerprintStatus", "fingerprintStartTime", "fingerprintEndTime", "inferenceStatus", "inferenceStartTime", "inferenceEndTime", "error_time"]
+    folder: StrictStr = Field(...)
+    __properties = ["name", "id", "extension", "error_message", "objectKey", "uploadStartTime", "uploadEndTime", "fingerprintStatus", "fingerprintStartTime", "fingerprintEndTime", "inferenceStatus", "inferenceStartTime", "inferenceEndTime", "error_time", "folder"]
 
     @validator('extension')
     def extension_validate_enum(cls, value):
         """Validates the enum"""
         if value not in ('mp3', 'wav', 'flac'):
             raise ValueError("must be one of enum values ('mp3', 'wav', 'flac')")
         return value
@@ -106,21 +106,22 @@
             return FileSmallDTO.parse_obj(obj)
 
         _obj = FileSmallDTO.parse_obj({
             "name": obj.get("name"),
             "id": obj.get("id"),
             "extension": obj.get("extension"),
             "error_message": obj.get("error_message"),
-            "folder": obj.get("folder"),
             "object_key": obj.get("objectKey"),
             "upload_start_time": obj.get("uploadStartTime"),
             "upload_end_time": obj.get("uploadEndTime"),
             "fingerprint_status": obj.get("fingerprintStatus"),
             "fingerprint_start_time": obj.get("fingerprintStartTime"),
             "fingerprint_end_time": obj.get("fingerprintEndTime"),
             "inference_status": obj.get("inferenceStatus"),
             "inference_start_time": obj.get("inferenceStartTime"),
             "inference_end_time": obj.get("inferenceEndTime"),
-            "error_time": obj.get("error_time")
+            "error_time": obj.get("error_time"),
+            "folder": obj.get("folder")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_upload_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_upload_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -85,7 +85,8 @@
         _obj = FileUploadDTO.parse_obj({
             "identifiers": [ConfigIdentifierDTO.from_dict(_item) for _item in obj.get("identifiers")] if obj.get("identifiers") is not None else None,
             "flags": obj.get("flags"),
             "access": [ConfigAccessDTO.from_dict(_item) for _item in obj.get("access")] if obj.get("access") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/file_w_ith_url_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/file_w_ith_url_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -71,7 +71,8 @@
 
         _obj = FileWIthUrlDTO.parse_obj({
             "file": FileDTO.from_dict(obj.get("file")) if obj.get("file") is not None else None,
             "url": obj.get("url")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/files_summary_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/files_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -108,7 +108,8 @@
             "musical_features_summary": [FieldSummaryDTO.from_dict(_item) for _item in obj.get("musicalFeaturesSummary")] if obj.get("musicalFeaturesSummary") is not None else None,
             "total_files": obj.get("totalFiles"),
             "bpm_min": obj.get("bpmMin"),
             "bpm_max": obj.get("bpmMax")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/forgot_password_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/forgot_password_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -77,7 +77,8 @@
 
         _obj = ForgotPasswordDTO.parse_obj({
             "email_or_username": obj.get("emailOrUsername"),
             "system": obj.get("system")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/genre_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/genre_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -67,7 +67,8 @@
 
         _obj = GenreDTO.parse_obj({
             "id": obj.get("id"),
             "name": obj.get("name")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/genre_minimal_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/genre_minimal_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -65,7 +65,8 @@
             return GenreMinimalDTO.parse_obj(obj)
 
         _obj = GenreMinimalDTO.parse_obj({
             "genre_name": obj.get("genreName")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/genres_summary_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/genres_summary_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -69,7 +69,8 @@
         _obj = GenresSummaryDTO.parse_obj({
             "name": obj.get("name"),
             "total": obj.get("total"),
             "genre_type": obj.get("genreType")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/init_put_recording_audio_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/init_put_recording_audio_dto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -69,7 +69,8 @@
         _obj = InitPutRecordingAudioDTO.parse_obj({
             "isrc": obj.get("isrc"),
             "object_key": obj.get("objectKey"),
             "url": obj.get("url")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/jwt_token_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/jwt_token_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -69,7 +69,8 @@
         _obj = JwtTokenDTO.parse_obj({
             "jwt_token": obj.get("jwtToken"),
             "expiration_date": obj.get("expirationDate"),
             "refresh_token": obj.get("refreshToken")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/login_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/login_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -71,7 +71,8 @@
             "username": obj.get("username"),
             "version": obj.get("version"),
             "email": obj.get("email"),
             "password": obj.get("password")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/musical_features_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/musical_features_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -23,29 +23,38 @@
 from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, validator
 
 class MusicalFeaturesDTO(BaseModel):
     """
     AI generated musical features of a recording.
     """
     space: Optional[StrictStr] = Field(None, description="Search for space")
-    language_of_performance: Optional[StrictStr] = Field(None, alias="languageOfPerformance")
+    energy: Optional[StrictStr] = Field(None, description="Search for energy")
+    engagement: Optional[StrictStr] = Field(None, description="Search for an engagement")
+    groovyness: Optional[StrictStr] = Field(None, description="Search for groovyness")
+    harmony: Optional[StrictStr] = Field(None, description="Search for a degree of harmoniousness")
+    pleasantness: Optional[StrictStr] = Field(None, description="Search for pleasantness")
+    primary_mood_cluster: Optional[StrictStr] = Field(None, alias="primaryMoodCluster", description="Search for a language of the lyrics")
+    primary_sound_character: Optional[StrictStr] = Field(None, alias="primarySoundCharacter", description="Search for a sound character")
     rhythm: Optional[StrictStr] = Field(None, description="Search for rhythm")
     roughness: Optional[StrictStr] = Field(None, description="Search for roughness")
     scale: Optional[StrictStr] = Field(None, description="Search for a tonal scale")
     sound_generation: Optional[StrictStr] = Field(None, alias="soundGeneration", description="Search for type of sound generation")
     tempo: Optional[StrictStr] = Field(None, description="Search for tempo")
     texture: Optional[StrictStr] = Field(None, description="Search for texture")
     timbre: Optional[StrictStr] = Field(None, description="Search for timbre")
     tonality: Optional[StrictStr] = Field(None, description="Search for tonality")
     valence: Optional[StrictStr] = Field(None, description="Search for a valence")
     vocals: Optional[StrictStr] = Field(None, description="Search for a vocal gender or instrumental songs")
     origin_decade: Optional[StrictStr] = Field(None, alias="originDecade", description="Search for origin decade")
     curateability: Optional[StrictStr] = Field(None, description="Search for curatebility")
     use_case: Optional[StrictStr] = Field(None, alias="useCase", description="Search for use case")
     channel_suitability: Optional[StrictStr] = Field(None, alias="channelSuitability", description="Search for social media suitability")
+    language_of_performance: Optional[StrictStr] = Field(None, alias="languageOfPerformance")
+    arousal: Optional[StrictStr] = Field(None, description="Search for an arousal")
+    dominant_instrument: Optional[StrictStr] = Field(None, alias="dominantInstrument", description="Search for a dominant instrument")
     primary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="primaryMoodClusterAffinity")
     secondary_mood_cluster: Optional[StrictStr] = Field(None, alias="secondaryMoodCluster", description="Search for a language of the lyrics")
     secondary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="secondaryMoodClusterAffinity")
     tertiary_mood_cluster: Optional[StrictStr] = Field(None, alias="tertiaryMoodCluster", description="Search for a language of the lyrics")
     tertiary_mood_cluster_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="tertiaryMoodClusterAffinity")
     vocals_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="vocalsAffinity")
     dominant_instrument_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="dominantInstrumentAffinity")
@@ -82,23 +91,14 @@
     origin_decade_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="originDecadeAffinity")
     language_of_performance_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="languageOfPerformanceAffinity")
     curateability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="curateabilityAffinity")
     use_case_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="useCaseAffinity")
     industry_suitability: Optional[StrictStr] = Field(None, alias="industrySuitability", description="Search for Industry suitability")
     industry_suitability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="industrySuitabilityAffinity")
     audience_region: Optional[StrictStr] = Field(None, alias="audienceRegion")
-    arousal: Optional[StrictStr] = Field(None, description="Search for an arousal")
-    dominant_instrument: Optional[StrictStr] = Field(None, alias="dominantInstrument", description="Search for a dominant instrument")
-    energy: Optional[StrictStr] = Field(None, description="Search for energy")
-    engagement: Optional[StrictStr] = Field(None, description="Search for an engagement")
-    groovyness: Optional[StrictStr] = Field(None, description="Search for groovyness")
-    harmony: Optional[StrictStr] = Field(None, description="Search for a degree of harmoniousness")
-    pleasantness: Optional[StrictStr] = Field(None, description="Search for pleasantness")
-    primary_mood_cluster: Optional[StrictStr] = Field(None, alias="primaryMoodCluster", description="Search for a language of the lyrics")
-    primary_sound_character: Optional[StrictStr] = Field(None, alias="primarySoundCharacter", description="Search for a sound character")
     valence_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="valenceAffinity")
     arousal_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="arousalAffinity")
     pleasantness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="pleasantnessAffinity")
     engagement_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="engagementAffinity")
     energy_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="energyAffinity")
     tempo_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="tempoAffinity")
     scale_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="scaleAffinity")
@@ -107,34 +107,94 @@
     harmony_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="harmonyAffinity")
     texture_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="textureAffinity")
     groovyness_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="groovynessAffinity")
     space_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="spaceAffinity")
     key_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="keyAffinity")
     channel_suitability_affinity: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="channelSuitabilityAffinity")
     key: Optional[StrictStr] = Field(None, description="Search for a harmonic key")
-    __properties = ["space", "languageOfPerformance", "rhythm", "roughness", "scale", "soundGeneration", "tempo", "texture", "timbre", "tonality", "valence", "vocals", "originDecade", "curateability", "useCase", "channelSuitability", "primaryMoodClusterAffinity", "secondaryMoodCluster", "secondaryMoodClusterAffinity", "tertiaryMoodCluster", "tertiaryMoodClusterAffinity", "vocalsAffinity", "dominantInstrumentAffinity", "secondaryInstrument", "secondaryInstrumentAffinity", "tertiaryInstrument", "tertiaryInstrumentAffinity", "soundGenerationAffinity", "rhythmAffinity", "primarySoundCharacterAffinity", "tonalityAffinity", "bpm", "productionRating", "productionRatingAffinity", "performanceRating", "performanceRatingAffinity", "songRating", "songRatingAffinity", "audienceAge", "audienceAgeAffinity", "secondaryAudienceAge", "secondaryAudienceAgeAffinity", "tertiaryAudienceAge", "tertiaryAudienceAgeAffinity", "audienceGender", "audienceGenderAffinity", "audienceRegionAffinity", "secondaryAudienceRegion", "secondaryAudienceRegionAffinity", "tertiaryAudienceRegion", "tertiaryAudienceRegionAffinity", "originRegion", "originRegionAffinity", "originDecadeAffinity", "languageOfPerformanceAffinity", "curateabilityAffinity", "useCaseAffinity", "industrySuitability", "industrySuitabilityAffinity", "audienceRegion", "arousal", "dominantInstrument", "energy", "engagement", "groovyness", "harmony", "pleasantness", "primaryMoodCluster", "primarySoundCharacter", "valenceAffinity", "arousalAffinity", "pleasantnessAffinity", "engagementAffinity", "energyAffinity", "tempoAffinity", "scaleAffinity", "timbreAffinity", "roughnessAffinity", "harmonyAffinity", "textureAffinity", "groovynessAffinity", "spaceAffinity", "keyAffinity", "channelSuitabilityAffinity", "key"]
+    __properties = ["space", "energy", "engagement", "groovyness", "harmony", "pleasantness", "primaryMoodCluster", "primarySoundCharacter", "rhythm", "roughness", "scale", "soundGeneration", "tempo", "texture", "timbre", "tonality", "valence", "vocals", "originDecade", "curateability", "useCase", "channelSuitability", "languageOfPerformance", "arousal", "dominantInstrument", "primaryMoodClusterAffinity", "secondaryMoodCluster", "secondaryMoodClusterAffinity", "tertiaryMoodCluster", "tertiaryMoodClusterAffinity", "vocalsAffinity", "dominantInstrumentAffinity", "secondaryInstrument", "secondaryInstrumentAffinity", "tertiaryInstrument", "tertiaryInstrumentAffinity", "soundGenerationAffinity", "rhythmAffinity", "primarySoundCharacterAffinity", "tonalityAffinity", "bpm", "productionRating", "productionRatingAffinity", "performanceRating", "performanceRatingAffinity", "songRating", "songRatingAffinity", "audienceAge", "audienceAgeAffinity", "secondaryAudienceAge", "secondaryAudienceAgeAffinity", "tertiaryAudienceAge", "tertiaryAudienceAgeAffinity", "audienceGender", "audienceGenderAffinity", "audienceRegionAffinity", "secondaryAudienceRegion", "secondaryAudienceRegionAffinity", "tertiaryAudienceRegion", "tertiaryAudienceRegionAffinity", "originRegion", "originRegionAffinity", "originDecadeAffinity", "languageOfPerformanceAffinity", "curateabilityAffinity", "useCaseAffinity", "industrySuitability", "industrySuitabilityAffinity", "audienceRegion", "valenceAffinity", "arousalAffinity", "pleasantnessAffinity", "engagementAffinity", "energyAffinity", "tempoAffinity", "scaleAffinity", "timbreAffinity", "roughnessAffinity", "harmonyAffinity", "textureAffinity", "groovynessAffinity", "spaceAffinity", "keyAffinity", "channelSuitabilityAffinity", "key"]
 
     @validator('space')
     def space_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
         if value not in ('very compact', 'compact', 'moderate space', 'wide', 'very wide'):
             raise ValueError("must be one of enum values ('very compact', 'compact', 'moderate space', 'wide', 'very wide')")
         return value
 
-    @validator('language_of_performance')
-    def language_of_performance_validate_enum(cls, value):
+    @validator('energy')
+    def energy_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in ('en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi'):
-            raise ValueError("must be one of enum values ('en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi')")
+        if value not in ('very quiet', 'quiet', 'moderate', 'loud', 'very loud', 'dynamic'):
+            raise ValueError("must be one of enum values ('very quiet', 'quiet', 'moderate', 'loud', 'very loud', 'dynamic')")
+        return value
+
+    @validator('engagement')
+    def engagement_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('very unengaging', 'unengaging', 'neutral engagement', 'engaging', 'very engaging', 'varying engagement'):
+            raise ValueError("must be one of enum values ('very unengaging', 'unengaging', 'neutral engagement', 'engaging', 'very engaging', 'varying engagement')")
+        return value
+
+    @validator('groovyness')
+    def groovyness_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('very steady', 'steady', 'moderate rhythm feel', 'groovy', 'very groovy'):
+            raise ValueError("must be one of enum values ('very steady', 'steady', 'moderate rhythm feel', 'groovy', 'very groovy')")
+        return value
+
+    @validator('harmony')
+    def harmony_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('very dissonant', 'dissonant', 'moderate harmonies', 'harmonious', 'very harmonious'):
+            raise ValueError("must be one of enum values ('very dissonant', 'dissonant', 'moderate harmonies', 'harmonious', 'very harmonious')")
+        return value
+
+    @validator('pleasantness')
+    def pleasantness_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('very unpleasant', 'unpleasant', 'neutral pleasantness', 'pleasant', 'very pleasant', 'varying pleasantness'):
+            raise ValueError("must be one of enum values ('very unpleasant', 'unpleasant', 'neutral pleasantness', 'pleasant', 'very pleasant', 'varying pleasantness')")
+        return value
+
+    @validator('primary_mood_cluster')
+    def primary_mood_cluster_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild'):
+            raise ValueError("must be one of enum values ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild')")
+        return value
+
+    @validator('primary_sound_character')
+    def primary_sound_character_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('brassy', 'bright', 'clear', 'deep', 'distorted', 'flat', 'full', 'groovy', 'melodious', 'natural', 'resonant', 'shrill', 'steady', 'thin', 'warm'):
+            raise ValueError("must be one of enum values ('brassy', 'bright', 'clear', 'deep', 'distorted', 'flat', 'full', 'groovy', 'melodious', 'natural', 'resonant', 'shrill', 'steady', 'thin', 'warm')")
         return value
 
     @validator('rhythm')
     def rhythm_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
@@ -269,14 +329,44 @@
         if value is None:
             return value
 
         if value not in ('Spotify', 'TikTok', 'Unfitting', 'YouTube'):
             raise ValueError("must be one of enum values ('Spotify', 'TikTok', 'Unfitting', 'YouTube')")
         return value
 
+    @validator('language_of_performance')
+    def language_of_performance_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi'):
+            raise ValueError("must be one of enum values ('en', 'de', 'no', 'fr', 'es', 'pt', 'fi', 'ru', 'it', 'la', 'el', 'ar', 'nl', 'ja', 'pl', 'sv', 'zu', 'da', 'cs', 'hu', 'af', 'hi', 'tr', 'zh', 'ms', 'pa', 'id', 'ko', 'vi')")
+        return value
+
+    @validator('arousal')
+    def arousal_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal'):
+            raise ValueError("must be one of enum values ('very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal')")
+        return value
+
+    @validator('dominant_instrument')
+    def dominant_instrument_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp'):
+            raise ValueError("must be one of enum values ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp')")
+        return value
+
     @validator('secondary_mood_cluster')
     def secondary_mood_cluster_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
         if value not in ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild'):
@@ -429,104 +519,14 @@
         if value is None:
             return value
 
         if value not in ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe'):
             raise ValueError("must be one of enum values ('Australia and New Zealand', 'Central America and the Carribean', 'Central and Southern Asia', 'Eastern Asia', 'Eastern Europe', 'Northern Africa and Western Asia', 'Northern America', 'Oceania', 'South America', 'South-Eastern Asia', 'Southern Europe', 'Sub-Saharan Africa', 'Western and Northern Europe')")
         return value
 
-    @validator('arousal')
-    def arousal_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal'):
-            raise ValueError("must be one of enum values ('very calm', 'calm', 'moderate arousal', 'energetic', 'very energetic', 'varying arousal')")
-        return value
-
-    @validator('dominant_instrument')
-    def dominant_instrument_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp'):
-            raise ValueError("must be one of enum values ('electric guitar', 'piano', 'electronics', 'guitar', 'strings', 'synthesizer', 'wind', 'saxophone', 'flute', 'trumpet', 'drum kit', 'keys', 'accordion', 'violin', 'harpsichord', 'choir', 'cello', 'electric bass', 'organ', 'brass', 'percussion', 'vocals', 'double bass', 'harp')")
-        return value
-
-    @validator('energy')
-    def energy_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('very quiet', 'quiet', 'moderate', 'loud', 'very loud', 'dynamic'):
-            raise ValueError("must be one of enum values ('very quiet', 'quiet', 'moderate', 'loud', 'very loud', 'dynamic')")
-        return value
-
-    @validator('engagement')
-    def engagement_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('very unengaging', 'unengaging', 'neutral engagement', 'engaging', 'very engaging', 'varying engagement'):
-            raise ValueError("must be one of enum values ('very unengaging', 'unengaging', 'neutral engagement', 'engaging', 'very engaging', 'varying engagement')")
-        return value
-
-    @validator('groovyness')
-    def groovyness_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('very steady', 'steady', 'moderate rhythm feel', 'groovy', 'very groovy'):
-            raise ValueError("must be one of enum values ('very steady', 'steady', 'moderate rhythm feel', 'groovy', 'very groovy')")
-        return value
-
-    @validator('harmony')
-    def harmony_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('very dissonant', 'dissonant', 'moderate harmonies', 'harmonious', 'very harmonious'):
-            raise ValueError("must be one of enum values ('very dissonant', 'dissonant', 'moderate harmonies', 'harmonious', 'very harmonious')")
-        return value
-
-    @validator('pleasantness')
-    def pleasantness_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('very unpleasant', 'unpleasant', 'neutral pleasantness', 'pleasant', 'very pleasant', 'varying pleasantness'):
-            raise ValueError("must be one of enum values ('very unpleasant', 'unpleasant', 'neutral pleasantness', 'pleasant', 'very pleasant', 'varying pleasantness')")
-        return value
-
-    @validator('primary_mood_cluster')
-    def primary_mood_cluster_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild'):
-            raise ValueError("must be one of enum values ('aggressive', 'amusing', 'anxious', 'calm', 'devotional', 'dreamy', 'energetic', 'enigmatic', 'epic', 'erotic', 'positive', 'sad', 'scary', 'wild')")
-        return value
-
-    @validator('primary_sound_character')
-    def primary_sound_character_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in ('brassy', 'bright', 'clear', 'deep', 'distorted', 'flat', 'full', 'groovy', 'melodious', 'natural', 'resonant', 'shrill', 'steady', 'thin', 'warm'):
-            raise ValueError("must be one of enum values ('brassy', 'bright', 'clear', 'deep', 'distorted', 'flat', 'full', 'groovy', 'melodious', 'natural', 'resonant', 'shrill', 'steady', 'thin', 'warm')")
-        return value
-
     @validator('key')
     def key_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
         if value not in ('C', 'C#', 'D', 'D#', 'E', 'F', 'F#', 'G', 'G#', 'A', 'A#', 'B', 'unclear'):
@@ -566,29 +566,38 @@
             return None
 
         if not isinstance(obj, dict):
             return MusicalFeaturesDTO.parse_obj(obj)
 
         _obj = MusicalFeaturesDTO.parse_obj({
             "space": obj.get("space"),
-            "language_of_performance": obj.get("languageOfPerformance"),
+            "energy": obj.get("energy"),
+            "engagement": obj.get("engagement"),
+            "groovyness": obj.get("groovyness"),
+            "harmony": obj.get("harmony"),
+            "pleasantness": obj.get("pleasantness"),
+            "primary_mood_cluster": obj.get("primaryMoodCluster"),
+            "primary_sound_character": obj.get("primarySoundCharacter"),
             "rhythm": obj.get("rhythm"),
             "roughness": obj.get("roughness"),
             "scale": obj.get("scale"),
             "sound_generation": obj.get("soundGeneration"),
             "tempo": obj.get("tempo"),
             "texture": obj.get("texture"),
             "timbre": obj.get("timbre"),
             "tonality": obj.get("tonality"),
             "valence": obj.get("valence"),
             "vocals": obj.get("vocals"),
             "origin_decade": obj.get("originDecade"),
             "curateability": obj.get("curateability"),
             "use_case": obj.get("useCase"),
             "channel_suitability": obj.get("channelSuitability"),
+            "language_of_performance": obj.get("languageOfPerformance"),
+            "arousal": obj.get("arousal"),
+            "dominant_instrument": obj.get("dominantInstrument"),
             "primary_mood_cluster_affinity": obj.get("primaryMoodClusterAffinity"),
             "secondary_mood_cluster": obj.get("secondaryMoodCluster"),
             "secondary_mood_cluster_affinity": obj.get("secondaryMoodClusterAffinity"),
             "tertiary_mood_cluster": obj.get("tertiaryMoodCluster"),
             "tertiary_mood_cluster_affinity": obj.get("tertiaryMoodClusterAffinity"),
             "vocals_affinity": obj.get("vocalsAffinity"),
             "dominant_instrument_affinity": obj.get("dominantInstrumentAffinity"),
@@ -625,23 +634,14 @@
             "origin_decade_affinity": obj.get("originDecadeAffinity"),
             "language_of_performance_affinity": obj.get("languageOfPerformanceAffinity"),
             "curateability_affinity": obj.get("curateabilityAffinity"),
             "use_case_affinity": obj.get("useCaseAffinity"),
             "industry_suitability": obj.get("industrySuitability"),
             "industry_suitability_affinity": obj.get("industrySuitabilityAffinity"),
             "audience_region": obj.get("audienceRegion"),
-            "arousal": obj.get("arousal"),
-            "dominant_instrument": obj.get("dominantInstrument"),
-            "energy": obj.get("energy"),
-            "engagement": obj.get("engagement"),
-            "groovyness": obj.get("groovyness"),
-            "harmony": obj.get("harmony"),
-            "pleasantness": obj.get("pleasantness"),
-            "primary_mood_cluster": obj.get("primaryMoodCluster"),
-            "primary_sound_character": obj.get("primarySoundCharacter"),
             "valence_affinity": obj.get("valenceAffinity"),
             "arousal_affinity": obj.get("arousalAffinity"),
             "pleasantness_affinity": obj.get("pleasantnessAffinity"),
             "engagement_affinity": obj.get("engagementAffinity"),
             "energy_affinity": obj.get("energyAffinity"),
             "tempo_affinity": obj.get("tempoAffinity"),
             "scale_affinity": obj.get("scaleAffinity"),
@@ -653,7 +653,8 @@
             "space_affinity": obj.get("spaceAffinity"),
             "key_affinity": obj.get("keyAffinity"),
             "channel_suitability_affinity": obj.get("channelSuitabilityAffinity"),
             "key": obj.get("key")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/p_line_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/p_line_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -67,7 +67,8 @@
 
         _obj = PLineDTO.parse_obj({
             "year": obj.get("year"),
             "text": obj.get("text")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/party_large_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/party_large_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -79,7 +79,8 @@
             "death_year": obj.get("deathYear"),
             "birth_place": obj.get("birthPlace"),
             "musicbrainz_type": obj.get("musicbrainzType"),
             "area": obj.get("area")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/party_small_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/party_small_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -67,7 +67,8 @@
 
         _obj = PartySmallDTO.parse_obj({
             "id": obj.get("id"),
             "full_name": obj.get("fullName")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/playlist_large_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/playlist_large_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -26,24 +26,24 @@
 
 class PlaylistLargeDTO(BaseModel):
     """
     Details on a playlist
     """
     name: StrictStr = Field(...)
     state: Optional[StrictStr] = None
+    usages: Optional[conlist(UsageDTO)] = None
     description: Optional[StrictStr] = None
     songtradr_playlist_guid: Optional[StrictStr] = Field(None, alias="songtradrPlaylistGuid")
+    tracks: Optional[conlist(RecordingPlaylistDTO)] = None
     asset_url: Optional[StrictStr] = Field(None, alias="assetURL")
     pretzel_tier: Optional[StrictStr] = Field(None, alias="pretzelTier")
     usage: Optional[StrictStr] = None
-    tracks: Optional[conlist(RecordingPlaylistDTO)] = None
-    usages: Optional[conlist(UsageDTO)] = None
     created: Optional[datetime] = None
     updated: Optional[datetime] = None
-    __properties = ["name", "state", "description", "songtradrPlaylistGuid", "assetURL", "pretzelTier", "usage", "tracks", "usages", "created", "updated"]
+    __properties = ["name", "state", "usages", "description", "songtradrPlaylistGuid", "tracks", "assetURL", "pretzelTier", "usage", "created", "updated"]
 
     @validator('state')
     def state_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
@@ -71,47 +71,48 @@
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in tracks (list)
-        _items = []
-        if self.tracks:
-            for _item in self.tracks:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['tracks'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in usages (list)
         _items = []
         if self.usages:
             for _item in self.usages:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['usages'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in tracks (list)
+        _items = []
+        if self.tracks:
+            for _item in self.tracks:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tracks'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> PlaylistLargeDTO:
         """Create an instance of PlaylistLargeDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return PlaylistLargeDTO.parse_obj(obj)
 
         _obj = PlaylistLargeDTO.parse_obj({
             "name": obj.get("name"),
             "state": obj.get("state"),
+            "usages": [UsageDTO.from_dict(_item) for _item in obj.get("usages")] if obj.get("usages") is not None else None,
             "description": obj.get("description"),
             "songtradr_playlist_guid": obj.get("songtradrPlaylistGuid"),
+            "tracks": [RecordingPlaylistDTO.from_dict(_item) for _item in obj.get("tracks")] if obj.get("tracks") is not None else None,
             "asset_url": obj.get("assetURL"),
             "pretzel_tier": obj.get("pretzelTier"),
             "usage": obj.get("usage"),
-            "tracks": [RecordingPlaylistDTO.from_dict(_item) for _item in obj.get("tracks")] if obj.get("tracks") is not None else None,
-            "usages": [UsageDTO.from_dict(_item) for _item in obj.get("usages")] if obj.get("usages") is not None else None,
             "created": obj.get("created"),
             "updated": obj.get("updated")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/product_medium_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/product_medium_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -32,18 +32,18 @@
     """
     duration: Optional[datetime] = None
     genres: Optional[conlist(GenreMinimalDTO, unique_items=True)] = None
     titles: Optional[conlist(TitleDTO, unique_items=True)] = None
     gtin: Optional[StrictStr] = None
     grid: Optional[StrictStr] = None
     release_date: Optional[datetime] = Field(None, alias="releaseDate")
-    takedown_date: Optional[datetime] = Field(None, alias="takedownDate")
     pline: Optional[PLineDTO] = None
+    takedown_date: Optional[datetime] = Field(None, alias="takedownDate")
     parties: Optional[conlist(ProductPartyDTO, unique_items=True)] = None
-    __properties = ["duration", "genres", "titles", "gtin", "grid", "releaseDate", "takedownDate", "pline", "parties"]
+    __properties = ["duration", "genres", "titles", "gtin", "grid", "releaseDate", "pline", "takedownDate", "parties"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -103,13 +103,14 @@
         _obj = ProductMediumDTO.parse_obj({
             "duration": obj.get("duration"),
             "genres": [GenreMinimalDTO.from_dict(_item) for _item in obj.get("genres")] if obj.get("genres") is not None else None,
             "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
             "gtin": obj.get("gtin"),
             "grid": obj.get("grid"),
             "release_date": obj.get("releaseDate"),
-            "takedown_date": obj.get("takedownDate"),
             "pline": PLineDTO.from_dict(obj.get("pline")) if obj.get("pline") is not None else None,
+            "takedown_date": obj.get("takedownDate"),
             "parties": [ProductPartyDTO.from_dict(_item) for _item in obj.get("parties")] if obj.get("parties") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/product_party_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/product_party_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -79,7 +79,8 @@
 
         _obj = ProductPartyDTO.parse_obj({
             "party": PartySmallDTO.from_dict(obj.get("party")) if obj.get("party") is not None else None,
             "contributor_types": [ContributorTypeDTO.from_dict(_item) for _item in obj.get("contributorTypes")] if obj.get("contributorTypes") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_for_similarity_search_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_for_similarity_search_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -71,7 +71,8 @@
 
         _obj = RecordingForSimilaritySearchDTO.parse_obj({
             "recording": RecordingSmallDTO.from_dict(obj.get("recording")) if obj.get("recording") is not None else None,
             "score": obj.get("score")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_genre_prediction_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_genre_prediction_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,7 +73,8 @@
         _obj = RecordingGenrePredictionDTO.parse_obj({
             "genre_type": obj.get("genreType"),
             "genre": GenreMinimalDTO.from_dict(obj.get("genre")) if obj.get("genre") is not None else None,
             "probability": obj.get("probability")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_large_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_large_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -31,26 +31,26 @@
 from songtradr_api_client_python.models.track_to_medium_product_dto import TrackToMediumProductDTO
 
 class RecordingLargeDTO(BaseModel):
     """
     Recording with a large field set.
     """
     duration: Optional[StrictInt] = None
+    isrc: StrictStr = Field(...)
     parties: Optional[conlist(RecordingPartyDTO, unique_items=True)] = None
     genres: Optional[conlist(GenreDTO, unique_items=True)] = None
     language_of_performance: Optional[StrictStr] = Field(None, alias="languageOfPerformance")
-    isrc: StrictStr = Field(...)
-    tags: Optional[conlist(RecordingTagSmallDTO)] = None
     titles: Optional[conlist(TitleDTO, unique_items=True)] = None
     tracks: Optional[conlist(TrackToMediumProductDTO, unique_items=True)] = None
     musical_features: Optional[MusicalFeaturesDTO] = Field(None, alias="musicalFeatures")
-    pline: Optional[PLineDTO] = None
+    tags: Optional[conlist(RecordingTagSmallDTO)] = None
     spotify_id: Optional[StrictStr] = Field(None, alias="spotifyId")
+    pline: Optional[PLineDTO] = None
     genre_predictions: Optional[conlist(RecordingGenrePredictionDTO, unique_items=True)] = Field(None, alias="genrePredictions")
-    __properties = ["duration", "parties", "genres", "languageOfPerformance", "isrc", "tags", "titles", "tracks", "musicalFeatures", "pline", "spotifyId", "genrePredictions"]
+    __properties = ["duration", "isrc", "parties", "genres", "languageOfPerformance", "titles", "tracks", "musicalFeatures", "tags", "spotifyId", "pline", "genrePredictions"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -82,21 +82,14 @@
         # override the default output from pydantic by calling `to_dict()` of each item in genres (list)
         _items = []
         if self.genres:
             for _item in self.genres:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['genres'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
-        _items = []
-        if self.tags:
-            for _item in self.tags:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['tags'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
         _items = []
         if self.titles:
             for _item in self.titles:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['titles'] = _items
@@ -106,14 +99,21 @@
             for _item in self.tracks:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['tracks'] = _items
         # override the default output from pydantic by calling `to_dict()` of musical_features
         if self.musical_features:
             _dict['musicalFeatures'] = self.musical_features.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
+        _items = []
+        if self.tags:
+            for _item in self.tags:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tags'] = _items
         # override the default output from pydantic by calling `to_dict()` of pline
         if self.pline:
             _dict['pline'] = self.pline.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in genre_predictions (list)
         _items = []
         if self.genre_predictions:
             for _item in self.genre_predictions:
@@ -129,21 +129,22 @@
             return None
 
         if not isinstance(obj, dict):
             return RecordingLargeDTO.parse_obj(obj)
 
         _obj = RecordingLargeDTO.parse_obj({
             "duration": obj.get("duration"),
+            "isrc": obj.get("isrc"),
             "parties": [RecordingPartyDTO.from_dict(_item) for _item in obj.get("parties")] if obj.get("parties") is not None else None,
             "genres": [GenreDTO.from_dict(_item) for _item in obj.get("genres")] if obj.get("genres") is not None else None,
             "language_of_performance": obj.get("languageOfPerformance"),
-            "isrc": obj.get("isrc"),
-            "tags": [RecordingTagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None,
             "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
             "tracks": [TrackToMediumProductDTO.from_dict(_item) for _item in obj.get("tracks")] if obj.get("tracks") is not None else None,
             "musical_features": MusicalFeaturesDTO.from_dict(obj.get("musicalFeatures")) if obj.get("musicalFeatures") is not None else None,
-            "pline": PLineDTO.from_dict(obj.get("pline")) if obj.get("pline") is not None else None,
+            "tags": [RecordingTagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None,
             "spotify_id": obj.get("spotifyId"),
+            "pline": PLineDTO.from_dict(obj.get("pline")) if obj.get("pline") is not None else None,
             "genre_predictions": [RecordingGenrePredictionDTO.from_dict(_item) for _item in obj.get("genrePredictions")] if obj.get("genrePredictions") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_list_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_list_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -79,7 +79,8 @@
             "recordings": [RecordingMediumDTO.from_dict(_item) for _item in obj.get("recordings")] if obj.get("recordings") is not None else None,
             "has_next_page": obj.get("hasNextPage"),
             "current_page_number": obj.get("currentPageNumber"),
             "total_results": obj.get("totalResults")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_medium_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_medium_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -28,25 +28,25 @@
 from songtradr_api_client_python.models.recording_tag_small_dto import RecordingTagSmallDTO
 from songtradr_api_client_python.models.title_dto import TitleDTO
 
 class RecordingMediumDTO(BaseModel):
     """
     Recording with a mid-sized field set.
     """
+    isrc: StrictStr = Field(...)
     recording_party_entities: Optional[conlist(RecordingPartyDTO, unique_items=True)] = Field(None, alias="recordingPartyEntities")
     genres: Optional[conlist(GenreDTO, unique_items=True)] = None
     language_of_performance: Optional[StrictStr] = Field(None, alias="languageOfPerformance")
     release_date: Optional[datetime] = Field(None, alias="releaseDate")
-    isrc: StrictStr = Field(...)
-    tags: Optional[conlist(RecordingTagSmallDTO)] = None
     titles: Optional[conlist(TitleDTO, unique_items=True)] = None
     musical_features: Optional[MusicalFeaturesDTO] = Field(None, alias="musicalFeatures")
+    tags: Optional[conlist(RecordingTagSmallDTO)] = None
     spotify_id: Optional[StrictStr] = Field(None, alias="spotifyId")
     genre_predictions: Optional[conlist(RecordingGenrePredictionDTO, unique_items=True)] = Field(None, alias="genrePredictions")
-    __properties = ["recordingPartyEntities", "genres", "languageOfPerformance", "releaseDate", "isrc", "tags", "titles", "musicalFeatures", "spotifyId", "genrePredictions"]
+    __properties = ["isrc", "recordingPartyEntities", "genres", "languageOfPerformance", "releaseDate", "titles", "musicalFeatures", "tags", "spotifyId", "genrePredictions"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -78,31 +78,31 @@
         # override the default output from pydantic by calling `to_dict()` of each item in genres (list)
         _items = []
         if self.genres:
             for _item in self.genres:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['genres'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
-        _items = []
-        if self.tags:
-            for _item in self.tags:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['tags'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
         _items = []
         if self.titles:
             for _item in self.titles:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['titles'] = _items
         # override the default output from pydantic by calling `to_dict()` of musical_features
         if self.musical_features:
             _dict['musicalFeatures'] = self.musical_features.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
+        _items = []
+        if self.tags:
+            for _item in self.tags:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tags'] = _items
         # override the default output from pydantic by calling `to_dict()` of each item in genre_predictions (list)
         _items = []
         if self.genre_predictions:
             for _item in self.genre_predictions:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['genrePredictions'] = _items
@@ -114,20 +114,21 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return RecordingMediumDTO.parse_obj(obj)
 
         _obj = RecordingMediumDTO.parse_obj({
+            "isrc": obj.get("isrc"),
             "recording_party_entities": [RecordingPartyDTO.from_dict(_item) for _item in obj.get("recordingPartyEntities")] if obj.get("recordingPartyEntities") is not None else None,
             "genres": [GenreDTO.from_dict(_item) for _item in obj.get("genres")] if obj.get("genres") is not None else None,
             "language_of_performance": obj.get("languageOfPerformance"),
             "release_date": obj.get("releaseDate"),
-            "isrc": obj.get("isrc"),
-            "tags": [RecordingTagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None,
             "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
             "musical_features": MusicalFeaturesDTO.from_dict(obj.get("musicalFeatures")) if obj.get("musicalFeatures") is not None else None,
+            "tags": [RecordingTagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None,
             "spotify_id": obj.get("spotifyId"),
             "genre_predictions": [RecordingGenrePredictionDTO.from_dict(_item) for _item in obj.get("genrePredictions")] if obj.get("genrePredictions") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -75,7 +75,8 @@
 
         _obj = RecordingMinimalWithMusicalFeaturesDTO.parse_obj({
             "isrc": obj.get("isrc"),
             "musical_features": [MusicalFeaturesDTO.from_dict(_item) for _item in obj.get("musicalFeatures")] if obj.get("musicalFeatures") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -77,7 +77,8 @@
         _obj = RecordingMinimalWithTaggramsDTO.parse_obj({
             "isrc": obj.get("isrc"),
             "timestamps": obj.get("timestamps"),
             "taggrams": [TaggramDTO.from_dict(_item) for _item in obj.get("taggrams")] if obj.get("taggrams") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -75,7 +75,8 @@
 
         _obj = RecordingMinimalWithTagstrengthsDTO.parse_obj({
             "isrc": obj.get("isrc"),
             "tagstrengths": [TagstrengthDTO.from_dict(_item) for _item in obj.get("tagstrengths")] if obj.get("tagstrengths") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_party_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_party_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -79,7 +79,8 @@
 
         _obj = RecordingPartyDTO.parse_obj({
             "party": PartySmallDTO.from_dict(obj.get("party")) if obj.get("party") is not None else None,
             "contributor_types": [ContributorTypeDTO.from_dict(_item) for _item in obj.get("contributorTypes")] if obj.get("contributorTypes") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_playlist_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_playlist_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -24,18 +24,18 @@
 from songtradr_api_client_python.models.recording_medium_dto import RecordingMediumDTO
 
 class RecordingPlaylistDTO(BaseModel):
     """
     Recording Playlist connection
     """
     recording: Optional[RecordingMediumDTO] = None
-    songtradr_track_guid: Optional[StrictStr] = Field(None, alias="songtradrTrackGuid")
     assigned_by_id: Optional[StrictInt] = Field(None, alias="assignedById")
     sequence: Optional[StrictInt] = None
-    __properties = ["recording", "songtradrTrackGuid", "assignedById", "sequence"]
+    songtradr_track_guid: Optional[StrictStr] = Field(None, alias="songtradrTrackGuid")
+    __properties = ["recording", "assignedById", "sequence", "songtradrTrackGuid"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -69,13 +69,14 @@
             return None
 
         if not isinstance(obj, dict):
             return RecordingPlaylistDTO.parse_obj(obj)
 
         _obj = RecordingPlaylistDTO.parse_obj({
             "recording": RecordingMediumDTO.from_dict(obj.get("recording")) if obj.get("recording") is not None else None,
-            "songtradr_track_guid": obj.get("songtradrTrackGuid"),
             "assigned_by_id": obj.get("assignedById"),
-            "sequence": obj.get("sequence")
+            "sequence": obj.get("sequence"),
+            "songtradr_track_guid": obj.get("songtradrTrackGuid")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_small_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -25,18 +25,18 @@
 from songtradr_api_client_python.models.title_dto import TitleDTO
 
 class RecordingSmallDTO(BaseModel):
     """
     Recording with a small field set.
     """
     duration: Optional[StrictInt] = None
-    parties: Optional[conlist(RecordingPartyDTO, unique_items=True)] = None
     isrc: StrictStr = Field(...)
+    parties: Optional[conlist(RecordingPartyDTO, unique_items=True)] = None
     titles: Optional[conlist(TitleDTO, unique_items=True)] = None
-    __properties = ["duration", "parties", "isrc", "titles"]
+    __properties = ["duration", "isrc", "parties", "titles"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -81,13 +81,14 @@
             return None
 
         if not isinstance(obj, dict):
             return RecordingSmallDTO.parse_obj(obj)
 
         _obj = RecordingSmallDTO.parse_obj({
             "duration": obj.get("duration"),
-            "parties": [RecordingPartyDTO.from_dict(_item) for _item in obj.get("parties")] if obj.get("parties") is not None else None,
             "isrc": obj.get("isrc"),
+            "parties": [RecordingPartyDTO.from_dict(_item) for _item in obj.get("parties")] if obj.get("parties") is not None else None,
             "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/recording_tag_small_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/recording_tag_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -69,7 +69,8 @@
             return RecordingTagSmallDTO.parse_obj(obj)
 
         _obj = RecordingTagSmallDTO.parse_obj({
             "tag": TagDTO.from_dict(obj.get("tag")) if obj.get("tag") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_file_recording_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_file_recording_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -791,7 +791,8 @@
             "iswc": obj.get("iswc"),
             "proprietary_id_gema": obj.get("proprietaryIdGema"),
             "title": obj.get("title"),
             "version_title": obj.get("versionTitle")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_playlist_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_playlist_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -96,7 +96,8 @@
             "pretzel_tier": obj.get("pretzelTier"),
             "usage": obj.get("usage"),
             "usages": obj.get("usages"),
             "recordings": [SaveRecordingPlaylistDTO.from_dict(_item) for _item in obj.get("recordings")] if obj.get("recordings") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_recording_genre_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_recording_genre_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -69,7 +69,8 @@
         _obj = SaveRecordingGenreDTO.parse_obj({
             "genre_name": obj.get("genreName"),
             "genre_type": obj.get("genreType"),
             "affinity": obj.get("affinity")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_recording_party_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_recording_party_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -74,7 +74,8 @@
 
         _obj = SaveRecordingPartyDTO.parse_obj({
             "full_name": obj.get("fullName"),
             "contributor_type": obj.get("contributorType")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_recording_playlist_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_recording_playlist_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -69,7 +69,8 @@
         _obj = SaveRecordingPlaylistDTO.parse_obj({
             "songtradr_track_guid": obj.get("songtradrTrackGuid"),
             "assigned_by_id": obj.get("assignedById"),
             "sequence": obj.get("sequence")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_recording_tag_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_recording_tag_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -67,7 +67,8 @@
 
         _obj = SaveRecordingTagDTO.parse_obj({
             "tag_name": obj.get("tagName"),
             "affinity": obj.get("affinity")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_referrer_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_referrer_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -67,7 +67,8 @@
 
         _obj = SaveReferrerDTO.parse_obj({
             "username": obj.get("username"),
             "url": obj.get("url")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_taggrams_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_taggrams_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -417,7 +417,8 @@
             "curateability": obj.get("curateability"),
             "use_case": obj.get("useCase"),
             "social_media": obj.get("socialMedia"),
             "industry_suitability": obj.get("industrySuitability")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/save_user_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/save_user_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -95,7 +95,8 @@
             "password": obj.get("password"),
             "full_name": obj.get("fullName"),
             "company_name": obj.get("companyName"),
             "language": obj.get("language")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/search_filter_values_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/search_filter_values_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -145,7 +145,8 @@
             "language_of_performance": obj.get("languageOfPerformance"),
             "curateability": obj.get("curateability"),
             "use_case": obj.get("useCase"),
             "channel_suitability": obj.get("channelSuitability")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/search_recording_granular_abstraction_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/search_recording_granular_abstraction_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -74,7 +74,8 @@
 
         _obj = SearchRecordingGranularAbstractionDTO.parse_obj({
             "strength": obj.get("strength"),
             "abstraction_name": obj.get("abstractionName")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/search_recording_granular_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/search_recording_granular_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -67,7 +67,8 @@
 
         _obj = SearchRecordingGranularDTO.parse_obj({
             "strength": obj.get("strength"),
             "tag_name": obj.get("tagName")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/sign_up_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/sign_up_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -71,7 +71,8 @@
             "email_address": obj.get("emailAddress"),
             "password": obj.get("password"),
             "full_name": obj.get("fullName"),
             "company_name": obj.get("companyName")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/tag_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/tag_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -77,7 +77,8 @@
         _obj = TagDTO.parse_obj({
             "id": obj.get("id"),
             "name": obj.get("name"),
             "categories": [CategoryMinimalDTO.from_dict(_item) for _item in obj.get("categories")] if obj.get("categories") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/tag_small_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/tag_small_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -67,7 +67,8 @@
 
         _obj = TagSmallDTO.parse_obj({
             "id": obj.get("id"),
             "name": obj.get("name")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/taggram_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/taggram_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,7 +73,8 @@
             "category_name": obj.get("categoryName"),
             "tag_name": obj.get("tagName"),
             "genre_name": obj.get("genreName"),
             "scale": obj.get("scale")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/tags_summary_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/tags_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -77,7 +77,8 @@
         _obj = TagsSummaryDTO.parse_obj({
             "name": obj.get("name"),
             "categories": [CategoryMinimalDTO.from_dict(_item) for _item in obj.get("categories")] if obj.get("categories") is not None else None,
             "total": obj.get("total")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/tagstrength_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/tagstrength_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,7 +73,8 @@
             "category_name": obj.get("categoryName"),
             "tag_name": obj.get("tagName"),
             "genre_name": obj.get("genreName"),
             "scale": obj.get("scale")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/title_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/title_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -65,7 +65,8 @@
             return TitleDTO.parse_obj(obj)
 
         _obj = TitleDTO.parse_obj({
             "title_text": obj.get("titleText")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/token_request.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -65,7 +65,8 @@
             return TokenRequest.parse_obj(obj)
 
         _obj = TokenRequest.parse_obj({
             "refresh_token": obj.get("refreshToken")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/track_to_medium_product_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/track_to_medium_product_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,7 +73,8 @@
         _obj = TrackToMediumProductDTO.parse_obj({
             "track_no": obj.get("trackNo"),
             "set_no": obj.get("setNo"),
             "product": ProductMediumDTO.from_dict(obj.get("product")) if obj.get("product") is not None else None
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/update_password_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/update_password_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -67,7 +67,8 @@
 
         _obj = UpdatePasswordDTO.parse_obj({
             "token": obj.get("token"),
             "password": obj.get("password")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/usage_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/usage_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -65,7 +65,8 @@
             return UsageDTO.parse_obj(obj)
 
         _obj = UsageDTO.parse_obj({
             "name": obj.get("name")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/models/user_dto.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/models/user_dto.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -39,19 +39,28 @@
     signup_allowed: StrictBool = Field(..., alias="signupAllowed")
     upload_allowed: StrictBool = Field(..., alias="uploadAllowed")
     fingerprint_allowed: StrictBool = Field(..., alias="fingerprintAllowed")
     audiotagging_allowed: StrictBool = Field(..., alias="audiotaggingAllowed")
     b2b_allowed: StrictBool = Field(..., alias="b2bAllowed")
     editor_allowed: StrictBool = Field(..., alias="editorAllowed")
     insights_allowed: StrictBool = Field(..., alias="insightsAllowed")
+    genres_allowed: StrictBool = Field(..., alias="genresAllowed")
+    moods_allowed: StrictBool = Field(..., alias="moodsAllowed")
+    instrumentation_allowed: StrictBool = Field(..., alias="instrumentationAllowed")
+    sound_features_allowed: StrictBool = Field(..., alias="soundFeaturesAllowed")
+    tonal_features_allowed: StrictBool = Field(..., alias="tonalFeaturesAllowed")
+    rhythm_features_allowed: StrictBool = Field(..., alias="rhythmFeaturesAllowed")
+    audience_allowed: StrictBool = Field(..., alias="audienceAllowed")
+    origin_allowed: StrictBool = Field(..., alias="originAllowed")
+    quality_allowed: StrictBool = Field(..., alias="qualityAllowed")
     reduced_musical_features: StrictBool = Field(..., alias="reducedMusicalFeatures")
     confirmed: StrictBool = Field(...)
     language: StrictStr = Field(...)
     admin: Optional[StrictBool] = None
-    __properties = ["username", "emailAddress", "companyName", "isAdmin", "fullSearchAllowed", "voiceSearchAllowed", "recordingDetailAllowed", "artistDetailAllowed", "playlistPredictionAllowed", "widgetsAllowed", "signupAllowed", "uploadAllowed", "fingerprintAllowed", "audiotaggingAllowed", "b2bAllowed", "editorAllowed", "insightsAllowed", "reducedMusicalFeatures", "confirmed", "language", "admin"]
+    __properties = ["username", "emailAddress", "companyName", "isAdmin", "fullSearchAllowed", "voiceSearchAllowed", "recordingDetailAllowed", "artistDetailAllowed", "playlistPredictionAllowed", "widgetsAllowed", "signupAllowed", "uploadAllowed", "fingerprintAllowed", "audiotaggingAllowed", "b2bAllowed", "editorAllowed", "insightsAllowed", "genresAllowed", "moodsAllowed", "instrumentationAllowed", "soundFeaturesAllowed", "tonalFeaturesAllowed", "rhythmFeaturesAllowed", "audienceAllowed", "originAllowed", "qualityAllowed", "reducedMusicalFeatures", "confirmed", "language", "admin"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -98,14 +107,24 @@
             "signup_allowed": obj.get("signupAllowed"),
             "upload_allowed": obj.get("uploadAllowed"),
             "fingerprint_allowed": obj.get("fingerprintAllowed"),
             "audiotagging_allowed": obj.get("audiotaggingAllowed"),
             "b2b_allowed": obj.get("b2bAllowed"),
             "editor_allowed": obj.get("editorAllowed"),
             "insights_allowed": obj.get("insightsAllowed"),
+            "genres_allowed": obj.get("genresAllowed"),
+            "moods_allowed": obj.get("moodsAllowed"),
+            "instrumentation_allowed": obj.get("instrumentationAllowed"),
+            "sound_features_allowed": obj.get("soundFeaturesAllowed"),
+            "tonal_features_allowed": obj.get("tonalFeaturesAllowed"),
+            "rhythm_features_allowed": obj.get("rhythmFeaturesAllowed"),
+            "audience_allowed": obj.get("audienceAllowed"),
+            "origin_allowed": obj.get("originAllowed"),
+            "quality_allowed": obj.get("qualityAllowed"),
             "reduced_musical_features": obj.get("reducedMusicalFeatures"),
             "confirmed": obj.get("confirmed"),
             "language": obj.get("language"),
             "admin": obj.get("admin")
         })
         return _obj
 
+
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python/rest.py` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python.egg-info/PKG-INFO` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songtradr-api-client-python
-Version: 1.12.23
+Version: 1.12.24
 Summary: Songtradr API
 Home-page: https://github.com/songtradr/songtradr-python-api-client-docs
 Author: Songtradr Inc.
 Author-email: info@songtradr.com
 Keywords: OpenAPI,OpenAPI-Generator,Songtradr API
 Description-Content-Type: text/markdown
```

### Comparing `songtradr-api-client-python-1.12.23/songtradr_api_client_python.egg-info/SOURCES.txt` & `songtradr-api-client-python-1.12.24/songtradr_api_client_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `songtradr-api-client-python-1.12.23/test/test_admin_api_user_dto.py` & `songtradr-api-client-python-1.12.24/test/test_admin_api_user_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_allowed_values_api.py` & `songtradr-api-client-python-1.12.24/test/test_allowed_values_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_api_key_dto.py` & `songtradr-api-client-python-1.12.24/test/test_api_key_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,16 +36,16 @@
             optional params are included """
         # uncomment below to create an instance of `ApiKeyDTO`
         """
         model = songtradr_api_client_python.models.api_key_dto.ApiKeyDTO()  # noqa: E501
         if include_optional :
             return ApiKeyDTO(
                 name = '', 
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 last_used_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 id = ''
             )
         else :
             return ApiKeyDTO(
                 name = '',
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 id = '',
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_api_keys_api.py` & `songtradr-api-client-python-1.12.24/test/test_api_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_category_medium_dto.py` & `songtradr-api-client-python-1.12.24/test/test_category_medium_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_category_minimal_dto.py` & `songtradr-api-client-python-1.12.24/test/test_category_minimal_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_config_access_dto.py` & `songtradr-api-client-python-1.12.24/test/test_config_access_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_config_identifier_dto.py` & `songtradr-api-client-python-1.12.24/test/test_config_identifier_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_contributor_type_dto.py` & `songtradr-api-client-python-1.12.24/test/test_contributor_type_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_create_api_key_dto.py` & `songtradr-api-client-python-1.12.24/test/test_create_api_key_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_error_response.py` & `songtradr-api-client-python-1.12.24/test/test_error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_field_summary_dto.py` & `songtradr-api-client-python-1.12.24/test/test_field_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_file_dto.py` & `songtradr-api-client-python-1.12.24/test/test_file_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -50,14 +50,15 @@
                 fingerprint_status = 'processing', 
                 fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 inference_status = 'processing', 
                 inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
+                    isrc = '', 
                     recording_party_entities = [
                         songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                             party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                 id = '', 
                                 full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -67,46 +68,44 @@
                     genres = [
                         songtradr_api_client_python.models.genre_dto.GenreDTO(
                             id = 56, 
                             name = '', )
                         ], 
                     language_of_performance = '', 
                     release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    isrc = '', 
-                    tags = [
-                        songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                            tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                id = 56, 
-                                name = '', 
-                                categories = [
-                                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                        category_name = '', )
-                                    ], ), )
-                        ], 
                     titles = [
                         songtradr_api_client_python.models.title_dto.TitleDTO(
                             title_text = '', )
                         ], 
                     musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                         space = 'very compact', 
-                        language_of_performance = 'en', 
+                        energy = 'very quiet', 
+                        engagement = 'very unengaging', 
+                        groovyness = 'very steady', 
+                        harmony = 'very dissonant', 
+                        pleasantness = 'very unpleasant', 
+                        primary_mood_cluster = 'aggressive', 
+                        primary_sound_character = 'brassy', 
                         rhythm = 'common time', 
                         roughness = 'very clear', 
                         scale = 'major key', 
                         sound_generation = 'acoustic', 
                         tempo = 'very slow', 
                         texture = 'very thin', 
                         timbre = 'very warm', 
                         tonality = 'monotonous', 
                         valence = 'very sad', 
                         vocals = 'instrumental', 
                         origin_decade = 'pre-1950s', 
                         curateability = 'curateable', 
                         use_case = 'background', 
                         channel_suitability = 'Spotify', 
+                        language_of_performance = 'en', 
+                        arousal = 'very calm', 
+                        dominant_instrument = 'electric guitar', 
                         primary_mood_cluster_affinity = 1.337, 
                         secondary_mood_cluster = 'aggressive', 
                         secondary_mood_cluster_affinity = 1.337, 
                         tertiary_mood_cluster = 'aggressive', 
                         tertiary_mood_cluster_affinity = 1.337, 
                         vocals_affinity = 1.337, 
                         dominant_instrument_affinity = 1.337, 
@@ -143,23 +142,14 @@
                         origin_decade_affinity = 1.337, 
                         language_of_performance_affinity = 1.337, 
                         curateability_affinity = 1.337, 
                         use_case_affinity = 1.337, 
                         industry_suitability = 'Automobiles and Parts', 
                         industry_suitability_affinity = 1.337, 
                         audience_region = 'Australia and New Zealand', 
-                        arousal = 'very calm', 
-                        dominant_instrument = 'electric guitar', 
-                        energy = 'very quiet', 
-                        engagement = 'very unengaging', 
-                        groovyness = 'very steady', 
-                        harmony = 'very dissonant', 
-                        pleasantness = 'very unpleasant', 
-                        primary_mood_cluster = 'aggressive', 
-                        primary_sound_character = 'brassy', 
                         valence_affinity = 1.337, 
                         arousal_affinity = 1.337, 
                         pleasantness_affinity = 1.337, 
                         engagement_affinity = 1.337, 
                         energy_affinity = 1.337, 
                         tempo_affinity = 1.337, 
                         scale_affinity = 1.337, 
@@ -168,14 +158,24 @@
                         harmony_affinity = 1.337, 
                         texture_affinity = 1.337, 
                         groovyness_affinity = 1.337, 
                         space_affinity = 1.337, 
                         key_affinity = 1.337, 
                         channel_suitability_affinity = 1.337, 
                         key = 'C', ), 
+                    tags = [
+                        songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                            tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                id = 56, 
+                                name = '', 
+                                categories = [
+                                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                        category_name = '', )
+                                    ], ), )
+                        ], 
                     spotify_id = '', 
                     genre_predictions = [
                         songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
                             genre_type = '', 
                             genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                                 genre_name = '', ), 
                             probability = 1.337, )
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_file_list_dto.py` & `songtradr-api-client-python-1.12.24/test/test_file_list_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -52,14 +52,15 @@
                         fingerprint_status = 'processing', 
                         fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_status = 'processing', 
                         inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
+                            isrc = '', 
                             recording_party_entities = [
                                 songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                                     party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                         id = '', 
                                         full_name = '', ), 
                                     contributor_types = [
                                         songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -69,46 +70,44 @@
                             genres = [
                                 songtradr_api_client_python.models.genre_dto.GenreDTO(
                                     id = 56, 
                                     name = '', )
                                 ], 
                             language_of_performance = '', 
                             release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            isrc = '', 
-                            tags = [
-                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                        id = 56, 
-                                        name = '', 
-                                        categories = [
-                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                                category_name = '', )
-                                            ], ), )
-                                ], 
                             titles = [
                                 songtradr_api_client_python.models.title_dto.TitleDTO(
                                     title_text = '', )
                                 ], 
                             musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                                 space = 'very compact', 
-                                language_of_performance = 'en', 
+                                energy = 'very quiet', 
+                                engagement = 'very unengaging', 
+                                groovyness = 'very steady', 
+                                harmony = 'very dissonant', 
+                                pleasantness = 'very unpleasant', 
+                                primary_mood_cluster = 'aggressive', 
+                                primary_sound_character = 'brassy', 
                                 rhythm = 'common time', 
                                 roughness = 'very clear', 
                                 scale = 'major key', 
                                 sound_generation = 'acoustic', 
                                 tempo = 'very slow', 
                                 texture = 'very thin', 
                                 timbre = 'very warm', 
                                 tonality = 'monotonous', 
                                 valence = 'very sad', 
                                 vocals = 'instrumental', 
                                 origin_decade = 'pre-1950s', 
                                 curateability = 'curateable', 
                                 use_case = 'background', 
                                 channel_suitability = 'Spotify', 
+                                language_of_performance = 'en', 
+                                arousal = 'very calm', 
+                                dominant_instrument = 'electric guitar', 
                                 primary_mood_cluster_affinity = 1.337, 
                                 secondary_mood_cluster = 'aggressive', 
                                 secondary_mood_cluster_affinity = 1.337, 
                                 tertiary_mood_cluster = 'aggressive', 
                                 tertiary_mood_cluster_affinity = 1.337, 
                                 vocals_affinity = 1.337, 
                                 dominant_instrument_affinity = 1.337, 
@@ -145,23 +144,14 @@
                                 origin_decade_affinity = 1.337, 
                                 language_of_performance_affinity = 1.337, 
                                 curateability_affinity = 1.337, 
                                 use_case_affinity = 1.337, 
                                 industry_suitability = 'Automobiles and Parts', 
                                 industry_suitability_affinity = 1.337, 
                                 audience_region = 'Australia and New Zealand', 
-                                arousal = 'very calm', 
-                                dominant_instrument = 'electric guitar', 
-                                energy = 'very quiet', 
-                                engagement = 'very unengaging', 
-                                groovyness = 'very steady', 
-                                harmony = 'very dissonant', 
-                                pleasantness = 'very unpleasant', 
-                                primary_mood_cluster = 'aggressive', 
-                                primary_sound_character = 'brassy', 
                                 valence_affinity = 1.337, 
                                 arousal_affinity = 1.337, 
                                 pleasantness_affinity = 1.337, 
                                 engagement_affinity = 1.337, 
                                 energy_affinity = 1.337, 
                                 tempo_affinity = 1.337, 
                                 scale_affinity = 1.337, 
@@ -170,14 +160,24 @@
                                 harmony_affinity = 1.337, 
                                 texture_affinity = 1.337, 
                                 groovyness_affinity = 1.337, 
                                 space_affinity = 1.337, 
                                 key_affinity = 1.337, 
                                 channel_suitability_affinity = 1.337, 
                                 key = 'C', ), 
+                            tags = [
+                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                        id = 56, 
+                                        name = '', 
+                                        categories = [
+                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                                category_name = '', )
+                                            ], ), )
+                                ], 
                             spotify_id = '', 
                             genre_predictions = [
                                 songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
                                     genre_type = '', 
                                     genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                                         genre_name = '', ), 
                                     probability = 1.337, )
@@ -204,14 +204,15 @@
                         fingerprint_status = 'processing', 
                         fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_status = 'processing', 
                         inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
+                            isrc = '', 
                             recording_party_entities = [
                                 songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                                     party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                         id = '', 
                                         full_name = '', ), 
                                     contributor_types = [
                                         songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -221,46 +222,44 @@
                             genres = [
                                 songtradr_api_client_python.models.genre_dto.GenreDTO(
                                     id = 56, 
                                     name = '', )
                                 ], 
                             language_of_performance = '', 
                             release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            isrc = '', 
-                            tags = [
-                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                        id = 56, 
-                                        name = '', 
-                                        categories = [
-                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                                category_name = '', )
-                                            ], ), )
-                                ], 
                             titles = [
                                 songtradr_api_client_python.models.title_dto.TitleDTO(
                                     title_text = '', )
                                 ], 
                             musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                                 space = 'very compact', 
-                                language_of_performance = 'en', 
+                                energy = 'very quiet', 
+                                engagement = 'very unengaging', 
+                                groovyness = 'very steady', 
+                                harmony = 'very dissonant', 
+                                pleasantness = 'very unpleasant', 
+                                primary_mood_cluster = 'aggressive', 
+                                primary_sound_character = 'brassy', 
                                 rhythm = 'common time', 
                                 roughness = 'very clear', 
                                 scale = 'major key', 
                                 sound_generation = 'acoustic', 
                                 tempo = 'very slow', 
                                 texture = 'very thin', 
                                 timbre = 'very warm', 
                                 tonality = 'monotonous', 
                                 valence = 'very sad', 
                                 vocals = 'instrumental', 
                                 origin_decade = 'pre-1950s', 
                                 curateability = 'curateable', 
                                 use_case = 'background', 
                                 channel_suitability = 'Spotify', 
+                                language_of_performance = 'en', 
+                                arousal = 'very calm', 
+                                dominant_instrument = 'electric guitar', 
                                 primary_mood_cluster_affinity = 1.337, 
                                 secondary_mood_cluster = 'aggressive', 
                                 secondary_mood_cluster_affinity = 1.337, 
                                 tertiary_mood_cluster = 'aggressive', 
                                 tertiary_mood_cluster_affinity = 1.337, 
                                 vocals_affinity = 1.337, 
                                 dominant_instrument_affinity = 1.337, 
@@ -297,23 +296,14 @@
                                 origin_decade_affinity = 1.337, 
                                 language_of_performance_affinity = 1.337, 
                                 curateability_affinity = 1.337, 
                                 use_case_affinity = 1.337, 
                                 industry_suitability = 'Automobiles and Parts', 
                                 industry_suitability_affinity = 1.337, 
                                 audience_region = 'Australia and New Zealand', 
-                                arousal = 'very calm', 
-                                dominant_instrument = 'electric guitar', 
-                                energy = 'very quiet', 
-                                engagement = 'very unengaging', 
-                                groovyness = 'very steady', 
-                                harmony = 'very dissonant', 
-                                pleasantness = 'very unpleasant', 
-                                primary_mood_cluster = 'aggressive', 
-                                primary_sound_character = 'brassy', 
                                 valence_affinity = 1.337, 
                                 arousal_affinity = 1.337, 
                                 pleasantness_affinity = 1.337, 
                                 engagement_affinity = 1.337, 
                                 energy_affinity = 1.337, 
                                 tempo_affinity = 1.337, 
                                 scale_affinity = 1.337, 
@@ -322,14 +312,24 @@
                                 harmony_affinity = 1.337, 
                                 texture_affinity = 1.337, 
                                 groovyness_affinity = 1.337, 
                                 space_affinity = 1.337, 
                                 key_affinity = 1.337, 
                                 channel_suitability_affinity = 1.337, 
                                 key = 'C', ), 
+                            tags = [
+                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                        id = 56, 
+                                        name = '', 
+                                        categories = [
+                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                                category_name = '', )
+                                            ], ), )
+                                ], 
                             spotify_id = '', 
                             genre_predictions = [
                                 songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
                                     genre_type = '', 
                                     genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                                         genre_name = '', ), 
                                     probability = 1.337, )
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_file_minimal_with_url_dto.py` & `songtradr-api-client-python-1.12.24/test/test_file_minimal_with_url_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_file_small_dto.py` & `songtradr-api-client-python-1.12.24/test/test_file_small_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -39,33 +39,33 @@
         model = songtradr_api_client_python.models.file_small_dto.FileSmallDTO()  # noqa: E501
         if include_optional :
             return FileSmallDTO(
                 name = '', 
                 id = 56, 
                 extension = 'mp3', 
                 error_message = '', 
-                folder = '', 
                 object_key = '', 
                 upload_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 upload_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 fingerprint_status = 'processing', 
                 fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 inference_status = 'processing', 
                 inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                error_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
+                error_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                folder = ''
             )
         else :
             return FileSmallDTO(
                 name = '',
                 id = 56,
                 extension = 'mp3',
-                folder = '',
                 object_key = '',
+                folder = '',
         )
         """
 
     def testFileSmallDTO(self):
         """Test FileSmallDTO"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_file_upload_dto.py` & `songtradr-api-client-python-1.12.24/test/test_file_upload_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_file_w_ith_url_dto.py` & `songtradr-api-client-python-1.12.24/test/test_file_w_ith_url_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -51,14 +51,15 @@
                     fingerprint_status = 'processing', 
                     fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_status = 'processing', 
                     inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
+                        isrc = '', 
                         recording_party_entities = [
                             songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                                 party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                     id = '', 
                                     full_name = '', ), 
                                 contributor_types = [
                                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -68,46 +69,44 @@
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        isrc = '', 
-                        tags = [
-                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                    id = 56, 
-                                    name = '', 
-                                    categories = [
-                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                            category_name = '', )
-                                        ], ), )
-                            ], 
                         titles = [
                             songtradr_api_client_python.models.title_dto.TitleDTO(
                                 title_text = '', )
                             ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            language_of_performance = 'en', 
+                            energy = 'very quiet', 
+                            engagement = 'very unengaging', 
+                            groovyness = 'very steady', 
+                            harmony = 'very dissonant', 
+                            pleasantness = 'very unpleasant', 
+                            primary_mood_cluster = 'aggressive', 
+                            primary_sound_character = 'brassy', 
                             rhythm = 'common time', 
                             roughness = 'very clear', 
                             scale = 'major key', 
                             sound_generation = 'acoustic', 
                             tempo = 'very slow', 
                             texture = 'very thin', 
                             timbre = 'very warm', 
                             tonality = 'monotonous', 
                             valence = 'very sad', 
                             vocals = 'instrumental', 
                             origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            language_of_performance = 'en', 
+                            arousal = 'very calm', 
+                            dominant_instrument = 'electric guitar', 
                             primary_mood_cluster_affinity = 1.337, 
                             secondary_mood_cluster = 'aggressive', 
                             secondary_mood_cluster_affinity = 1.337, 
                             tertiary_mood_cluster = 'aggressive', 
                             tertiary_mood_cluster_affinity = 1.337, 
                             vocals_affinity = 1.337, 
                             dominant_instrument_affinity = 1.337, 
@@ -144,23 +143,14 @@
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', 
-                            arousal = 'very calm', 
-                            dominant_instrument = 'electric guitar', 
-                            energy = 'very quiet', 
-                            engagement = 'very unengaging', 
-                            groovyness = 'very steady', 
-                            harmony = 'very dissonant', 
-                            pleasantness = 'very unpleasant', 
-                            primary_mood_cluster = 'aggressive', 
-                            primary_sound_character = 'brassy', 
                             valence_affinity = 1.337, 
                             arousal_affinity = 1.337, 
                             pleasantness_affinity = 1.337, 
                             engagement_affinity = 1.337, 
                             energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
@@ -169,14 +159,24 @@
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
                             key = 'C', ), 
+                        tags = [
+                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                    id = 56, 
+                                    name = '', 
+                                    categories = [
+                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                            category_name = '', )
+                                        ], ), )
+                            ], 
                         spotify_id = '', 
                         genre_predictions = [
                             songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
                                 genre_type = '', 
                                 genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                                     genre_name = '', ), 
                                 probability = 1.337, )
@@ -199,14 +199,15 @@
                     fingerprint_status = 'processing', 
                     fingerprint_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     fingerprint_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_status = 'processing', 
                     inference_start_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     inference_end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
+                        isrc = '', 
                         recording_party_entities = [
                             songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                                 party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                     id = '', 
                                     full_name = '', ), 
                                 contributor_types = [
                                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -216,46 +217,44 @@
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        isrc = '', 
-                        tags = [
-                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                    id = 56, 
-                                    name = '', 
-                                    categories = [
-                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                            category_name = '', )
-                                        ], ), )
-                            ], 
                         titles = [
                             songtradr_api_client_python.models.title_dto.TitleDTO(
                                 title_text = '', )
                             ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            language_of_performance = 'en', 
+                            energy = 'very quiet', 
+                            engagement = 'very unengaging', 
+                            groovyness = 'very steady', 
+                            harmony = 'very dissonant', 
+                            pleasantness = 'very unpleasant', 
+                            primary_mood_cluster = 'aggressive', 
+                            primary_sound_character = 'brassy', 
                             rhythm = 'common time', 
                             roughness = 'very clear', 
                             scale = 'major key', 
                             sound_generation = 'acoustic', 
                             tempo = 'very slow', 
                             texture = 'very thin', 
                             timbre = 'very warm', 
                             tonality = 'monotonous', 
                             valence = 'very sad', 
                             vocals = 'instrumental', 
                             origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            language_of_performance = 'en', 
+                            arousal = 'very calm', 
+                            dominant_instrument = 'electric guitar', 
                             primary_mood_cluster_affinity = 1.337, 
                             secondary_mood_cluster = 'aggressive', 
                             secondary_mood_cluster_affinity = 1.337, 
                             tertiary_mood_cluster = 'aggressive', 
                             tertiary_mood_cluster_affinity = 1.337, 
                             vocals_affinity = 1.337, 
                             dominant_instrument_affinity = 1.337, 
@@ -292,23 +291,14 @@
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', 
-                            arousal = 'very calm', 
-                            dominant_instrument = 'electric guitar', 
-                            energy = 'very quiet', 
-                            engagement = 'very unengaging', 
-                            groovyness = 'very steady', 
-                            harmony = 'very dissonant', 
-                            pleasantness = 'very unpleasant', 
-                            primary_mood_cluster = 'aggressive', 
-                            primary_sound_character = 'brassy', 
                             valence_affinity = 1.337, 
                             arousal_affinity = 1.337, 
                             pleasantness_affinity = 1.337, 
                             engagement_affinity = 1.337, 
                             energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
@@ -317,14 +307,24 @@
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
                             key = 'C', ), 
+                        tags = [
+                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                    id = 56, 
+                                    name = '', 
+                                    categories = [
+                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                            category_name = '', )
+                                        ], ), )
+                            ], 
                         spotify_id = '', 
                         genre_predictions = [
                             songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
                                 genre_type = '', 
                                 genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                                     genre_name = '', ), 
                                 probability = 1.337, )
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_files_summary_dto.py` & `songtradr-api-client-python-1.12.24/test/test_files_summary_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_forgot_password_dto.py` & `songtradr-api-client-python-1.12.24/test/test_forgot_password_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_genre_dto.py` & `songtradr-api-client-python-1.12.24/test/test_genre_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_genre_minimal_dto.py` & `songtradr-api-client-python-1.12.24/test/test_genre_minimal_dto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_genres_summary_dto.py` & `songtradr-api-client-python-1.12.24/test/test_genres_summary_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_init_put_recording_audio_dto.py` & `songtradr-api-client-python-1.12.24/test/test_init_put_recording_audio_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_jwt_token_dto.py` & `songtradr-api-client-python-1.12.24/test/test_jwt_token_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_login_dto.py` & `songtradr-api-client-python-1.12.24/test/test_login_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_musical_features_dto.py` & `songtradr-api-client-python-1.12.24/test/test_musical_features_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,29 +36,38 @@
             optional params are included """
         # uncomment below to create an instance of `MusicalFeaturesDTO`
         """
         model = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO()  # noqa: E501
         if include_optional :
             return MusicalFeaturesDTO(
                 space = 'very compact', 
-                language_of_performance = 'en', 
+                energy = 'very quiet', 
+                engagement = 'very unengaging', 
+                groovyness = 'very steady', 
+                harmony = 'very dissonant', 
+                pleasantness = 'very unpleasant', 
+                primary_mood_cluster = 'aggressive', 
+                primary_sound_character = 'brassy', 
                 rhythm = 'common time', 
                 roughness = 'very clear', 
                 scale = 'major key', 
                 sound_generation = 'acoustic', 
                 tempo = 'very slow', 
                 texture = 'very thin', 
                 timbre = 'very warm', 
                 tonality = 'monotonous', 
                 valence = 'very sad', 
                 vocals = 'instrumental', 
                 origin_decade = 'pre-1950s', 
                 curateability = 'curateable', 
                 use_case = 'background', 
                 channel_suitability = 'Spotify', 
+                language_of_performance = 'en', 
+                arousal = 'very calm', 
+                dominant_instrument = 'electric guitar', 
                 primary_mood_cluster_affinity = 1.337, 
                 secondary_mood_cluster = 'aggressive', 
                 secondary_mood_cluster_affinity = 1.337, 
                 tertiary_mood_cluster = 'aggressive', 
                 tertiary_mood_cluster_affinity = 1.337, 
                 vocals_affinity = 1.337, 
                 dominant_instrument_affinity = 1.337, 
@@ -95,23 +104,14 @@
                 origin_decade_affinity = 1.337, 
                 language_of_performance_affinity = 1.337, 
                 curateability_affinity = 1.337, 
                 use_case_affinity = 1.337, 
                 industry_suitability = 'Automobiles and Parts', 
                 industry_suitability_affinity = 1.337, 
                 audience_region = 'Australia and New Zealand', 
-                arousal = 'very calm', 
-                dominant_instrument = 'electric guitar', 
-                energy = 'very quiet', 
-                engagement = 'very unengaging', 
-                groovyness = 'very steady', 
-                harmony = 'very dissonant', 
-                pleasantness = 'very unpleasant', 
-                primary_mood_cluster = 'aggressive', 
-                primary_sound_character = 'brassy', 
                 valence_affinity = 1.337, 
                 arousal_affinity = 1.337, 
                 pleasantness_affinity = 1.337, 
                 engagement_affinity = 1.337, 
                 energy_affinity = 1.337, 
                 tempo_affinity = 1.337, 
                 scale_affinity = 1.337,
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_p_line_dto.py` & `songtradr-api-client-python-1.12.24/test/test_p_line_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_party_api.py` & `songtradr-api-client-python-1.12.24/test/test_party_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_party_large_dto.py` & `songtradr-api-client-python-1.12.24/test/test_party_large_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_party_small_dto.py` & `songtradr-api-client-python-1.12.24/test/test_party_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_playlist_api.py` & `songtradr-api-client-python-1.12.24/test/test_playlist_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_playlist_large_dto.py` & `songtradr-api-client-python-1.12.24/test/test_playlist_large_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -37,22 +37,24 @@
         # uncomment below to create an instance of `PlaylistLargeDTO`
         """
         model = songtradr_api_client_python.models.playlist_large_dto.PlaylistLargeDTO()  # noqa: E501
         if include_optional :
             return PlaylistLargeDTO(
                 name = '', 
                 state = 'active', 
+                usages = [
+                    songtradr_api_client_python.models.usage_dto.UsageDTO(
+                        name = '', )
+                    ], 
                 description = '', 
                 songtradr_playlist_guid = '', 
-                asset_url = '', 
-                pretzel_tier = '', 
-                usage = '', 
                 tracks = [
                     songtradr_api_client_python.models.recording_playlist_dto.RecordingPlaylistDTO(
                         recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
+                            isrc = '', 
                             recording_party_entities = [
                                 songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                                     party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                         id = '', 
                                         full_name = '', ), 
                                     contributor_types = [
                                         songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -62,46 +64,44 @@
                             genres = [
                                 songtradr_api_client_python.models.genre_dto.GenreDTO(
                                     id = 56, 
                                     name = '', )
                                 ], 
                             language_of_performance = '', 
                             release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            isrc = '', 
-                            tags = [
-                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                        id = 56, 
-                                        name = '', 
-                                        categories = [
-                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                                category_name = '', )
-                                            ], ), )
-                                ], 
                             titles = [
                                 songtradr_api_client_python.models.title_dto.TitleDTO(
                                     title_text = '', )
                                 ], 
                             musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                                 space = 'very compact', 
-                                language_of_performance = 'en', 
+                                energy = 'very quiet', 
+                                engagement = 'very unengaging', 
+                                groovyness = 'very steady', 
+                                harmony = 'very dissonant', 
+                                pleasantness = 'very unpleasant', 
+                                primary_mood_cluster = 'aggressive', 
+                                primary_sound_character = 'brassy', 
                                 rhythm = 'common time', 
                                 roughness = 'very clear', 
                                 scale = 'major key', 
                                 sound_generation = 'acoustic', 
                                 tempo = 'very slow', 
                                 texture = 'very thin', 
                                 timbre = 'very warm', 
                                 tonality = 'monotonous', 
                                 valence = 'very sad', 
                                 vocals = 'instrumental', 
                                 origin_decade = 'pre-1950s', 
                                 curateability = 'curateable', 
                                 use_case = 'background', 
                                 channel_suitability = 'Spotify', 
+                                language_of_performance = 'en', 
+                                arousal = 'very calm', 
+                                dominant_instrument = 'electric guitar', 
                                 primary_mood_cluster_affinity = 1.337, 
                                 secondary_mood_cluster = 'aggressive', 
                                 secondary_mood_cluster_affinity = 1.337, 
                                 tertiary_mood_cluster = 'aggressive', 
                                 tertiary_mood_cluster_affinity = 1.337, 
                                 vocals_affinity = 1.337, 
                                 dominant_instrument_affinity = 1.337, 
@@ -138,23 +138,14 @@
                                 origin_decade_affinity = 1.337, 
                                 language_of_performance_affinity = 1.337, 
                                 curateability_affinity = 1.337, 
                                 use_case_affinity = 1.337, 
                                 industry_suitability = 'Automobiles and Parts', 
                                 industry_suitability_affinity = 1.337, 
                                 audience_region = 'Australia and New Zealand', 
-                                arousal = 'very calm', 
-                                dominant_instrument = 'electric guitar', 
-                                energy = 'very quiet', 
-                                engagement = 'very unengaging', 
-                                groovyness = 'very steady', 
-                                harmony = 'very dissonant', 
-                                pleasantness = 'very unpleasant', 
-                                primary_mood_cluster = 'aggressive', 
-                                primary_sound_character = 'brassy', 
                                 valence_affinity = 1.337, 
                                 arousal_affinity = 1.337, 
                                 pleasantness_affinity = 1.337, 
                                 engagement_affinity = 1.337, 
                                 energy_affinity = 1.337, 
                                 tempo_affinity = 1.337, 
                                 scale_affinity = 1.337, 
@@ -163,30 +154,39 @@
                                 harmony_affinity = 1.337, 
                                 texture_affinity = 1.337, 
                                 groovyness_affinity = 1.337, 
                                 space_affinity = 1.337, 
                                 key_affinity = 1.337, 
                                 channel_suitability_affinity = 1.337, 
                                 key = 'C', ), 
+                            tags = [
+                                songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                    tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                        id = 56, 
+                                        name = '', 
+                                        categories = [
+                                            songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                                category_name = '', )
+                                            ], ), )
+                                ], 
                             spotify_id = '', 
                             genre_predictions = [
                                 songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
                                     genre_type = '', 
                                     genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                                         genre_name = '', ), 
                                     probability = 1.337, )
                                 ], ), 
-                        songtradr_track_guid = '', 
                         assigned_by_id = 56, 
-                        sequence = 56, )
-                    ], 
-                usages = [
-                    songtradr_api_client_python.models.usage_dto.UsageDTO(
-                        name = '', )
+                        sequence = 56, 
+                        songtradr_track_guid = '', )
                     ], 
+                asset_url = '', 
+                pretzel_tier = '', 
+                usage = '', 
                 created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 updated = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else :
             return PlaylistLargeDTO(
                 name = '',
         )
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_product_medium_dto.py` & `songtradr-api-client-python-1.12.24/test/test_product_medium_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -47,18 +47,18 @@
                 titles = [
                     songtradr_api_client_python.models.title_dto.TitleDTO(
                         title_text = '', )
                     ], 
                 gtin = '', 
                 grid = '', 
                 release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 pline = songtradr_api_client_python.models.p_line_dto.PLineDTO(
                     year = 56, 
                     text = '', ), 
+                takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 parties = [
                     songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
                         party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                             id = '', 
                             full_name = '', ), 
                         contributor_types = [
                             songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_product_party_dto.py` & `songtradr-api-client-python-1.12.24/test/test_product_party_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_api.py` & `songtradr-api-client-python-1.12.24/test/test_recording_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_for_similarity_search_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_for_similarity_search_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -37,46 +37,46 @@
         # uncomment below to create an instance of `RecordingForSimilaritySearchDTO`
         """
         model = songtradr_api_client_python.models.recording_for_similarity_search_dto.RecordingForSimilaritySearchDTO()  # noqa: E501
         if include_optional :
             return RecordingForSimilaritySearchDTO(
                 recording = songtradr_api_client_python.models.recording_small_dto.RecordingSmallDTO(
                     duration = 56, 
+                    isrc = '', 
                     parties = [
                         songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                             party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                 id = '', 
                                 full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                     type_name = '', )
                                 ], )
                         ], 
-                    isrc = '', 
                     titles = [
                         songtradr_api_client_python.models.title_dto.TitleDTO(
                             title_text = '', )
                         ], ), 
                 score = 1.337
             )
         else :
             return RecordingForSimilaritySearchDTO(
                 recording = songtradr_api_client_python.models.recording_small_dto.RecordingSmallDTO(
                     duration = 56, 
+                    isrc = '', 
                     parties = [
                         songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                             party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                 id = '', 
                                 full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                     type_name = '', )
                                 ], )
                         ], 
-                    isrc = '', 
                     titles = [
                         songtradr_api_client_python.models.title_dto.TitleDTO(
                             title_text = '', )
                         ], ),
                 score = 1.337,
         )
         """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_genre_prediction_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_genre_prediction_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_large_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_large_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,14 +36,15 @@
             optional params are included """
         # uncomment below to create an instance of `RecordingLargeDTO`
         """
         model = songtradr_api_client_python.models.recording_large_dto.RecordingLargeDTO()  # noqa: E501
         if include_optional :
             return RecordingLargeDTO(
                 duration = 56, 
+                isrc = '', 
                 parties = [
                     songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                         party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                             id = '', 
                             full_name = '', ), 
                         contributor_types = [
                             songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -52,25 +53,14 @@
                     ], 
                 genres = [
                     songtradr_api_client_python.models.genre_dto.GenreDTO(
                         id = 56, 
                         name = '', )
                     ], 
                 language_of_performance = '', 
-                isrc = '', 
-                tags = [
-                    songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                        tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                            id = 56, 
-                            name = '', 
-                            categories = [
-                                songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                    category_name = '', )
-                                ], ), )
-                    ], 
                 titles = [
                     songtradr_api_client_python.models.title_dto.TitleDTO(
                         title_text = '', )
                     ], 
                 tracks = [
                     songtradr_api_client_python.models.track_to_medium_product_dto.TrackToMediumProductDTO(
                         track_no = '', 
@@ -84,46 +74,55 @@
                             titles = [
                                 songtradr_api_client_python.models.title_dto.TitleDTO(
                                     title_text = '', )
                                 ], 
                             gtin = '', 
                             grid = '', 
                             release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                            takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                             pline = songtradr_api_client_python.models.p_line_dto.PLineDTO(
                                 year = 56, 
                                 text = '', ), 
+                            takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                             parties = [
                                 songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
                                     party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                         id = '', 
                                         full_name = '', ), 
                                     contributor_types = [
                                         songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                             type_name = '', )
                                         ], )
                                 ], ), )
                     ], 
                 musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                     space = 'very compact', 
-                    language_of_performance = 'en', 
+                    energy = 'very quiet', 
+                    engagement = 'very unengaging', 
+                    groovyness = 'very steady', 
+                    harmony = 'very dissonant', 
+                    pleasantness = 'very unpleasant', 
+                    primary_mood_cluster = 'aggressive', 
+                    primary_sound_character = 'brassy', 
                     rhythm = 'common time', 
                     roughness = 'very clear', 
                     scale = 'major key', 
                     sound_generation = 'acoustic', 
                     tempo = 'very slow', 
                     texture = 'very thin', 
                     timbre = 'very warm', 
                     tonality = 'monotonous', 
                     valence = 'very sad', 
                     vocals = 'instrumental', 
                     origin_decade = 'pre-1950s', 
                     curateability = 'curateable', 
                     use_case = 'background', 
                     channel_suitability = 'Spotify', 
+                    language_of_performance = 'en', 
+                    arousal = 'very calm', 
+                    dominant_instrument = 'electric guitar', 
                     primary_mood_cluster_affinity = 1.337, 
                     secondary_mood_cluster = 'aggressive', 
                     secondary_mood_cluster_affinity = 1.337, 
                     tertiary_mood_cluster = 'aggressive', 
                     tertiary_mood_cluster_affinity = 1.337, 
                     vocals_affinity = 1.337, 
                     dominant_instrument_affinity = 1.337, 
@@ -160,23 +159,14 @@
                     origin_decade_affinity = 1.337, 
                     language_of_performance_affinity = 1.337, 
                     curateability_affinity = 1.337, 
                     use_case_affinity = 1.337, 
                     industry_suitability = 'Automobiles and Parts', 
                     industry_suitability_affinity = 1.337, 
                     audience_region = 'Australia and New Zealand', 
-                    arousal = 'very calm', 
-                    dominant_instrument = 'electric guitar', 
-                    energy = 'very quiet', 
-                    engagement = 'very unengaging', 
-                    groovyness = 'very steady', 
-                    harmony = 'very dissonant', 
-                    pleasantness = 'very unpleasant', 
-                    primary_mood_cluster = 'aggressive', 
-                    primary_sound_character = 'brassy', 
                     valence_affinity = 1.337, 
                     arousal_affinity = 1.337, 
                     pleasantness_affinity = 1.337, 
                     engagement_affinity = 1.337, 
                     energy_affinity = 1.337, 
                     tempo_affinity = 1.337, 
                     scale_affinity = 1.337, 
@@ -185,18 +175,28 @@
                     harmony_affinity = 1.337, 
                     texture_affinity = 1.337, 
                     groovyness_affinity = 1.337, 
                     space_affinity = 1.337, 
                     key_affinity = 1.337, 
                     channel_suitability_affinity = 1.337, 
                     key = 'C', ), 
+                tags = [
+                    songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                        tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                            id = 56, 
+                            name = '', 
+                            categories = [
+                                songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                    category_name = '', )
+                                ], ), )
+                    ], 
+                spotify_id = '', 
                 pline = songtradr_api_client_python.models.p_line_dto.PLineDTO(
                     year = 56, 
                     text = '', ), 
-                spotify_id = '', 
                 genre_predictions = [
                     songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
                         genre_type = '', 
                         genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                             genre_name = '', ), 
                         probability = 1.337, )
                     ]
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_list_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_list_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -37,14 +37,15 @@
         # uncomment below to create an instance of `RecordingListDTO`
         """
         model = songtradr_api_client_python.models.recording_list_dto.RecordingListDTO()  # noqa: E501
         if include_optional :
             return RecordingListDTO(
                 recordings = [
                     songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
+                        isrc = '', 
                         recording_party_entities = [
                             songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                                 party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                     id = '', 
                                     full_name = '', ), 
                                 contributor_types = [
                                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -54,46 +55,44 @@
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        isrc = '', 
-                        tags = [
-                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                    id = 56, 
-                                    name = '', 
-                                    categories = [
-                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                            category_name = '', )
-                                        ], ), )
-                            ], 
                         titles = [
                             songtradr_api_client_python.models.title_dto.TitleDTO(
                                 title_text = '', )
                             ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            language_of_performance = 'en', 
+                            energy = 'very quiet', 
+                            engagement = 'very unengaging', 
+                            groovyness = 'very steady', 
+                            harmony = 'very dissonant', 
+                            pleasantness = 'very unpleasant', 
+                            primary_mood_cluster = 'aggressive', 
+                            primary_sound_character = 'brassy', 
                             rhythm = 'common time', 
                             roughness = 'very clear', 
                             scale = 'major key', 
                             sound_generation = 'acoustic', 
                             tempo = 'very slow', 
                             texture = 'very thin', 
                             timbre = 'very warm', 
                             tonality = 'monotonous', 
                             valence = 'very sad', 
                             vocals = 'instrumental', 
                             origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            language_of_performance = 'en', 
+                            arousal = 'very calm', 
+                            dominant_instrument = 'electric guitar', 
                             primary_mood_cluster_affinity = 1.337, 
                             secondary_mood_cluster = 'aggressive', 
                             secondary_mood_cluster_affinity = 1.337, 
                             tertiary_mood_cluster = 'aggressive', 
                             tertiary_mood_cluster_affinity = 1.337, 
                             vocals_affinity = 1.337, 
                             dominant_instrument_affinity = 1.337, 
@@ -130,23 +129,14 @@
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', 
-                            arousal = 'very calm', 
-                            dominant_instrument = 'electric guitar', 
-                            energy = 'very quiet', 
-                            engagement = 'very unengaging', 
-                            groovyness = 'very steady', 
-                            harmony = 'very dissonant', 
-                            pleasantness = 'very unpleasant', 
-                            primary_mood_cluster = 'aggressive', 
-                            primary_sound_character = 'brassy', 
                             valence_affinity = 1.337, 
                             arousal_affinity = 1.337, 
                             pleasantness_affinity = 1.337, 
                             engagement_affinity = 1.337, 
                             energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
@@ -155,14 +145,24 @@
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
                             key = 'C', ), 
+                        tags = [
+                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                    id = 56, 
+                                    name = '', 
+                                    categories = [
+                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                            category_name = '', )
+                                        ], ), )
+                            ], 
                         spotify_id = '', 
                         genre_predictions = [
                             songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
                                 genre_type = '', 
                                 genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                                     genre_name = '', ), 
                                 probability = 1.337, )
@@ -172,14 +172,15 @@
                 current_page_number = 56, 
                 total_results = 56
             )
         else :
             return RecordingListDTO(
                 recordings = [
                     songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
+                        isrc = '', 
                         recording_party_entities = [
                             songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                                 party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                     id = '', 
                                     full_name = '', ), 
                                 contributor_types = [
                                     songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -189,46 +190,44 @@
                         genres = [
                             songtradr_api_client_python.models.genre_dto.GenreDTO(
                                 id = 56, 
                                 name = '', )
                             ], 
                         language_of_performance = '', 
                         release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        isrc = '', 
-                        tags = [
-                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                    id = 56, 
-                                    name = '', 
-                                    categories = [
-                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                            category_name = '', )
-                                        ], ), )
-                            ], 
                         titles = [
                             songtradr_api_client_python.models.title_dto.TitleDTO(
                                 title_text = '', )
                             ], 
                         musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                             space = 'very compact', 
-                            language_of_performance = 'en', 
+                            energy = 'very quiet', 
+                            engagement = 'very unengaging', 
+                            groovyness = 'very steady', 
+                            harmony = 'very dissonant', 
+                            pleasantness = 'very unpleasant', 
+                            primary_mood_cluster = 'aggressive', 
+                            primary_sound_character = 'brassy', 
                             rhythm = 'common time', 
                             roughness = 'very clear', 
                             scale = 'major key', 
                             sound_generation = 'acoustic', 
                             tempo = 'very slow', 
                             texture = 'very thin', 
                             timbre = 'very warm', 
                             tonality = 'monotonous', 
                             valence = 'very sad', 
                             vocals = 'instrumental', 
                             origin_decade = 'pre-1950s', 
                             curateability = 'curateable', 
                             use_case = 'background', 
                             channel_suitability = 'Spotify', 
+                            language_of_performance = 'en', 
+                            arousal = 'very calm', 
+                            dominant_instrument = 'electric guitar', 
                             primary_mood_cluster_affinity = 1.337, 
                             secondary_mood_cluster = 'aggressive', 
                             secondary_mood_cluster_affinity = 1.337, 
                             tertiary_mood_cluster = 'aggressive', 
                             tertiary_mood_cluster_affinity = 1.337, 
                             vocals_affinity = 1.337, 
                             dominant_instrument_affinity = 1.337, 
@@ -265,23 +264,14 @@
                             origin_decade_affinity = 1.337, 
                             language_of_performance_affinity = 1.337, 
                             curateability_affinity = 1.337, 
                             use_case_affinity = 1.337, 
                             industry_suitability = 'Automobiles and Parts', 
                             industry_suitability_affinity = 1.337, 
                             audience_region = 'Australia and New Zealand', 
-                            arousal = 'very calm', 
-                            dominant_instrument = 'electric guitar', 
-                            energy = 'very quiet', 
-                            engagement = 'very unengaging', 
-                            groovyness = 'very steady', 
-                            harmony = 'very dissonant', 
-                            pleasantness = 'very unpleasant', 
-                            primary_mood_cluster = 'aggressive', 
-                            primary_sound_character = 'brassy', 
                             valence_affinity = 1.337, 
                             arousal_affinity = 1.337, 
                             pleasantness_affinity = 1.337, 
                             engagement_affinity = 1.337, 
                             energy_affinity = 1.337, 
                             tempo_affinity = 1.337, 
                             scale_affinity = 1.337, 
@@ -290,14 +280,24 @@
                             harmony_affinity = 1.337, 
                             texture_affinity = 1.337, 
                             groovyness_affinity = 1.337, 
                             space_affinity = 1.337, 
                             key_affinity = 1.337, 
                             channel_suitability_affinity = 1.337, 
                             key = 'C', ), 
+                        tags = [
+                            songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                                tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                    id = 56, 
+                                    name = '', 
+                                    categories = [
+                                        songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                            category_name = '', )
+                                        ], ), )
+                            ], 
                         spotify_id = '', 
                         genre_predictions = [
                             songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
                                 genre_type = '', 
                                 genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                                     genre_name = '', ), 
                                 probability = 1.337, )
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_medium_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_medium_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -35,14 +35,15 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `RecordingMediumDTO`
         """
         model = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO()  # noqa: E501
         if include_optional :
             return RecordingMediumDTO(
+                isrc = '', 
                 recording_party_entities = [
                     songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                         party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                             id = '', 
                             full_name = '', ), 
                         contributor_types = [
                             songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -52,46 +53,44 @@
                 genres = [
                     songtradr_api_client_python.models.genre_dto.GenreDTO(
                         id = 56, 
                         name = '', )
                     ], 
                 language_of_performance = '', 
                 release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                isrc = '', 
-                tags = [
-                    songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                        tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                            id = 56, 
-                            name = '', 
-                            categories = [
-                                songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                    category_name = '', )
-                                ], ), )
-                    ], 
                 titles = [
                     songtradr_api_client_python.models.title_dto.TitleDTO(
                         title_text = '', )
                     ], 
                 musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                     space = 'very compact', 
-                    language_of_performance = 'en', 
+                    energy = 'very quiet', 
+                    engagement = 'very unengaging', 
+                    groovyness = 'very steady', 
+                    harmony = 'very dissonant', 
+                    pleasantness = 'very unpleasant', 
+                    primary_mood_cluster = 'aggressive', 
+                    primary_sound_character = 'brassy', 
                     rhythm = 'common time', 
                     roughness = 'very clear', 
                     scale = 'major key', 
                     sound_generation = 'acoustic', 
                     tempo = 'very slow', 
                     texture = 'very thin', 
                     timbre = 'very warm', 
                     tonality = 'monotonous', 
                     valence = 'very sad', 
                     vocals = 'instrumental', 
                     origin_decade = 'pre-1950s', 
                     curateability = 'curateable', 
                     use_case = 'background', 
                     channel_suitability = 'Spotify', 
+                    language_of_performance = 'en', 
+                    arousal = 'very calm', 
+                    dominant_instrument = 'electric guitar', 
                     primary_mood_cluster_affinity = 1.337, 
                     secondary_mood_cluster = 'aggressive', 
                     secondary_mood_cluster_affinity = 1.337, 
                     tertiary_mood_cluster = 'aggressive', 
                     tertiary_mood_cluster_affinity = 1.337, 
                     vocals_affinity = 1.337, 
                     dominant_instrument_affinity = 1.337, 
@@ -128,23 +127,14 @@
                     origin_decade_affinity = 1.337, 
                     language_of_performance_affinity = 1.337, 
                     curateability_affinity = 1.337, 
                     use_case_affinity = 1.337, 
                     industry_suitability = 'Automobiles and Parts', 
                     industry_suitability_affinity = 1.337, 
                     audience_region = 'Australia and New Zealand', 
-                    arousal = 'very calm', 
-                    dominant_instrument = 'electric guitar', 
-                    energy = 'very quiet', 
-                    engagement = 'very unengaging', 
-                    groovyness = 'very steady', 
-                    harmony = 'very dissonant', 
-                    pleasantness = 'very unpleasant', 
-                    primary_mood_cluster = 'aggressive', 
-                    primary_sound_character = 'brassy', 
                     valence_affinity = 1.337, 
                     arousal_affinity = 1.337, 
                     pleasantness_affinity = 1.337, 
                     engagement_affinity = 1.337, 
                     energy_affinity = 1.337, 
                     tempo_affinity = 1.337, 
                     scale_affinity = 1.337, 
@@ -153,14 +143,24 @@
                     harmony_affinity = 1.337, 
                     texture_affinity = 1.337, 
                     groovyness_affinity = 1.337, 
                     space_affinity = 1.337, 
                     key_affinity = 1.337, 
                     channel_suitability_affinity = 1.337, 
                     key = 'C', ), 
+                tags = [
+                    songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                        tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                            id = 56, 
+                            name = '', 
+                            categories = [
+                                songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                    category_name = '', )
+                                ], ), )
+                    ], 
                 spotify_id = '', 
                 genre_predictions = [
                     songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
                         genre_type = '', 
                         genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                             genre_name = '', ), 
                         probability = 1.337, )
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_minimal_with_musical_features_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_minimal_with_musical_features_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -39,29 +39,38 @@
         model = songtradr_api_client_python.models.recording_minimal_with_musical_features_dto.RecordingMinimalWithMusicalFeaturesDTO()  # noqa: E501
         if include_optional :
             return RecordingMinimalWithMusicalFeaturesDTO(
                 isrc = '', 
                 musical_features = [
                     songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                         space = 'very compact', 
-                        language_of_performance = 'en', 
+                        energy = 'very quiet', 
+                        engagement = 'very unengaging', 
+                        groovyness = 'very steady', 
+                        harmony = 'very dissonant', 
+                        pleasantness = 'very unpleasant', 
+                        primary_mood_cluster = 'aggressive', 
+                        primary_sound_character = 'brassy', 
                         rhythm = 'common time', 
                         roughness = 'very clear', 
                         scale = 'major key', 
                         sound_generation = 'acoustic', 
                         tempo = 'very slow', 
                         texture = 'very thin', 
                         timbre = 'very warm', 
                         tonality = 'monotonous', 
                         valence = 'very sad', 
                         vocals = 'instrumental', 
                         origin_decade = 'pre-1950s', 
                         curateability = 'curateable', 
                         use_case = 'background', 
                         channel_suitability = 'Spotify', 
+                        language_of_performance = 'en', 
+                        arousal = 'very calm', 
+                        dominant_instrument = 'electric guitar', 
                         primary_mood_cluster_affinity = 1.337, 
                         secondary_mood_cluster = 'aggressive', 
                         secondary_mood_cluster_affinity = 1.337, 
                         tertiary_mood_cluster = 'aggressive', 
                         tertiary_mood_cluster_affinity = 1.337, 
                         vocals_affinity = 1.337, 
                         dominant_instrument_affinity = 1.337, 
@@ -98,23 +107,14 @@
                         origin_decade_affinity = 1.337, 
                         language_of_performance_affinity = 1.337, 
                         curateability_affinity = 1.337, 
                         use_case_affinity = 1.337, 
                         industry_suitability = 'Automobiles and Parts', 
                         industry_suitability_affinity = 1.337, 
                         audience_region = 'Australia and New Zealand', 
-                        arousal = 'very calm', 
-                        dominant_instrument = 'electric guitar', 
-                        energy = 'very quiet', 
-                        engagement = 'very unengaging', 
-                        groovyness = 'very steady', 
-                        harmony = 'very dissonant', 
-                        pleasantness = 'very unpleasant', 
-                        primary_mood_cluster = 'aggressive', 
-                        primary_sound_character = 'brassy', 
                         valence_affinity = 1.337, 
                         arousal_affinity = 1.337, 
                         pleasantness_affinity = 1.337, 
                         engagement_affinity = 1.337, 
                         energy_affinity = 1.337, 
                         tempo_affinity = 1.337, 
                         scale_affinity = 1.337,
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_minimal_with_taggrams_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_minimal_with_taggrams_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_minimal_with_tagstrengths_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_minimal_with_tagstrengths_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_party_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_party_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_playlist_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_playlist_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,14 +36,15 @@
             optional params are included """
         # uncomment below to create an instance of `RecordingPlaylistDTO`
         """
         model = songtradr_api_client_python.models.recording_playlist_dto.RecordingPlaylistDTO()  # noqa: E501
         if include_optional :
             return RecordingPlaylistDTO(
                 recording = songtradr_api_client_python.models.recording_medium_dto.RecordingMediumDTO(
+                    isrc = '', 
                     recording_party_entities = [
                         songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                             party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                 id = '', 
                                 full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -53,46 +54,44 @@
                     genres = [
                         songtradr_api_client_python.models.genre_dto.GenreDTO(
                             id = 56, 
                             name = '', )
                         ], 
                     language_of_performance = '', 
                     release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    isrc = '', 
-                    tags = [
-                        songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
-                            tag = songtradr_api_client_python.models.tag_dto.TagDTO(
-                                id = 56, 
-                                name = '', 
-                                categories = [
-                                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
-                                        category_name = '', )
-                                    ], ), )
-                        ], 
                     titles = [
                         songtradr_api_client_python.models.title_dto.TitleDTO(
                             title_text = '', )
                         ], 
                     musical_features = songtradr_api_client_python.models.musical_features_dto.MusicalFeaturesDTO(
                         space = 'very compact', 
-                        language_of_performance = 'en', 
+                        energy = 'very quiet', 
+                        engagement = 'very unengaging', 
+                        groovyness = 'very steady', 
+                        harmony = 'very dissonant', 
+                        pleasantness = 'very unpleasant', 
+                        primary_mood_cluster = 'aggressive', 
+                        primary_sound_character = 'brassy', 
                         rhythm = 'common time', 
                         roughness = 'very clear', 
                         scale = 'major key', 
                         sound_generation = 'acoustic', 
                         tempo = 'very slow', 
                         texture = 'very thin', 
                         timbre = 'very warm', 
                         tonality = 'monotonous', 
                         valence = 'very sad', 
                         vocals = 'instrumental', 
                         origin_decade = 'pre-1950s', 
                         curateability = 'curateable', 
                         use_case = 'background', 
                         channel_suitability = 'Spotify', 
+                        language_of_performance = 'en', 
+                        arousal = 'very calm', 
+                        dominant_instrument = 'electric guitar', 
                         primary_mood_cluster_affinity = 1.337, 
                         secondary_mood_cluster = 'aggressive', 
                         secondary_mood_cluster_affinity = 1.337, 
                         tertiary_mood_cluster = 'aggressive', 
                         tertiary_mood_cluster_affinity = 1.337, 
                         vocals_affinity = 1.337, 
                         dominant_instrument_affinity = 1.337, 
@@ -129,23 +128,14 @@
                         origin_decade_affinity = 1.337, 
                         language_of_performance_affinity = 1.337, 
                         curateability_affinity = 1.337, 
                         use_case_affinity = 1.337, 
                         industry_suitability = 'Automobiles and Parts', 
                         industry_suitability_affinity = 1.337, 
                         audience_region = 'Australia and New Zealand', 
-                        arousal = 'very calm', 
-                        dominant_instrument = 'electric guitar', 
-                        energy = 'very quiet', 
-                        engagement = 'very unengaging', 
-                        groovyness = 'very steady', 
-                        harmony = 'very dissonant', 
-                        pleasantness = 'very unpleasant', 
-                        primary_mood_cluster = 'aggressive', 
-                        primary_sound_character = 'brassy', 
                         valence_affinity = 1.337, 
                         arousal_affinity = 1.337, 
                         pleasantness_affinity = 1.337, 
                         engagement_affinity = 1.337, 
                         energy_affinity = 1.337, 
                         tempo_affinity = 1.337, 
                         scale_affinity = 1.337, 
@@ -154,25 +144,35 @@
                         harmony_affinity = 1.337, 
                         texture_affinity = 1.337, 
                         groovyness_affinity = 1.337, 
                         space_affinity = 1.337, 
                         key_affinity = 1.337, 
                         channel_suitability_affinity = 1.337, 
                         key = 'C', ), 
+                    tags = [
+                        songtradr_api_client_python.models.recording_tag_small_dto.RecordingTagSmallDTO(
+                            tag = songtradr_api_client_python.models.tag_dto.TagDTO(
+                                id = 56, 
+                                name = '', 
+                                categories = [
+                                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                                        category_name = '', )
+                                    ], ), )
+                        ], 
                     spotify_id = '', 
                     genre_predictions = [
                         songtradr_api_client_python.models.recording_genre_prediction_dto.RecordingGenrePredictionDTO(
                             genre_type = '', 
                             genre = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO(
                                 genre_name = '', ), 
                             probability = 1.337, )
                         ], ), 
-                songtradr_track_guid = '', 
                 assigned_by_id = 56, 
-                sequence = 56
+                sequence = 56, 
+                songtradr_track_guid = ''
             )
         else :
             return RecordingPlaylistDTO(
         )
         """
 
     def testRecordingPlaylistDTO(self):
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_small_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -36,25 +36,25 @@
             optional params are included """
         # uncomment below to create an instance of `RecordingSmallDTO`
         """
         model = songtradr_api_client_python.models.recording_small_dto.RecordingSmallDTO()  # noqa: E501
         if include_optional :
             return RecordingSmallDTO(
                 duration = 56, 
+                isrc = '', 
                 parties = [
                     songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO(
                         party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                             id = '', 
                             full_name = '', ), 
                         contributor_types = [
                             songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
                                 type_name = '', )
                             ], )
                     ], 
-                isrc = '', 
                 titles = [
                     songtradr_api_client_python.models.title_dto.TitleDTO(
                         title_text = '', )
                     ]
             )
         else :
             return RecordingSmallDTO(
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_recording_tag_small_dto.py` & `songtradr-api-client-python-1.12.24/test/test_recording_tag_small_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_save_file_recording_dto.py` & `songtradr-api-client-python-1.12.24/test/test_save_file_recording_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_save_playlist_dto.py` & `songtradr-api-client-python-1.12.24/test/test_save_playlist_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_save_recording_genre_dto.py` & `songtradr-api-client-python-1.12.24/test/test_save_recording_genre_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_save_recording_party_dto.py` & `songtradr-api-client-python-1.12.24/test/test_save_recording_party_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_save_recording_playlist_dto.py` & `songtradr-api-client-python-1.12.24/test/test_save_recording_playlist_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_save_recording_tag_dto.py` & `songtradr-api-client-python-1.12.24/test/test_save_recording_tag_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_save_referrer_dto.py` & `songtradr-api-client-python-1.12.24/test/test_save_referrer_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_save_taggrams_dto.py` & `songtradr-api-client-python-1.12.24/test/test_save_taggrams_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_save_user_dto.py` & `songtradr-api-client-python-1.12.24/test/test_save_user_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_search_filter_values_dto.py` & `songtradr-api-client-python-1.12.24/test/test_search_filter_values_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_search_recording_granular_abstraction_dto.py` & `songtradr-api-client-python-1.12.24/test/test_search_recording_granular_abstraction_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_search_recording_granular_dto.py` & `songtradr-api-client-python-1.12.24/test/test_search_recording_granular_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_sign_up_dto.py` & `songtradr-api-client-python-1.12.24/test/test_sign_up_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_tag_dto.py` & `songtradr-api-client-python-1.12.24/test/test_tag_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_tag_small_dto.py` & `songtradr-api-client-python-1.12.24/test/test_tag_small_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_taggram_dto.py` & `songtradr-api-client-python-1.12.24/test/test_taggram_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_tags_summary_dto.py` & `songtradr-api-client-python-1.12.24/test/test_tags_summary_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_tagstrength_dto.py` & `songtradr-api-client-python-1.12.24/test/test_tagstrength_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_title_dto.py` & `songtradr-api-client-python-1.12.24/test/test_title_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_token_request.py` & `songtradr-api-client-python-1.12.24/test/test_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_track_to_medium_product_dto.py` & `songtradr-api-client-python-1.12.24/test/test_track_to_medium_product_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -50,18 +50,18 @@
                     titles = [
                         songtradr_api_client_python.models.title_dto.TitleDTO(
                             title_text = '', )
                         ], 
                     gtin = '', 
                     grid = '', 
                     release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     pline = songtradr_api_client_python.models.p_line_dto.PLineDTO(
                         year = 56, 
                         text = '', ), 
+                    takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     parties = [
                         songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
                             party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                 id = '', 
                                 full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
@@ -81,18 +81,18 @@
                     titles = [
                         songtradr_api_client_python.models.title_dto.TitleDTO(
                             title_text = '', )
                         ], 
                     gtin = '', 
                     grid = '', 
                     release_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     pline = songtradr_api_client_python.models.p_line_dto.PLineDTO(
                         year = 56, 
                         text = '', ), 
+                    takedown_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     parties = [
                         songtradr_api_client_python.models.product_party_dto.ProductPartyDTO(
                             party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
                                 id = '', 
                                 full_name = '', ), 
                             contributor_types = [
                                 songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_update_password_dto.py` & `songtradr-api-client-python-1.12.24/test/test_update_password_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_usage_dto.py` & `songtradr-api-client-python-1.12.24/test/test_usage_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_user_api.py` & `songtradr-api-client-python-1.12.24/test/test_user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `songtradr-api-client-python-1.12.23/test/test_user_dto.py` & `songtradr-api-client-python-1.12.24/test/test_user_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
-    The version of the OpenAPI document: 1.12.23
+    The version of the OpenAPI document: 1.12.24
     Contact: info@songtradr.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -52,14 +52,23 @@
                 signup_allowed = True, 
                 upload_allowed = True, 
                 fingerprint_allowed = True, 
                 audiotagging_allowed = True, 
                 b2b_allowed = True, 
                 editor_allowed = True, 
                 insights_allowed = True, 
+                genres_allowed = True, 
+                moods_allowed = True, 
+                instrumentation_allowed = True, 
+                sound_features_allowed = True, 
+                tonal_features_allowed = True, 
+                rhythm_features_allowed = True, 
+                audience_allowed = True, 
+                origin_allowed = True, 
+                quality_allowed = True, 
                 reduced_musical_features = True, 
                 confirmed = True, 
                 language = '', 
                 admin = True
             )
         else :
             return UserDTO(
@@ -75,14 +84,23 @@
                 signup_allowed = True,
                 upload_allowed = True,
                 fingerprint_allowed = True,
                 audiotagging_allowed = True,
                 b2b_allowed = True,
                 editor_allowed = True,
                 insights_allowed = True,
+                genres_allowed = True,
+                moods_allowed = True,
+                instrumentation_allowed = True,
+                sound_features_allowed = True,
+                tonal_features_allowed = True,
+                rhythm_features_allowed = True,
+                audience_allowed = True,
+                origin_allowed = True,
+                quality_allowed = True,
                 reduced_musical_features = True,
                 confirmed = True,
                 language = '',
         )
         """
 
     def testUserDTO(self):
```

