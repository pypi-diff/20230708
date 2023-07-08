# Comparing `tmp/pyllamacpp-2.4.0.tar.gz` & `tmp/pyllamacpp-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllamacpp-2.4.0.tar", last modified: Sat May 27 02:19:28 2023, max compression
+gzip compressed data, was "pyllamacpp-2.4.1.tar", last modified: Sat Jul  8 18:17:10 2023, max compression
```

## Comparing `pyllamacpp-2.4.0.tar` & `pyllamacpp-2.4.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/baby-llama/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/baby-llama/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/benchmark/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/embedding/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/main/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/perplexity/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/perplexity/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/quantize/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/quantize/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/quantize-stats/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/quantize-stats/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/save-load-state/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/save-load-state/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/examples/server/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/examples/server/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/pocs/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/pocs/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/pocs/vdot/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/pocs/vdot/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/scripts/build-info.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/llama.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-27 02:19:18.000000 pyllamacpp-2.4.0/llama.cpp/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.233762 pyllamacpp-2.4.0/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.241762 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.237763 pyllamacpp-2.4.0/pyllamacpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyllamacpp/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/pyllamacpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-05-27 02:19:28.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-05-27 02:19:28.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:19:28.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 02:19:28.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:19:27.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-27 02:19:28.000000 pyllamacpp-2.4.0/pyllamacpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:19:28.245763 pyllamacpp-2.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/src/llama.cpp_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43672 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-27 02:19:17.000000 pyllamacpp-2.4.0/src/main.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/examples/baby-llama/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/examples/baby-llama/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/examples/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/examples/benchmark/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/examples/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/examples/embedding/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/examples/main/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/examples/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/examples/perplexity/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/examples/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/examples/quantize/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/examples/quantize-stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/examples/quantize-stats/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/examples/save-load-state/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/examples/save-load-state/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/examples/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/examples/server/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/pocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/pocs/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/pocs/vdot/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/pocs/vdot/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/scripts/build-info.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/llama.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-08 18:17:00.000000 pyllamacpp-2.4.1/llama.cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.962417 pyllamacpp-2.4.1/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.970417 pyllamacpp-2.4.1/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.970417 pyllamacpp-2.4.1/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.970417 pyllamacpp-2.4.1/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.970417 pyllamacpp-2.4.1/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.970417 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.970417 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.966417 pyllamacpp-2.4.1/pyllamacpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pyllamacpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pyllamacpp/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pyllamacpp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pyllamacpp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pyllamacpp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pyllamacpp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pyllamacpp/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/pyllamacpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-07-08 18:17:10.000000 pyllamacpp-2.4.1/pyllamacpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-08 18:17:10.000000 pyllamacpp-2.4.1/pyllamacpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 18:17:10.000000 pyllamacpp-2.4.1/pyllamacpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-08 18:17:10.000000 pyllamacpp-2.4.1/pyllamacpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 18:17:10.000000 pyllamacpp-2.4.1/pyllamacpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 18:17:10.000000 pyllamacpp-2.4.1/pyllamacpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 18:17:10.974417 pyllamacpp-2.4.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/src/llama.cpp_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    64007 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-08 18:16:59.000000 pyllamacpp-2.4.1/src/main.h
```

### Comparing `pyllamacpp-2.4.0/CMakeLists.txt` & `pyllamacpp-2.4.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/LICENSE` & `pyllamacpp-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/PKG-INFO` & `pyllamacpp-2.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyLLaMACpp
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
 [![Downloads](https://static.pepy.tech/badge/pyllamacpp)](https://pepy.tech/project/pyllamacpp)
+<a target="_blank" href="https://colab.research.google.com/github/abdeladim-s/pyllamacpp/blob/main/examples/PyLLaMACpp.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
 
 Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp)
 
 
 <p align="center">
   <img src="./docs/demo.gif">
 </p>
@@ -168,27 +171,34 @@
 Bob: Welcome! I'm here to assist you with anything you need. What can I do for you today?
 """
 
 prompt_prefix = "\nUser:"
 prompt_suffix = "\nBob:"
 
 model = Model(model_path='/path/to/ggml/model',
+              n_ctx=512,
               prompt_context=prompt_context,
               prompt_prefix=prompt_prefix,
               prompt_suffix=prompt_suffix)
 
 while True:
   try:
     prompt = input("User: ")
     if prompt == '':
       continue
     print(f"Bob: ", end='')
-    for token in model.generate(prompt, antiprompt='User:'):
+    for token in model.generate(prompt,
+                                antiprompt='User:',
+                                n_threads=6,
+                                n_batch=1024,
+                                n_predict=256,
+                                n_keep=48,
+                                repeat_penalty=1.0, ):
       print(f"{token}", end='', flush=True)
-      print()
+    print()
   except KeyboardInterrupt:
     break
 ```
 
 # Supported models
 All models supported by `llama.cpp` should be supported basically:
```

### Comparing `pyllamacpp-2.4.0/README.md` & `pyllamacpp-2.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # PyLLaMACpp
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
 [![Downloads](https://static.pepy.tech/badge/pyllamacpp)](https://pepy.tech/project/pyllamacpp)
+<a target="_blank" href="https://colab.research.google.com/github/abdeladim-s/pyllamacpp/blob/main/examples/PyLLaMACpp.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
 
 Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp)
 
 
 <p align="center">
   <img src="./docs/demo.gif">
 </p>
@@ -155,27 +158,34 @@
 Bob: Welcome! I'm here to assist you with anything you need. What can I do for you today?
 """
 
 prompt_prefix = "\nUser:"
 prompt_suffix = "\nBob:"
 
 model = Model(model_path='/path/to/ggml/model',
+              n_ctx=512,
               prompt_context=prompt_context,
               prompt_prefix=prompt_prefix,
               prompt_suffix=prompt_suffix)
 
 while True:
   try:
     prompt = input("User: ")
     if prompt == '':
       continue
     print(f"Bob: ", end='')
-    for token in model.generate(prompt, antiprompt='User:'):
+    for token in model.generate(prompt,
+                                antiprompt='User:',
+                                n_threads=6,
+                                n_batch=1024,
+                                n_predict=256,
+                                n_keep=48,
+                                repeat_penalty=1.0, ):
       print(f"{token}", end='', flush=True)
-      print()
+    print()
   except KeyboardInterrupt:
     break
 ```
 
 # Supported models
 All models supported by `llama.cpp` should be supported basically:
```

### Comparing `pyllamacpp-2.4.0/llama.cpp/CMakeLists.txt` & `pyllamacpp-2.4.1/llama.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/llama.cpp/examples/CMakeLists.txt` & `pyllamacpp-2.4.1/llama.cpp/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/llama.cpp/scripts/build-info.cmake` & `pyllamacpp-2.4.1/llama.cpp/scripts/build-info.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/llama.cpp/tests/CMakeLists.txt` & `pyllamacpp-2.4.1/llama.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/CMakeLists.txt` & `pyllamacpp-2.4.1/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/LICENSE` & `pyllamacpp-2.4.1/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/attr.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/buffer_info.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/cast.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/chrono.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/complex.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/class.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/common.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/descr.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/init.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/internals.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/type_caster_base.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/detail/typeid.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/eigen.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/embed.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/eval.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/functional.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/gil.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/iostream.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/numpy.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/operators.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/options.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/pybind11.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/pytypes.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/stl/filesystem.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/stl.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/include/pybind11/stl_bind.h` & `pyllamacpp-2.4.1/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tests/CMakeLists.txt` & `pyllamacpp-2.4.1/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pyllamacpp-2.4.1/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tests/test_embed/CMakeLists.txt` & `pyllamacpp-2.4.1/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/FindCatch.cmake` & `pyllamacpp-2.4.1/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/FindEigen3.cmake` & `pyllamacpp-2.4.1/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/FindPythonLibsNew.cmake` & `pyllamacpp-2.4.1/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/check-style.sh` & `pyllamacpp-2.4.1/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/cmake_uninstall.cmake.in` & `pyllamacpp-2.4.1/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/libsize.py` & `pyllamacpp-2.4.1/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/make_changelog.py` & `pyllamacpp-2.4.1/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/pybind11Common.cmake` & `pyllamacpp-2.4.1/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/pybind11Config.cmake.in` & `pyllamacpp-2.4.1/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/pybind11NewTools.cmake` & `pyllamacpp-2.4.1/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/pybind11Tools.cmake` & `pyllamacpp-2.4.1/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/setup_global.py.in` & `pyllamacpp-2.4.1/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pybind11/tools/setup_main.py.in` & `pyllamacpp-2.4.1/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pyllamacpp/_logger.py` & `pyllamacpp-2.4.1/pyllamacpp/_logger.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pyllamacpp/cli.py` & `pyllamacpp-2.4.1/pyllamacpp/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,80 +32,80 @@
 from pyllamacpp.model import Model
 
 LLAMA_CONTEXT_PARAMS_SCHEMA = {
     'n_ctx': {
         'type': int,
         'description': "text context",
         'options': None,
-        'default': -1
-    },
-    'n_parts': {
-        'type': int,
-        'description': "",
-        'options': None,
-        'default': -1
+        'default': 512
     },
     'seed': {
         'type': int,
         'description': "RNG seed",
         'options': None,
         'default': -1
     },
     'f16_kv': {
         'type': bool,
         'description': "use fp16 for KV cache",
         'options': None,
-        'default': 0
+        'default': False
     },
     'logits_all': {
         'type': bool,
         'description': "the llama_eval() call computes all logits, not just the last one",
         'options': None,
-        'default': 0
+        'default': False
     },
     'vocab_only': {
         'type': bool,
         'description': "only load the vocabulary, no weights",
         'options': None,
-        'default': 0
+        'default': False
     },
     'use_mlock': {
         'type': bool,
         'description': "force system to keep model in RAM",
         'options': None,
-        'default': 0
+        'default': False
     },
     'embedding': {
         'type': bool,
         'description': "embedding mode only",
         'options': None,
-        'default': 0
+        'default': False
     }
 }
 
 GPT_PARAMS_SCHEMA = {
     'n_predict': {
             'type': int,
             'description': "Number of tokens to predict",
             'options': None,
-            'default': 50
+            'default': 256
     },
     'n_threads': {
             'type': int,
             'description': "Number of threads",
             'options': None,
             'default': 4
     },
     'repeat_last_n': {
             'type': int,
             'description': "Last n tokens to penalize",
             'options': None,
             'default': 64
     },
     # sampling params
+    'n_keep': {
+        'type': int,
+        'description': "n_keep",
+        'options': None,
+        'default': 48
+    },
     'top_k': {
             'type': int,
             'description': "top_k",
             'options': None,
             'default': 40
     },
     'top_p': {
@@ -120,21 +120,21 @@
             'options': None,
             'default': 0.8
     },
     'repeat_penalty': {
             'type': float,
             'description': "repeat_penalty",
             'options': None,
-            'default': 1.3
+            'default': 1.0
     },
     'n_batch': {
             'type': int,
             'description': "batch size for prompt processing",
             'options': None,
-            'default': True
+            'default': 1024
     }
 }
 
 
 def _get_llama_context_params(args) -> dict:
     """
     Helper function to get params from argparse as a `dict`
```

### Comparing `pyllamacpp-2.4.0/pyllamacpp/model.py` & `pyllamacpp-2.4.1/pyllamacpp/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 
         self.reset()
 
     def reset(self) -> None:
         """Resets the context"""
         self._prompt_context_tokens = pp.llama_tokenize(self._ctx, self.prompt_cntext, True)
         self._prompt_prefix_tokens = pp.llama_tokenize(self._ctx, self.prompt_prefix, True)
-        self._prompt_suffix_tokens = pp.llama_tokenize(self._ctx, self.prompt_suffix, True)
+        self._prompt_suffix_tokens = pp.llama_tokenize(self._ctx, self.prompt_suffix, False)
         self._last_n_tokens = [0] * self._n_ctx  # n_ctx elements
         self._n_past = 0
 
     def tokenize(self, text: str):
         """
         Returns a list of tokens for the text
         :param text: text to be tokenized
@@ -130,14 +130,16 @@
 
     def generate(self,
                  prompt: str,
                  n_predict: Union[None, int] = None,
                  n_threads: int = 4,
                  seed: Union[None, int] = None,
                  antiprompt: str = None,
+                 n_batch: int = 512,
+                 n_keep: int = 0,
                  top_k: int = 40,
                  top_p: float = 0.95,
                  tfs_z: float = 1.00,
                  typical_p: float = 1.00,
                  temp: float = 0.8,
                  repeat_penalty: float = 1.10,
                  repeat_last_n: int = 64,
@@ -153,14 +155,16 @@
         :param prompt: The prompt :)
         :param n_predict: if n_predict is not None, the inference will stop if it reaches `n_predict` tokens, otherwise
                           it will continue until `EOS`
         :param n_threads: The number of CPU threads
         :param seed: Set rng seed, leave it None for random
         :param antiprompt: aka the stop word, the generation will stop if this word is predicted,
                            keep it None to handle it in your own way
+        :param n_batch: batch size for prompt processing (must be >=32 to use BLAS)
+        :param n_keep: number of tokens to keep from initial prompt
         :param top_k: top K sampling parameter, <= 0 to use vocab size
         :param top_p: top P sampling parameter, 1.0 = disabled
         :param tfs_z: tfs_z sampling parameter, 1.0 = disabled
         :param typical_p: typical_p sampling parameter, 1.0 = disabled
         :param temp: Temperature, 1.0 = disabled
         :param repeat_penalty: repeat penalty sampling parameter, 1.0 = disabled
         :param repeat_last_n: last n tokens to penalize (0 = disable penalty, -1 = context size)
@@ -170,14 +174,16 @@
         :param mirostat_tau: target entropy
         :param mirostat_eta: learning rate
         :param infinite_generation: set it to `True` to make the generation go infinitely
 
         :return: Tokens generator
         """
         # update params
+        self.gpt_params.n_batch = n_batch
+        self.gpt_params.n_keep = n_keep
         self.gpt_params.top_k = top_k
         self.gpt_params.top_p = top_p
         self.gpt_params.tfs_z = tfs_z
         self.gpt_params.typical_p = typical_p
         self.gpt_params.temp = temp
         self.gpt_params.repeat_penalty = repeat_penalty
         self.gpt_params.repeat_last_n = repeat_last_n
@@ -189,22 +195,26 @@
 
         if seed is not None:
             pp.llama_set_rng_seed(self._ctx, seed)
         else:
             seed = int(time.time())
             pp.llama_set_rng_seed(self._ctx, seed)
 
-        input_tokens = self._prompt_prefix_tokens + pp.llama_tokenize(self._ctx, prompt,
-                                                                      True) + self._prompt_suffix_tokens
+        input_tokens = self._prompt_prefix_tokens + \
+                       pp.llama_tokenize(self._ctx, prompt, len(self._prompt_prefix_tokens) == 0) + \
+                       self._prompt_suffix_tokens
+
+        # input_tokens = pp.llama_tokenize(self._ctx, prompt, True)
+
         if len(input_tokens) > self._n_ctx - 4:
             raise Exception('Prompt too long!')
         predicted_tokens = []
         predicted_token = 0
 
-        # add global context for the first time
+        # add global context if no past yet
         if self._n_past == 0:
             for tok in self._prompt_context_tokens:
                 predicted_tokens.append(tok)
                 self._last_n_tokens.pop(0)
                 self._last_n_tokens.append(tok)
 
         # consume input tokens
@@ -222,28 +232,29 @@
 
         while infinite_generation or predicted_token != pp.llama_token_eos():
             if len(predicted_tokens) > 0:
                 # infinite text generation via context swapping
                 if (self._n_past + len(predicted_tokens)) > n_ctx:
                     n_left = self._n_past - self.gpt_params.n_keep
                     self._n_past = max(1, self.gpt_params.n_keep)
-                    predicted_tokens[:0] = self._last_n_tokens[n_ctx - n_left // 2 - len(predicted_tokens):len(self._last_n_tokens) - len(predicted_tokens)]
+                    predicted_tokens[:0] = self._last_n_tokens[
+                                           n_ctx - n_left // 2 - len(predicted_tokens):len(self._last_n_tokens) - len(
+                                               predicted_tokens)]
 
                 for i in range(0, len(predicted_tokens), self.gpt_params.n_batch):
                     n_eval = len(predicted_tokens) - i
                     if n_eval > self.gpt_params.n_batch:
                         n_eval = self.gpt_params.n_batch
 
-                    if (pp.llama_eval(self._ctx,
-                                      predicted_tokens[i:],
-                                      n_eval,
-                                      self._n_past,
-                                      n_threads)):
-                        raise Exception("Model eval failed!")
-                self._n_past += n_eval
+                    pp.llama_eval(self._ctx,
+                                  predicted_tokens[i:],
+                                  n_eval,
+                                  self._n_past,
+                                  n_threads)
+                    self._n_past += n_eval
 
             predicted_tokens.clear()
 
             # sampling
             predicted_token = pp.sample_next_token(self._ctx, self.gpt_params, self._last_n_tokens)
 
             predicted_tokens.append(predicted_token)
@@ -313,15 +324,15 @@
                      presence_penalty: float = 0.00,
                      mirostat: int = 0,
                      mirostat_tau: int = 5.00,
                      mirostat_eta: int = 0.1,
                      n_batch: int = 8,
                      n_keep: int = 0,
                      interactive: bool = False,
-                     antiprompt: List = [],
+                     anti_prompt: List = [],
                      instruct: bool = False,
                      verbose_prompt: bool = False,
                      ) -> str:
         """
         The generate function from `llama.cpp`
 
         :param prompt: the prompt
@@ -339,15 +350,15 @@
         :param presence_penalty: 0.0 = disabled
         :param mirostat: 0 = disabled, 1 = mirostat, 2 = mirostat 2.0
         :param mirostat_tau: target entropy
         :param mirostat_eta: learning rate
         :param n_batch: GPT params n_batch
         :param n_keep: GPT params n_keep
         :param interactive: interactive communication
-        :param antiprompt: list of anti prompts
+        :param anti_prompt: list of anti prompts
         :param instruct: Activate instruct mode
         :param verbose_prompt: verbose prompt
         :return: the new generated text
         """
         self.gpt_params.prompt = prompt
         self.gpt_params.n_predict = n_predict
         self.gpt_params.n_threads = n_threads
@@ -362,15 +373,15 @@
         self.gpt_params.presence_penalty = presence_penalty
         self.gpt_params.mirostat = mirostat
         self.gpt_params.mirostat_tau = mirostat_tau
         self.gpt_params.mirostat_eta = mirostat_eta
         self.gpt_params.n_batch = n_batch
         self.gpt_params.n_keep = n_keep
         self.gpt_params.interactive = interactive
-        self.gpt_params.antiprompt = antiprompt
+        self.gpt_params.anti_prompt = anti_prompt
         self.gpt_params.instruct = instruct
         self.gpt_params.verbose_prompt = verbose_prompt
 
         # assign new_text_callback
         self.res = ""
         Model._new_text_callback = new_text_callback
 
@@ -394,10 +405,51 @@
     def llama_print_timings(self):
         pp.llama_print_timings(self._ctx)
 
     @staticmethod
     def llama_print_system_info():
         pp.llama_print_system_info()
 
+    def get_embeddings(self) -> List[float]:
+        """
+        Get the embeddings for the input
+
+        :return the last embeddings vector from the context (shape: [n_embd] (1-dimensional))
+        """
+        assert self.llama_params.embedding, "The model should be instanciated with embedding=True to get the embeddings"
+        return pp.llama_get_embeddings(self._ctx)
+
+    def get_prompt_embeddings(self,
+                              prompt: str,
+                              n_threads: int = 4,
+                              n_batch: int = 512
+                              ) -> List[float]:
+        """
+        Get the embeddings of a specific prompt
+
+        :warning: this will reset the context
+
+        :param prompt: the prompt :)
+        :param n_threads: The number of CPU threads
+        :param n_batch: batch size for prompt processing (must be >=32 to use BLAS)
+        :return The embeddings vector
+        """
+        assert self.llama_params.embedding, "The model should be instanced with embedding=True to get the embeddings"
+        self.reset()
+        tokens = self.tokenize(prompt)
+        for i in range(0, len(tokens), n_batch):
+            n_eval = len(tokens) - i
+            if n_eval > n_batch:
+                n_eval = n_batch
+
+            pp.llama_eval(self._ctx,
+                          tokens[i:],
+                          n_eval,
+                          0,
+                          n_threads)
+        embeddings = self.get_embeddings()
+        self.reset()
+        return embeddings
+
     def __del__(self):
         if self._ctx:
             pp.llama_free(self._ctx)
```

### Comparing `pyllamacpp-2.4.0/pyllamacpp/utils.py` & `pyllamacpp-2.4.1/pyllamacpp/utils.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pyllamacpp/webui.py` & `pyllamacpp-2.4.1/pyllamacpp/webui.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pyllamacpp.egg-info/PKG-INFO` & `pyllamacpp-2.4.1/pyllamacpp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyLLaMACpp
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
 [![Downloads](https://static.pepy.tech/badge/pyllamacpp)](https://pepy.tech/project/pyllamacpp)
+<a target="_blank" href="https://colab.research.google.com/github/abdeladim-s/pyllamacpp/blob/main/examples/PyLLaMACpp.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
 
 Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp)
 
 
 <p align="center">
   <img src="./docs/demo.gif">
 </p>
@@ -168,27 +171,34 @@
 Bob: Welcome! I'm here to assist you with anything you need. What can I do for you today?
 """
 
 prompt_prefix = "\nUser:"
 prompt_suffix = "\nBob:"
 
 model = Model(model_path='/path/to/ggml/model',
+              n_ctx=512,
               prompt_context=prompt_context,
               prompt_prefix=prompt_prefix,
               prompt_suffix=prompt_suffix)
 
 while True:
   try:
     prompt = input("User: ")
     if prompt == '':
       continue
     print(f"Bob: ", end='')
