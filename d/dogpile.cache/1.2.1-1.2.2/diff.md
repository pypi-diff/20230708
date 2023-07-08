# Comparing `tmp/dogpile.cache-1.2.1.tar.gz` & `tmp/dogpile.cache-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogpile.cache-1.2.1.tar", last modified: Sat May 20 15:56:55 2023, max compression
+gzip compressed data, was "dogpile.cache-1.2.2.tar", last modified: Sat Jul  8 20:59:39 2023, max compression
```

## Comparing `dogpile.cache-1.2.1.tar` & `dogpile.cache-1.2.2.tar`

### file list

```diff
@@ -1,132 +1,148 @@
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.666309 dogpile.cache-1.2.1/
--rw-r--r--   0 classic   (1000) classic   (1000)     1059 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/LICENSE
--rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/MANIFEST.in
--rw-r--r--   0 classic   (1000) classic   (1000)     4895 2023-05-20 15:56:55.666309 dogpile.cache-1.2.1/PKG-INFO
--rw-r--r--   0 classic   (1000) classic   (1000)     4176 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/README.rst
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.658309 dogpile.cache-1.2.1/docs/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.659309 dogpile.cache-1.2.1/docs/_sources/
--rw-r--r--   0 classic   (1000) classic   (1000)     1587 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/api.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    39675 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/changelog.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    10222 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/core_usage.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/front.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     1215 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/index.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     9296 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/recipes.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    11625 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_sources/usage.rst.txt
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.661309 dogpile.cache-1.2.1/docs/_static/
--rw-r--r--   0 classic   (1000) classic   (1000)    14813 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/basic.css
--rw-r--r--   0 classic   (1000) classic   (1000)      107 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/changelog.css
--rw-r--r--   0 classic   (1000) classic   (1000)     4472 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/doctools.js
--rw-r--r--   0 classic   (1000) classic   (1000)      420 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/documentation_options.js
--rw-r--r--   0 classic   (1000) classic   (1000)      286 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/file.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4758 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/language_data.js
--rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/minus.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4208 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/nature.css
--rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/nature_override.css
--rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/plus.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4846 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/pygments.css
--rw-r--r--   0 classic   (1000) classic   (1000)    18215 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/searchtools.js
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/site_custom_css.css
--rw-r--r--   0 classic   (1000) classic   (1000)     4712 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/sphinx_highlight.js
--rw-r--r--   0 classic   (1000) classic   (1000)      204 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/_static/sphinx_paramlinks.css
--rw-r--r--   0 classic   (1000) classic   (1000)   480641 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/api.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.663309 dogpile.cache-1.2.1/docs/build/
--rw-r--r--   0 classic   (1000) classic   (1000)     3373 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/Makefile
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.663309 dogpile.cache-1.2.1/docs/build/_static/
--rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/_static/nature_override.css
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/_static/site_custom_css.css
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.663309 dogpile.cache-1.2.1/docs/build/_templates/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/_templates/site_custom_sidebars.html
--rw-r--r--   0 classic   (1000) classic   (1000)     1587 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/api.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      266 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/builder.py
--rw-------   0 classic   (1000) classic   (1000)    39675 2023-05-20 15:56:52.000000 dogpile.cache-1.2.1/docs/build/changelog.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     7408 2023-05-20 15:56:52.000000 dogpile.cache-1.2.1/docs/build/conf.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10222 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/core_usage.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/front.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     1215 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/index.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     9296 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/recipes.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      178 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/requirements.txt
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.663309 dogpile.cache-1.2.1/docs/build/unreleased/
--rw-r--r--   0 classic   (1000) classic   (1000)      410 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/unreleased/README.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    11625 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/docs/build/usage.rst
--rw-r--r--   0 classic   (1000) classic   (1000)   133773 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/changelog.html
--rw-r--r--   0 classic   (1000) classic   (1000)    28473 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/core_usage.html
--rw-r--r--   0 classic   (1000) classic   (1000)     6491 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/front.html
--rw-r--r--   0 classic   (1000) classic   (1000)    67475 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/genindex.html
--rw-r--r--   0 classic   (1000) classic   (1000)    15002 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/index.html
--rw-r--r--   0 classic   (1000) classic   (1000)     5957 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/py-modindex.html
--rw-r--r--   0 classic   (1000) classic   (1000)    32467 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/recipes.html
--rw-r--r--   0 classic   (1000) classic   (1000)     3508 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/search.html
--rw-r--r--   0 classic   (1000) classic   (1000)    74956 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/searchindex.js
--rw-r--r--   0 classic   (1000) classic   (1000)   111860 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/docs/usage.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.656309 dogpile.cache-1.2.1/dogpile/
--rw-r--r--   0 classic   (1000) classic   (1000)      106 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/__init__.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.656309 dogpile.cache-1.2.1/dogpile/cache/
--rw-r--r--   0 classic   (1000) classic   (1000)      180 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    16890 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/api.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.657309 dogpile.cache-1.2.1/dogpile/cache/backends/
--rw-r--r--   0 classic   (1000) classic   (1000)     1197 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    13749 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/file.py
--rw-r--r--   0 classic   (1000) classic   (1000)    20835 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/memcached.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3030 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/memory.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1167 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/null.py
--rw-r--r--   0 classic   (1000) classic   (1000)    11764 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/backends/redis.py
--rw-r--r--   0 classic   (1000) classic   (1000)      601 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/exception.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.657309 dogpile.cache-1.2.1/dogpile/cache/plugins/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/plugins/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2964 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/plugins/mako_cache.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3610 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/proxy.py
--rw-r--r--   0 classic   (1000) classic   (1000)    68481 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/region.py
--rw-r--r--   0 classic   (1000) classic   (1000)     5418 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/cache/util.py
--rw-r--r--   0 classic   (1000) classic   (1000)      565 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/core.py
--rw-r--r--   0 classic   (1000) classic   (1000)     7077 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/lock.py
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/py.typed
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.657309 dogpile.cache-1.2.1/dogpile/util/
--rw-r--r--   0 classic   (1000) classic   (1000)      339 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/util/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1735 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/util/compat.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4479 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/util/langhelpers.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2801 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/util/nameregistry.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4532 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/dogpile/util/readwrite_lock.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.664309 dogpile.cache-1.2.1/dogpile.cache.egg-info/
--rw-r--r--   0 classic   (1000) classic   (1000)     4895 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/PKG-INFO
--rw-r--r--   0 classic   (1000) classic   (1000)     2952 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/SOURCES.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/dependency_links.txt
--rw-r--r--   0 classic   (1000) classic   (1000)       73 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/entry_points.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/not-zip-safe
--rw-r--r--   0 classic   (1000) classic   (1000)       34 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/requires.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        8 2023-05-20 15:56:55.000000 dogpile.cache-1.2.1/dogpile.cache.egg-info/top_level.txt
--rw-r--r--   0 classic   (1000) classic   (1000)      838 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/hash_port.py
--rw-r--r--   0 classic   (1000) classic   (1000)      513 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/log_tests.ini
--rw-r--r--   0 classic   (1000) classic   (1000)     1660 2023-05-20 15:56:55.666309 dogpile.cache-1.2.1/setup.cfg
--rw-r--r--   0 classic   (1000) classic   (1000)      558 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/setup.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.664309 dogpile.cache-1.2.1/tests/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/__init__.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.665309 dogpile.cache-1.2.1/tests/cache/
--rw-r--r--   0 classic   (1000) classic   (1000)      870 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    17363 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/_fixtures.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.665309 dogpile.cache-1.2.1/tests/cache/plugins/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/plugins/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1389 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/plugins/test_mako_cache.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2972 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_dbm_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)    18860 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_decorator.py
--rw-r--r--   0 classic   (1000) classic   (1000)      405 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_mako.py
--rw-r--r--   0 classic   (1000) classic   (1000)    16050 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_memcached_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)      361 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_memory_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1934 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_null_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)     6693 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_redis_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3468 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_redis_sentinel_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)    32235 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/cache/test_region.py
--rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/conftest.py
--rw-r--r--   0 classic   (1000) classic   (1000)      552 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/test_backgrounding.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10397 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/test_lock.py
--rw-r--r--   0 classic   (1000) classic   (1000)      893 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/test_utils.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.665309 dogpile.cache-1.2.1/tests/tls/
--rw-r--r--   0 classic   (1000) classic   (1000)     2354 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/ca-root.crt
--rw-r--r--   0 classic   (1000) classic   (1000)     2354 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/client-ca-root.crt
--rw-r--r--   0 classic   (1000) classic   (1000)     1692 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/client.crt
--rw-r--r--   0 classic   (1000) classic   (1000)     1679 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/client.key
--rw-r--r--   0 classic   (1000) classic   (1000)     1675 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/server.key
--rw-r--r--   0 classic   (1000) classic   (1000)     4021 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/tls/server_chain.pem
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:55.665309 dogpile.cache-1.2.1/tests/util/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/util/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1535 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tests/util/test_nameregistry.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2401 2023-05-20 15:56:45.000000 dogpile.cache-1.2.1/tox.ini
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.261108 dogpile.cache-1.2.2/
+-rw-r--r--   0 classic   (1000) classic   (1000)      213 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/.gitignore
+-rw-r--r--   0 classic   (1000) classic   (1000)       99 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/.gitreview
+-rw-r--r--   0 classic   (1000) classic   (1000)      653 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 classic   (1000) classic   (1000)     1059 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/LICENSE
+-rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/MANIFEST.in
+-rw-r--r--   0 classic   (1000) classic   (1000)     4895 2023-07-08 20:59:39.261108 dogpile.cache-1.2.2/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     4176 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/README.rst
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.242110 dogpile.cache-1.2.2/docs/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.244110 dogpile.cache-1.2.2/docs/_sources/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1587 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_sources/api.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    39994 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_sources/changelog.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    10222 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_sources/core_usage.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_sources/front.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1215 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_sources/index.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     9296 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_sources/recipes.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    11625 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_sources/usage.rst.txt
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.247109 dogpile.cache-1.2.2/docs/_static/
+-rw-r--r--   0 classic   (1000) classic   (1000)    14813 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/basic.css
+-rw-r--r--   0 classic   (1000) classic   (1000)      107 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/changelog.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     4472 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/doctools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      420 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/documentation_options.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      286 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/file.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4758 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/language_data.js
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/minus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4208 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/nature.css
+-rw-r--r--   0 classic   (1000) classic   (1000)      507 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/nature_override.css
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/plus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4846 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/pygments.css
+-rw-r--r--   0 classic   (1000) classic   (1000)    18215 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/searchtools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/site_custom_css.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     4712 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/sphinx_highlight.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      204 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/_static/sphinx_paramlinks.css
+-rw-r--r--   0 classic   (1000) classic   (1000)   480394 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/api.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.249109 dogpile.cache-1.2.2/docs/build/
+-rw-r--r--   0 classic   (1000) classic   (1000)     3373 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/Makefile
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.250109 dogpile.cache-1.2.2/docs/build/_static/
+-rw-r--r--   0 classic   (1000) classic   (1000)      507 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/_static/nature_override.css
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/_static/site_custom_css.css
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.250109 dogpile.cache-1.2.2/docs/build/_templates/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/_templates/site_custom_sidebars.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     1587 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/api.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      266 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/builder.py
+-rw-------   0 classic   (1000) classic   (1000)    39994 2023-07-08 20:59:32.000000 dogpile.cache-1.2.2/docs/build/changelog.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     7408 2023-07-08 20:59:32.000000 dogpile.cache-1.2.2/docs/build/conf.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10222 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/core_usage.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/front.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     1215 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/index.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     3077 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/make.bat
+-rw-r--r--   0 classic   (1000) classic   (1000)     9296 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/recipes.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      178 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/requirements.txt
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.250109 dogpile.cache-1.2.2/docs/build/unreleased/
+-rw-r--r--   0 classic   (1000) classic   (1000)      410 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/unreleased/README.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    11625 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/docs/build/usage.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)   135360 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/changelog.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    28473 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/core_usage.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     6491 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/front.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    67475 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/genindex.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    15105 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/index.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     5957 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/py-modindex.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    32467 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/recipes.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     3508 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/search.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    75051 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/searchindex.js
+-rw-r--r--   0 classic   (1000) classic   (1000)   111729 2023-07-08 20:59:38.000000 dogpile.cache-1.2.2/docs/usage.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.236110 dogpile.cache-1.2.2/dogpile/
+-rw-r--r--   0 classic   (1000) classic   (1000)      106 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/__init__.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.237110 dogpile.cache-1.2.2/dogpile/cache/
+-rw-r--r--   0 classic   (1000) classic   (1000)      180 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16976 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/api.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.238110 dogpile.cache-1.2.2/dogpile/cache/backends/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1197 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/backends/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    13749 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/backends/file.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    20835 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/backends/memcached.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3030 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/backends/memory.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1167 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/backends/null.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    11764 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/backends/redis.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      601 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/exception.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.238110 dogpile.cache-1.2.2/dogpile/cache/plugins/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/plugins/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2964 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/plugins/mako_cache.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3630 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/proxy.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    68503 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/region.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     5418 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/cache/util.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      565 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/core.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     7077 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/lock.py
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/py.typed
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.239110 dogpile.cache-1.2.2/dogpile/util/
+-rw-r--r--   0 classic   (1000) classic   (1000)      339 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/util/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1735 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/util/compat.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4479 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/util/langhelpers.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2801 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/util/nameregistry.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4532 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/util/readwrite_lock.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      131 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/dogpile/util/typing.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.253109 dogpile.cache-1.2.2/dogpile.cache.egg-info/
+-rw-r--r--   0 classic   (1000) classic   (1000)     4895 2023-07-08 20:59:39.000000 dogpile.cache-1.2.2/dogpile.cache.egg-info/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     3962 2023-07-08 20:59:39.000000 dogpile.cache-1.2.2/dogpile.cache.egg-info/SOURCES.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-07-08 20:59:39.000000 dogpile.cache-1.2.2/dogpile.cache.egg-info/dependency_links.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)       73 2023-07-08 20:59:39.000000 dogpile.cache-1.2.2/dogpile.cache.egg-info/entry_points.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-07-08 20:59:39.000000 dogpile.cache-1.2.2/dogpile.cache.egg-info/not-zip-safe
+-rw-r--r--   0 classic   (1000) classic   (1000)       87 2023-07-08 20:59:39.000000 dogpile.cache-1.2.2/dogpile.cache.egg-info/requires.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        8 2023-07-08 20:59:39.000000 dogpile.cache-1.2.2/dogpile.cache.egg-info/top_level.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)      838 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/hash_port.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      513 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/log_tests.ini
+-rw-r--r--   0 classic   (1000) classic   (1000)      807 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/mypy.ini
+-rw-r--r--   0 classic   (1000) classic   (1000)     1708 2023-07-08 20:59:39.262108 dogpile.cache-1.2.2/setup.cfg
+-rw-r--r--   0 classic   (1000) classic   (1000)      558 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/setup.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.255109 dogpile.cache-1.2.2/tests/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/__init__.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.258108 dogpile.cache-1.2.2/tests/cache/
+-rw-r--r--   0 classic   (1000) classic   (1000)      870 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    17363 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/_fixtures.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.258108 dogpile.cache-1.2.2/tests/cache/plugins/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/plugins/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1389 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/plugins/test_mako_cache.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2972 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/test_dbm_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    18860 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/test_decorator.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      405 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/test_mako.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16050 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/test_memcached_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      361 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/test_memory_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1934 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/test_null_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     6693 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/test_redis_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3468 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/test_redis_sentinel_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    32235 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/cache/test_region.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/conftest.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      552 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/test_backgrounding.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10397 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/test_lock.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      893 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/test_utils.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.259108 dogpile.cache-1.2.2/tests/tls/
+-rw-r--r--   0 classic   (1000) classic   (1000)      368 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/README.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     2354 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/ca-root.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     2354 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/client-ca-root.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1692 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/client.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1679 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/client.key
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.260108 dogpile.cache-1.2.2/tests/tls/generate/
+-rw-r--r--   0 classic   (1000) classic   (1000)     2892 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/generate/Makefile
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.261108 dogpile.cache-1.2.2/tests/tls/generate/conf/
+-rw-r--r--   0 classic   (1000) classic   (1000)      565 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/generate/conf/ca-intermediate.conf
+-rw-r--r--   0 classic   (1000) classic   (1000)      564 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/generate/conf/ca-root.conf
+-rw-r--r--   0 classic   (1000) classic   (1000)      564 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/generate/conf/client-ca-root.conf
+-rw-r--r--   0 classic   (1000) classic   (1000)      492 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/generate/conf/client.conf
+-rw-r--r--   0 classic   (1000) classic   (1000)      475 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/generate/conf/server.conf
+-rwxr-xr-x   0 classic   (1000) classic   (1000)     1567 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/generate/tool
+-rw-r--r--   0 classic   (1000) classic   (1000)     1675 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/server.key
+-rw-r--r--   0 classic   (1000) classic   (1000)     4021 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/tls/server_chain.pem
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:39.261108 dogpile.cache-1.2.2/tests/util/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/util/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1535 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tests/util/test_nameregistry.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2401 2023-07-08 20:59:20.000000 dogpile.cache-1.2.2/tox.ini
```

### Comparing `dogpile.cache-1.2.1/LICENSE` & `dogpile.cache-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/PKG-INFO` & `dogpile.cache-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogpile.cache
-Version: 1.2.1
+Version: 1.2.2
 Summary: A caching front-end based on the Dogpile lock.
 Home-page: https://github.com/sqlalchemy/dogpile.cache
 Author: Mike Bayer
 Author-email: mike_mp@zzzcomputing.com
 License: MIT
 Project-URL: Documentation, https://dogpilecache.sqlalchemy.org
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/dogpile.cache/
```

### Comparing `dogpile.cache-1.2.1/README.rst` & `dogpile.cache-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_sources/api.rst.txt` & `dogpile.cache-1.2.2/docs/_sources/api.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_sources/changelog.rst.txt` & `dogpile.cache-1.2.2/docs/_sources/changelog.rst.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 =========
 Changelog
 =========
 
 .. changelog::
