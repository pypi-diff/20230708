# Comparing `tmp/khoj_assistant-0.7.2.dev4.tar.gz` & `tmp/khoj_assistant-0.7.2.dev42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jul  4 05:28:18 2023, max compression
+gzip compressed data, last modified: Sat Jul  8 03:36:16 2023, max compression
```

## Comparing `khoj_assistant-0.7.2.dev4.tar` & `khoj_assistant-0.7.2.dev42.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/__init__.py
--rw-r--r--   0        0        0    10727 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/configure.py
--rw-r--r--   0        0        0     5282 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3910 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    15023 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    13551 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6930 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     6739 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    19388 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3583 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1813 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0      549 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0   205167 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6056 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4065 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13517 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5392 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    18345 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     4646 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7560 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11054 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2040 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2385 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2500 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6852 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4136 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/LICENSE
--rw-r--r--   0        0        0    23342 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/README.md
--rw-r--r--   0        0        0     2792 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/pyproject.toml
--rw-r--r--   0        0        0    25706 2023-07-04 05:28:18.000000 khoj_assistant-0.7.2.dev4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11048 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/configure.py
+-rw-r--r--   0        0        0     5247 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3910 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    17859 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    14688 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6930 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     7322 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    18700 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3660 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1813 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     4829 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     3991 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     8304 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13517 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5397 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    20657 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/routers/api.py
+-rw-r--r--   0        0        0      167 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     4646 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7566 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11054 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2040 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2396 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2500 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6889 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4136 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/LICENSE
+-rw-r--r--   0        0        0    24572 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/README.md
+-rw-r--r--   0        0        0     2792 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/pyproject.toml
+-rw-r--r--   0        0        0    26937 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/PKG-INFO
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/configure.py` & `khoj_assistant-0.7.2.dev42/src/khoj/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,20 +63,22 @@
 
     app.mount("/static", StaticFiles(directory=constants.web_directory), name="static")
     app.include_router(api, prefix="/api")
     app.include_router(api_beta, prefix="/api/beta")
     app.include_router(web_client)
 
 
-@schedule.repeat(schedule.every(61).minutes)
-def update_search_index():
-    state.search_index_lock.acquire()
-    state.model = configure_search(state.model, state.config, regenerate=False)
-    state.search_index_lock.release()
-    logger.info("📬 Search index updated via Scheduler")
+if not state.demo:
+
+    @schedule.repeat(schedule.every(61).minutes)
+    def update_search_index():
+        state.search_index_lock.acquire()
+        state.model = configure_search(state.model, state.config, regenerate=False)
+        state.search_index_lock.release()
+        logger.info("📬 Search index updated via Scheduler")
 
 
 def configure_search_types(config: FullConfig):
     # Extract core search types
     core_search_types = {e.name: e.value for e in SearchType}
     # Extract configured plugin search types
     plugin_search_types = {}
@@ -199,15 +201,15 @@
         # Load Metadata Logs from Conversation Logfile
         with conversation_logfile.open("r") as f:
             conversation_processor.meta_log = json.load(f)
         logger.debug(f"Loaded conversation logs from {conversation_logfile}")
     else:
         # Initialize Conversation Logs
         conversation_processor.meta_log = {}
-        conversation_processor.chat_session = ""
+        conversation_processor.chat_session = []
 
     return conversation_processor
 
 
 @schedule.repeat(schedule.every(17).minutes)
 def save_chat_session():
     # No need to create empty log file
@@ -219,42 +221,49 @@
     ):
         return
 
     # Summarize Conversation Logs for this Session
     chat_session = state.processor_config.conversation.chat_session
     openai_api_key = state.processor_config.conversation.openai_api_key
     conversation_log = state.processor_config.conversation.meta_log
-    model = state.processor_config.conversation.model
+    chat_model = state.processor_config.conversation.chat_model
     session = {
-        "summary": summarize(chat_session, summary_type="chat", model=model, api_key=openai_api_key),
+        "summary": summarize(chat_session, model=chat_model, api_key=openai_api_key),
         "session-start": conversation_log.get("session", [{"session-end": 0}])[-1]["session-end"],
         "session-end": len(conversation_log["chat"]),
     }
     if "session" in conversation_log:
         conversation_log["session"].append(session)
     else:
         conversation_log["session"] = [session]
 
     # Save Conversation Metadata Logs to Disk
     conversation_logfile = resolve_absolute_path(state.processor_config.conversation.conversation_logfile)
     conversation_logfile.parent.mkdir(parents=True, exist_ok=True)  # create conversation directory if doesn't exist
     with open(conversation_logfile, "w+", encoding="utf-8") as logfile:
         json.dump(conversation_log, logfile, indent=2)
 
-    state.processor_config.conversation.chat_session = None
+    state.processor_config.conversation.chat_session = []
     logger.info("📩 Saved current chat session to conversation logs")
 
 
 @schedule.repeat(schedule.every(59).minutes)
 def upload_telemetry():
     if not state.config or not state.config.app.should_log_telemetry or not state.telemetry:
         message = "📡 No telemetry to upload" if not state.telemetry else "📡 Telemetry logging disabled"
         logger.debug(message)
         return
 
     try:
         logger.debug(f"📡 Upload usage telemetry to {constants.telemetry_server}:\n{state.telemetry}")
+        for log in state.telemetry:
+            for field in log:
+                # Check if the value for the field is JSON serializable
+                try:
+                    json.dumps(log[field])
+                except TypeError:
+                    log[field] = str(log[field])
         requests.post(constants.telemetry_server, json=state.telemetry)
     except Exception as e:
         logger.error(f"📡 Error uploading telemetry: {e}")
     else:
         state.telemetry = []
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/main.py` & `khoj_assistant-0.7.2.dev42/src/khoj/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,16 @@
     fh = logging.FileHandler(state.config_file.parent / "khoj.log", encoding="utf-8")
     fh.setLevel(logging.DEBUG)
     logger.addHandler(fh)
 
     logger.info("🌘 Starting Khoj")
 
     if not args.gui:
-        if not state.demo:
-            # Setup task scheduler
-            poll_task_scheduler()
+        # Setup task scheduler
+        poll_task_scheduler()
 
         # Start Server
         configure_server(args, required=False)
         configure_routes(app)
         start_server(app, host=args.host, port=args.port, socket=args.socket)
     else:
         # Setup GUI
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/chat.html`

 * *Files 12% similar despite different names*

```diff
@@ -47,46 +47,94 @@
 
             renderMessage(message+references, by, dt);
         }
 
         function chat() {
             // Extract required fields for search from form
             let query = document.getElementById("chat-input").value.trim();
+            let results_count = localStorage.getItem("khojResultsCount") || 5;
             console.log(`Query: ${query}`);
 
             // Short circuit on empty query
             if (query.length === 0)
                 return;
 
             // Add message by user to chat body
             renderMessage(query, "you");
             document.getElementById("chat-input").value = "";
 
             // Generate backend API URL to execute query
-            let url = `/api/chat?q=${encodeURIComponent(query)}&client=web`;
+            let url = `/api/chat?q=${encodeURIComponent(query)}&n=${results_count}&client=web`;
 
-            // Call specified Khoj API
+            let chat_body = document.getElementById("chat-body");
+            let new_response = document.createElement("div");
+            new_response.classList.add("chat-message", "khoj");
+            new_response.attributes["data-meta"] = "🏮 Khoj at " + formatDate(new Date());
+            chat_body.appendChild(new_response);
+
+            let new_response_text = document.createElement("div");
+            new_response_text.classList.add("chat-message-text", "khoj");
+            new_response.appendChild(new_response_text);
+
+            // Temporary status message to indicate that Khoj is thinking
+            new_response_text.innerHTML = "🤔";
+            document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
+
+            // Call specified Khoj API which returns a streamed response of type text/plain
             fetch(url)
-                .then(response => response.json())
-                .then(data => {
-                    // Render message by Khoj to chat body
-                    console.log(data.response);
-                    renderMessageWithReference(data.response, "khoj", data.context);
+                .then(response => {
+                    const reader = response.body.getReader();
+                    const decoder = new TextDecoder();
+
+                    function readStream() {
+                        reader.read().then(({ done, value }) => {
+                            if (done) {
+                                return;
+                            }
+
+                            // Decode message chunk from stream
+                            const chunk = decoder.decode(value, { stream: true });
+                            if (chunk.includes("### compiled references:")) {
+                                const additionalResponse = chunk.split("### compiled references:")[0];
+                                new_response_text.innerHTML += additionalResponse;
+
+                                const rawReference = chunk.split("### compiled references:")[1];
+                                const rawReferenceAsJson = JSON.parse(rawReference);
+                                let polishedReference = rawReferenceAsJson.map((reference, index) => generateReference(reference, index))
+                                    .join("<sup>,</sup>");
+
+                                new_response_text.innerHTML += polishedReference;
+                                document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
+                            } else {
+                                // Display response from Khoj
+                                if (new_response_text.innerHTML === "🤔") {
+                                    // Clear temporary status message
+                                    new_response_text.innerHTML = "";
+                                }
+                                new_response_text.innerHTML += chunk;
+                                readStream();
+                            }
+
+                            // Scroll to bottom of chat window as chat response is streamed
+                            document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
+                        });
+                    }
+                    readStream();
                 });
         }
 
         function incrementalChat(event) {
             // Send chat message on 'Enter'
             if (event.key === 'Enter') {
                 chat();
             }
         }
 
         window.onload = function () {
-            fetch('/api/chat?client=web')
+            fetch('/api/chat/init?client=web')
                 .then(response => response.json())
                 .then(data => {
                     if (data.detail) {
                         // If the server returns a 500 error with detail, render it as a message.
                         renderMessage("Hi 👋🏾, to get started <br/>1. Get your <a class='inline-chat-link' href='https://platform.openai.com/account/api-keys'>OpenAI API key</a><br/>2. Save it in the Khoj <a class='inline-chat-link' href='/config/processor/conversation'>chat settings</a> <br/>3. Click Configure on the Khoj <a class='inline-chat-link' href='/config'>settings page</a>", "khoj");
 
                         // Disable chat input field and update placeholder text
@@ -380,15 +428,15 @@
             color: black;
             text-decoration: none;
         }
     </style>
     <script>
         var khojBannerSubmit = document.getElementById("khoj-banner-submit");
 
-        khojBannerSubmit.addEventListener("click", function(event) {
+        khojBannerSubmit?.addEventListener("click", function(event) {
             event.preventDefault();
             var email = document.getElementById("khoj-banner-email").value;
             fetch("https://lantern.khoj.dev/beta/users/", {
                     method: "POST",
                     body: JSON.stringify({
                         email: email
                     }),
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/config.html`

 * *Files 18% similar despite different names*

```diff
@@ -165,14 +165,18 @@
                         </button>
                     </div>
                 {% endif %}
             </div>
         </div>
     </div>
     <div class="section">
+        <div id="results-count">
+            <label for="results-count-slider">Results Count: <span id="results-count-value">5</span></label>
+            <input type="range" id="results-count-slider" name="results-count-slider" min="1" max="10" step="1" value="5">
+        </div>
         <div id="status" style="display: none;"></div>
         <button id="configure" type="submit">⚙️ Configure</button>
         <button id="reinitialize" type="submit">🔄 Reinitialize</button>
     </div>
 </div>
 <script>
     function clearContentType(content_type) {
@@ -272,9 +276,29 @@
             console.error('Error:', error);
             document.getElementById("status").innerHTML = "Unable to reinitialize. Raise issue on Khoj Discord or Github.";
             document.getElementById("status").style.display = "block";
             reinitialize.disabled = false;
             reinitialize.innerHTML = "🔄 Reinitialize";
         });
     });
+
+    // Setup the results count slider
+    const resultsCountSlider = document.getElementById('results-count-slider');
+    const resultsCountValue = document.getElementById('results-count-value');
+
+    // Set the initial value of the slider
+    resultsCountValue.textContent = resultsCountSlider.value;
+
+    // Store the slider value in localStorage when it changes
+    resultsCountSlider.addEventListener('input', () => {
+        resultsCountValue.textContent = resultsCountSlider.value;
+        localStorage.setItem('khojResultsCount', resultsCountSlider.value);
+    });
+
+    // Get the slider value from localStorage on page load
+    const storedResultsCount = localStorage.getItem('khojResultsCount');
+    if (storedResultsCount) {
+        resultsCountSlider.value = storedResultsCount;
+        resultsCountValue.textContent = storedResultsCount;
+    }
 </script>
 {% endblock %}
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/content_type_input.html`

 * *Files 5% similar despite different names*

```diff
@@ -6,39 +6,39 @@
             <img class="card-icon" src="/static/assets/icons/{{ content_type }}.svg" alt="{{ content_type|capitalize }}">
             <span class="card-title-text">{{ content_type|capitalize }}</span>
         </h2>
         <form id="config-form">
             <table>
                 <tr>
                     <td>
-                        <label for="input-files">Input Files</label>
+                        <label for="input-files" title="Add a {{content_type}} file for Khoj to index">Files</label>
                     </td>
                     <td id="input-files-cell">
                         {% if current_config['input_files'] is none %}
-                            <input type="text" id="input-files" name="input-files">
+                            <input type="text" id="input-files" name="input-files" placeholder="~\Documents\notes.{{content_type}}">
                         {% else %}
                             {% for input_file in current_config['input_files'] %}
-                                <input type="text" id="input-files" name="input-files" value="{{ input_file }}">
+                                <input type="text" id="input-files" name="input-files" value="{{ input_file }}" placeholder="~\Documents\notes.{{content_type}}">
                             {% endfor %}
                         {% endif %}
                     </td>
                     <td>
                         <button type="button" id="input-files-button">Add</button>
                     </td>
                 </tr>
                 <tr>
                     <td>
-                        <label for="input-filter">Input Filter</label>
+                        <label for="input-filter" title="Add a folder with {{content_type}} files for Khoj to index">Folders</label>
                     </td>
                     <td id="input-filter-cell">
                         {% if current_config['input_filter'] is none %}
-                            <input type="text" id="input-filter" name="input-filter">
+                            <input type="text" id="input-filter" name="input-filter" placeholder="~/Documents/{{content_type}}">
                         {% else %}
                             {% for input_filter in current_config['input_filter'] %}
-                                <input type="text" id="input-filter" name="input-filter" value="{{ input_filter }}">
+                                <input type="text" id="input-filter" name="input-filter" placeholder="~/Documents/{{content_type}}" value="{{ input_filter.split('/*')[0] }}">
                             {% endfor %}
                         {% endif %}
                     </td>
                     <td>
                         <button type="button" id="input-filter-button">Add</button>
                     </td>
                 </tr>
@@ -102,19 +102,27 @@
             validNodes.push(nodes[i]);
         }
         return validNodes;
     }
 
     submit.addEventListener("click", function(event) {
         event.preventDefault();
+        let suffix = ""
+        if ('{{content_type}}' == "markdown")
+            suffix = "**/*.md"
+        else if ('{{content_type}}' == "org")
+            suffix = "**/*.org"
+        else if ('{{content_type}}' === "pdf")
+            suffix = "**/*.pdf"
+
         var inputFileNodes = document.getElementsByName("input-files");
         var input_files = getValidInputNodes(inputFileNodes).map(node => node.value);
 
         var inputFilterNodes = document.getElementsByName("input-filter");
-        var input_filter = getValidInputNodes(inputFilterNodes).map(node => node.value);
+        var input_filter = getValidInputNodes(inputFilterNodes).map(node => `${node.value}/${suffix}`);
 
         if (input_files.length === 0 && input_filter.length === 0) {
             alert("You must specify at least one input file or input filter.");
             return;
         }
 
         if (input_files.length == 0) {
```

#### html2text {}

```diff
@@ -1,15 +1,13 @@
 {% extends "base_config.html" %} {% block content %}
 ***** [{{ content_type|capitalize }}] {{ content_type|capitalize }} *****
-             {% if current_config['input_files'] is none %} [input-files
-Input Files  ] {% else %} {% for input_file in current_config              Add
-             ['input_files'] %} [{{ input_file }}    ] {% endfor %} {%
-             endif %}
-             {% if current_config['input_filter'] is none %} [input-filter
-Input Filter ] {% else %} {% for input_filter in current_config            Add
-             ['input_filter'] %} [{{ input_filter }}  ] {% endfor %} {%
-             endif %}
+        {% if current_config['input_files'] is none %} [input-files
+Files   ] {% else %} {% for input_file in current_config['input_files'] %}  Add
+        [{{ input_file }}    ] {% endfor %} {% endif %}
+        {% if current_config['input_filter'] is none %} [input-filter
+Folders ] {% else %} {% for input_filter in current_config['input_filter']  Add
+        %} [{{ input_filter.split('/*')[0] }}] {% endfor %} {% endif %}
 Compressed JSONL (Output) [{{ current_config['compressed_jsonl'] }}]
 Embeddings File (Output)  [{{ current_config['embeddings_file'] }}]
 Index Heading Entries     [{{ current_config['index_heading_entries'] }}]
 Save
  {% endblock %}
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -108,44 +108,38 @@
             return renderedResults.outerHTML;
         }
 
         function search(rerank=false) {
             // Extract required fields for search from form
             query = document.getElementById("query").value.trim();
             type = document.getElementById("type").value;
-            results_count = document.getElementById("results-count").value || 6;
-            console.log(`Query: ${query}, Type: ${type}`);
+            searchHint = document.getElementById("info-hint");
+            results_count = localStorage.getItem("khojResultsCount") || 5;
+            console.log(`Query: ${query}, Type: ${type}, Results Count: ${results_count}`);
 
             // Short circuit on empty query
-            if (query.length === 0)
+            if (query.length === 0) {
+                searchHint.style.display = "none";
                 return;
+            }
 
             // If set query field in url query param on rerank
             if (rerank)
                 setQueryFieldInUrl(query);
 
             // Execute Search and Render Results
             url = createRequestUrl(query, type, results_count, rerank);
             fetch(url)
                 .then(response => response.json())
                 .then(data => {
                     console.log(data);
                     document.getElementById("results").innerHTML = render_results(data, query, type);
                 });
-        }
 
-        function updateIndex() {
-            type = document.getElementById("type").value;
-            fetch(`/api/update?t=${type}&client=web`)
-                .then(response => response.json())
-                .then(data => {
-                    console.log(data);
-                    document.getElementById("results").innerHTML =
-                        render_results(data);
-                });
+            setTimeout(() => { searchHint.style.display = "block"; }, 3000);
         }
 
         function incrementalSearch(event) {
             type = document.getElementById("type").value;
             // Search with reranking on 'Enter'
             if (event.key === 'Enter') {
                 search(rerank=true);
@@ -198,35 +192,24 @@
 
         function setTypeFieldInUrl(type) {
             var url = new URL(window.location.href);
             url.searchParams.set("t", type.value);
             window.history.pushState({}, "", url.href);
         }
 
-        function setCountFieldInUrl(results_count) {
-            var url = new URL(window.location.href);
-            url.searchParams.set("n", results_count.value);
-            window.history.pushState({}, "", url.href);
-        }
-
         function setQueryFieldInUrl(query) {
             var url = new URL(window.location.href);
             url.searchParams.set("q", query);
             window.history.pushState({}, "", url.href);
         }
 
         window.onload = function () {
             // Dynamically populate type dropdown based on enabled content types and type passed as URL query parameter
             populate_type_dropdown();
 
-            // Set results count field with value passed in URL query parameters, if any.
-            var results_count = new URLSearchParams(window.location.search).get("n");
-            if (results_count)
-                document.getElementById("results-count").value = results_count;
-
             // Fill query field with value passed in URL query parameters, if any.
             var query_via_url = new URLSearchParams(window.location.search).get("q");
             if (query_via_url)
                 document.getElementById("query").value = query_via_url;
         }
     </script>
 
@@ -263,42 +246,42 @@
 
         <!--Add Text Box To Enter Query, Trigger Incremental Search OnChange -->
         <input type="text" id="query" class="option" onkeyup=incrementalSearch(event) autofocus="autofocus" placeholder="What is the meaning of life?">
 
         <div id="options">
             <!--Add Dropdown to Select Query Type -->
             <select id="type" class="option" onchange="setTypeFieldInUrl(this)"></select>
+        </div>
 
-            <!--Add Button To Regenerate -->
-            <button id="update" class="option" onclick="updateIndex()">Update</button>
-
-            <!--Add Results Count Input To Set Results Count -->
-            <input type="number" id="results-count" min="1" max="100" value="6" placeholder="results count" onchange="setCountFieldInUrl(this)">
+        <!--Add Hints to Guide Search -->
+        <div id="info-hint" style="display: none">
+            Unexpected results? Hit Enter to get better results.
+            Else click Reinitialize on the <a href="/config">settings page</a> to fix it.
         </div>
 
         <!-- Section to Render Results -->
         <div id="results"></div>
     </body>
 
     <style>
         @media only screen and (max-width: 600px) {
             body {
                 display: grid;
                 grid-template-columns: 1fr;
-                grid-template-rows: 1fr auto auto minmax(80px, 100%);
+                grid-template-rows: 1fr auto auto auto minmax(80px, 100%);
             }
             body > * {
                 grid-column: 1;
             }
         }
         @media only screen and (min-width: 600px) {
             body {
                 display: grid;
                 grid-template-columns: 1fr min(70vw, 100%) 1fr;
-                grid-template-rows: 1fr auto auto minmax(80px, 100%);
+                grid-template-rows: 1fr auto auto auto minmax(80px, 100%);
                 padding-top: 60vw;
             }
             body > * {
                 grid-column: 2;
             }
         }
         body {
@@ -314,35 +297,39 @@
         body > * {
             padding: 10px;
             margin: 10px;
         }
         #options {
             padding: 0;
             display: grid;
-            grid-template-columns: 1fr 1fr minmax(70px, 0.5fr);
+            grid-template-columns: 1fr;
         }
         #options > * {
             padding: 15px;
             border-radius: 5px;
             border: 1px solid #475569;
             background: #f9fafc
         }
         .option:hover {
             box-shadow: 0 0 11px #aaa;
         }
-        #options > select {
-            margin-right: 10px;
-        }
         #options > button {
             margin-right: 10px;
         }
 
         #query {
             font-size: larger;
         }
+        #info-hint {
+            font-size: small;
+            color: #aaa;
+            text-align: center;
+            margin: 5px 0 0 0;
+            padding: 0;
+        }
         #results {
             font-size: medium;
             margin: 0px;
             line-height: 20px;
         }
         .results-image {
             display: grid;
```

#### html2text {}

```diff
@@ -3,8 +3,9 @@
 
 {% if demo %}
 Enroll_in_Khoj_cloud_to_get_your_own_Github_assistant
  [                    ] Submit
 [Khoj] {% else %} [Khoj] {% endif %}  Chat Search {% if not demo %} Settings {%
 endif %}
  [                    ]
-  Update  [Unknown INPUT type]
+Unexpected results? Hit Enter to get better results. Else click Reinitialize on
+the settings_page to fix it.
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/processor_conversation_input.html`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,44 @@
             <img class="card-icon" src="/static/assets/icons/chat.svg" alt="Chat">
             <span class="card-title-text">Chat</span>
         </h2>
         <form id="config-form">
             <table>
                 <tr>
                     <td>
-                        <label for="openai-api-key">OpenAI API key</label>
+                        <label for="openai-api-key" title="Get your OpenAI key from https://platform.openai.com/account/api-keys">OpenAI API key</label>
                     </td>
                     <td>
                         <input type="text" id="openai-api-key" name="openai-api-key" value="{{ current_config['openai_api_key'] }}">
                     </td>
                 </tr>
-            </table>
-            <table >
-                <tr style="display: none;">
+                <tr>
                     <td>
-                        <label for="conversation-logfile">Conversation Logfile</label>
+                        <label for="chat-model">Chat Model</label>
                     </td>
                     <td>
-                        <input type="text" id="conversation-logfile" name="conversation-logfile" value="{{ current_config['conversation_logfile'] }}">
+                        <input type="text" id="chat-model" name="chat-model" value="{{ current_config['chat_model'] }}">
                     </td>
                 </tr>
+            </table>
+            <table style="display: none;">
                 <tr>
                     <td>
-                        <label for="model">Model</label>
+                        <label for="conversation-logfile">Conversation Logfile</label>
                     </td>
                     <td>
-                        <input type="text" id="model" name="model" value="{{ current_config['model'] }}">
+                        <input type="text" id="conversation-logfile" name="conversation-logfile" value="{{ current_config['conversation_logfile'] }}">
                     </td>
                 </tr>
                 <tr>
                     <td>
-                        <label for="chat-model">Chat Model</label>
+                        <label for="model">Model</label>
                     </td>
                     <td>
-                        <input type="text" id="chat-model" name="chat-model" value="{{ current_config['chat_model'] }}">
+                        <input type="text" id="model" name="model" value="{{ current_config['model'] }}">
                     </td>
                 </tr>
             </table>
             <div class="section">
                 <div id="success" style="display: none;" ></div>
                 <button id="submit" type="submit">Save</button>
             </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 {% extends "base_config.html" %} {% block content %}
 ***** [Chat] Chat *****
 OpenAI API key [{{ current_config['openai_api_key'] }}]
+Chat Model     [{{ current_config['chat_model'] }}]
 Conversation Logfile [{{ current_config['conversation_logfile'] }}]
 Model                [{{ current_config['model'] }}]
-Chat Model           [{{ current_config['chat_model'] }}]
 Save
  {% endblock %}
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.2.dev42/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/prompts.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,20 +33,15 @@
 """.strip()
 )
 
 
 ## Summarize Chat
 ## --
 summarize_chat = PromptTemplate.from_template(
-    """
-You are an AI. Summarize the conversation below from your perspective:
-
-{text}
-
-Summarize the conversation from the AI's first-person perspective:"""
+    f"{personality.format()} Summarize the conversation from your first person perspective"
 )
 
 
 ## Summarize Notes
 ## --
 summarize_notes = PromptTemplate.from_template(
     """
@@ -98,15 +93,15 @@
 
 ["Who did I visit the Angkor Wat Temple in Cambodia with?"]
 
 A: You visited the Angkor Wat Temple in Cambodia with Pablo, Namita and Xi.
 
 Q: What national parks did I go to last year?
 
-["National park I visited in {last_new_year} dt>=\\"{last_new_year_date}\\" dt<\\"{current_new_year_date}\\""]
+["National park I visited in {last_new_year} dt>='{last_new_year_date}' dt<'{current_new_year_date}'"]
 
 A: You visited the Grand Canyon and Yellowstone National Park in {last_new_year}.
 
 Q: How are you feeling today?
 
 []
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.2.dev42/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.2.dev42/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.2.dev42/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.2.dev42/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.2.dev42/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.2.dev42/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,16 +100,16 @@
         for pdf_file in pdf_files:
             try:
                 loader = PyPDFLoader(pdf_file)
                 pdf_entries_per_file = [page.page_content for page in loader.load()]
                 entry_to_location_map += zip(pdf_entries_per_file, [pdf_file] * len(pdf_entries_per_file))
                 entries.extend(pdf_entries_per_file)
             except Exception as e:
-                logger.error(f"Error processing file: {pdf_file}. This file will not be indexed.")
-                logger.error(e)
+                logger.warning(f"Unable to process file: {pdf_file}. This file will not be indexed.")
+                logger.warning(e)
 
         return entries, dict(entry_to_location_map)
 
     @staticmethod
     def convert_pdf_entries_to_maps(parsed_entries: List[str], entry_to_file_map) -> List[Entry]:
         "Convert each PDF entries into a dictionary"
         entries = []
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/routers/api.py` & `khoj_assistant-0.7.2.dev42/src/khoj/routers/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 import concurrent.futures
 import math
 import time
 import yaml
 import logging
 from datetime import datetime
 from typing import List, Optional, Union
+from functools import partial
 
 # External Packages
 from fastapi import APIRouter, HTTPException, Header, Request
 from sentence_transformers import util
 
 # Internal Packages
 from khoj.configure import configure_processor, configure_search
 from khoj.processor.conversation.gpt import converse, extract_questions
-from khoj.processor.conversation.utils import message_to_log, message_to_prompt
+from khoj.processor.conversation.utils import message_to_log, reciprocal_conversation_to_chatml
 from khoj.search_type import image_search, text_search
 from khoj.search_filter.date_filter import DateFilter
 from khoj.search_filter.file_filter import FileFilter
 from khoj.search_filter.word_filter import WordFilter
 from khoj.utils.config import TextSearchModel
 from khoj.utils.helpers import log_telemetry, timer
 from khoj.utils.rawconfig import (
@@ -30,19 +31,21 @@
     TextContentConfig,
     ConversationProcessorConfig,
     GithubContentConfig,
 )
 from khoj.utils.state import SearchType
 from khoj.utils import state, constants
 from khoj.utils.yaml import save_config_to_file_updated_state
+from fastapi.responses import StreamingResponse
 
 # Initialize Router
 api = APIRouter()
 logger = logging.getLogger(__name__)
 
+# If it's a demo instance, prevent updating any of the configuration.
 if not state.demo:
 
     @api.get("/config/data", response_model=FullConfig)
     def get_config_data():
         return state.config
 
     @api.post("/config/data")
@@ -74,14 +77,25 @@
     async def remove_content_config_data(content_type: str):
         if not state.config or not state.config.content_type:
             return {"status": "ok"}
 
         if state.config.content_type:
             state.config.content_type[content_type] = None
 
+        if content_type == "github":
+            state.model.github_search = None
+        elif content_type == "plugins":
+            state.model.plugin_search = None
+        elif content_type == "pdf":
+            state.model.pdf_search = None
+        elif content_type == "markdown":
+            state.model.markdown_search = None
+        elif content_type == "org":
+            state.model.org_search = None
+
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
     @api.post("/delete/config/data/processor/conversation", status_code=200)
@@ -116,14 +130,15 @@
 
     @api.post("/config/data/processor/conversation", status_code=200)
     async def set_processor_conversation_config_data(updated_config: Union[ConversationProcessorConfig, None]):
         if not state.config:
             state.config = FullConfig()
             state.config.search_type = SearchConfig.parse_obj(constants.default_config["search-type"])
         state.config.processor = ProcessorConfig(conversation=updated_config)
+        state.processor_config = configure_processor(state.config.processor)
         try:
             save_config_to_file_updated_state()
             return {"status": "ok"}
         except Exception as e:
             return {"status": "error", "message": str(e)}
 
 
@@ -318,15 +333,15 @@
             # Sort results across all content types and take top results
             results = sorted(results, key=lambda x: float(x.score), reverse=True)[:results_count]
 
     # Cache results
     state.query_cache[query_cache_key] = results
 
     user_state = {
-        "client_host": request.client.host,
+        "client_host": request.client.host if request.client else "unknown",
         "user_agent": user_agent or "unknown",
         "referer": referer or "unknown",
         "host": host or "unknown",
     }
 
     # Only log telemetry if query is new and not a continuation of previous query
     if state.previous_query is None or state.previous_query not in user_query:
@@ -374,107 +389,159 @@
     except ValueError as e:
         logger.error(e)
         raise HTTPException(status_code=500, detail=str(e))
     else:
         logger.info("📬 Processor reconfigured via API")
 
     user_state = {
-        "client_host": request.client.host,
+        "client_host": request.client.host if request.client else None,
         "user_agent": user_agent or "unknown",
         "referer": referer or "unknown",
         "host": host or "unknown",
     }
 
     state.telemetry += [
         log_telemetry(
             telemetry_type="api", api="update", client=client, app_config=state.config.app, properties=user_state
         )
     ]
 
     return {"status": "ok", "message": "khoj reloaded"}
 
 
-@api.get("/chat")
+@api.get("/chat/init")
+def chat_init(
+    request: Request,
+    client: Optional[str] = None,
+    user_agent: Optional[str] = Header(None),
+    referer: Optional[str] = Header(None),
+    host: Optional[str] = Header(None),
+):
+    if (
+        state.processor_config is None
+        or state.processor_config.conversation is None
+        or state.processor_config.conversation.openai_api_key is None
+    ):
+        raise HTTPException(
+            status_code=500, detail="Set your OpenAI API key via Khoj settings and restart it to use Khoj Chat."
+        )
+
+    # Load Conversation History
+    meta_log = state.processor_config.conversation.meta_log
+
+    user_state = {
+        "client_host": request.client.host if request.client else None,
+        "user_agent": user_agent or "unknown",
+        "referer": referer or "unknown",
+        "host": host or "unknown",
+    }
+
+    state.telemetry += [
+        log_telemetry(
+            telemetry_type="api", api="chat", client=client, app_config=state.config.app, properties=user_state
+        )
+    ]
+
+    return {"status": "ok", "response": meta_log.get("chat", [])}
+
+
+@api.get("/chat", response_class=StreamingResponse)
 async def chat(
     request: Request,
     q: Optional[str] = None,
+    n: Optional[int] = 5,
     client: Optional[str] = None,
     user_agent: Optional[str] = Header(None),
     referer: Optional[str] = Header(None),
     host: Optional[str] = Header(None),
-):
+) -> StreamingResponse:
+    def _save_to_conversation_log(
+        q: str,
+        gpt_response: str,
+        user_message_time: str,
+        compiled_references: List[str],
+        inferred_queries: List[str],
+        meta_log,
+    ):
+        state.processor_config.conversation.chat_session += reciprocal_conversation_to_chatml([q, gpt_response])
+        state.processor_config.conversation.meta_log["chat"] = message_to_log(
+            q,
+            gpt_response,
+            user_message_metadata={"created": user_message_time},
+            khoj_message_metadata={"context": compiled_references, "intent": {"inferred-queries": inferred_queries}},
+            conversation_log=meta_log.get("chat", []),
+        )
+
     if (
         state.processor_config is None
         or state.processor_config.conversation is None
         or state.processor_config.conversation.openai_api_key is None
     ):
         raise HTTPException(
             status_code=500, detail="Set your OpenAI API key via Khoj settings and restart it to use Khoj Chat."
         )
 
     # Load Conversation History
-    chat_session = state.processor_config.conversation.chat_session
     meta_log = state.processor_config.conversation.meta_log
 
-    # If user query is empty, return chat history
+    # If user query is empty, return nothing
     if not q:
-        return {"status": "ok", "response": meta_log.get("chat", [])}
+        return StreamingResponse(None)
 
     # Initialize Variables
     api_key = state.processor_config.conversation.openai_api_key
-    model = state.processor_config.conversation.model
     chat_model = state.processor_config.conversation.chat_model
     user_message_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     conversation_type = "general" if q.startswith("@general") else "notes"
     compiled_references = []
     inferred_queries = []
 
     if conversation_type == "notes":
         # Infer search queries from user message
         with timer("Extracting search queries took", logger):
-            inferred_queries = extract_questions(q, model=model, api_key=api_key, conversation_log=meta_log)
+            inferred_queries = extract_questions(q, api_key=api_key, conversation_log=meta_log)
 
         # Collate search results as context for GPT
         with timer("Searching knowledge base took", logger):
             result_list = []
             for query in inferred_queries:
                 result_list.extend(
-                    await search(query, request=request, n=5, r=True, score_threshold=-5.0, dedupe=False)
+                    await search(query, request=request, n=n, r=True, score_threshold=-5.0, dedupe=False)
                 )
             compiled_references = [item.additional["compiled"] for item in result_list]
 
     # Switch to general conversation type if no relevant notes found for the given query
     conversation_type = "notes" if compiled_references else "general"
     logger.debug(f"Conversation Type: {conversation_type}")
 
-    try:
-        with timer("Generating chat response took", logger):
-            gpt_response = converse(compiled_references, q, meta_log, model=chat_model, api_key=api_key)
-        status = "ok"
-    except Exception as e:
-        gpt_response = str(e)
-        status = "error"
-
-    # Update Conversation History
-    state.processor_config.conversation.chat_session = message_to_prompt(q, chat_session, gpt_message=gpt_response)
-    state.processor_config.conversation.meta_log["chat"] = message_to_log(
-        q,
-        gpt_response,
-        user_message_metadata={"created": user_message_time},
-        khoj_message_metadata={"context": compiled_references, "intent": {"inferred-queries": inferred_queries}},
-        conversation_log=meta_log.get("chat", []),
-    )
-
     user_state = {
-        "client_host": request.client.host,
+        "client_host": request.client.host if request.client else None,
         "user_agent": user_agent or "unknown",
         "referer": referer or "unknown",
         "host": host or "unknown",
     }
 
     state.telemetry += [
         log_telemetry(
             telemetry_type="api", api="chat", client=client, app_config=state.config.app, properties=user_state
         )
     ]
 
-    return {"status": status, "response": gpt_response, "context": compiled_references}
+    try:
+        with timer("Generating chat response took", logger):
+            partial_completion = partial(
+                _save_to_conversation_log,
+                q,
+                user_message_time=user_message_time,
+                compiled_references=compiled_references,
+                inferred_queries=inferred_queries,
+                meta_log=meta_log,
+            )
+
+            gpt_response = converse(
+                compiled_references, q, meta_log, model=chat_model, api_key=api_key, completion_func=partial_completion
+            )
+
+    except Exception as e:
+        gpt_response = str(e)
+
+    return StreamingResponse(gpt_response, media_type="text/event-stream", status_code=200)
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.2.dev42/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.2.dev42/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.2.dev42/src/khoj/search_filter/date_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class DateFilter(BaseFilter):
     # Date Range Filter Regexes
     # Example filter queries:
     # - dt>="yesterday" dt<"tomorrow"
     # - dt>="last week"
     # - dt:"2 years ago"
-    date_regex = r"dt([:><=]{1,2})\"(.*?)\""
+    date_regex = r"dt([:><=]{1,2})[\"'](.*?)[\"']"
 
     def __init__(self, entry_key="raw"):
         self.entry_key = entry_key
         self.date_to_entry_ids = defaultdict(set)
         self.cache = LRU()
 
     def load(self, entries, *args, **kwargs):
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.2.dev42/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.2.dev42/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.2.dev42/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.2.dev42/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/utils/cli.py` & `khoj_assistant-0.7.2.dev42/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/utils/config.py` & `khoj_assistant-0.7.2.dev42/src/khoj/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,14 @@
 
 class ConversationProcessorConfigModel:
     def __init__(self, processor_config: ConversationProcessorConfig):
         self.openai_api_key = processor_config.openai_api_key
         self.model = processor_config.model
         self.chat_model = processor_config.chat_model
         self.conversation_logfile = Path(processor_config.conversation_logfile)
-        self.chat_session = ""
+        self.chat_session: List[str] = []
         self.meta_log: dict = {}
 
 
 @dataclass
 class ProcessorConfigModel:
     conversation: ConversationProcessorConfigModel = None
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/utils/constants.py` & `khoj_assistant-0.7.2.dev42/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.2.dev42/src/khoj/utils/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,15 +171,19 @@
         with open(app_env_filename, "w") as f:
             f.write("server_id=" + server_id + "\n")
 
     return server_id
 
 
 def log_telemetry(
-    telemetry_type: str, api: str = None, client: str = None, app_config: AppConfig = None, properties: dict = None
+    telemetry_type: str,
+    api: str = None,
+    client: Optional[str] = None,
+    app_config: Optional[AppConfig] = None,
+    properties: dict = None,
 ):
     """Log basic app usage telemetry like client, os, api called"""
     # Do not log usage telemetry, if telemetry is disabled via app config
     if not app_config or not app_config.should_log_telemetry:
         return []
 
     # Populate telemetry data to log
```

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.2.dev42/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/utils/models.py` & `khoj_assistant-0.7.2.dev42/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.2.dev42/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/utils/state.py` & `khoj_assistant-0.7.2.dev42/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.2.dev42/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/.gitignore` & `khoj_assistant-0.7.2.dev42/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/LICENSE` & `khoj_assistant-0.7.2.dev42/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/README.md` & `khoj_assistant-0.7.2.dev42/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
   - [Khoj Obsidian](#upgrade-khoj-on-obsidian)
 - [Uninstall](#uninstall)
 - [Troubleshoot](#Troubleshoot)
 - [Advanced Usage](#advanced-usage)
   - [Access Khoj on Mobile](#access-khoj-on-mobile)
   - [Use OpenAI Models for Search](#use-openai-models-for-search)
   - [Search across Different Languages](#search-across-different-languages)
+  - [Boostrap Khoj Search for Offline Usage Later](#bootstrap-khoj-search-for-offline-usage-later)
 - [Miscellaneous](#Miscellaneous)
   - [Setup OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
   - [GPT API](#gpt-api)
 - [Performance](#Performance)
   - [Query Performance](#Query-performance)
   - [Indexing Performance](#Indexing-performance)
   - [Miscellaneous](#Miscellaneous-1)
@@ -304,14 +305,27 @@
 + encoder: "paraphrase-multilingual-MiniLM-L12-v2"
      cross-encoder: "cross-encoder/ms-marco-MiniLM-L-6-v2"
      model_directory: "~/.khoj/search/asymmetric/"
   ```
 
   2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:8000/api/update?t=force)
 
+### Bootstrap Khoj Search for Offline Usage later
+
+  You can bootstrap Khoj pre-emptively to run on machines that do not have internet access. An example use-case would be to run Khoj on an air-gapped machine.
+  Note: *Only search can currently run in fully offline mode, not chat.*
+
+  - With Internet
+    1. Manually download the [asymmetric text](https://huggingface.co/sentence-transformers/multi-qa-MiniLM-L6-cos-v1), [symmetric text](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2)and [image search](https://huggingface.co/sentence-transformers/clip-ViT-B-32) models from HuggingFace
+    2. Pip install khoj (and dependencies) in an associated virtualenv. E.g `python -m venv .venv && source .venv/bin/activate && pip install khoj-assistant`
+  - Without Internet
+    1. Copy each of the search models into their respective folders, `asymmetric`, `symmetric` and `image` under the `~/.khoj/search/` directory on the air-gapped machine
+    2. Copy the khoj virtual environment directory onto the air-gapped machine, activate the environment and start and khoj as normal. E.g `source .venv/bin/activate && khoj`
+
+
 ## Miscellaneous
 ### Set your OpenAI API key in Khoj
 If you want, Khoj can be configured to use OpenAI for search and chat.<br />
 Add your OpenAI API to Khoj by using either of the two options below:
  - Open your [Khoj settings](http://localhost:8000/config/processor/conversation), add your OpenAI API key, and click *Save*. Then go to your [Khoj settings](http://localhost:8000/config) and click `Configure`. This will refresh Khoj with your OpenAI API key.
  - Set `openai-api-key` field under `processor.conversation` section in your `khoj.yml`[^1] to your [OpenAI API key](https://beta.openai.com/account/api-keys) and restart khoj:
     ```diff
```

### Comparing `khoj_assistant-0.7.2.dev4/pyproject.toml` & `khoj_assistant-0.7.2.dev42/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev4/PKG-INFO` & `khoj_assistant-0.7.2.dev42/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.2.dev4
+Version: 0.7.2.dev42
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
@@ -91,14 +91,15 @@
   - [Khoj Obsidian](#upgrade-khoj-on-obsidian)
 - [Uninstall](#uninstall)
 - [Troubleshoot](#Troubleshoot)
 - [Advanced Usage](#advanced-usage)
   - [Access Khoj on Mobile](#access-khoj-on-mobile)
   - [Use OpenAI Models for Search](#use-openai-models-for-search)
   - [Search across Different Languages](#search-across-different-languages)
+  - [Boostrap Khoj Search for Offline Usage Later](#bootstrap-khoj-search-for-offline-usage-later)
 - [Miscellaneous](#Miscellaneous)
   - [Setup OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
   - [GPT API](#gpt-api)
 - [Performance](#Performance)
   - [Query Performance](#Query-performance)
   - [Indexing Performance](#Indexing-performance)
   - [Miscellaneous](#Miscellaneous-1)
@@ -362,14 +363,27 @@
 + encoder: "paraphrase-multilingual-MiniLM-L12-v2"
      cross-encoder: "cross-encoder/ms-marco-MiniLM-L-6-v2"
      model_directory: "~/.khoj/search/asymmetric/"
   ```
 
   2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:8000/api/update?t=force)
 
+### Bootstrap Khoj Search for Offline Usage later
+
+  You can bootstrap Khoj pre-emptively to run on machines that do not have internet access. An example use-case would be to run Khoj on an air-gapped machine.
+  Note: *Only search can currently run in fully offline mode, not chat.*
+
+  - With Internet
+    1. Manually download the [asymmetric text](https://huggingface.co/sentence-transformers/multi-qa-MiniLM-L6-cos-v1), [symmetric text](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2)and [image search](https://huggingface.co/sentence-transformers/clip-ViT-B-32) models from HuggingFace
+    2. Pip install khoj (and dependencies) in an associated virtualenv. E.g `python -m venv .venv && source .venv/bin/activate && pip install khoj-assistant`
+  - Without Internet
+    1. Copy each of the search models into their respective folders, `asymmetric`, `symmetric` and `image` under the `~/.khoj/search/` directory on the air-gapped machine
+    2. Copy the khoj virtual environment directory onto the air-gapped machine, activate the environment and start and khoj as normal. E.g `source .venv/bin/activate && khoj`
+
+
 ## Miscellaneous
 ### Set your OpenAI API key in Khoj
 If you want, Khoj can be configured to use OpenAI for search and chat.<br />
 Add your OpenAI API to Khoj by using either of the two options below:
  - Open your [Khoj settings](http://localhost:8000/config/processor/conversation), add your OpenAI API key, and click *Save*. Then go to your [Khoj settings](http://localhost:8000/config) and click `Configure`. This will refresh Khoj with your OpenAI API key.
  - Set `openai-api-key` field under `processor.conversation` section in your `khoj.yml`[^1] to your [OpenAI API key](https://beta.openai.com/account/api-keys) and restart khoj:
     ```diff
```