-    for token in model.generate(prompt, antiprompt='User:'):
+    for token in model.generate(prompt,
+                                antiprompt='User:',
+                                n_threads=6,
+                                n_batch=1024,
+                                n_predict=256,
+                                n_keep=48,
+                                repeat_penalty=1.0, ):
       print(f"{token}", end='', flush=True)
-      print()
+    print()
   except KeyboardInterrupt:
     break
 ```
 
 # Supported models
 All models supported by `llama.cpp` should be supported basically:
```

### Comparing `pyllamacpp-2.4.0/pyllamacpp.egg-info/SOURCES.txt` & `pyllamacpp-2.4.1/pyllamacpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/pyproject.toml` & `pyllamacpp-2.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/setup.py` & `pyllamacpp-2.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyllamacpp",
-    version="2.4.0",
+    version="2.4.1",
     author="Abdeladim Sadiki",
     description="Python bindings for llama.cpp",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pyllamacpp")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
```

### Comparing `pyllamacpp-2.4.0/src/llama.cpp_LICENSE` & `pyllamacpp-2.4.1/src/llama.cpp_LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.4.0/src/main.cpp` & `pyllamacpp-2.4.1/src/main.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -104,15 +104,28 @@
 }
 
 std::vector<llama_token> llama_tokenize_wrapper(
         struct llama_context_wrapper * ctx_w,
         const std::string & text,
         bool   add_bos){
 
-        struct llama_context * ctx = ctx_w->ptr;
+    struct llama_context * ctx = ctx_w->ptr;
+    std::vector<llama_token> tokens((text.size() + (int)add_bos));
+    int new_size = llama_tokenize(ctx, text.c_str(), tokens.data(), tokens.size(), add_bos);
+    assert(new_size >= 0);
+    tokens.resize(new_size);
+    return tokens;
+}
+
+
+std::vector<llama_token> llama_tokenize_wrapper_2(
+        struct llama_context * ctx,
+        const std::string & text,
+        bool   add_bos){
+
         std::vector<llama_token> tokens((text.size() + (int)add_bos));
         int new_size = llama_tokenize(ctx, text.c_str(), tokens.data(), tokens.size(), add_bos);
         assert(new_size >= 0);
         tokens.resize(new_size);
         return tokens;
 }
 