+    :version: 1.2.2
+    :released: Sat Jul 8 2023
+
+    .. change::
+        :tags: bug, typing
+        :tickets: 240
+
+        Made use of pep-673 ``Self`` type for method chained methods such as
+        :meth:`.CacheRegion.configure` and :meth:`.ProxyBackend.wrap`. Pull request
+        courtesy Viicos.
+
+.. changelog::
     :version: 1.2.1
     :released: Sat May 20 2023
 
     .. change::
         :tags: bug, typing
         :tickets: 238
```

### Comparing `dogpile.cache-1.2.1/docs/_sources/core_usage.rst.txt` & `dogpile.cache-1.2.2/docs/_sources/core_usage.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_sources/front.rst.txt` & `dogpile.cache-1.2.2/docs/_sources/front.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_sources/index.rst.txt` & `dogpile.cache-1.2.2/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_sources/recipes.rst.txt` & `dogpile.cache-1.2.2/docs/_sources/recipes.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_sources/usage.rst.txt` & `dogpile.cache-1.2.2/docs/_sources/usage.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_static/basic.css` & `dogpile.cache-1.2.2/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_static/doctools.js` & `dogpile.cache-1.2.2/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_static/language_data.js` & `dogpile.cache-1.2.2/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_static/nature.css` & `dogpile.cache-1.2.2/docs/_static/nature.css`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_static/pygments.css` & `dogpile.cache-1.2.2/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_static/searchtools.js` & `dogpile.cache-1.2.2/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/_static/sphinx_highlight.js` & `dogpile.cache-1.2.2/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/api.html` & `dogpile.cache-1.2.2/docs/api.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>API &#8212; dogpile.cache 1.2.1 documentation</title>
+    <title>API &#8212; dogpile.cache 1.2.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -29,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">API</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -517,15 +517,15 @@
 <p><a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments" title="dogpile.cache.region.CacheRegion.cache_multi_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_multi_on_arguments()</span></code></a></p>
 <p><a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create" title="dogpile.cache.region.CacheRegion.get_or_create"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_or_create()</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.configure">
-<span class="sig-name descname"><span class="pre">configure</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">timedelta</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">arguments</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_argument_dict</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_prefix</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">wrap</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Type</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">()</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">replace_existing_backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">region_invalidator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy" title="dogpile.cache.region.RegionInvalidationStrategy"><span class="pre">RegionInvalidationStrategy</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><span class="pre">CacheRegion</span></a></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.configure" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">configure</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">timedelta</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">arguments</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_argument_dict</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_prefix</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">wrap</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Type</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">()</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">replace_existing_backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">region_invalidator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy" title="dogpile.cache.region.RegionInvalidationStrategy"><span class="pre">RegionInvalidationStrategy</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Self</span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.configure" title="Permalink to this definition">¶</a></dt>
 <dd><p>Configure a <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>.</p>
 <p>The <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a> itself
 is returned.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.backend"></span><strong>backend</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.backend">¶</a> – Required.  This is the name of the
@@ -3528,15 +3528,15 @@
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.wrap">
-<span class="sig-name descname"><span class="pre">wrap</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><span class="pre">CacheBackend</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.wrap" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">wrap</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><span class="pre">CacheBackend</span></a></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Self</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.wrap" title="Permalink to this definition">¶</a></dt>
 <dd><p>Take a backend as an argument and setup the self.proxied property.
 Return an object that be used as a backend by a <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>
 object.</p>
 </dd></dl>
 
 </dd></dl>
 
@@ -4356,15 +4356,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">API</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * API
 ****** APIÂ¶ ******
 ***** RegionÂ¶ *****
   classdogpile.cache.region.CacheRegion(name: str | None = None,
   function_key_generator: ~typing.Callable[[...], ~typing.Callable[[...], str]]
   = <function function_key_generator>, function_multi_key_generator:
   ~typing.Callable[[...], ~typing.Callable[[...], ~typing.Sequence[str]]] =
@@ -190,15 +190,15 @@
             CacheRegion.cache_multi_on_arguments()
             CacheRegion.get_or_create()
         configure(backend: str, expiration_time: float | timedelta | None =
         None, arguments: Mapping[str, Any] | None = None,
         _config_argument_dict: Mapping[str, Any] | None = None, _config_prefix:
         str | None = None, wrap: Sequence[ProxyBackend | Type[ProxyBackend]] =
         (), replace_existing_backend: bool = False, region_invalidator:
-        RegionInvalidationStrategy | None = None) &#x2192; CacheRegionÂ¶
+        RegionInvalidationStrategy | None = None) &#x2192; SelfÂ¶
             Configure a CacheRegion.
             The CacheRegion itself is returned.
         configure_from_config(config_dict, prefix)Â¶
             Configure from a configuration dictionary and a prefix.
             Example:
             local_region = make_region()
             memcached_region = make_region()
@@ -1636,15 +1636,15 @@
             â that will have the undesirable effect of modifying the returned
             values as well.
             New in version 1.1.
             The default implementation of this method for CacheBackend calls
             upon the CacheBackend.set_multi() method.
             See also
             BytesBackend
-        wrap(backend: CacheBackend) &#x2192; ProxyBackendÂ¶
+        wrap(backend: CacheBackend) &#x2192; SelfÂ¶
             Take a backend as an argument and setup the self.proxied property.
             Return an object that be used as a backend by a CacheRegion object.
 **** Null BackendÂ¶ ****
 The Null backend does not do any caching at all. It can be used to test
 behavior without caching, or as a means of disabling caching for a region that
 is otherwise used normally.
 New in version 0.5.4.
@@ -2135,10 +2135,10 @@
 *** Next topic ***
 Changelog
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * API
 © Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.1/docs/build/Makefile` & `dogpile.cache-1.2.2/docs/build/Makefile`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/build/api.rst` & `dogpile.cache-1.2.2/docs/build/api.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/build/changelog.rst` & `dogpile.cache-1.2.2/docs/build/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 =========
 Changelog
 =========
 
 .. changelog::
