# Comparing `tmp/wagtail-cjkcms-23.7.3.tar.gz` & `tmp/wagtail-cjkcms-23.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cjkcms-23.7.3.tar", last modified: Mon Jul  3 18:02:33 2023, max compression
+gzip compressed data, was "wagtail-cjkcms-23.8.1.tar", last modified: Wed Aug  2 09:07:53 2023, max compression
```

## Comparing `wagtail-cjkcms-23.7.3.tar` & `wagtail-cjkcms-23.8.1.tar`

### file list

```diff
@@ -1,275 +1,390 @@
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.782288 wagtail-cjkcms-23.7.3/
--rw-r--r--   0 grze      (1000) grze      (1000)     7844 2023-07-03 18:01:32.000000 wagtail-cjkcms-23.7.3/CHANGELOG.md
--rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/LICENSE
--rw-r--r--   0 grze      (1000) grze      (1000)      239 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/MANIFEST.in
--rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-07-03 18:02:33.782288 wagtail-cjkcms-23.7.3/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     1688 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/README.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.738955 wagtail-cjkcms-23.7.3/cjkcms/
--rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-07-03 18:00:48.000000 wagtail-cjkcms-23.7.3/cjkcms/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.738955 wagtail-cjkcms-23.7.3/cjkcms/api/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/api/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/api/mailchimp.py
--rw-r--r--   0 grze      (1000) grze      (1000)      173 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/apps.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.738955 wagtail-cjkcms-23.7.3/cjkcms/bin/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/bin/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/bin/cjkcms.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.738955 wagtail-cjkcms-23.7.3/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     3223 2023-07-02 10:36:27.000000 wagtail-cjkcms-23.7.3/cjkcms/blocks/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)    10539 2023-07-02 10:10:41.000000 wagtail-cjkcms-23.7.3/cjkcms/blocks/base_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     8757 2023-07-02 10:38:05.000000 wagtail-cjkcms-23.7.3/cjkcms/blocks/content_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9537 2023-07-02 19:16:58.000000 wagtail-cjkcms-23.7.3/cjkcms/blocks/html_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/blocks/layout_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/blocks/searchable_html_block.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.738955 wagtail-cjkcms-23.7.3/cjkcms/draftail/
--rw-r--r--   0 grze      (1000) grze      (1000)      305 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/draftail/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/draftail/draftail_extensions.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5157 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/draftail/draftail_icons.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3191 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/fields.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.738955 wagtail-cjkcms-23.7.3/cjkcms/finders/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/finders/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2459 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/finders/oembed.py
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/forms.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1804 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/image_formats.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.728121 wagtail-cjkcms-23.7.3/cjkcms/management/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.749788 wagtail-cjkcms-23.7.3/cjkcms/management/commands/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/management/commands/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      453 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/management/commands/clear-embeds.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2565 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/management/commands/import-csv.py
--rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/management/commands/init-collections.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/management/commands/init-navbar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/management/commands/init-website.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.749788 wagtail-cjkcms-23.7.3/cjkcms/migrations/
--rw-r--r--   0 grze      (1000) grze      (1000)   216350 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0001_initial.py
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
--rw-r--r--   0 grze      (1000) grze      (1000)      668 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1027 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1334 2023-05-31 15:55:06.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
--rw-r--r--   0 grze      (1000) grze      (1000)      685 2023-06-04 21:40:37.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0009_navbar_language.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3479 2023-07-02 11:44:17.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0010_filmstrip_filmpanel.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1393 2023-07-02 17:30:25.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1466 2023-07-03 18:00:31.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/migrations/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.749788 wagtail-cjkcms-23.7.3/cjkcms/models/
--rw-r--r--   0 grze      (1000) grze      (1000)      232 2023-05-31 15:50:31.000000 wagtail-cjkcms-23.7.3/cjkcms/models/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      335 2023-05-31 16:04:59.000000 wagtail-cjkcms-23.7.3/cjkcms/models/admin_sidebar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2356 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/models/cms_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6302 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/models/integration_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    23813 2023-07-02 20:11:09.000000 wagtail-cjkcms-23.7.3/cjkcms/models/page_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    15369 2023-07-02 11:08:25.000000 wagtail-cjkcms-23.7.3/cjkcms/models/snippet_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    19011 2023-07-03 17:59:54.000000 wagtail-cjkcms-23.7.3/cjkcms/models/wagtailsettings_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/search_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9541 2023-07-02 17:18:42.000000 wagtail-cjkcms-23.7.3/cjkcms/settings.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.728121 wagtail-cjkcms-23.7.3/cjkcms/static/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.728121 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.749788 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/
--rw-r--r--   0 grze      (1000) grze      (1000)    93729 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/bootstrap-icons.css
--rw-r--r--   0 grze      (1000) grze      (1000)    49971 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/bootstrap-icons.json
--rw-r--r--   0 grze      (1000) grze      (1000)    55169 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.749788 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/fonts/
--rw-r--r--   0 grze      (1000) grze      (1000)   164360 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
--rw-r--r--   0 grze      (1000) grze      (1000)   121340 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.749788 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/css/
--rw-r--r--   0 grze      (1000) grze      (1000)      846 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/css/cjkcms-admin.css
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-06-04 21:08:12.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/css/cjkcms-editor.css
--rw-r--r--   0 grze      (1000) grze      (1000)     4614 2023-07-02 11:08:20.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/css/cjkcms-front.css
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.728121 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.749788 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/avatars/
--rw-r--r--   0 grze      (1000) grze      (1000)      535 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/avatars/default.png
--rw-r--r--   0 grze      (1000) grze      (1000)      384 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/avatars/default.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.749788 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/icons/quote.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.749788 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/logos/
--rw-r--r--   0 grze      (1000) grze      (1000)     4166 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
--rw-r--r--   0 grze      (1000) grze      (1000)     4218 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.749788 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/patterns/
--rw-r--r--   0 grze      (1000) grze      (1000)    47935 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    31707 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    38190 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.749788 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/js/
--rw-r--r--   0 grze      (1000) grze      (1000)      444 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/js/cjkcms-editor.js
--rw-r--r--   0 grze      (1000) grze      (1000)     5565 2023-07-02 11:07:19.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/js/cjkcms-front.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.760621 wagtail-cjkcms-23.7.3/cjkcms/static/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cookieconsent/cookieconsent.css
--rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/static/cookieconsent/cookieconsent.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.760621 wagtail-cjkcms-23.7.3/cjkcms/templates/
--rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/404.html
--rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/500.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.760621 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.760621 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     1443 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/accordion_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      974 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/article_block_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1132 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)      188 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/base_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2505 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/base_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      740 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/button_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      746 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      856 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_blurb.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      730 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_head.html
--rw-r--r--   0 grze      (1000) grze      (1000)      771 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_head_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      990 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_horizontal.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_img.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2618 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_landing1.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_landing2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      450 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      276 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/carousel_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      406 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/column_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/document_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/download_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      103 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/embed_video_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       95 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/external_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1484 2023-07-02 12:08:07.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/film_strip_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      424 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/grid_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/h1_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/h2_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/h3_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      790 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/hero_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/image_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      627 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/image_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1020 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/modal_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      164 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/page_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      787 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      642 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      956 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
--rw-r--r--   0 grze      (1000) grze      (1000)      858 2023-07-03 13:15:10.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      610 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-02 17:20:14.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1065 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagepreview_form.html
--rw-r--r--   0 grze      (1000) grze      (1000)      244 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pricelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      353 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/quote_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      852 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      998 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
--rw-r--r--   0 grze      (1000) grze      (1000)      216 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       91 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/rich_text_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1095 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/table_block.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.760621 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/cookieconsent/languages.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.771455 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/formfields/
--rw-r--r--   0 grze      (1000) grze      (1000)      267 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/formfields/date.html
--rw-r--r--   0 grze      (1000) grze      (1000)      416 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/formfields/datetime.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.771455 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/formfields/mailchimp/
--rw-r--r--   0 grze      (1000) grze      (1000)     9267 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)     6469 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
--rw-r--r--   0 grze      (1000) grze      (1000)      264 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/formfields/time.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.771455 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      465 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/align-left.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/check-square-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/columns.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      359 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/desktop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      571 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/font.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      292 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/google.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      813 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      666 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/hashtag.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      840 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/header.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/list-alt.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      459 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/map.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      448 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/newspaper-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      721 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      635 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/recycle.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      174 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/stop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      505 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/th-large.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      762 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/universal-access.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      548 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/usd.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      225 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/window-maximize.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      199 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/window-minimize.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.771455 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      689 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      579 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/classifier_nav.html
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/codered_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      268 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/form_honeypot.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1061 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/pagination.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.771455 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/stream_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      532 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.771455 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/
--rw-r--r--   0 grze      (1000) grze      (1000)     2002 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/article_index_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2031 2023-07-02 17:41:05.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/article_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1018 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/article_page.search.html
--rw-r--r--   0 grze      (1000) grze      (1000)     8684 2023-07-03 17:38:35.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/base.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/form_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-07-02 17:27:50.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/form_page.mini.html
--rw-r--r--   0 grze      (1000) grze      (1000)      248 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/form_page_landing.html
--rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/home_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      491 2023-07-02 12:27:06.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/page.mini.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2610 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      582 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/search_result.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2462 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/stream_form_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-07-02 17:46:00.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/web_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-07-02 17:29:59.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/web_page_notitle.html
--rw-r--r--   0 grze      (1000) grze      (1000)      122 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/robots.txt
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.771455 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/
--rw-r--r--   0 grze      (1000) grze      (1000)     1943 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html
--rw-r--r--   0 grze      (1000) grze      (1000)      430 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/footer.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2027 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/frontend_assets.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2712 2023-06-05 10:52:40.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/navbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      836 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html
--rw-r--r--   0 grze      (1000) grze      (1000)      386 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/navbar_search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/tracking_g3.html
--rw-r--r--   0 grze      (1000) grze      (1000)      832 2023-07-02 11:03:38.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/tracking_g4.html
--rw-r--r--   0 grze      (1000) grze      (1000)      892 2023-07-03 17:56:11.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/tracking_matomo.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.771455 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/widgets/
--rw-r--r--   0 grze      (1000) grze      (1000)     1444 2023-07-02 10:12:54.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.738955 wagtail-cjkcms-23.7.3/cjkcms/templates/wagtailadmin/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.771455 wagtail-cjkcms-23.7.3/cjkcms/templates/wagtailadmin/block_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      839 2023-06-04 21:09:36.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-r--r--   0 grze      (1000) grze      (1000)      550 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/wagtailadmin/block_forms/struct.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.771455 wagtail-cjkcms-23.7.3/cjkcms/templates/wagtailadmin/shared/
--rw-r--r--   0 grze      (1000) grze      (1000)      885 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.782288 wagtail-cjkcms-23.7.3/cjkcms/templatetags/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templatetags/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      327 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templatetags/auth_extras.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6785 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templatetags/cjkcms_tags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4962 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templatetags/friendly_loader.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templatetags/gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/templatetags/txtutils_tags.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.782288 wagtail-cjkcms-23.7.3/cjkcms/tests/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/tests/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4226 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/tests/test_articlepages.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3506 2023-07-02 20:34:24.000000 wagtail-cjkcms-23.7.3/cjkcms/tests/test_bin.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2629 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/tests/test_gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4639 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/tests/test_search_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/tests/test_settings.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3511 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/tests/test_templatetags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2678 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/tests/test_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1520 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/tests/test_webpage.py
--rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/utils.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4488 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/views.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6557 2023-05-31 16:27:47.000000 wagtail-cjkcms-23.7.3/cjkcms/wagtail_hooks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1531 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/cjkcms/widgets.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.782288 wagtail-cjkcms-23.7.3/docs/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.782288 wagtail-cjkcms-23.7.3/docs/how-to/
--rw-r--r--   0 grze      (1000) grze      (1000)     1481 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/docs/how-to/oembed_finder.md
--rw-r--r--   0 grze      (1000) grze      (1000)      537 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/docs/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)     5520 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/docs/installation.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.782288 wagtail-cjkcms-23.7.3/docs/management_commands/
--rw-r--r--   0 grze      (1000) grze      (1000)      318 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/docs/management_commands/clear-embeds.md
--rw-r--r--   0 grze      (1000) grze      (1000)      193 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/docs/management_commands/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)      420 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/docs/management_commands/init-collections.md
--rw-r--r--   0 grze      (1000) grze      (1000)      936 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/docs/quick-start.md
--rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/docs/requirements.txt
--rw-r--r--   0 grze      (1000) grze      (1000)     1220 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/docs/why-another-cms.md
--rw-r--r--   0 grze      (1000) grze      (1000)       93 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/pyproject.toml
--rw-r--r--   0 grze      (1000) grze      (1000)     1555 2023-07-03 18:02:33.793121 wagtail-cjkcms-23.7.3/setup.cfg
--rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-05-31 14:14:01.000000 wagtail-cjkcms-23.7.3/setup.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-07-03 18:02:33.782288 wagtail-cjkcms-23.7.3/wagtail_cjkcms.egg-info/
--rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-07-03 18:02:33.000000 wagtail-cjkcms-23.7.3/wagtail_cjkcms.egg-info/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     9951 2023-07-03 18:02:33.000000 wagtail-cjkcms-23.7.3/wagtail_cjkcms.egg-info/SOURCES.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-07-03 18:02:33.000000 wagtail-cjkcms-23.7.3/wagtail_cjkcms.egg-info/dependency_links.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-07-03 18:02:33.000000 wagtail-cjkcms-23.7.3/wagtail_cjkcms.egg-info/entry_points.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       79 2023-07-03 18:02:33.000000 wagtail-cjkcms-23.7.3/wagtail_cjkcms.egg-info/requires.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-07-03 18:02:33.000000 wagtail-cjkcms-23.7.3/wagtail_cjkcms.egg-info/top_level.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/
+-rw-r--r--   0 grze      (1000) grze      (1000)     8050 2023-08-02 08:53:39.000000 wagtail-cjkcms-23.8.1/CHANGELOG.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/LICENSE
+-rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/MANIFEST.in
+-rw-r--r--   0 grze      (1000) grze      (1000)     4857 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)     1884 2023-08-02 08:54:00.000000 wagtail-cjkcms-23.8.1/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.365078 wagtail-cjkcms-23.8.1/cjkcms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-08-02 08:48:04.000000 wagtail-cjkcms-23.8.1/cjkcms/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.365078 wagtail-cjkcms-23.8.1/cjkcms/api/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/api/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/api/mailchimp.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      173 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/apps.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.365078 wagtail-cjkcms-23.8.1/cjkcms/bin/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/bin/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/bin/cjkcms.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.365078 wagtail-cjkcms-23.8.1/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3288 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/blocks/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    10539 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/blocks/base_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9427 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/blocks/content_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9537 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/blocks/html_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/blocks/layout_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/blocks/searchable_html_block.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.365078 wagtail-cjkcms-23.8.1/cjkcms/draftail/
+-rw-r--r--   0 grze      (1000) grze      (1000)      305 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/draftail/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/draftail/draftail_extensions.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5157 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/draftail/draftail_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3191 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/fields.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.365078 wagtail-cjkcms-23.8.1/cjkcms/finders/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/finders/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2459 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/finders/oembed.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/forms.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1804 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/image_formats.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.345078 wagtail-cjkcms-23.8.1/cjkcms/management/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.365078 wagtail-cjkcms-23.8.1/cjkcms/management/commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/management/commands/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      453 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/management/commands/clear-embeds.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2565 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/management/commands/import-csv.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/management/commands/init-collections.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/management/commands/init-navbar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/management/commands/init-website.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.365078 wagtail-cjkcms-23.8.1/cjkcms/migrations/
+-rw-r--r--   0 grze      (1000) grze      (1000)   216350 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0001_initial.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      668 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1027 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1334 2023-06-01 06:19:54.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      685 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0009_navbar_language.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3479 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0010_filmstrip_filmpanel.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1393 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1466 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/migrations/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.365078 wagtail-cjkcms-23.8.1/cjkcms/models/
+-rw-r--r--   0 grze      (1000) grze      (1000)      232 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/models/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      335 2023-06-01 06:19:54.000000 wagtail-cjkcms-23.8.1/cjkcms/models/admin_sidebar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2356 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/models/cms_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6302 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/models/integration_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    23813 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/models/page_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    15369 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/models/snippet_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    19011 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/models/wagtailsettings_models.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.345078 wagtail-cjkcms-23.8.1/cjkcms/project_template/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/
+-rw-r--r--   0 grze      (1000) grze      (1000)      722 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/.editorconfig
+-rw-r--r--   0 grze      (1000) grze      (1000)      364 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/.gitattributes
+-rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/.gitignore
+-rw-r--r--   0 grze      (1000) grze      (1000)      792 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/blocks/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2141 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/blocks/blocks.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/migrations/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4982 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/migrations/0001_initial.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2047 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/migrations/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/models/
+-rw-r--r--   0 grze      (1000) grze      (1000)      295 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/models/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2819 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/models/cms_models.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.345078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/templates/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.345078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/templates/home/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/templates/home/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2282 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/home/templates/home/blocks/event_presentation.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/manage.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/settings/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/settings/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5312 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/settings/base.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      324 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/settings/dev.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/settings/local.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1595 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/settings/production.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.345078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/static/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/static/css/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/static/css/devsite.css
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/static/js/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/static/js/devsite.js
+-rw-r--r--   0 grze      (1000) grze      (1000)      911 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      438 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/project_name/wsgi.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      123 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/requirements.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/search/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/search/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.345078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/search/templates/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/search/templates/search/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1097 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/search/templates/search/search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1019 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/basic/search/views.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/
+-rw-r--r--   0 grze      (1000) grze      (1000)      245 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/.babelrc
+-rw-r--r--   0 grze      (1000) grze      (1000)      159 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/.browserslistrc
+-rw-r--r--   0 grze      (1000) grze      (1000)      722 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/.editorconfig
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/.eslintrc
+-rw-r--r--   0 grze      (1000) grze      (1000)      364 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/.gitattributes
+-rw-r--r--   0 grze      (1000) grze      (1000)      270 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/.gitignore
+-rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/.nvmrc
+-rw-r--r--   0 grze      (1000) grze      (1000)      182 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/.stylelintrc.json
+-rw-r--r--   0 grze      (1000) grze      (1000)      792 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/
+-rw-r--r--   0 grze      (1000) grze      (1000)      131 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/.gitignore
+-rw-r--r--   0 grze      (1000) grze      (1000)      733 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.345078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/src/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/src/application/
+-rw-r--r--   0 grze      (1000) grze      (1000)      574 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/src/application/app.js
+-rw-r--r--   0 grze      (1000) grze      (1000)      226 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/src/application/app2.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/src/components/
+-rw-r--r--   0 grze      (1000) grze      (1000)       41 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/src/components/sidebar.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/src/styles/
+-rw-r--r--   0 grze      (1000) grze      (1000)      380 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/src/styles/index.scss
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/vendors/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/vendors/.gitkeep
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/vendors/images/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/vendors/images/.gitkeep
+-rw-r--r--   0 grze      (1000) grze      (1000)   273404 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/vendors/images/sample.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)   238213 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/vendors/images/webpack.png
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/webpack/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1473 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/webpack/webpack.common.js
+-rw-r--r--   0 grze      (1000) grze      (1000)     1716 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/webpack/webpack.config.dev.js
+-rw-r--r--   0 grze      (1000) grze      (1000)      986 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/webpack/webpack.config.prod.js
+-rw-r--r--   0 grze      (1000) grze      (1000)     1485 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/frontend/webpack/webpack.config.watch.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/blocks/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2141 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/blocks/blocks.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/migrations/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4982 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/migrations/0001_initial.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2047 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/migrations/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/models/
+-rw-r--r--   0 grze      (1000) grze      (1000)      295 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/models/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2819 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/models/cms_models.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.345078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/templates/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.345078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/templates/home/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.375078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/templates/home/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2282 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/home/templates/home/blocks/event_presentation.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/manage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)   683340 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/package-lock.json
+-rw-r--r--   0 grze      (1000) grze      (1000)     1741 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/package.json
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/settings/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/settings/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5312 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/settings/base.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      324 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/settings/dev.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/settings/local.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1595 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/settings/production.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.355078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/static/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/static/css/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/static/css/devsite.css
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/static/js/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/static/js/devsite.js
+-rw-r--r--   0 grze      (1000) grze      (1000)      911 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      438 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/project_name/wsgi.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      123 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/requirements.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/search/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/search/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.355078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/search/templates/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/search/templates/search/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1097 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/search/templates/search/search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1019 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/project_template/webpack/search/views.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/search_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9824 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/settings.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.355078 wagtail-cjkcms-23.8.1/cjkcms/static/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.355078 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/
+-rw-r--r--   0 grze      (1000) grze      (1000)    93729 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/bootstrap-icons.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    49971 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/bootstrap-icons.json
+-rw-r--r--   0 grze      (1000) grze      (1000)    55169 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/fonts/
+-rw-r--r--   0 grze      (1000) grze      (1000)   164360 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
+-rw-r--r--   0 grze      (1000) grze      (1000)   121340 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/css/
+-rw-r--r--   0 grze      (1000) grze      (1000)      846 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/css/cjkcms-admin.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/css/cjkcms-editor.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     4614 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/css/cjkcms-front.css
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.355078 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/avatars/
+-rw-r--r--   0 grze      (1000) grze      (1000)      535 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/avatars/default.png
+-rw-r--r--   0 grze      (1000) grze      (1000)      384 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/avatars/default.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/icons/quote.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/logos/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4166 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)     4218 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/patterns/
+-rw-r--r--   0 grze      (1000) grze      (1000)    47935 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    31707 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    38190 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/js/
+-rw-r--r--   0 grze      (1000) grze      (1000)      444 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/js/cjkcms-editor.js
+-rw-r--r--   0 grze      (1000) grze      (1000)     5565 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/js/cjkcms-front.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/static/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cookieconsent/cookieconsent.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/static/cookieconsent/cookieconsent.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/templates/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/404.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/500.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.385078 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.395078 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1443 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/accordion_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      974 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/article_block_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1132 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      188 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/base_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2505 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/base_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      740 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/button_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      746 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      856 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_blurb.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      730 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_head.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      771 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      990 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_img.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2618 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_landing1.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_landing2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      450 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      276 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/carousel_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      406 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/column_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/document_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/download_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      103 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/embed_video_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       95 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/external_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1484 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/film_strip_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      424 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/grid_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/h1_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/h2_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/h3_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      790 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/hero_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/image_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      627 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/image_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1020 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/modal_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      164 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/page_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      787 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      642 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      956 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      858 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      610 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      244 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pricelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      353 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/quote_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      852 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      998 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      216 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       91 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/rich_text_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1095 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/table_block.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.395078 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/cookieconsent/languages.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.395078 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/formfields/
+-rw-r--r--   0 grze      (1000) grze      (1000)      267 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/formfields/date.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      416 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/formfields/datetime.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.395078 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/formfields/mailchimp/
+-rw-r--r--   0 grze      (1000) grze      (1000)     9267 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     6469 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      264 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/formfields/time.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.395078 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      465 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/align-left.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/check-square-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/columns.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      359 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/desktop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      571 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/font.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      292 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/google.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      813 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      666 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/hashtag.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      840 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/header.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/list-alt.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      459 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/map.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      448 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/newspaper-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      721 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      635 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/recycle.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      174 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/stop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      505 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/th-large.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      762 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/universal-access.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      548 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/usd.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      225 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/window-maximize.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      199 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/window-minimize.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.395078 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      689 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      579 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/classifier_nav.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/codered_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      268 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/form_honeypot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1061 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/pagination.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.395078 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/stream_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      532 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2002 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/article_index_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2031 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/article_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1018 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/article_page.search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     8961 2023-08-02 08:47:02.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/base.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      248 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/form_page_landing.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/home_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      491 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/page.mini.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2610 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      582 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/search_result.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/web_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/web_page_notitle.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      122 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/robots.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1943 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      430 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/footer.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2027 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2712 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/navbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      836 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      386 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/navbar_search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/tracking_g3.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      832 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      694 2023-08-02 08:47:12.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/tracking_matomo.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      230 2023-08-02 08:47:09.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/tracking_matomo_noscript.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/widgets/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1444 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.355078 wagtail-cjkcms-23.8.1/cjkcms/templates/wagtailadmin/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/cjkcms/templates/wagtailadmin/block_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      839 2023-06-05 15:04:30.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      550 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/wagtailadmin/block_forms/struct.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/cjkcms/templates/wagtailadmin/shared/
+-rw-r--r--   0 grze      (1000) grze      (1000)      885 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/cjkcms/templatetags/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templatetags/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      327 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templatetags/auth_extras.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6845 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/templatetags/cjkcms_tags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4962 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templatetags/friendly_loader.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templatetags/gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/templatetags/txtutils_tags.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/cjkcms/tests/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/tests/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4226 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/tests/test_articlepages.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3506 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/tests/test_bin.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2629 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/tests/test_gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4760 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/tests/test_search_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/tests/test_settings.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3762 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/tests/test_templatetags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2673 2023-08-02 08:43:23.000000 wagtail-cjkcms-23.8.1/cjkcms/tests/test_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1520 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/tests/test_webpage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/utils.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4488 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/views.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6557 2023-06-01 06:19:54.000000 wagtail-cjkcms-23.8.1/cjkcms/wagtail_hooks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1531 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/cjkcms/widgets.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/docs/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/docs/how-to/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1481 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/docs/how-to/oembed_finder.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      537 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/docs/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     5520 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/docs/installation.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/docs/management_commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)      318 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/docs/management_commands/clear-embeds.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      193 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/docs/management_commands/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      420 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/docs/management_commands/init-collections.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      936 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/docs/quick-start.md
+-rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/docs/requirements.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)     1220 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/docs/why-another-cms.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     2154 2023-08-02 09:07:36.000000 wagtail-cjkcms-23.8.1/pyproject.toml
+-rw-r--r--   0 grze      (1000) grze      (1000)      230 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/setup.cfg
+-rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-05-23 09:02:14.000000 wagtail-cjkcms-23.8.1/setup.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-08-02 09:07:53.405078 wagtail-cjkcms-23.8.1/wagtail_cjkcms.egg-info/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4857 2023-08-02 09:07:53.000000 wagtail-cjkcms-23.8.1/wagtail_cjkcms.egg-info/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)    14186 2023-08-02 09:07:53.000000 wagtail-cjkcms-23.8.1/wagtail_cjkcms.egg-info/SOURCES.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-08-02 09:07:53.000000 wagtail-cjkcms-23.8.1/wagtail_cjkcms.egg-info/dependency_links.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-08-02 09:07:53.000000 wagtail-cjkcms-23.8.1/wagtail_cjkcms.egg-info/entry_points.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)      189 2023-08-02 09:07:53.000000 wagtail-cjkcms-23.8.1/wagtail_cjkcms.egg-info/requires.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-08-02 09:07:53.000000 wagtail-cjkcms-23.8.1/wagtail_cjkcms.egg-info/top_level.txt
```

### Comparing `wagtail-cjkcms-23.7.3/CHANGELOG.md` & `wagtail-cjkcms-23.8.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -195,8 +195,12 @@
 - Added ButtonLink title in collapsed view
 
 # 23.7.2 (2023-07-03)
 - Fixed leftover {{ page }} in base.html
 
 # 23.7.4 (2023-07-03)
 - Removed Universal Google Analytics