@@ -179,17 +192,20 @@
 
 float * llama_get_logits_wrapper(struct llama_context_wrapper * ctx_w){
    struct llama_context * ctx = ctx_w->ptr;
   return llama_get_logits(ctx);
 
 }
 
-float * llama_get_embeddings_wrapper(struct llama_context_wrapper * ctx_w){
+std::vector<float> llama_get_embeddings_wrapper(struct llama_context_wrapper * ctx_w){
     struct llama_context * ctx = ctx_w->ptr;
-    return llama_get_embeddings(ctx);
+    int n_embed = llama_n_embd(ctx);
+    float * embed_ptr = llama_get_embeddings(ctx);
+    std::vector<float> embeddings(embed_ptr, embed_ptr + n_embed);
+    return embeddings;
 }
 
 const char * llama_token_to_str_wrapper(struct llama_context_wrapper * ctx_w, llama_token token){
     struct llama_context * ctx = ctx_w->ptr;
     return llama_token_to_str(ctx, token);
 }
 
@@ -301,15 +317,15 @@
 }
 
 void llama_reset_timings_wrapper(struct llama_context_wrapper * ctx_w){
     struct llama_context * ctx = ctx_w->ptr;
     return llama_reset_timings(ctx);
 }
 
-llama_token sample_next_token(struct llama_context_wrapper * ctx_w, gpt_params params, std::vector<llama_token> last_n_tokens){
+llama_token sample_next_token(struct llama_context_wrapper * ctx_w, gpt_params params, std::vector<llama_token> & last_n_tokens){
     // helper function to sample next token (based on the main example)
     struct llama_context * ctx = ctx_w->ptr;
     const int n_ctx = llama_n_ctx(ctx);
     llama_token id = 0;
 
     const float   temp            = params.temp;
     const int32_t top_k           = params.top_k <= 0 ? llama_n_vocab(ctx) : params.top_k;
@@ -384,14 +400,15 @@
 //        last_n_tokens.push_back(id);
     }
 
     return id;
 }
 
 