+    :version: 1.2.2
+    :released: Sat Jul 8 2023
+
+    .. change::
+        :tags: bug, typing
+        :tickets: 240
+
+        Made use of pep-673 ``Self`` type for method chained methods such as
+        :meth:`.CacheRegion.configure` and :meth:`.ProxyBackend.wrap`. Pull request
+        courtesy Viicos.
+
+.. changelog::
     :version: 1.2.1
     :released: Sat May 20 2023
 
     .. change::
         :tags: bug, typing
         :tickets: 238
```

### Comparing `dogpile.cache-1.2.1/docs/build/conf.py` & `dogpile.cache-1.2.2/docs/build/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = dogpile.__version__
 # The full version, including alpha/beta/rc tags.
-release = "1.2.1"
+release = "1.2.2"
 
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
```

### Comparing `dogpile.cache-1.2.1/docs/build/core_usage.rst` & `dogpile.cache-1.2.2/docs/build/core_usage.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/build/front.rst` & `dogpile.cache-1.2.2/docs/build/front.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/build/index.rst` & `dogpile.cache-1.2.2/docs/build/index.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/build/recipes.rst` & `dogpile.cache-1.2.2/docs/build/recipes.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/build/usage.rst` & `dogpile.cache-1.2.2/docs/build/usage.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/docs/changelog.html` & `dogpile.cache-1.2.2/docs/changelog.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Changelog &#8212; dogpile.cache 1.2.1 documentation</title>
+    <title>Changelog &#8212; dogpile.cache 1.2.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -25,26 +25,40 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
   <section id="changelog">
 <h1>Changelog<a class="headerlink" href="#changelog" title="Permalink to this heading">¶</a></h1>