-- Added support for Matomo Analytics
+- Added support for Matomo Analytics
+
+# 23.8.1 (2023-08-02)
+- Break down matomo tracking code snippet into two, moving the "noscript" section to the bottom of html file
+- Add instructions for using pytest excluding the project_template folder
```

### Comparing `wagtail-cjkcms-23.7.3/LICENSE` & `wagtail-cjkcms-23.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/README.md` & `wagtail-cjkcms-23.8.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,9 +19,13 @@
 ## Testing
 ### running pytest from devsite folder:
 pytest ../wagtail-cjkcms/cjkcms --ds=devsite.settings.dev --doctest-modules --durations=0
 
 ### running pytest from testproject folder:
 pytest ../cjkcms --ds=testproject.settings.dev --doctest-modules --durations=0
 
+### running pytest from testproject folder, excluding project_template folder:
+pytest ../cjkcms --ds=testproject.settings.dev --doctest-modules --durations=0 --ignore=../cjkcm
+s/project_template
+
 ## Contact & support
 Please use [Github's Issue Tracker](https://github.com/cjkpl/wagtail-cjkcms/issues) to report bugs, request features, or request support.
```

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/api/mailchimp.py` & `wagtail-cjkcms-23.8.1/cjkcms/api/mailchimp.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/bin/cjkcms.py` & `wagtail-cjkcms-23.8.1/cjkcms/bin/cjkcms.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/blocks/__init__.py` & `wagtail-cjkcms-23.8.1/cjkcms/blocks/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     CarouselBlock,
     FilmStripBlock,
     ImageGalleryBlock,
     ModalBlock,
     NavDocumentLinkWithSubLinkBlock,
     NavExternalLinkWithSubLinkBlock,
     NavPageLinkWithSubLinkBlock,
+    NavSocialLinkBock,
     PriceListBlock,
     ReusableContentBlock,
 )
 from .layout_blocks import CardGridBlock, GridBlock, HeroBlock
 from cjkcms.settings import cms_settings
 
 # Collections of blocks commonly used together.
@@ -75,14 +76,15 @@
     ("reusable_content", ReusableContentBlock()),
 ]
 
 NAVIGATION_STREAMBLOCKS = [
     ("page_link", NavPageLinkWithSubLinkBlock()),
     ("external_link", NavExternalLinkWithSubLinkBlock()),
     ("document_link", NavDocumentLinkWithSubLinkBlock()),
+    ("social_link", NavSocialLinkBock()),
 ]
 
 BASIC_LAYOUT_STREAMBLOCKS = [
     ("row", GridBlock(HTML_STREAMBLOCKS)),
     (
         "html",
         SearchableHTMLBlock(icon="code", form_classname="monospace", label=_("HTML")),
```

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/blocks/base_blocks.py` & `wagtail-cjkcms-23.8.1/cjkcms/blocks/base_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/blocks/content_blocks.py` & `wagtail-cjkcms-23.8.1/cjkcms/blocks/content_blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -230,24 +230,46 @@
 
     class Meta:
         template = "cjkcms/blocks/document_link_block.html"
         label = _("Document Link")
         label_format = "{display_text} (Document Link)"
 
 
+class NavSocialLinkBock(NavBaseLinkBlock):
+    """
+    Social link. Renders a link selected from a list of social media types.
+    Data taken from SocialMediaSettings.
+    """
+
+    medium = blocks.ChoiceBlock(
+        choices=cms_settings.CJKCMS_SOCIAL_MEDIA_CHOICES,
+        default=cms_settings.CJKCMS_SOCIAL_MEDIA_DEFAULT,
+        required=False,
+        label=_("Social medium"),
+        help_text=_(
+            "Make sure to provide links to soc media in Settings->SocialMedia."
+        ),
+    )
+
+    class Meta:
+        label = _("Social media link")
+        label_format = "{display_text} (Social media link)"
+
+
 class NavSubLinkBlock(BaseBlock):
     """
     Streamblock for rendering nested sub-links.
     """
 
     sub_links = blocks.StreamBlock(
         [
             ("page_link", NavPageLinkBlock()),
             ("external_link", NavExternalLinkBlock()),
             ("document_link", NavDocumentLinkBlock()),
+            ("social_link", NavSocialLinkBock()),
         ],
         required=False,
         label=_("Sub-links"),
     )
 
 
 class NavExternalLinkWithSubLinkBlock(NavSubLinkBlock, NavExternalLinkBlock):
```

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/blocks/html_blocks.py` & `wagtail-cjkcms-23.8.1/cjkcms/blocks/html_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/blocks/layout_blocks.py` & `wagtail-cjkcms-23.8.1/cjkcms/blocks/layout_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/draftail/draftail_extensions.py` & `wagtail-cjkcms-23.8.1/cjkcms/draftail/draftail_extensions.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/draftail/draftail_icons.py` & `wagtail-cjkcms-23.8.1/cjkcms/draftail/draftail_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/fields.py` & `wagtail-cjkcms-23.8.1/cjkcms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/finders/oembed.py` & `wagtail-cjkcms-23.8.1/cjkcms/finders/oembed.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/image_formats.py` & `wagtail-cjkcms-23.8.1/cjkcms/image_formats.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/management/commands/import-csv.py` & `wagtail-cjkcms-23.8.1/cjkcms/management/commands/import-csv.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/management/commands/init-collections.py` & `wagtail-cjkcms-23.8.1/cjkcms/management/commands/init-collections.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/management/commands/init-navbar.py` & `wagtail-cjkcms-23.8.1/cjkcms/management/commands/init-navbar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/management/commands/init-website.py` & `wagtail-cjkcms-23.8.1/cjkcms/management/commands/init-website.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0001_initial.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0008_alter_layoutsettings_navbar_langselector.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0009_navbar_language.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0009_navbar_language.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0010_filmstrip_filmpanel.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0010_filmstrip_filmpanel.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0011_cjkcmspage_related_classifier_term_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py` & `wagtail-cjkcms-23.8.1/cjkcms/migrations/0012_remove_analyticssettings_ga_tracking_id_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/models/cms_models.py` & `wagtail-cjkcms-23.8.1/cjkcms/models/cms_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/models/integration_models.py` & `wagtail-cjkcms-23.8.1/cjkcms/models/integration_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/models/page_models.py` & `wagtail-cjkcms-23.8.1/cjkcms/models/page_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/models/snippet_models.py` & `wagtail-cjkcms-23.8.1/cjkcms/models/snippet_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/models/wagtailsettings_models.py` & `wagtail-cjkcms-23.8.1/cjkcms/models/wagtailsettings_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/settings.py` & `wagtail-cjkcms-23.8.1/cjkcms/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,14 +254,24 @@
             "centre-align",
             "left-align",
             "right-align",
         ],
         "minimal": ["bold", "italic", "link"],
     }
 
+    CJKCMS_SOCIAL_MEDIA_DEFAULT = "twitter"
+    CJKCMS_SOCIAL_MEDIA_CHOICES = [
+        ("facebook", "Facebook"),
+        ("twitter", "Twitter"),
+        ("instagram", "Instagram"),
+        ("linkedin", "LinkedIn"),
+        ("youtube", "YouTube"),
+        ("vimeo", "Vimeo"),
+    ]
+
     def __getattribute__(self, attr: str):
         # First load from Django settings.
         # If it does not exist, load from _DefaultSettings.
         try:
             return getattr(settings, attr)
         except AttributeError:
             return super().__getattribute__(attr)
```

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/bootstrap-icons.css` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/bootstrap-icons.json` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/bootstrap-icons.scss` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/css/cjkcms-admin.css` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/css/cjkcms-admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/css/cjkcms-editor.css` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/css/cjkcms-editor.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/css/cjkcms-front.css` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/css/cjkcms-front.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/avatars/default.png` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/avatars/default.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/icons/quote.svg` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/patterns/pattern1.jpg` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/patterns/pattern2.jpg` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/images/patterns/pattern3.jpg` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cjkcms/js/cjkcms-front.js` & `wagtail-cjkcms-23.8.1/cjkcms/static/cjkcms/js/cjkcms-front.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cookieconsent/cookieconsent.css` & `wagtail-cjkcms-23.8.1/cjkcms/static/cookieconsent/cookieconsent.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/static/cookieconsent/cookieconsent.js` & `wagtail-cjkcms-23.8.1/cjkcms/static/cookieconsent/cookieconsent.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/404.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/404.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/500.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/500.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/accordion_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/accordion_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/article_block_card.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/article_block_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/article_masonry_card.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/base_link_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/base_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/button_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/button_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_blurb.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_blurb.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_foot.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_head.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_head.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_head_foot.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_horizontal.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_horizontal2.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_img.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_img.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_landing1.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_landing1.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/card_landing2.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/card_landing2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/carousel_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/carousel_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/download_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/download_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/film_strip_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/film_strip_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/hero_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/hero_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/image_gallery_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/image_link_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/image_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/modal_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/modal_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pagepreview_card.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/blocks/table_block.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/blocks/table_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/cookieconsent/languages.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/cookieconsent/languages.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/check-square-o.svg` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/check-square-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/font.svg` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/font.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/hashtag.svg` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/hashtag.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/header.svg` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/header.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/list-alt.svg` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/list-alt.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/puzzle-piece.svg` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/recycle.svg` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/recycle.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/universal-access.svg` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/universal-access.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/icons/usd.svg` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/icons/usd.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/classifier_nav.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/classifier_nav.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/pagination.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/article_index_page.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/article_index_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/article_page.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/article_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/article_page.search.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/article_page.search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/base.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -184,11 +184,16 @@
                             languages:
                                 {% include "cjkcms/cookieconsent/languages.html" with settings=settings.cjkcms.AnalyticsSettings %}
                         });
                     });
                 </script>
             {% endif %}
         {% endblock %}