+
 std::string gpt_random_prompt(std::mt19937 & rng) {
     const int r = rng() % 10;
     switch (r) {
         case 0: return "So";
         case 1: return "Once upon a time";
         case 2: return "When";
         case 3: return "The";
@@ -453,15 +470,15 @@
 
         return 0;
     }
 
     // Add a space in front of the first character to match OG llama tokenizer behavior
     params.prompt.insert(0, 1, ' ');
 
-    std::string path_session = params.path_session;
+    std::string path_session = params.path_prompt_cache;
     std::vector<llama_token> session_tokens;
 
     if (!path_session.empty()) {
         fprintf(stderr, "%s: attempting to load saved session from '%s'\n", __func__, path_session.c_str());
 
         // fopen to check for existing session
         FILE * fp = std::fopen(path_session.c_str(), "rb");
@@ -786,15 +803,15 @@
         }
 
         // display text
         if (input_echo) {
             for (auto id : embd) {
                 // @NOTE: model.cpp_generate invokes llama_generate() with a python callback function.
                 // @NOTE: we need to make sure that when the python callback function is called, it gets callback with raw bytes
-                // @NOTE: of generated token, else pybind with implicityl try to decode it to Unicode, and cause UnicodeDecodeError
+                // @NOTE: of generated token, else pybind with implicitly try to decode it to Unicode, and cause UnicodeDecodeError
                 std::string tok_str = llama_token_to_str(ctx, id);
                 new_text_callback(py::bytes(tok_str));
             }
             fflush(stdout);
         }
         // reset color to default if we there is no pending user input
 //        if (input_echo && (int)embd_inp.size() == n_consumed) {
@@ -818,14 +835,450 @@
         }
     }
 
     llama_print_timings(ctx);
     return 0;
 }
 