+<section id="change-1.2.2">
+<h2 class="release-version">1.2.2<a class="headerlink" href="#change-1.2.2" title="Permalink to this heading">¶</a></h2>
+Released: Sat Jul 8 2023<section id="change-1.2.2-bug">
+<h3>bug<a class="headerlink" href="#change-1.2.2-bug" title="Permalink to this heading">¶</a></h3>
+<ul class="simple">
+<li><p class="caption" id="change-1.2.2-0"><span class="target" id="change-56baad91a44f06af15bd33d4b093c196"><strong>[bug] [typing]</strong> <a class="changelog-reference headerlink reference internal" href="#change-56baad91a44f06af15bd33d4b093c196">¶</a></span><p>Made use of pep-673 <code class="docutils literal notranslate"><span class="pre">Self</span></code> type for method chained methods such as
+<a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.configure" title="dogpile.cache.region.CacheRegion.configure"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.configure()</span></code></a> and <a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend.wrap" title="dogpile.cache.proxy.ProxyBackend.wrap"><code class="xref py py-meth docutils literal notranslate"><span class="pre">ProxyBackend.wrap()</span></code></a>. Pull request
+courtesy Viicos.</p>
+<p>References: <a class="reference external" href="https://github.com/sqlalchemy/dogpile.cache/issues/240">#240</a></p>
+</p>
+</li>
+</ul>
+</section>
+</section>
 <section id="change-1.2.1">
 <h2 class="release-version">1.2.1<a class="headerlink" href="#change-1.2.1" title="Permalink to this heading">¶</a></h2>
 Released: Sat May 20 2023<section id="change-1.2.1-bug">
 <h3>bug<a class="headerlink" href="#change-1.2.1-bug" title="Permalink to this heading">¶</a></h3>
 <ul class="simple">
 <li><p class="caption" id="change-1.2.1-0"><span class="target" id="change-75c1354759a03cf148c4d208630af607"><strong>[bug] [typing]</strong> <a class="changelog-reference headerlink reference internal" href="#change-75c1354759a03cf148c4d208630af607">¶</a></span><p>Added py.typed file to root so that typing tools such as Mypy recognize
 dogpile as typed. Pull request courtesy Daverball.</p>
@@ -1365,14 +1379,18 @@
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <div>
     <h3><a href="index.html">Table of Contents</a></h3>
     <ul>
 <li><a class="reference internal" href="#">Changelog</a><ul>
