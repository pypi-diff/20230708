# Comparing `tmp/configparserc-1.4.1.tar.gz` & `tmp/configparserc-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/configparserc-1.4.1.tar", last modified: Tue Jun 20 01:23:57 2023, max compression
+gzip compressed data, was "dist/configparserc-1.4.2.tar", last modified: Fri Jul  7 23:06:06 2023, max compression
```

## Comparing `configparserc-1.4.1.tar` & `configparserc-1.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 01:23:57.000000 configparserc-1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)    11363 2023-06-20 01:23:42.000000 configparserc-1.4.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      187 2023-06-20 01:23:42.000000 configparserc-1.4.1/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-06-20 01:23:42.000000 configparserc-1.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5363 2023-06-20 01:23:57.000000 configparserc-1.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3746 2023-06-20 01:23:42.000000 configparserc-1.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc/
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-06-20 01:23:42.000000 configparserc-1.4.1/configparserc/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1437023 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc/config.c
--rw-rw-rw-   0 root         (0) root         (0)     3082 2023-06-20 01:23:42.000000 configparserc-1.4.1/configparserc/config.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc/include/
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-06-20 01:23:42.000000 configparserc-1.4.1/configparserc/include/_config.h
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-20 01:23:42.000000 configparserc-1.4.1/configparserc/py.typed
--rw-r--r--   0 root         (0) root         (0)   341654 2023-06-20 01:23:56.000000 configparserc-1.4.1/configparserc/tools.c
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-20 01:23:42.000000 configparserc-1.4.1/configparserc/tools.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5363 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-20 01:23:57.000000 configparserc-1.4.1/configparserc.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-06-20 01:23:57.000000 configparserc-1.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    14641 2023-06-20 01:23:42.000000 configparserc-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 23:06:06.000000 configparserc-1.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11363 2023-07-07 23:05:50.000000 configparserc-1.4.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      187 2023-07-07 23:05:50.000000 configparserc-1.4.2/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-07-07 23:05:50.000000 configparserc-1.4.2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-07-07 23:06:06.000000 configparserc-1.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3746 2023-07-07 23:05:50.000000 configparserc-1.4.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 23:06:06.000000 configparserc-1.4.2/configparserc/
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-07 23:05:50.000000 configparserc-1.4.2/configparserc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1437267 2023-07-07 23:06:06.000000 configparserc-1.4.2/configparserc/config.c
+-rw-rw-rw-   0 root         (0) root         (0)     3082 2023-07-07 23:05:50.000000 configparserc-1.4.2/configparserc/config.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 23:06:06.000000 configparserc-1.4.2/configparserc/include/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-07-07 23:05:50.000000 configparserc-1.4.2/configparserc/include/_config.h
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-07 23:05:50.000000 configparserc-1.4.2/configparserc/py.typed
+-rw-r--r--   0 root         (0) root         (0)   341814 2023-07-07 23:06:05.000000 configparserc-1.4.2/configparserc/tools.c
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-07 23:05:50.000000 configparserc-1.4.2/configparserc/tools.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 23:06:06.000000 configparserc-1.4.2/configparserc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-07-07 23:06:06.000000 configparserc-1.4.2/configparserc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-07 23:06:06.000000 configparserc-1.4.2/configparserc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 23:06:06.000000 configparserc-1.4.2/configparserc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 23:06:06.000000 configparserc-1.4.2/configparserc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 23:06:06.000000 configparserc-1.4.2/configparserc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-07 23:06:06.000000 configparserc-1.4.2/configparserc.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-07 23:06:06.000000 configparserc-1.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    14643 2023-07-07 23:05:50.000000 configparserc-1.4.2/setup.py
```

### Comparing `configparserc-1.4.1/LICENSE` & `configparserc-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.1/NOTICE` & `configparserc-1.4.2/NOTICE`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.1/PKG-INFO` & `configparserc-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configparserc
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python (Cython) based implementation of ConfigParser based on POSIX and stdlib functions.
 Home-page: https://gitlab.com/onegreyonewhite/configparserc
 Author: Sergey Klyuykov
 Author-email: onegreyonewhite@mail.ru
 License: Apache Software License
 Project-URL: Issue Tracker, https://gitlab.com/onegreyonewhite/configparserc/-/issues
 Project-URL: Source Code, https://gitlab.com/onegreyonewhite/configparserc.git
```

### Comparing `configparserc-1.4.1/README.rst` & `configparserc-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.1/configparserc/__init__.py` & `configparserc-1.4.2/configparserc/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 """
 