+// @NOTE: Experimental
+class LLaMAModel {
+
+public:
+    struct llama_context * ctx;
+//    gpt_params params;
+    std::string path_session;
+    std::vector<llama_token> session_tokens;
+    std::vector<llama_token> embd_inp;
+    std::vector<llama_token> last_n_tokens;
+    int n_ctx;
+    int n_past             = 0;
+    int n_remain = 25;
+    int n_consumed         = 0;
+    int n_session_consumed = 0;
+    bool is_antiprompt        = false;
+    bool input_echo           = true;
+    bool need_to_save_session = false;
+    size_t n_matching_session_tokens = 0;
+    bool is_interacting = false;
+
+    std::vector<llama_token> embd;
+    std::vector<llama_token> embd_out;
+
+    // Constructor
+    LLaMAModel(struct llama_context_wrapper * ctx_w, gpt_params g_params, int n): last_n_tokens(n) {
+        ctx = ctx_w->ptr;
+        g_ctx = &ctx;
+        n_ctx = n;
+        last_n_tokens.reserve(n_ctx);
+        std::fill(last_n_tokens.begin(), last_n_tokens.end(), 0);
+    }
+
+    int setup(gpt_params & params){
+        path_session = params.path_prompt_cache;
+        if (!path_session.empty()) {
+            fprintf(stderr, "%s: attempting to load saved session from '%s'\n", __func__, path_session.c_str());
+
+            // fopen to check for existing session
+            FILE * fp = std::fopen(path_session.c_str(), "rb");
+            if (fp != NULL) {
+                std::fclose(fp);
+
+                session_tokens.resize(params.n_ctx);
+                size_t n_token_count_out = 0;
+                if (!llama_load_session_file(ctx, path_session.c_str(), session_tokens.data(), session_tokens.capacity(), &n_token_count_out)) {
+                    fprintf(stderr, "%s: error: failed to load session file '%s'\n", __func__, path_session.c_str());
+                    return 1;
+                }
+                session_tokens.resize(n_token_count_out);
+                llama_set_rng_seed(ctx, params.seed);
+
+                fprintf(stderr, "%s: loaded a session with prompt size of %d tokens\n", __func__, (int) session_tokens.size());
+            } else {
+                fprintf(stderr, "%s: session file does not exist, will create\n", __func__);
+            }
+        }
+
+
+        // in instruct mode, we inject a prefix and a suffix to each input by the user
+        if (params.instruct) {
+            params.interactive_first = true;
+            params.antiprompt.push_back("### Instruction:\n\n");
+        }
+
+        // enable interactive mode if interactive start is specified
+        if (params.interactive_first) {
+            params.interactive = true;
+        }
+
+
+        if (params.verbose_prompt) {
+            fprintf(stderr, "\n");
+            fprintf(stderr, "%s: prompt: '%s'\n", __func__, params.prompt.c_str());
+            fprintf(stderr, "%s: number of tokens in prompt = %zu\n", __func__, embd_inp.size());
+            for (int i = 0; i < (int) embd_inp.size(); i++) {
+                fprintf(stderr, "%6d -> '%s'\n", embd_inp[i], llama_token_to_str(ctx, embd_inp[i]));
+            }
+            if (params.n_keep > 0) {
+                fprintf(stderr, "%s: static prompt based on n_keep: '", __func__);
+                for (int i = 0; i < params.n_keep; i++) {
+                    fprintf(stderr, "%s", llama_token_to_str(ctx, embd_inp[i]));
+                }
+                fprintf(stderr, "'\n");
+            }
+            fprintf(stderr, "\n");
+        }
+
+        fprintf(stderr, "sampling: repeat_last_n = %d, repeat_penalty = %f, presence_penalty = %f, frequency_penalty = %f, top_k = %d, tfs_z = %f, top_p = %f, typical_p = %f, temp = %f, mirostat = %d, mirostat_lr = %f, mirostat_ent = %f\n",
+                params.repeat_last_n, params.repeat_penalty, params.presence_penalty, params.frequency_penalty, params.top_k, params.tfs_z, params.top_p, params.typical_p, params.temp, params.mirostat, params.mirostat_eta, params.mirostat_tau);
+        fprintf(stderr, "generate: n_ctx = %d, n_batch = %d, n_predict = %d, n_keep = %d\n", n_ctx, params.n_batch, params.n_predict, params.n_keep);
+        fprintf(stderr, "\n\n");
+
+        need_to_save_session = !path_session.empty() && n_matching_session_tokens < embd_inp.size();
+        n_remain = params.n_predict;
+        // tokenize the prompt
+        if (params.interactive_first || params.instruct || !params.prompt.empty() || session_tokens.empty()) {
+            // Add a space in front of the first character to match OG llama tokenizer behavior
+            params.prompt.insert(0, 1, ' ');
+
+            embd_inp = llama_tokenize_wrapper_2(ctx, params.prompt, true);
+        } else {
+            embd_inp = session_tokens;
+        }
+
+        if ((int) embd_inp.size() > n_ctx - 4) {
+            fprintf(stderr, "%s: error: prompt is too long (%d tokens, max %d)\n", __func__, (int) embd_inp.size(), n_ctx - 4);
+            return 1;
+        }
+        // debug message about similarity of saved session, if applicable
+        size_t n_matching_session_tokens = 0;
+        if (session_tokens.size()) {
+            for (llama_token id : session_tokens) {
+                if (n_matching_session_tokens >= embd_inp.size() || id != embd_inp[n_matching_session_tokens]) {
+                    break;
+                }
+                n_matching_session_tokens++;
+            }
+            if (params.prompt.empty() && n_matching_session_tokens == embd_inp.size()) {
+                fprintf(stderr, "%s: using full prompt from session file\n", __func__);
+            } else if (n_matching_session_tokens >= embd_inp.size()) {
+                fprintf(stderr, "%s: session file has exact match for prompt!\n", __func__);
+            } else if (n_matching_session_tokens < (embd_inp.size() / 2)) {
+                fprintf(stderr, "%s: warning: session file has low similarity to prompt (%zu / %zu tokens); will mostly be reevaluated\n",
+                        __func__, n_matching_session_tokens, embd_inp.size());
+            } else {
+                fprintf(stderr, "%s: session file matches %zu / %zu tokens of prompt\n",
+                        __func__, n_matching_session_tokens, embd_inp.size());
+            }
+        }
+
+        if (params.n_keep < 0 || params.n_keep > (int) embd_inp.size() || params.instruct) {
+            params.n_keep = (int)embd_inp.size();
+        }
+        if (params.interactive) {
+            is_interacting = params.interactive_first;
+        }
+
+        return 0;
+    }
+
+    void update_prompt(gpt_params & params, std::string buffer){
+        // prefix & suffix for instruct mode
+        const auto inp_pfx = llama_tokenize_wrapper_2(ctx, "\n\n### Instruction:\n\n", true);
+        const auto inp_sfx = llama_tokenize_wrapper_2(ctx, "\n\n### Response:\n\n", false);
+
+
+        if (!params.input_prefix.empty()) {
+            buffer += params.input_prefix;
+            printf("%s", buffer.c_str());
+        }
+
+        // Add tokens to embd only if the input buffer is non-empty
+        // Entering a empty line lets the user pass control back
+        if (buffer.length() > 1) {
+            // append input suffix if any
+            if (!params.input_suffix.empty()) {
+                buffer += params.input_suffix;
+                printf("%s", params.input_suffix.c_str());
+            }
+
+            // instruct mode: insert instruction prefix
+            if (params.instruct && !is_antiprompt) {
+                n_consumed = embd_inp.size();
+                embd_inp.insert(embd_inp.end(), inp_pfx.begin(), inp_pfx.end());
+            }
+
+            auto line_inp = llama_tokenize_wrapper_2(ctx, buffer, false);
+            embd_inp.insert(embd_inp.end(), line_inp.begin(), line_inp.end());
+
+            // instruct mode: insert response suffix
+            if (params.instruct) {
+                embd_inp.insert(embd_inp.end(), inp_sfx.begin(), inp_sfx.end());
+            }
+
+            n_remain -= line_inp.size();
+        }
+//        input_echo = false;
+
+    }
+
+    int generate(gpt_params & params){
+        // determine newline token
+        auto llama_token_newline = llama_tokenize_wrapper_2(ctx, "\n", false);
+
+
+        // predict
+        if (embd.size() > 0) {
+            // infinite text generation via context swapping
+            // if we run out of context:
+            // - take the n_keep first tokens from the original prompt (via n_past)
+            // - take half of the last (n_ctx - n_keep) tokens and recompute the logits in batches
+            if (n_past + (int) embd.size() > n_ctx) {
+                const int n_left = n_past - params.n_keep;
+
+                // always keep the first token - BOS
+                n_past = std::max(1, params.n_keep);
+
+                // insert n_left/2 tokens at the start of embd from last_n_tokens
+                embd.insert(embd.begin(), last_n_tokens.begin() + n_ctx - n_left/2 - embd.size(), last_n_tokens.end() - embd.size());
+
+                // stop saving session if we run out of context
+                path_session.clear();
+
+                //printf("\n---\n");
+                //printf("resetting: '");
+                //for (int i = 0; i < (int) embd.size(); i++) {
+                //    printf("%s", llama_token_to_str(ctx, embd[i]));
+                //}
+                //printf("'\n");
+                //printf("\n---\n");
+            }
+
+            // try to reuse a matching prefix from the loaded session instead of re-eval (via n_past)
+            if (n_session_consumed < (int) session_tokens.size()) {
+                size_t i = 0;
+                for ( ; i < embd.size(); i++) {
+                    if (embd[i] != session_tokens[n_session_consumed]) {
+                        session_tokens.resize(n_session_consumed);
+                        break;
+                    }
+
+                    n_past++;
+                    n_session_consumed++;
+
+                    if (n_session_consumed >= (int) session_tokens.size()) {
+                        ++i;
+                        break;
+                    }
+                }
+                if (i > 0) {
+                    embd.erase(embd.begin(), embd.begin() + i);
+                }
+            }
+
+            // evaluate tokens in batches
+            // embd is typically prepared beforehand to fit within a batch, but not always
+            for (int i = 0; i < (int) embd.size(); i += params.n_batch) {
+                int n_eval = (int) embd.size() - i;
+                if (n_eval > params.n_batch) {
+                    n_eval = params.n_batch;
+                }
+                if (llama_eval(ctx, &embd[i], n_eval, n_past, params.n_threads)) {
+                    fprintf(stderr, "%s : failed to eval\n", __func__);
+                    return 1;
+                }
+                n_past += n_eval;
+            }
+
+            if (embd.size() > 0 && !path_session.empty()) {
+                session_tokens.insert(session_tokens.end(), embd.begin(), embd.end());
+                n_session_consumed = session_tokens.size();
+            }
+        }
+
+        embd.clear();
+        embd_out.clear();
+
+        if ((int) embd_inp.size() <= n_consumed && !is_interacting) {
+            // out of user input, sample next token
+            const float   temp            = params.temp;
+            const int32_t top_k           = params.top_k <= 0 ? llama_n_vocab(ctx) : params.top_k;
+            const float   top_p           = params.top_p;
+            const float   tfs_z           = params.tfs_z;
+            const float   typical_p       = params.typical_p;
+            const int32_t repeat_last_n   = params.repeat_last_n < 0 ? n_ctx : params.repeat_last_n;
+            const float   repeat_penalty  = params.repeat_penalty;
+            const float   alpha_presence  = params.presence_penalty;
+            const float   alpha_frequency = params.frequency_penalty;
+            const int     mirostat        = params.mirostat;
+            const float   mirostat_tau    = params.mirostat_tau;
+            const float   mirostat_eta    = params.mirostat_eta;
+            const bool    penalize_nl     = params.penalize_nl;
+
+            // optionally save the session on first sample (for faster prompt loading next time)
+            if (!path_session.empty() && need_to_save_session) {
+                need_to_save_session = false;
+                llama_save_session_file(ctx, path_session.c_str(), session_tokens.data(), session_tokens.size());
+            }
+
+            llama_token id = 0;
+
+            {
+                auto logits  = llama_get_logits(ctx);
+                auto n_vocab = llama_n_vocab(ctx);
+
+                // Apply params.logit_bias map
+                for (auto it = params.logit_bias.begin(); it != params.logit_bias.end(); it++) {
+                    logits[it->first] += it->second;
+                }
+
+                std::vector<llama_token_data> candidates;
+                candidates.reserve(n_vocab);
+                for (llama_token token_id = 0; token_id < n_vocab; token_id++) {
+                    candidates.emplace_back(llama_token_data{token_id, logits[token_id], 0.0f});
+                }
+
+                llama_token_data_array candidates_p = { candidates.data(), candidates.size(), false };
+
+                // Apply penalties
+                float nl_logit = logits[llama_token_nl()];
+                auto last_n_repeat = std::min(std::min((int)last_n_tokens.size(), repeat_last_n), n_ctx);
+                llama_sample_repetition_penalty(ctx, &candidates_p,
+                                                last_n_tokens.data() + last_n_tokens.size() - last_n_repeat,
+                                                last_n_repeat, repeat_penalty);
+                llama_sample_frequency_and_presence_penalties(ctx, &candidates_p,
+                                                              last_n_tokens.data() + last_n_tokens.size() - last_n_repeat,
+                                                              last_n_repeat, alpha_frequency, alpha_presence);
+                if (!penalize_nl) {
+                    logits[llama_token_nl()] = nl_logit;
+                }
+
+                if (temp <= 0) {
+                    // Greedy sampling
+                    id = llama_sample_token_greedy(ctx, &candidates_p);
+                } else {
+                    if (mirostat == 1) {
+                        static float mirostat_mu = 2.0f * mirostat_tau;
+                        const int mirostat_m = 100;
+                        llama_sample_temperature(ctx, &candidates_p, temp);
+                        id = llama_sample_token_mirostat(ctx, &candidates_p, mirostat_tau, mirostat_eta, mirostat_m, &mirostat_mu);
+                    } else if (mirostat == 2) {
+                        static float mirostat_mu = 2.0f * mirostat_tau;
+                        llama_sample_temperature(ctx, &candidates_p, temp);
+                        id = llama_sample_token_mirostat_v2(ctx, &candidates_p, mirostat_tau, mirostat_eta, &mirostat_mu);
+                    } else {
+                        // Temperature sampling
+                        llama_sample_top_k(ctx, &candidates_p, top_k, 1);
+                        llama_sample_tail_free(ctx, &candidates_p, tfs_z, 1);
+                        llama_sample_typical(ctx, &candidates_p, typical_p, 1);
+                        llama_sample_top_p(ctx, &candidates_p, top_p, 1);
+                        llama_sample_temperature(ctx, &candidates_p, temp);
+                        id = llama_sample_token(ctx, &candidates_p);
+                    }
+                }
+                // printf("`%d`", candidates_p.size);
+
+                last_n_tokens.erase(last_n_tokens.begin());
+                last_n_tokens.push_back(id);
+            }
+
+            // replace end of text token with newline token when in interactive mode
+            if (id == llama_token_eos() && params.interactive && !params.instruct) {
+                id = llama_token_newline.front();
+                if (params.antiprompt.size() != 0) {
+                    // tokenize and inject first reverse prompt
+                    const auto first_antiprompt = llama_tokenize_wrapper_2(ctx, params.antiprompt.front(), false);
+                    embd_inp.insert(embd_inp.end(), first_antiprompt.begin(), first_antiprompt.end());
+                }
+            }
+
+            // add it to the context
+            embd.push_back(id);
+
+            // echo this to console
+            input_echo = true;
+
+            // decrement remaining sampling budget
+            --n_remain;
+        } else {
+            // some user input remains from prompt or interaction, forward it to processing
+            while ((int) embd_inp.size() > n_consumed) {
+                embd.push_back(embd_inp[n_consumed]);
+                last_n_tokens.erase(last_n_tokens.begin());
+                last_n_tokens.push_back(embd_inp[n_consumed]);
+                ++n_consumed;
+                if ((int) embd.size() >= params.n_batch) {
+                    break;
+                }
+            }
+        }
+
+
+//        // display text
+//        if (input_echo) {
+//            for (auto id : embd) {
+//                embd_out.push_back(id);
+//            }
+//        }
+
+        // if not currently processing queued inputs;
+        if ((int) embd_inp.size() <= n_consumed) {
+
+            // check for reverse prompt
+            if (params.antiprompt.size()) {
+                std::string last_output;
+                for (auto id : last_n_tokens) {
+                    last_output += llama_token_to_str(ctx, id);
+                }
+
+                is_antiprompt = false;
+                // Check if each of the reverse prompts appears at the end of the output.
+                // If we're not running interactively, the reverse prompt might be tokenized with some following characters
+                // so we'll compensate for that by widening the search window a bit.
+                for (std::string & antiprompt : params.antiprompt) {
+                    size_t extra_padding = params.interactive ? 0 : 2;
+                    size_t search_start_pos = last_output.length() > static_cast<size_t>(antiprompt.length() + extra_padding)
+                                              ? last_output.length() - static_cast<size_t>(antiprompt.length() + extra_padding)
+                                              : 0;
+
+                    if (last_output.find(antiprompt.c_str(), search_start_pos) != std::string::npos) {
+                        if (params.interactive) {
+                            is_interacting = true;
+                        }
+                        is_antiprompt = true;
+                        return 2;  // break
+                    }
+                }
+            }
+
+            if (n_past > 0) {
+                is_interacting = false;
+            }
+        }
+
+        // end of text token
+        if (!embd.empty() && embd.back() == llama_token_eos()) {
+            if (params.instruct) {
+                is_interacting = true;
+            } else {
+                fprintf(stderr, " [end of text]\n");
+                return 2;
+            }
+        }
+
+        if (params.interactive && n_remain <= 0 && params.n_predict != -1) {
+            n_remain = params.n_predict;
+            is_interacting = true;
+        }
+
+        return 0;
+    }
+
+};
+///////////////////
+
 
 PYBIND11_MODULE(_pyllamacpp, m) {
     m.doc() = R"pbdoc(
         PyLLaMACpp: Python binding for llama.cpp
         -----------------------
 
         .. currentmodule:: _pyllamacpp
@@ -836,15 +1289,14 @@
     )pbdoc";
 
     py::class_<gpt_params>(m,"gpt_params" /*,py::dynamic_attr()*/)
         .def(py::init<>())
         .def_readwrite("seed", &gpt_params::seed)
         .def_readwrite("n_threads", &gpt_params::n_threads)
         .def_readwrite("n_predict", &gpt_params::n_predict)