+<li><a class="reference internal" href="#change-1.2.2">1.2.2</a><ul>
+<li><a class="reference internal" href="#change-1.2.2-bug">bug</a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#change-1.2.1">1.2.1</a><ul>
 <li><a class="reference internal" href="#change-1.2.1-bug">bug</a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#change-1.2.0">1.2.0</a><ul>
 <li><a class="reference internal" href="#change-1.2.0-feature">feature</a></li>
 </ul>
@@ -1596,15 +1614,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
```

#### html2text {}

```diff
@@ -5,17 +5,26 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Changelog
 ****** ChangelogÂ¶ ******
+***** 1.2.2Â¶ *****
+Released: Sat Jul 8 2023
+**** bugÂ¶ ****
+    * [bug] [typing] Â¶
+      Made use of pep-673 Self type for method chained methods such as
+      CacheRegion.configure() and ProxyBackend.wrap(). Pull request courtesy
+      Viicos.
+      References: #240
+
 ***** 1.2.1Â¶ *****
 Released: Sat May 20 2023
 **** bugÂ¶ ****
     * [bug] [typing] Â¶
       Added py.typed file to root so that typing tools such as Mypy recognize
       dogpile as typed. Pull request courtesy Daverball.
       References: #238
@@ -847,14 +856,16 @@
     * [no_tags] Â¶
       Initial release.
 [no_tags] Â¶
 Includes a pylibmc backend and a plain dictionary backend.
 
 **** Table_of_Contents ****
     * Changelog
+          o 1.2.2
+                # bug
           o 1.2.1
                 # bug
           o 1.2.0
                 # feature
           o 1.1.8
                 # bug
           o 1.1.7
@@ -966,10 +977,10 @@
 [q                   ] [Go]
 *** Previous topic ***
 API
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Changelog
 © Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.1/docs/core_usage.html` & `dogpile.cache-1.2.2/docs/core_usage.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>dogpile Core &#8212; dogpile.cache 1.2.1 documentation</title>
+    <title>dogpile Core &#8212; dogpile.cache 1.2.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -29,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">dogpile Core</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -327,15 +327,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              >next</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">dogpile Core</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * dogpile Core
 ****** dogpile CoreÂ¶ ******
 dogpile provides a locking interface around a âvalue creationâ and âvalue
 retrievalâ pair of functions.
 Changed in version 0.6.0: The dogpile package encapsulates the functionality
 that was previously provided by the separate dogpile.core package.
 The primary interface is the Lock object, which provides for the invocation of
@@ -234,10 +234,10 @@
 *** Next topic ***
 API
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * dogpile Core
 © Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.1/docs/front.html` & `dogpile.cache-1.2.2/docs/front.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Front Matter &#8212; dogpile.cache 1.2.1 documentation</title>
+    <title>Front Matter &#8212; dogpile.cache 1.2.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -29,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to dogpile.cache’s documentation!"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Front Matter</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -120,15 +120,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to dogpile.cache’s documentation!"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Front Matter</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Front Matter
 ****** Front MatterÂ¶ ******
 Information about the dogpile.cache project.
 ***** Project HomepageÂ¶ *****
 dogpile.cache is hosted on GitHub at https://github.com/sqlalchemy/
 dogpile.cache.
 Releases and project status are available on Pypi at https://pypi.python.org/
@@ -44,10 +44,10 @@
 *** Next topic ***
 Usage_Guide
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Front Matter
 © Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.1/docs/genindex.html` & `dogpile.cache-1.2.2/docs/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; dogpile.cache 1.2.1 documentation</title>
+    <title>Index &#8212; dogpile.cache 1.2.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -20,15 +20,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -1135,15 +1135,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Index
 ****** Index ******
 Symbols | A | B | C | D | E | F | G | H | I | K | L | M | N | P | R | S | T | U
 | V | W
 ***** Symbols *****
     * **kw_(dogpile.cache.plugins.mako_cache.MakoPlugin.get_parameter)
           o (dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create
@@ -369,10 +369,10 @@
           o (dogpile.cache.region.RegionInvalidationStrategy       method)
             method)
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Index
 © Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.1/docs/index.html` & `dogpile.cache-1.2.2/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Welcome to dogpile.cache’s documentation! &#8212; dogpile.cache 1.2.1 documentation</title>
+    <title>Welcome to dogpile.cache’s documentation! &#8212; dogpile.cache 1.2.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -25,15 +25,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              accesskey="N">next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Welcome to dogpile.cache’s documentation!</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -92,14 +92,15 @@
 <li class="toctree-l2"><a class="reference internal" href="api.html#module-dogpile.cache.exception">Exceptions</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#module-dogpile.cache.plugins.mako_cache">Plugins</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#utilities">Utilities</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#dogpile-core">dogpile Core</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="changelog.html">Changelog</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.2.2">1.2.2</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.2.1">1.2.1</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.2.0">1.2.0</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.8">1.1.8</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.7">1.1.7</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.6">1.1.6</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.5">1.1.5</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.4">1.1.4</a></li>
@@ -204,15 +205,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              >next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Welcome to dogpile.cache’s documentation!</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Welcome to dogpile.cacheâs documentation!
 ****** Welcome to dogpile.cacheâs documentation!Â¶ ******
 Dogpile consists of two subsystems, one building on top of the other.
 dogpile provides the concept of a âdogpile lockâ, a control structure which
 allows a single thread of execution to be selected as the âcreatorâ of some
 resource, while allowing other threads of execution to refer to the previous
 version of this resource as the creation proceeds; if there is no previous
@@ -51,14 +51,15 @@
           o Backend_API
           o Backends
           o Exceptions
           o Plugins
           o Utilities
           o dogpile_Core
     * Changelog
+          o 1.2.2
           o 1.2.1
           o 1.2.0
           o 1.1.8
           o 1.1.7
           o 1.1.6
           o 1.1.5
           o 1.1.4
@@ -117,10 +118,10 @@
 [q                   ] [Go]
 *** Next topic ***
 Front_Matter
 **** Navigation ****
     * index
     * modules |
     * next |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Welcome to dogpile.cacheâs documentation!
 © Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.1/docs/py-modindex.html` & `dogpile.cache-1.2.2/docs/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; dogpile.cache 1.2.1 documentation</title>
+    <title>Python Module Index &#8212; dogpile.cache 1.2.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -132,15 +132,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Python Module Index
 ****** Python Module Index ******
 d
      
     d
 [-] dogpile
         dogpile.cache.api
@@ -25,10 +25,10 @@
         dogpile.cache.proxy
         dogpile.cache.region
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Python Module Index
 © Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.1/docs/recipes.html` & `dogpile.cache-1.2.2/docs/recipes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Recipes &#8212; dogpile.cache 1.2.1 documentation</title>
+    <title>Recipes &#8212; dogpile.cache 1.2.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -29,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Recipes</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -341,15 +341,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              >next</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Recipes</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Recipes
 ****** RecipesÂ¶ ******
 ***** Invalidating a group of related keysÂ¶ *****
 This recipe presents a way to track the cache keys related to a particular
 region, for the purposes of invalidating a series of keys that relate to a
 particular id.
 Three cached functions, user_fn_one(), user_fn_two(), user_fn_three() each