-__version__ = '1.4.1'
+__version__ = '1.4.2'
```

### Comparing `configparserc-1.4.1/configparserc/config.c` & `configparserc-1.4.2/configparserc/config.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "configparserc/include/_config.h"
         ],
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -109,15 +109,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -393,17 +393,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -473,14 +470,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -2190,30 +2192,30 @@
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetNameInClass.proto */
 #define __Pyx_GetNameInClass(var, nmspace, name)  (var) = __Pyx__GetNameInClass(nmspace, name)
 static PyObject *__Pyx__GetNameInClass(PyObject *nmspace, PyObject *name);
 
 /* CLineInTraceback.proto */
@@ -26327,15 +26329,15 @@
   }
   if (unlikely(!o)) return 0;
   return o;
 }
 
 static void __pyx_tp_dealloc_13configparserc_6config_Empty(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_13configparserc_6config_Empty[] = {
@@ -26420,15 +26422,15 @@
   PyObject *o = (&((PyTypeObject*)PyExc_Exception)[0])->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
 
 static void __pyx_tp_dealloc_13configparserc_6config_ConfigParserException(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   PyObject_GC_Track(o);
   (&((PyTypeObject*)PyExc_Exception)[0])->tp_dealloc(o);
 }
@@ -26615,15 +26617,15 @@
   }
   if (unlikely(!o)) return 0;
   return o;
 }
 
 static void __pyx_tp_dealloc_13configparserc_6config_BaseType(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_13configparserc_6config_BaseType[] = {
@@ -27252,15 +27254,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_13configparserc_6config_ListType(PyObject *o) {
   struct __pyx_obj_13configparserc_6config_ListType *p = (struct __pyx_obj_13configparserc_6config_ListType *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   Py_CLEAR(p->separator);
   __pyx_tp_dealloc_13configparserc_6config_BaseType(o);
 }
 
@@ -27442,15 +27444,15 @@
   PyObject *o = (&PyDict_Type)->tp_new(t, a, k);
   if (unlikely(!o)) return 0;
   return o;
 }
 
 static void __pyx_tp_dealloc_13configparserc_6config___BaseDict(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   PyObject_GC_Track(o);
   (&PyDict_Type)->tp_dealloc(o);
 }
@@ -27572,15 +27574,15 @@
   p->__pyx___format_exclude_sections = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_13configparserc_6config_ConfigParserC(PyObject *o) {
   struct __pyx_obj_13configparserc_6config_ConfigParserC *p = (struct __pyx_obj_13configparserc_6config_ConfigParserC *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx___sections_map);
   Py_CLEAR(p->section_defaults);
   Py_CLEAR(p->__pyx___format_kwargs);
@@ -27766,15 +27768,15 @@
   p->__pyx___type_map = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_13configparserc_6config_Section(PyObject *o) {
   struct __pyx_obj_13configparserc_6config_Section *p = (struct __pyx_obj_13configparserc_6config_Section *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   Py_CLEAR(p->config);
   Py_CLEAR(p->__pyx___type_map);
@@ -29080,21 +29082,21 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -32994,18 +32996,18 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -33051,22 +33053,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `configparserc-1.4.1/configparserc/config.pyi` & `configparserc-1.4.2/configparserc/config.pyi`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.1/configparserc/include/_config.h` & `configparserc-1.4.2/configparserc/include/_config.h`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.1/configparserc/tools.c` & `configparserc-1.4.2/configparserc/tools.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-g0",
@@ -31,16 +31,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -107,15 +107,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -391,17 +391,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -471,14 +468,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -4483,15 +4485,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_13configparserc_5tools_File(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
```

### Comparing `configparserc-1.4.1/configparserc/tools.pyi` & `configparserc-1.4.2/configparserc/tools.pyi`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.1/configparserc.egg-info/PKG-INFO` & `configparserc-1.4.2/configparserc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configparserc
-Version: 1.4.1
+Version: 1.4.2
 Summary: Python (Cython) based implementation of ConfigParser based on POSIX and stdlib functions.
 Home-page: https://gitlab.com/onegreyonewhite/configparserc
 Author: Sergey Klyuykov
 Author-email: onegreyonewhite@mail.ru
 License: Apache Software License
 Project-URL: Issue Tracker, https://gitlab.com/onegreyonewhite/configparserc/-/issues
 Project-URL: Source Code, https://gitlab.com/onegreyonewhite/configparserc.git
```

### Comparing `configparserc-1.4.1/setup.cfg` & `configparserc-1.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `configparserc-1.4.1/setup.py` & `configparserc-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
 
 kwargs = dict(
     name='configparserc',
     packages=find_packages(exclude=['tests']+ext_list),
     ext_modules_list=ext_list,
     install_requires=[
         'pytimeparse2~=1.7.1',
-        'pyyaml>=3.13,<6'
+        'pyyaml>=3.13,<6.1'
     ],
     project_urls={
         "Issue Tracker": "https://gitlab.com/onegreyonewhite/configparserc/-/issues",
         "Source Code": "https://gitlab.com/onegreyonewhite/configparserc.git",
         "Releases": "https://pypi.org/project/configparserc/#history",
     },
 )
```