-        
+        {% block tracking_bottom %}
+            {% if settings.cjkcms.AnalyticsSettings.matomo_site_id and settings.cjkcms.AnalyticsSettings.matomo_hostname %}
+                {% include "cjkcms/snippets/tracking_matomo_noscript.html" %}
+            {% endif %}
+        {% endblock %}
+
         {% include "wagtailseo/struct_data.html" %}
     </body>
 </html>
```

#### html2text {}

```diff
@@ -67,8 +67,12 @@
 {% block footer %}{% endblock %} {% block required_scripts %} {% endblock %} {%
 block frontend_scripts %} {% include "cjkcms/snippets/frontend_scripts.html" %}
 {% endblock %} {% block cjkcms_scripts %}
  {% endblock %} {% block custom_scripts %} {# Leave blank for client sites to
 implement. #} {#
  #} {% endblock %} {% block cookie_consent_scripts %} {% if
 settings.cjkcms.AnalyticsSettings.cookie_consent %}
- {% endif %} {% endblock %} {% include "wagtailseo/struct_data.html" %}
+ {% endif %} {% endblock %} {% block tracking_bottom %} {% if
+settings.cjkcms.AnalyticsSettings.matomo_site_id and
+settings.cjkcms.AnalyticsSettings.matomo_hostname %} {% include "cjkcms/
+snippets/tracking_matomo_noscript.html" %} {% endif %} {% endblock %} {%
+include "wagtailseo/struct_data.html" %}
```

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/search.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/search_result.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/search_result.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/pages/web_page.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/pages/web_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/bottom_corner_lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/frontend_assets.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/frontend_scripts.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/navbar.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/navbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/navbar_lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/snippets/tracking_g4.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/wagtailadmin/block_forms/struct.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/wagtailadmin/block_forms/struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html` & `wagtail-cjkcms-23.8.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templatetags/cjkcms_tags.py` & `wagtail-cjkcms-23.8.1/cjkcms/templatetags/cjkcms_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,7 +243,12 @@
         return class_type.__class__.search_name_plural
     elif hasattr(class_type.__class__, "_meta") and hasattr(
         class_type.__class__._meta, "verbose_name_plural"
     ):
         return class_type.__class__._meta.verbose_name_plural
     else:
         return f"{class_type.__class__.__name__}s"
+
+
+@register.simple_tag
+def define(val=None):
+    return val
```

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templatetags/friendly_loader.py` & `wagtail-cjkcms-23.8.1/cjkcms/templatetags/friendly_loader.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templatetags/gravatar.py` & `wagtail-cjkcms-23.8.1/cjkcms/templatetags/gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/templatetags/txtutils_tags.py` & `wagtail-cjkcms-23.8.1/cjkcms/templatetags/txtutils_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/tests/test_articlepages.py` & `wagtail-cjkcms-23.8.1/cjkcms/tests/test_articlepages.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/tests/test_bin.py` & `wagtail-cjkcms-23.8.1/cjkcms/tests/test_bin.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/tests/test_gravatar.py` & `wagtail-cjkcms-23.8.1/cjkcms/tests/test_gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/tests/test_search_blocks.py` & `wagtail-cjkcms-23.8.1/cjkcms/tests/test_search_blocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import pytest
 
 from wagtail.models import Page
 from django.urls import reverse