-        .def_readwrite("n_parts", &gpt_params::n_parts)
         .def_readwrite("n_ctx", &gpt_params::n_ctx)
         .def_readwrite("n_batch", &gpt_params::n_batch)
         .def_readwrite("n_keep", &gpt_params::n_keep)
 
         .def_readwrite("logit_bias", &gpt_params::logit_bias)
         .def_readwrite("top_k", &gpt_params::top_k)
         .def_readwrite("top_p", &gpt_params::top_p)
@@ -857,15 +1309,15 @@
         .def_readwrite("presence_penalty", &gpt_params::presence_penalty)
         .def_readwrite("mirostat", &gpt_params::mirostat)
         .def_readwrite("mirostat_tau", &gpt_params::mirostat_tau)
         .def_readwrite("mirostat_eta", &gpt_params::mirostat_eta)
 
         .def_readwrite("model", &gpt_params::model)
         .def_readwrite("prompt", &gpt_params::prompt)
-        .def_readwrite("path_session", &gpt_params::path_session)
+        .def_readwrite("path_prompt_cache", &gpt_params::path_prompt_cache)
         .def_readwrite("input_prefix", &gpt_params::input_prefix)
         .def_readwrite("input_suffix", &gpt_params::input_suffix)
         .def_readwrite("antiprompt", &gpt_params::antiprompt)
 
         .def_readwrite("lora_adapter", &gpt_params::lora_adapter)
         .def_readwrite("lora_base", &gpt_params::lora_base)
 