@@ -247,10 +247,10 @@
 *** Next topic ***
 dogpile_Core
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Recipes
 © Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.1/docs/search.html` & `dogpile.cache-1.2.2/docs/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; dogpile.cache 1.2.1 documentation</title>
+    <title>Search &#8212; dogpile.cache 1.2.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -26,15 +26,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -86,15 +86,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
```

#### html2text {}

```diff
@@ -3,19 +3,19 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Search
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Search
 © Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.1/docs/searchindex.js` & `dogpile.cache-1.2.2/docs/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -366,15 +366,15 @@
         "modul": [0, 1, 4, 6],
         "insid": [0, 6],
         "myapp": [0, 5, 6],
         "tool": [0, 1, 3, 6],
         "foo": [0, 6],
         "ignor": [0, 1, 6],
         "initi": [0, 1, 2, 6],
-        "self": [0, 5, 6],
+        "self": [0, 1, 5, 6],
         "cl": [0, 6],
         "suitabl": [0, 6],
         "caveat": [0, 6],
         "instanc": [0, 1, 2, 5, 6],
         "myclass": [0, 6],
         "again": [0, 2, 6],
         "skip": [0, 6],
@@ -426,15 +426,15 @@
         "datetim": [0, 1, 6],
         "though": [0, 1, 6],
         "upon": [0, 1, 2, 6],
         "after": [0, 1, 5, 6],
         "sinc": [0, 5, 6],
         "last": [0, 6],
         "constructor": [0, 6],
-        "chain": [0, 6],
+        "chain": [0, 1, 6],
         "custom": [0, 1, 5, 6],
         "augment": [0, 1, 6],
         "chang": [0, 1, 2, 4, 5],
         "flag": [0, 1, 6],
         "alreadi": [0, 1, 6],
         "7": [0, 4, 5, 6],
         "strategi": [0, 1, 2, 6],
@@ -979,34 +979,38 @@
         "my_foo": 0,
         "foo1": 0,
         "refer": [0, 1, 2, 4],
         "garbag": 0,
         "collect": 0,
         "possibli": 0,
         "sat": 1,
-        "20": 1,
+        "jul": 1,
         "2023": 1,
+        "pep": 1,
+        "673": 1,
+        "courtesi": 1,
+        "viico": 1,
+        "240": 1,
+        "20": 1,
         "file": [1, 4, 6],
         "root": 1,
         "mypi": 1,
         "dogpil": [1, 3, 5, 6],
-        "courtesi": 1,
         "daverbal": 1,
         "238": 1,
         "wed": 1,
         "apr": 1,
         "26": 1,
         "region": [1, 4, 5],
         "api": [1, 4, 5, 6],
         "defin": [1, 5, 6],
         "simon": 1,
         "hewitt": 1,
         "236": 1,
         "fri": 1,
-        "jul": 1,
         "2022": 1,
         "memcach": [1, 2, 6],
         "223": 1,
         "228": 1,
         "tue": 1,
         "jun": 1,
         "redi": [1, 4, 6],
@@ -1061,15 +1065,14 @@
         "issu": [1, 2, 3, 6],
         "forego": 1,
         "come": 1,
         "out": [1, 5],
         "alessio": 1,
         "bogon": 1,
         "191": 1,
-        "pep": 1,
         "484": 1,
         "annot": 1,
         "aug": 1,
         "173": 1,
         "instal": [1, 4, 6],
         "cfg": 1,
         "wheel": 1,
@@ -2410,18 +2413,19 @@
         "dogpile Core": [
             [0, "dogpile-core"],
             [2, "dogpile-core"]
         ],
         "Changelog": [
             [1, "changelog"]
         ],