-from django.test import Client, TestCase
+from django.test import Client, TestCase, override_settings
 
 from cjkcms.models.cms_models import ArticlePage
 
 
+@override_settings(
+    STATICFILES_STORAGE="django.contrib.staticfiles.storage.StaticFilesStorage"
+)
 @pytest.mark.django_db
 class TestSearchBlocks(TestCase):
     """
     CjkCMS content blocks should be searchable.
     For each content block, create a page with that content block and some text,
     confirm that the search returns the page.
     """
```

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/tests/test_settings.py` & `wagtail-cjkcms-23.8.1/cjkcms/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/tests/test_templatetags.py` & `wagtail-cjkcms-23.8.1/cjkcms/tests/test_templatetags.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
+from datetime import datetime
 
 from django.template import engines
 from django.test import TestCase
 from wagtail.models import Site
+
 from cjkcms.models import AdobeApiSettings
-from datetime import datetime
 
 django_engine = engines["django"]
 html_id_re = re.compile(r"^[A-Za-z][A-Za-z0-9_:.-]*$")
 
 version_re = re.compile(
     r"^(\d+!)?(\d+)(\.\d+)+([\.\-\_])?((a(lpha)?|b(eta)?|c|r(c|ev)?|pre(view)?)\d*)?(\.?(post|dev)\d*)?$"  # noqa: E501
 )
@@ -77,22 +78,28 @@
             [".png", ".jpg", ".webp", ".svg"],
             f"Django setting BRAND_LOGO_LONG does not seem to return one of [png,jpg,webp,svg]: {rt}",  # noqa: E501
         )
 
     def test_AdobeApiKeyInTemplate(self):
         site = Site.objects.filter(is_default_site=True)[0]
         adobe_api_key = AdobeApiSettings.for_site(site=site)
-        adobe_api_key.adobe_embed_id = "test_key"
+        adobe_api_key.adobe_embed_id = "test_key"  # type: ignore
         adobe_api_key.save()
 
         rt = django_engine.from_string(
             "{% load wagtailsettings_tags %}{% get_settings use_default_site=True %}{{ settings.cjkcms.AdobeApiSettings.adobe_embed_id }}"  # noqa: E501
         ).render(None)
         self.assertEqual(
             rt, "test_key", "Adobe API key not returned in template context"
         )
 
     def test_current_year(self):
         rt = django_engine.from_string(
             "{% load cjkcms_tags %}{% current_year %}"
         ).render(None)
         self.assertEqual(rt, str(datetime.now().year), "Current year not returned")
+
+    def test_define_tag(self):
+        rt = django_engine.from_string(
+            "{% load cjkcms_tags %}{% define 'test' %}{{ test }}"
+        ).render(None)
+        self.assertEqual(rt, "test", "define tag did not return 'test'")
```

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/tests/test_urls.py` & `wagtail-cjkcms-23.8.1/cjkcms/tests/test_urls.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import pytest
-import unittest
 
 from django.urls import reverse