@@ -1001,14 +1453,30 @@
     m.def("llama_print_timings", &llama_print_timings_wrapper);
     m.def("llama_reset_timings", &llama_reset_timings_wrapper);
 
     m.def("llama_print_system_info", &llama_print_system_info);
 
     m.def("llama_generate", &llama_generate);
 
+    py::class_<LLaMAModel>(m,"LLaMAModel")
+        .def(py::init<llama_context_wrapper *, gpt_params, int>())
+        .def_readwrite("embd", &LLaMAModel::embd)
+        .def_readwrite("n_remain", &LLaMAModel::n_remain)
+        .def_readwrite("is_antiprompt", &LLaMAModel::is_antiprompt)
+        .def_readwrite("n_consumed", &LLaMAModel::n_consumed)
+        .def_readwrite("last_n_tokens", &LLaMAModel::last_n_tokens)
+        .def_readwrite("input_echo", &LLaMAModel::input_echo)
+        .def_readwrite("embd_out", &LLaMAModel::embd_out)
+
+        .def("setup", &LLaMAModel::setup)
+        .def("generate", &LLaMAModel::generate)
+        .def("update_prompt", &LLaMAModel::update_prompt)
+
+       ;
+
 
 #ifdef VERSION_INFO
     m.attr("__version__") = MACRO_STRINGIFY(VERSION_INFO);
 #else
     m.attr("__version__") = "dev";
 #endif
 }