-        "1.2.1": [
-            [1, "change-1.2.1"]
+        "1.2.2": [
+            [1, "change-1.2.2"]
         ],
         "bug": [
+            [1, "change-1.2.2-bug"],
             [1, "change-1.2.1-bug"],
             [1, "change-1.1.8-bug"],
             [1, "change-1.1.6-bug"],
             [1, "change-1.1.4-bug"],
             [1, "change-1.1.3-bug"],
             [1, "change-1.1.1-bug"],
             [1, "change-1.0.2-bug"],
@@ -2447,14 +2451,17 @@
             [1, "change-0.5.0-bug"],
             [1, "change-0.4.3-bug"],
             [1, "change-0.4.1-bug"],
             [1, "change-0.4.0-bug"],
             [1, "change-0.3.1-bug"],
             [1, "change-0.3.0-bug"]
         ],
+        "1.2.1": [
+            [1, "change-1.2.1"]
+        ],
         "1.2.0": [
             [1, "change-1.2.0"]
         ],
         "feature": [
             [1, "change-1.2.0-feature"],
             [1, "change-1.1.2-feature"],
             [1, "change-1.1.0-feature"],
```

### Comparing `dogpile.cache-1.2.1/docs/usage.html` & `dogpile.cache-1.2.2/docs/usage.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Usage Guide &#8212; dogpile.cache 1.2.1 documentation</title>
+    <title>Usage Guide &#8212; dogpile.cache 1.2.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
     <script src="_static/sphinx_highlight.js"></script>
@@ -29,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Usage Guide</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -294,15 +294,15 @@
 </dd></dl>
 
 <p>One you have a <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>, the <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.cache_on_arguments" title="dogpile.cache.region.CacheRegion.cache_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_on_arguments()</span></code></a> method can
 be used to decorate functions, but the cache itself can’t be used until
 <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.configure" title="dogpile.cache.region.CacheRegion.configure"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.configure()</span></code></a> is called.  The interface for that method is as follows:</p>
 <dl class="py method">
 <dt class="sig sig-object py">
-<span class="sig-prename descclassname"><span class="pre">CacheRegion.</span></span><span class="sig-name descname"><span class="pre">configure</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">timedelta</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">arguments</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_argument_dict</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_prefix</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">wrap</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Type</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">()</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">replace_existing_backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">region_invalidator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="api.html#dogpile.cache.region.RegionInvalidationStrategy" title="dogpile.cache.region.RegionInvalidationStrategy"><span class="pre">RegionInvalidationStrategy</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><span class="pre">CacheRegion</span></a></span></span></dt>
+<span class="sig-prename descclassname"><span class="pre">CacheRegion.</span></span><span class="sig-name descname"><span class="pre">configure</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">timedelta</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">arguments</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_argument_dict</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_prefix</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">wrap</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Type</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">()</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">replace_existing_backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">region_invalidator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="api.html#dogpile.cache.region.RegionInvalidationStrategy" title="dogpile.cache.region.RegionInvalidationStrategy"><span class="pre">RegionInvalidationStrategy</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Self</span></span></span></dt>
 <dd><p>Configure a <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>.</p>
 <p>The <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a> itself
 is returned.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.backend"></span><strong>backend</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.backend">¶</a> – Required.  This is the name of the
@@ -946,15 +946,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              >next</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.1 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.2 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Usage Guide</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2011-2023 Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.0.1.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Usage Guide
 ****** Usage GuideÂ¶ ******
 ***** OverviewÂ¶ *****
 At the time of this writing, popular key/value servers include Memcached, Redis
 and many others. While these tools all have different usage focuses, they all
 have in common that the storage model is based on the retrieval of a value
 based on a key; as such, they are all potentially suitable for caching,
@@ -101,15 +101,15 @@
 used to decorate functions, but the cache itself canât be used until
 CacheRegion.configure() is called. The interface for that method is as follows:
   CacheRegion.configure(backend: str, expiration_time: float | timedelta | None
   = None, arguments: Mapping[str, Any] | None = None, _config_argument_dict:
   Mapping[str, Any] | None = None, _config_prefix: str | None = None, wrap:
   Sequence[ProxyBackend | Type[ProxyBackend]] = (), replace_existing_backend:
   bool = False, region_invalidator: RegionInvalidationStrategy | None = None)
-  &#x2192; CacheRegion
+  &#x2192; Self
       Configure a CacheRegion.
       The CacheRegion itself is returned.
 The CacheRegion can also be configured from a dictionary, using the
 CacheRegion.configure_from_config() method:
   CacheRegion.configure_from_config(config_dict, prefix)
       Configure from a configuration dictionary and a prefix.
       Example:
@@ -427,10 +427,10 @@
 *** Next topic ***
 Recipes
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.2.1_documentation »
+    * dogpile.cache_1.2.2_documentation »
     * Usage Guide
 © Copyright 2011-2023 Mike Bayer. Created using Sphinx 7.0.1.
```

### Comparing `dogpile.cache-1.2.1/dogpile/cache/api.py` & `dogpile.cache-1.2.2/dogpile/cache/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 from typing import cast
 from typing import Mapping
 from typing import NamedTuple
 from typing import Optional
 from typing import Sequence
 from typing import Union
 
+from ..util.typing import Self
+
 
 class NoValue:
     """Describe a missing cache value.
 
     The :data:`.NO_VALUE` constant should be used.
 
     """
 
     @property
-    def payload(self):
+    def payload(self) -> Self:
         return self
 
     def __repr__(self):
         """Ensure __repr__ is a consistent value in case NoValue is used to
         fill another cache key.
 
         """
@@ -186,15 +188,17 @@
         :param arguments: The ``arguments`` parameter
          passed to :func:`.make_registry`.
 
         """
         raise NotImplementedError()
 
     @classmethod
-    def from_config_dict(cls, config_dict, prefix):
+    def from_config_dict(
+        cls, config_dict: Mapping[str, Any], prefix: str
+    ) -> Self:
         prefix_len = len(prefix)
         return cls(
             dict(
                 (key[prefix_len:], config_dict[key])
                 for key in config_dict
                 if key.startswith(prefix)
             )
```

### Comparing `dogpile.cache-1.2.1/dogpile/cache/backends/__init__.py` & `dogpile.cache-1.2.2/dogpile/cache/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/cache/backends/file.py` & `dogpile.cache-1.2.2/dogpile/cache/backends/file.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/cache/backends/memcached.py` & `dogpile.cache-1.2.2/dogpile/cache/backends/memcached.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/cache/backends/memory.py` & `dogpile.cache-1.2.2/dogpile/cache/backends/memory.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/cache/backends/null.py` & `dogpile.cache-1.2.2/dogpile/cache/backends/null.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/cache/backends/redis.py` & `dogpile.cache-1.2.2/dogpile/cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/cache/exception.py` & `dogpile.cache-1.2.2/dogpile/cache/exception.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/cache/plugins/mako_cache.py` & `dogpile.cache-1.2.2/dogpile/cache/plugins/mako_cache.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/cache/proxy.py` & `dogpile.cache-1.2.2/dogpile/cache/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 Provides a utility and a decorator class that allow for modifying the behavior
 of different backends without altering the class itself or having to extend the
 base backend.
 
 .. versionadded:: 0.5.0  Added support for the :class:`.ProxyBackend` class.
 
 """
-
 from typing import Mapping
 from typing import Optional
 from typing import Sequence
 
 from .api import BackendFormatted
 from .api import BackendSetType
 from .api import CacheBackend
 from .api import CacheMutex
 from .api import KeyType
 from .api import SerializedReturnType
+from ..util.typing import Self
 
 
 class ProxyBackend(CacheBackend):
     """A decorator class for altering the functionality of backends.
 
     Basic usage::
 
@@ -63,15 +63,15 @@
     .. versionadded:: 0.5.0
 
     """
 
     def __init__(self, *arg, **kw):
         pass
 
-    def wrap(self, backend: CacheBackend) -> "ProxyBackend":
+    def wrap(self, backend: CacheBackend) -> Self:
         """Take a backend as an argument and setup the self.proxied property.
         Return an object that be used as a backend by a :class:`.CacheRegion`
         object.
         """
         assert isinstance(backend, CacheBackend) or isinstance(
             backend, ProxyBackend
         )
```

### Comparing `dogpile.cache-1.2.1/dogpile/cache/region.py` & `dogpile.cache-1.2.2/dogpile/cache/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from .util import repr_obj
 from .. import Lock
 from .. import NeedRegenerationException
 from ..util import coerce_string_conf
 from ..util import memoized_property
 from ..util import NameRegistry
 from ..util import PluginLoader
+from ..util.typing import Self
 
 value_version = 2
 """An integer placed in the :class:`.CachedValue`
 so that new versions of dogpile.cache can detect cached
 values from a previous, backwards-incompatible version.
 
 """
@@ -422,15 +423,15 @@
         expiration_time: Optional[Union[float, datetime.timedelta]] = None,
         arguments: Optional[BackendArguments] = None,
         _config_argument_dict: Optional[Mapping[str, Any]] = None,
         _config_prefix: Optional[str] = None,
         wrap: Sequence[Union[ProxyBackend, Type[ProxyBackend]]] = (),
         replace_existing_backend: bool = False,
         region_invalidator: Optional[RegionInvalidationStrategy] = None,
-    ) -> "CacheRegion":
+    ) -> Self:
         """Configure a :class:`.CacheRegion`.
 
         The :class:`.CacheRegion` itself
         is returned.
 
         :param backend:   Required.  This is the name of the
          :class:`.CacheBackend` to use, and is resolved by loading
```

### Comparing `dogpile.cache-1.2.1/dogpile/cache/util.py` & `dogpile.cache-1.2.2/dogpile/cache/util.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/core.py` & `dogpile.cache-1.2.2/dogpile/core.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/lock.py` & `dogpile.cache-1.2.2/dogpile/lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/util/compat.py` & `dogpile.cache-1.2.2/dogpile/util/compat.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/util/langhelpers.py` & `dogpile.cache-1.2.2/dogpile/util/langhelpers.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/util/nameregistry.py` & `dogpile.cache-1.2.2/dogpile/util/nameregistry.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile/util/readwrite_lock.py` & `dogpile.cache-1.2.2/dogpile/util/readwrite_lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/dogpile.cache.egg-info/PKG-INFO` & `dogpile.cache-1.2.2/dogpile.cache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogpile.cache
-Version: 1.2.1
+Version: 1.2.2
 Summary: A caching front-end based on the Dogpile lock.
 Home-page: https://github.com/sqlalchemy/dogpile.cache
 Author: Mike Bayer
 Author-email: mike_mp@zzzcomputing.com
 License: MIT
 Project-URL: Documentation, https://dogpilecache.sqlalchemy.org
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/dogpile.cache/
```

### Comparing `dogpile.cache-1.2.1/dogpile.cache.egg-info/SOURCES.txt` & `dogpile.cache-1.2.2/dogpile.cache.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+.gitignore
+.gitreview
+.pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.rst
 hash_port.py
 log_tests.ini
+mypy.ini
 setup.cfg
 setup.py
 tox.ini
 ./dogpile/__init__.py
 ./dogpile/core.py
 ./dogpile/lock.py
 ./dogpile/py.typed
@@ -25,14 +29,15 @@
 ./dogpile/cache/plugins/__init__.py
 ./dogpile/cache/plugins/mako_cache.py
 ./dogpile/util/__init__.py
 ./dogpile/util/compat.py
 ./dogpile/util/langhelpers.py
 ./dogpile/util/nameregistry.py
 ./dogpile/util/readwrite_lock.py
+./dogpile/util/typing.py
 docs/api.html
 docs/changelog.html
 docs/core_usage.html
 docs/front.html
 docs/genindex.html
 docs/index.html
 docs/py-modindex.html
@@ -66,28 +71,53 @@
 docs/build/api.rst
 docs/build/builder.py
 docs/build/changelog.rst
 docs/build/conf.py
 docs/build/core_usage.rst
 docs/build/front.rst
 docs/build/index.rst
+docs/build/make.bat
 docs/build/recipes.rst
 docs/build/requirements.txt
 docs/build/usage.rst
 docs/build/_static/nature_override.css
 docs/build/_static/site_custom_css.css
 docs/build/_templates/site_custom_sidebars.html
 docs/build/unreleased/README.txt
+dogpile/__init__.py
+dogpile/core.py
+dogpile/lock.py
+dogpile/py.typed
 dogpile.cache.egg-info/PKG-INFO
 dogpile.cache.egg-info/SOURCES.txt
 dogpile.cache.egg-info/dependency_links.txt
 dogpile.cache.egg-info/entry_points.txt
 dogpile.cache.egg-info/not-zip-safe
 dogpile.cache.egg-info/requires.txt
 dogpile.cache.egg-info/top_level.txt
+dogpile/cache/__init__.py
+dogpile/cache/api.py
+dogpile/cache/exception.py
+dogpile/cache/proxy.py
+dogpile/cache/region.py
+dogpile/cache/util.py
+dogpile/cache/backends/__init__.py
+dogpile/cache/backends/file.py
+dogpile/cache/backends/memcached.py
+dogpile/cache/backends/memory.py
+dogpile/cache/backends/null.py
+dogpile/cache/backends/redis.py
+dogpile/cache/plugins/__init__.py
+dogpile/cache/plugins/mako_cache.py
+dogpile/util/__init__.py
+dogpile/util/compat.py
+dogpile/util/langhelpers.py
+dogpile/util/nameregistry.py
+dogpile/util/readwrite_lock.py
+dogpile/util/typing.py
 tests/__init__.py
 tests/conftest.py
 tests/test_backgrounding.py
 tests/test_lock.py
 tests/test_utils.py
 tests/cache/__init__.py
 tests/cache/_fixtures.py
@@ -98,15 +128,23 @@
 tests/cache/test_memory_backend.py
 tests/cache/test_null_backend.py
 tests/cache/test_redis_backend.py
 tests/cache/test_redis_sentinel_backend.py
 tests/cache/test_region.py
 tests/cache/plugins/__init__.py
 tests/cache/plugins/test_mako_cache.py
+tests/tls/README.rst
 tests/tls/ca-root.crt
 tests/tls/client-ca-root.crt
 tests/tls/client.crt
 tests/tls/client.key
 tests/tls/server.key
 tests/tls/server_chain.pem
+tests/tls/generate/Makefile
+tests/tls/generate/tool
+tests/tls/generate/conf/ca-intermediate.conf
+tests/tls/generate/conf/ca-root.conf
+tests/tls/generate/conf/client-ca-root.conf
+tests/tls/generate/conf/client.conf
+tests/tls/generate/conf/server.conf
 tests/util/__init__.py
 tests/util/test_nameregistry.py
```

### Comparing `dogpile.cache-1.2.1/hash_port.py` & `dogpile.cache-1.2.2/hash_port.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/log_tests.ini` & `dogpile.cache-1.2.2/log_tests.ini`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/setup.cfg` & `dogpile.cache-1.2.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 	Documentation=https://dogpilecache.sqlalchemy.org
 	Issue Tracker=https://github.com/sqlalchemy/dogpile.cache/
 
 [options]
 install_requires = 
 	decorator>=4.0.0
 	stevedore>=3.0.0
+	typing_extensions>=4.0.1;python_version<'3.11'
 zip_safe = False
 packages = find:
 python_requires = >=3.6
 include_package_data = True
 package_dir = 
 	=.
```

### Comparing `dogpile.cache-1.2.1/setup.py` & `dogpile.cache-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/cache/__init__.py` & `dogpile.cache-1.2.2/tests/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/cache/_fixtures.py` & `dogpile.cache-1.2.2/tests/cache/_fixtures.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/cache/plugins/test_mako_cache.py` & `dogpile.cache-1.2.2/tests/cache/plugins/test_mako_cache.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/cache/test_dbm_backend.py` & `dogpile.cache-1.2.2/tests/cache/test_dbm_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/cache/test_decorator.py` & `dogpile.cache-1.2.2/tests/cache/test_decorator.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/cache/test_memcached_backend.py` & `dogpile.cache-1.2.2/tests/cache/test_memcached_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/cache/test_null_backend.py` & `dogpile.cache-1.2.2/tests/cache/test_null_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/cache/test_redis_backend.py` & `dogpile.cache-1.2.2/tests/cache/test_redis_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/cache/test_redis_sentinel_backend.py` & `dogpile.cache-1.2.2/tests/cache/test_redis_sentinel_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/cache/test_region.py` & `dogpile.cache-1.2.2/tests/cache/test_region.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/conftest.py` & `dogpile.cache-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/test_backgrounding.py` & `dogpile.cache-1.2.2/tests/test_backgrounding.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/test_lock.py` & `dogpile.cache-1.2.2/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/test_utils.py` & `dogpile.cache-1.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/tls/ca-root.crt` & `dogpile.cache-1.2.2/tests/tls/ca-root.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/tls/client-ca-root.crt` & `dogpile.cache-1.2.2/tests/tls/client-ca-root.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/tls/client.crt` & `dogpile.cache-1.2.2/tests/tls/client.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/tls/client.key` & `dogpile.cache-1.2.2/tests/tls/client.key`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/tls/server.key` & `dogpile.cache-1.2.2/tests/tls/server.key`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/tls/server_chain.pem` & `dogpile.cache-1.2.2/tests/tls/server_chain.pem`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tests/util/test_nameregistry.py` & `dogpile.cache-1.2.2/tests/util/test_nameregistry.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.2.1/tox.ini` & `dogpile.cache-1.2.2/tox.ini`

 * *Files identical despite different names*