-from django.test import Client
-from django.test.utils import override_settings
+from django.test import Client, TestCase, override_settings
 
 from wagtail.models import Site
 from wagtail.images.tests.utils import Image, get_test_image_file
 
 from cjkcms.models import LayoutSettings
 
-# from cjkcms.tests.testapp.models import EventPage, EventIndexPage, EventOccurrence
-
 
+@override_settings(
+    STATICFILES_STORAGE="django.contrib.staticfiles.storage.StaticFilesStorage"
+)
 @pytest.mark.django_db
-class TestSiteURLs(unittest.TestCase):
+class TestSiteURLs(TestCase):
     def setUp(self):
         self.client = Client()
 
     # @TODO: this fails, even though in browser tests returns 404
     @override_settings(DEBUG=False)
     def test_404(self):
         response = self.client.get("/testing/404/page/")
@@ -53,22 +52,22 @@
             follow=False,
         )
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.context["results"], None)
 
 
 @pytest.mark.django_db
-class TestFavicon(unittest.TestCase):
+class TestFavicon(TestCase):
     def test_404(self):
         client = Client()
         # Get the default site
         site = Site.objects.filter(is_default_site=True)[0]
         # Ensure the favicon is blank
         layout = LayoutSettings.for_site(site)
-        layout.favicon = None
+        layout.favicon = None  # type: ignore
         layout.save()
         # Expect a 404
         response = client.get("/favicon.ico")
         self.assertEqual(response.status_code, 404)
 
     def test_301(self):
         client = Client()