```

### Comparing `pyllamacpp-2.4.0/src/main.h` & `pyllamacpp-2.4.1/src/main.h`

 * *Files 15% similar despite different names*

```diff
@@ -12,22 +12,23 @@
  */
 
 #include <string>
 #include <vector>
 #include <random>
 #include <thread>
 
+
 struct gpt_params {
-    int32_t seed          = -1;   // RNG seed
+    int32_t seed          = -1;  // RNG seed
     int32_t n_threads     = std::min(4, (int32_t) std::thread::hardware_concurrency());
     int32_t n_predict     = -1;  // new tokens to predict
-    int32_t n_parts       = -1;   // amount of model parts (-1 = determine from model dimensions)
-    int32_t n_ctx         = 512;  // context size
-    int32_t n_batch       = 512;  // batch size for prompt processing (must be >=32 to use BLAS)
-    int32_t n_keep        = 0;    // number of tokens to keep from initial prompt
+    int32_t n_ctx         = 512; // context size
+    int32_t n_batch       = 512; // batch size for prompt processing (must be >=32 to use BLAS)
+    int32_t n_keep        = 0;   // number of tokens to keep from initial prompt
+    int32_t n_gpu_layers  = 0;   // number of layers to store in VRAM
 
     // sampling parameters
     std::unordered_map<llama_token, float> logit_bias; // logit bias for specific tokens
     int32_t top_k             = 40;    // <= 0 to use vocab size
     float   top_p             = 0.95f; // 1.0 = disabled
     float   tfs_z             = 1.00f; // 1.0 = disabled
     float   typical_p         = 1.00f; // 1.0 = disabled
@@ -36,28 +37,29 @@
     int32_t repeat_last_n     = 64;    // last n tokens to penalize (0 = disable penalty, -1 = context size)
     float   frequency_penalty = 0.00f; // 0.0 = disabled
     float   presence_penalty  = 0.00f; // 0.0 = disabled
     int     mirostat          = 0;     // 0 = disabled, 1 = mirostat, 2 = mirostat 2.0
     float   mirostat_tau      = 5.00f; // target entropy
     float   mirostat_eta      = 0.10f; // learning rate
 
-    std::string model  = "models/lamma-7B/ggml-model.bin"; // model path
-    std::string prompt = "";
-    std::string path_session = "";       // path to file for saving/loading model eval state
-    std::string input_prefix = "";       // string to prefix user inputs with
-    std::string input_suffix = "";       // string to suffix user inputs with
+    std::string model             = "models/7B/ggml-model.bin"; // model path
+    std::string prompt            = "";
+    std::string path_prompt_cache = "";  // path to file for saving/loading prompt eval state
+    std::string input_prefix      = "";  // string to prefix user inputs with
+    std::string input_suffix      = "";  // string to suffix user inputs with
     std::vector<std::string> antiprompt; // string upon seeing which more user input is prompted
 
     std::string lora_adapter = "";  // lora adapter path
-    std::string lora_base = "";     // base model path for the lora adapter
+    std::string lora_base    = "";  // base model path for the lora adapter
 
     bool memory_f16        = true;  // use f16 instead of f32 for memory kv
     bool random_prompt     = false; // do not randomize prompt if none provided
     bool use_color         = false; // use color to distinguish generations and inputs
     bool interactive       = false; // interactive mode
+    bool prompt_cache_all  = false; // save user input and generations to prompt cache
 
     bool embedding         = false; // get only sentence embedding
     bool interactive_first = false; // wait for user input immediately
     bool multiline_input   = false; // reverse the usage of `\`
 
     bool instruct          = false; // instruction mode (used for Alpaca models)
     bool penalize_nl       = true;  // consider newlines as a repeatable token
```