@@ -76,12 +75,12 @@
         site = Site.objects.filter(is_default_site=True)[0]
         # Set a dummy favicon
         layout = LayoutSettings.for_site(site)
         img = Image.objects.create(
             title="Test image",
             file=get_test_image_file(),
         )
-        layout.favicon = img
+        layout.favicon = img  # type: ignore
         layout.save()
         # Expect a 301 redirect
         response = client.get("/favicon.ico")
         self.assertEqual(response.status_code, 301)
```

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/tests/test_webpage.py` & `wagtail-cjkcms-23.8.1/cjkcms/tests/test_webpage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/utils.py` & `wagtail-cjkcms-23.8.1/cjkcms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/views.py` & `wagtail-cjkcms-23.8.1/cjkcms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/wagtail_hooks.py` & `wagtail-cjkcms-23.8.1/cjkcms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/cjkcms/widgets.py` & `wagtail-cjkcms-23.8.1/cjkcms/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/docs/how-to/oembed_finder.md` & `wagtail-cjkcms-23.8.1/docs/how-to/oembed_finder.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/docs/index.md` & `wagtail-cjkcms-23.8.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/docs/installation.md` & `wagtail-cjkcms-23.8.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/docs/quick-start.md` & `wagtail-cjkcms-23.8.1/docs/quick-start.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.7.3/docs/why-another-cms.md` & `wagtail-cjkcms-23.8.1/docs/why-another-cms.md`

 * *Files identical despite different names*

