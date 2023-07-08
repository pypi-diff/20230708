# Comparing `tmp/pmdsky_debug_py-6.0.0-py3-none-any.whl.zip` & `tmp/pmdsky_debug_py-7.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 846702 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1831 b- defN 23-Jun-27 04:28 pmdsky_debug_py/__init__.py
--rw-r--r--  2.0 unx       30 b- defN 23-Jun-27 04:28 pmdsky_debug_py/_release.py
--rw-r--r--  2.0 unx   778781 b- defN 23-Jun-27 04:28 pmdsky_debug_py/eu.py
--rw-r--r--  2.0 unx   745826 b- defN 23-Jun-27 04:28 pmdsky_debug_py/eu_itcm.py
--rw-r--r--  2.0 unx   766901 b- defN 23-Jun-27 04:28 pmdsky_debug_py/jp.py
--rw-r--r--  2.0 unx   745826 b- defN 23-Jun-27 04:28 pmdsky_debug_py/jp_itcm.py
--rw-r--r--  2.0 unx   786248 b- defN 23-Jun-27 04:28 pmdsky_debug_py/na.py
--rw-r--r--  2.0 unx   745837 b- defN 23-Jun-27 04:28 pmdsky_debug_py/na_itcm.py
--rw-r--r--  2.0 unx   243251 b- defN 23-Jun-27 04:28 pmdsky_debug_py/protocol.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 04:28 pmdsky_debug_py/py.typed
--rw-r--r--  2.0 unx     1320 b- defN 23-Jun-27 04:29 pmdsky_debug_py-6.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 04:29 pmdsky_debug_py-6.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-27 04:29 pmdsky_debug_py-6.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1155 b- defN 23-Jun-27 04:29 pmdsky_debug_py-6.0.0.dist-info/RECORD
-14 files, 4817114 bytes uncompressed, 844804 bytes compressed:  82.5%
+Zip file size: 846636 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1831 b- defN 23-Jul-08 04:27 pmdsky_debug_py/__init__.py
+-rw-r--r--  2.0 unx       30 b- defN 23-Jul-08 04:27 pmdsky_debug_py/_release.py
+-rw-r--r--  2.0 unx   778876 b- defN 23-Jul-08 04:27 pmdsky_debug_py/eu.py
+-rw-r--r--  2.0 unx   745946 b- defN 23-Jul-08 04:27 pmdsky_debug_py/eu_itcm.py
+-rw-r--r--  2.0 unx   766996 b- defN 23-Jul-08 04:27 pmdsky_debug_py/jp.py
+-rw-r--r--  2.0 unx   745946 b- defN 23-Jul-08 04:27 pmdsky_debug_py/jp_itcm.py
+-rw-r--r--  2.0 unx   786343 b- defN 23-Jul-08 04:27 pmdsky_debug_py/na.py
+-rw-r--r--  2.0 unx   745957 b- defN 23-Jul-08 04:27 pmdsky_debug_py/na_itcm.py
+-rw-r--r--  2.0 unx   243248 b- defN 23-Jul-08 04:27 pmdsky_debug_py/protocol.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-08 04:27 pmdsky_debug_py/py.typed
+-rw-r--r--  2.0 unx     1320 b- defN 23-Jul-08 04:28 pmdsky_debug_py-7.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-08 04:28 pmdsky_debug_py-7.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-08 04:28 pmdsky_debug_py-7.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1155 b- defN 23-Jul-08 04:28 pmdsky_debug_py-7.0.0.dist-info/RECORD
+14 files, 4817756 bytes uncompressed, 844738 bytes compressed:  82.5%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pmdsky_debug_py/protocol.py
 Comment: 
 
 Filename: pmdsky_debug_py/py.typed
 Comment: 
 
-Filename: pmdsky_debug_py-6.0.0.dist-info/METADATA
+Filename: pmdsky_debug_py-7.0.0.dist-info/METADATA
 Comment: 
 
-Filename: pmdsky_debug_py-6.0.0.dist-info/WHEEL
+Filename: pmdsky_debug_py-7.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: pmdsky_debug_py-6.0.0.dist-info/top_level.txt
+Filename: pmdsky_debug_py-7.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pmdsky_debug_py-6.0.0.dist-info/RECORD
+Filename: pmdsky_debug_py-7.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pmdsky_debug_py/_release.py

```diff
@@ -1 +1 @@
-RELEASE = "v0.6.0+aa2e93eb51"
+RELEASE = "v0.7.0+2a97086e57"
```

## pmdsky_debug_py/eu.py

```diff
@@ -563,15 +563,15 @@
 
     MemsetSimple = Symbol(
         [0x32A4],
         [0x20032A4],
         None,
         (
             "A simple implementation of the memset(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memset"
+            " function was probably manually implemented by the developers. See memset"
             " for what's probably the real libc function.\n\nr0: ptr\nr1: value\nr2:"
             " len (# bytes)"
         ),
     )
 
     Memset32 = Symbol(
         [0x32BC],
@@ -585,15 +585,15 @@
 
     MemcpySimple = Symbol(
         [0x32D4],
         [0x20032D4],
         None,
         (
             "A simple implementation of the memcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memcpy"
+            " function was probably manually implemented by the developers. See memcpy"
             " for what's probably the real libc function.\n\nThis function copies from"
             " src to dst in backwards byte order, so this is safe to call for"
             " overlapping src and dst if src <= dst.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     Memcpy16 = Symbol(
@@ -963,15 +963,15 @@
 
     DebugPrint0 = Symbol(
         [0xC250, 0xC284],
         [0x200C250, 0x200C284],
         None,
         (
             "Would log a printf format string in the debug binary.\n\nThis still"
-            " constructs the string with Vsprintf, but doesn't actually do anything"
+            " constructs the string with vsprintf, but doesn't actually do anything"
             " with it in the final binary.\n\nr0: format\n...: variadic"
         ),
     )
 
     GetDebugFlag2 = Symbol(
         [0xC2BC],
         [0x200C2BC],
@@ -1299,19 +1299,19 @@
             0x2042DA0,
             0x2052750,
             0x2054DDC,
             0x2060D64,
         ],
         None,
         (
-            "Functionally the same as Sprintf, just defined statically in many"
+            "Functionally the same as sprintf, just defined statically in many"
             " different places.\n\nSince this is essentially just a wrapper around"
             " vsprintf(3), this function was probably statically defined in a header"
             " somewhere and included in a bunch of different places. See the actual"
-            " Sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
+            " sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
             " variadic\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
     ItemZInit = Symbol(
         [0xD8A4], [0x200D8A4], None, "Zero-initializes an item struct.\n\nr0: item"
@@ -3110,26 +3110,26 @@
 
     StrcpySimple = Symbol(
         [0x253CC],
         [0x20253CC],
         None,
         (
             "A simple implementation of the strcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strcpy"
+            " function was probably manually implemented by the developers. See strcpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src"
         ),
     )
 
     StrncpySimple = Symbol(
         [0x253E8],
         [0x20253E8],
         None,
         (
             "A simple implementation of the strncpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncpy"
+            " function was probably manually implemented by the developers. See strncpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     StrncpySimpleNoPad = Symbol(
         [0x2543C],
         [0x202543C],
@@ -3142,15 +3142,15 @@
 
     StrncmpSimple = Symbol(
         [0x25478],
         [0x2025478],
         None,
         (
             "A simple implementation of the strncmp(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncmp"
+            " function was probably manually implemented by the developers. See strncmp"
             " for what's probably the real libc function.\n\nr0: s1\nr1: s2\nr2:"
             " n\nreturn: comparison value"
         ),
     )
 
     StrncpySimpleNoPadSafe = Symbol(
         [0x254C0],
@@ -6585,22 +6585,22 @@
         None,
         (
             "Initializes a file_stream structure for file I/O.\n\nThis function must"
             " always be called before opening a file.\n\nr0: file_stream pointer"
         ),
     )
 
-    Abs = Symbol(
+    abs = Symbol(
         [0x868F4],
         [0x20868F4],
         None,
         "Takes the absolute value of an integer.\n\nr0: x\nreturn: abs(x)",
     )
 
-    Mbtowc = Symbol(
+    mbtowc = Symbol(
         [0x87554],
         [0x2087554],
         None,
         (
             "The mbtowc(3) C library function.\n\nr0: pwc\nr1: s\nr2: n\nreturn: number"
             " of consumed bytes, or -1 on failure"
         ),
@@ -6624,99 +6624,99 @@
         (
             "Wrapper around TryAssignByte.\n\nAccesses the TryAssignByte function with"
             " a weird chain of pointer dereferences.\n\nr0: pointer\nr1: value\nreturn:"
             " true on success, false on failure"
         ),
     )
 
-    Wcstombs = Symbol(
+    wcstombs = Symbol(
         [0x875BC],
         [0x20875BC],
         None,
         (
             "The wcstombs(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn:"
             " characters converted"
         ),
     )
 
-    Memcpy = Symbol(
+    memcpy = Symbol(
         [0x87634],
         [0x2087634],
         None,
-        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Memmove = Symbol(
+    memmove = Symbol(
         [0x87654],
         [0x2087654],
         None,
         (
             "The memmove(3) C library function.\n\nThe implementation is nearly the"
-            " same as Memcpy, but it copies bytes from back to front if src <"
-            " dst.\n\nr0: dest\nr1: src\nr2: n"
+            " same as memcpy, but it copies bytes from back to front if src <"
+            " dst.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest"
         ),
     )
 
-    Memset = Symbol(
+    memset = Symbol(
         [0x876A0],
         [0x20876A0],
         None,
         (
             "The memset(3) C library function.\n\nThis is just a wrapper around"
-            " MemsetInternal that returns the pointer at the end.\n\nr0: s\nr1: c (int,"
-            " but must be a single-byte value)\nr2: n\nreturn: s"
+            " memset_internal that returns the pointer at the end.\n\nr0: s\nr1: c"
+            " (int, but must be a single-byte value)\nr2: n\nreturn: s"
         ),
     )
 
-    Memchr = Symbol(
+    memchr = Symbol(
         [0x876B4],
         [0x20876B4],
         None,
         (
             "The memchr(3) C library function.\n\nr0: s\nr1: c\nr2: n\nreturn: pointer"
             " to first occurrence of c in s, or a null pointer if no match"
         ),
     )
 
-    Memcmp = Symbol(
+    memcmp = Symbol(
         [0x876E0],
         [0x20876E0],
         None,
         (
             "The memcmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    MemsetInternal = Symbol(
+    memset_internal = Symbol(
         [0x87720],
         [0x2087720],
         None,
         (
             "The actual memory-setting implementation for the memset(3) C library"
             " function.\n\nThis function is optimized to set bytes in 4-byte chunks for"
             " n >= 32, correctly handling any unaligned bytes at the front/back. In"
             " this case, it also further optimizes by unrolling a for loop to set 8"
             " 4-byte values at once (effectively a 32-byte chunk).\n\nr0: s\nr1: c"
             " (int, but must be a single-byte value)\nr2: n"
         ),
     )
 
-    VsprintfInternalSlice = Symbol(
+    __vsprintf_internal_slice = Symbol(
         [0x8900C],
         [0x208900C],
         None,
         (
-            "This is what implements the bulk of VsprintfInternal.\n\nThe"
+            "This is what implements the bulk of __vsprintf_internal.\n\nThe"
             " __vsprintf_internal in the modern-day version of glibc relies on"
             " __vfprintf_internal; this function has a slightly different interface,"
             " but it serves a similar role.\n\nr0: function pointer to append to the"
-            " string being built (VsprintfInternal uses TryAppendToSlice)\nr1: string"
-            " buffer slice\nr2: format\nr3: ap\nreturn: number of characters printed,"
-            " excluding the null-terminator"
+            " string being built (__vsprintf_internal uses TryAppendToSlice)\nr1:"
+            " string buffer slice\nr2: format\nr3: ap\nreturn: number of characters"
+            " printed, excluding the null-terminator"
         ),
     )
 
     TryAppendToSlice = Symbol(
         [0x89830],
         [0x2089830],
         None,
@@ -6724,258 +6724,258 @@
             "Best-effort append the given data to a slice. If the slice's capacity is"
             " reached, any remaining data will be truncated.\n\nr0: slice pointer\nr1:"
             " buffer of data to append\nr2: number of bytes in the data buffer\nreturn:"
             " true"
         ),
     )
 
-    VsprintfInternal = Symbol(
+    __vsprintf_internal = Symbol(
         [0x89874],
         [0x2089874],
         None,
         (
-            "This is what implements Vsprintf. It's akin to __vsprintf_internal in the"
+            "This is what implements vsprintf. It's akin to __vsprintf_internal in the"
             " modern-day version of glibc (in fact, it's probably an older version of"
-            " this).\n\nr0: str\nr1: maxlen (Vsprintf passes UINT32_MAX for this)\nr2:"
+            " this).\n\nr0: str\nr1: maxlen (vsprintf passes UINT32_MAX for this)\nr2:"
             " format\nr3: ap\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
-    Vsprintf = Symbol(
+    vsprintf = Symbol(
         [0x898DC],
         [0x20898DC],
         None,
         (
             "The vsprintf(3) C library function.\n\nr0: str\nr1: format\nr2:"
             " ap\nreturn: number of characters printed, excluding the null-terminator"
         ),
     )
 
-    Snprintf = Symbol(
+    snprintf = Symbol(
         [0x898F4],
         [0x20898F4],
         None,
         (
-            "The snprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The snprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real snprintf.\n\nr0: str\nr1: n\nr2:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Sprintf = Symbol(
+    sprintf = Symbol(
         [0x8991C],
         [0x208991C],
         None,
         (
-            "The sprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The sprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real sprintf.\n\nr0: str\nr1:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Strlen = Symbol(
+    strlen = Symbol(
         [0x89A10],
         [0x2089A10],
         None,
         "The strlen(3) C library function.\n\nr0: s\nreturn: length of s",
     )
 
-    Strcpy = Symbol(
+    strcpy = Symbol(
         [0x89A2C],
         [0x2089A2C],
         None,
         (
             "The strcpy(3) C library function.\n\nThis function is optimized to copy"
             " characters in aligned 4-byte chunks if possible, correctly handling any"
-            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src"
+            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src\nreturn: dest"
         ),
     )
 
-    Strncpy = Symbol(
+    strncpy = Symbol(
         [0x89AF4],
         [0x2089AF4],
         None,
-        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcat = Symbol(
+    strcat = Symbol(
         [0x89B44],
         [0x2089B44],
         None,
-        "The strcat(3) C library function.\n\nr0: dest\nr1: src",
+        "The strcat(3) C library function.\n\nr0: dest\nr1: src\nreturn: dest",
     )
 
-    Strncat = Symbol(
+    strncat = Symbol(
         [0x89B74],
         [0x2089B74],
         None,
-        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcmp = Symbol(
+    strcmp = Symbol(
         [0x89BC4],
         [0x2089BC4],
         None,
         (
-            "The strcmp(3) C library function.\n\nSimilarly to Strcpy, this function is"
+            "The strcmp(3) C library function.\n\nSimilarly to strcpy, this function is"
             " optimized to compare characters in aligned 4-byte chunks if"
             " possible.\n\nr0: s1\nr1: s2\nreturn: comparison value"
         ),
     )
 
-    Strncmp = Symbol(
+    strncmp = Symbol(
         [0x89CD8],
         [0x2089CD8],
         None,
         (
             "The strncmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    Strchr = Symbol(
+    strchr = Symbol(
         [0x89D0C],
         [0x2089D0C],
         None,
         (
             "The strchr(3) C library function.\n\nr0: string\nr1: c\nreturn: pointer to"
             " the located byte c, or null pointer if no match"
         ),
     )
 
-    Strcspn = Symbol(
+    strcspn = Symbol(
         [0x89D48],
         [0x2089D48],
         None,
         (
             "The strcspn(3) C library function.\n\nr0: string\nr1: stopset\nreturn:"
             " offset of the first character in string within stopset"
         ),
     )
 
-    Strstr = Symbol(
+    strstr = Symbol(
         [0x89E08],
         [0x2089E08],
         None,
         (
             "The strstr(3) C library function.\n\nr0: haystack\nr1: needle\nreturn:"
             " pointer into haystack where needle starts, or null pointer if no match"
         ),
     )
 
-    Wcslen = Symbol(
+    wcslen = Symbol(
         [0x8B780],
         [0x208B780],
         None,
         "The wcslen(3) C library function.\n\nr0: ws\nreturn: length of ws",
     )
 
-    AddFloat = Symbol(
+    __addsf3 = Symbol(
         [0x8F050],
         [0x208F050],
         None,
         (
             "This appears to be the libgcc implementation of __addsf3 (not sure which"
             " gcc version), which implements the addition operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a + b"
         ),
     )
 
-    DivideFloat = Symbol(
+    __divsf3 = Symbol(
         [0x8F5CC],
         [0x208F5CC],
         None,
         (
             "This appears to be the libgcc implementation of __divsf3 (not sure which"
             " gcc version), which implements the division operator for IEEE 754"
             " floating-point numbers.\n\nr0: dividend\nr1: divisor\nreturn: dividend /"
             " divisor"
         ),
     )
 
-    FloatToDouble = Symbol(
+    __extendsfdf2 = Symbol(
         [0x8F984],
         [0x208F984],
         None,
         (
             "This appears to be the libgcc implementation of __extendsfdf2 (not sure"
             " which gcc version), which implements the float to double cast operation"
             " for IEEE 754 floating-point numbers.\n\nr0: float\nreturn: (double)float"
         ),
     )
 
-    FloatToInt = Symbol(
+    __fixsfsi = Symbol(
         [0x8FA08],
         [0x208FA08],
         None,
         (
             "This appears to be the libgcc implementation of __fixsfsi (not sure which"
             " gcc version), which implements the float to int cast operation for IEEE"
             " 754 floating-point numbers. The output saturates if the input is out of"
             " the representable range for the int type.\n\nr0: float\nreturn:"
             " (int)float"
         ),
     )
 
-    IntToFloat = Symbol(
+    __floatsisf = Symbol(
         [0x8FA3C],
         [0x208FA3C],
         None,
         (
             "This appears to be the libgcc implementation of __floatsisf (not sure"
             " which gcc version), which implements the int to float cast operation for"
             " IEEE 754 floating-point numbers.\n\nr0: int\nreturn: (float)int"
         ),
     )
 
-    UIntToFloat = Symbol(
+    __floatunsisf = Symbol(
         [0x8FA84],
         [0x208FA84],
         None,
         (
             "This appears to be the libgcc implementation of __floatunsisf (not sure"
             " which gcc version), which implements the unsigned int to float cast"
             " operation for IEEE 754 floating-point numbers.\n\nr0: uint\nreturn:"
             " (float)uint"
         ),
     )
 
-    MultiplyFloat = Symbol(
+    __mulsf3 = Symbol(
         [0x8FACC],
         [0x208FACC],
         None,
         (
             "This appears to be the libgcc implementation of __mulsf3 (not sure which"
             " gcc version), which implements the multiplication operator for IEEE 754"
             " floating-point numbers."
         ),
     )
 
-    Sqrtf = Symbol(
+    sqrtf = Symbol(
         [0x8FCAC],
         [0x208FCAC],
         None,
         "The sqrtf(3) C library function.\n\nr0: x\nreturn: sqrt(x)",
     )
 
-    SubtractFloat = Symbol(
+    __subsf3 = Symbol(
         [0x8FD9C],
         [0x208FD9C],
         None,
         (
             "This appears to be the libgcc implementation of __subsf3 (not sure which"
             " gcc version), which implements the subtraction operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a - b"
         ),
     )
 
-    DivideInt = Symbol(
+    __divsi3 = Symbol(
         [0x9023C],
         [0x209023C],
         None,
         (
             "This appears to be the libgcc implementation of __divsi3 (not sure which"
             " gcc version), which implements the division operator for signed"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
@@ -6985,39 +6985,39 @@
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
             " (remainder << 32)"
         ),
     )
 
-    DivideUInt = Symbol(
+    __udivsi3 = Symbol(
         [0x90448],
         [0x2090448],
         None,
         (
             "This appears to be the libgcc implementation of __udivsi3 (not sure which"
             " gcc version), which implements the division operator for unsigned"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
             " (dividend / divisor) in the lower 32 bits and the remainder (dividend %"
             " divisor) in the upper 32 bits. In accordance with the Procedure Call"
             " Standard for the Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nNote: This function falls through to"
-            " DivideUIntNoZeroCheck.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
-            " (remainder << 32)"
+            " __udivsi3_no_zero_check.\n\nr0: dividend\nr1: divisor\nreturn: (quotient)"
+            " | (remainder << 32)"
         ),
     )
 
-    DivideUIntNoZeroCheck = Symbol(
+    __udivsi3_no_zero_check = Symbol(
         [0x90450],
         [0x2090450],
         None,
         (
-            "Subsidiary function to DivideUInt. Skips the initial check for divisor =="
+            "Subsidiary function to __udivsi3. Skips the initial check for divisor =="
             " 0.\n\nThe return value is a 64-bit integer, with the quotient (dividend /"
             " divisor) in the lower 32 bits and the remainder (dividend % divisor) in"
             " the upper 32 bits. In accordance with the Procedure Call Standard for the"
             " Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nThis function appears to only be called"
```

## pmdsky_debug_py/eu_itcm.py

```diff
@@ -556,15 +556,15 @@
 
     MemsetSimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the memset(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memset"
+            " function was probably manually implemented by the developers. See memset"
             " for what's probably the real libc function.\n\nr0: ptr\nr1: value\nr2:"
             " len (# bytes)"
         ),
     )
 
     Memset32 = Symbol(
         None,
@@ -578,15 +578,15 @@
 
     MemcpySimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the memcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memcpy"
+            " function was probably manually implemented by the developers. See memcpy"
             " for what's probably the real libc function.\n\nThis function copies from"
             " src to dst in backwards byte order, so this is safe to call for"
             " overlapping src and dst if src <= dst.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     Memcpy16 = Symbol(
@@ -953,15 +953,15 @@
 
     DebugPrint0 = Symbol(
         None,
         None,
         None,
         (
             "Would log a printf format string in the debug binary.\n\nThis still"
-            " constructs the string with Vsprintf, but doesn't actually do anything"
+            " constructs the string with vsprintf, but doesn't actually do anything"
             " with it in the final binary.\n\nr0: format\n...: variadic"
         ),
     )
 
     GetDebugFlag2 = Symbol(
         None,
         None,
@@ -1249,19 +1249,19 @@
     )
 
     SprintfStatic = Symbol(
         None,
         None,
         None,
         (
-            "Functionally the same as Sprintf, just defined statically in many"
+            "Functionally the same as sprintf, just defined statically in many"
             " different places.\n\nSince this is essentially just a wrapper around"
             " vsprintf(3), this function was probably statically defined in a header"
             " somewhere and included in a bunch of different places. See the actual"
-            " Sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
+            " sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
             " variadic\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
     ItemZInit = Symbol(None, None, None, "Zero-initializes an item struct.\n\nr0: item")
 
@@ -3020,26 +3020,26 @@
 
     StrcpySimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the strcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strcpy"
+            " function was probably manually implemented by the developers. See strcpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src"
         ),
     )
 
     StrncpySimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the strncpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncpy"
+            " function was probably manually implemented by the developers. See strncpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     StrncpySimpleNoPad = Symbol(
         None,
         None,
@@ -3052,15 +3052,15 @@
 
     StrncmpSimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the strncmp(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncmp"
+            " function was probably manually implemented by the developers. See strncmp"
             " for what's probably the real libc function.\n\nr0: s1\nr1: s2\nr2:"
             " n\nreturn: comparison value"
         ),
     )
 
     StrncpySimpleNoPadSafe = Symbol(
         None,
@@ -6387,22 +6387,22 @@
         None,
         (
             "Initializes a file_stream structure for file I/O.\n\nThis function must"
             " always be called before opening a file.\n\nr0: file_stream pointer"
         ),
     )
 
-    Abs = Symbol(
+    abs = Symbol(
         None,
         None,
         None,
         "Takes the absolute value of an integer.\n\nr0: x\nreturn: abs(x)",
     )
 
-    Mbtowc = Symbol(
+    mbtowc = Symbol(
         None,
         None,
         None,
         (
             "The mbtowc(3) C library function.\n\nr0: pwc\nr1: s\nr2: n\nreturn: number"
             " of consumed bytes, or -1 on failure"
         ),
@@ -6426,99 +6426,99 @@
         (
             "Wrapper around TryAssignByte.\n\nAccesses the TryAssignByte function with"
             " a weird chain of pointer dereferences.\n\nr0: pointer\nr1: value\nreturn:"
             " true on success, false on failure"
         ),
     )
 
-    Wcstombs = Symbol(
+    wcstombs = Symbol(
         None,
         None,
         None,
         (
             "The wcstombs(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn:"
             " characters converted"
         ),
     )
 
-    Memcpy = Symbol(
+    memcpy = Symbol(
         None,
         None,
         None,
-        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Memmove = Symbol(
+    memmove = Symbol(
         None,
         None,
         None,
         (
             "The memmove(3) C library function.\n\nThe implementation is nearly the"
-            " same as Memcpy, but it copies bytes from back to front if src <"
-            " dst.\n\nr0: dest\nr1: src\nr2: n"
+            " same as memcpy, but it copies bytes from back to front if src <"
+            " dst.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest"
         ),
     )
 
-    Memset = Symbol(
+    memset = Symbol(
         None,
         None,
         None,
         (
             "The memset(3) C library function.\n\nThis is just a wrapper around"
-            " MemsetInternal that returns the pointer at the end.\n\nr0: s\nr1: c (int,"
-            " but must be a single-byte value)\nr2: n\nreturn: s"
+            " memset_internal that returns the pointer at the end.\n\nr0: s\nr1: c"
+            " (int, but must be a single-byte value)\nr2: n\nreturn: s"
         ),
     )
 
-    Memchr = Symbol(
+    memchr = Symbol(
         None,
         None,
         None,
         (
             "The memchr(3) C library function.\n\nr0: s\nr1: c\nr2: n\nreturn: pointer"
             " to first occurrence of c in s, or a null pointer if no match"
         ),
     )
 
-    Memcmp = Symbol(
+    memcmp = Symbol(
         None,
         None,
         None,
         (
             "The memcmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    MemsetInternal = Symbol(
+    memset_internal = Symbol(
         None,
         None,
         None,
         (
             "The actual memory-setting implementation for the memset(3) C library"
             " function.\n\nThis function is optimized to set bytes in 4-byte chunks for"
             " n >= 32, correctly handling any unaligned bytes at the front/back. In"
             " this case, it also further optimizes by unrolling a for loop to set 8"
             " 4-byte values at once (effectively a 32-byte chunk).\n\nr0: s\nr1: c"
             " (int, but must be a single-byte value)\nr2: n"
         ),
     )
 
-    VsprintfInternalSlice = Symbol(
+    __vsprintf_internal_slice = Symbol(
         None,
         None,
         None,
         (
-            "This is what implements the bulk of VsprintfInternal.\n\nThe"
+            "This is what implements the bulk of __vsprintf_internal.\n\nThe"
             " __vsprintf_internal in the modern-day version of glibc relies on"
             " __vfprintf_internal; this function has a slightly different interface,"
             " but it serves a similar role.\n\nr0: function pointer to append to the"
-            " string being built (VsprintfInternal uses TryAppendToSlice)\nr1: string"
-            " buffer slice\nr2: format\nr3: ap\nreturn: number of characters printed,"
-            " excluding the null-terminator"
+            " string being built (__vsprintf_internal uses TryAppendToSlice)\nr1:"
+            " string buffer slice\nr2: format\nr3: ap\nreturn: number of characters"
+            " printed, excluding the null-terminator"
         ),
     )
 
     TryAppendToSlice = Symbol(
         None,
         None,
         None,
@@ -6526,252 +6526,255 @@
             "Best-effort append the given data to a slice. If the slice's capacity is"
             " reached, any remaining data will be truncated.\n\nr0: slice pointer\nr1:"
             " buffer of data to append\nr2: number of bytes in the data buffer\nreturn:"
             " true"
         ),
     )
 
-    VsprintfInternal = Symbol(
+    __vsprintf_internal = Symbol(
         None,
         None,
         None,
         (
-            "This is what implements Vsprintf. It's akin to __vsprintf_internal in the"
+            "This is what implements vsprintf. It's akin to __vsprintf_internal in the"
             " modern-day version of glibc (in fact, it's probably an older version of"
-            " this).\n\nr0: str\nr1: maxlen (Vsprintf passes UINT32_MAX for this)\nr2:"
+            " this).\n\nr0: str\nr1: maxlen (vsprintf passes UINT32_MAX for this)\nr2:"
             " format\nr3: ap\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
-    Vsprintf = Symbol(
+    vsprintf = Symbol(
         None,
         None,
         None,
         (
             "The vsprintf(3) C library function.\n\nr0: str\nr1: format\nr2:"
             " ap\nreturn: number of characters printed, excluding the null-terminator"
         ),
     )
 
-    Snprintf = Symbol(
+    snprintf = Symbol(
         None,
         None,
         None,
         (
-            "The snprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The snprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real snprintf.\n\nr0: str\nr1: n\nr2:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Sprintf = Symbol(
+    sprintf = Symbol(
         None,
         None,
         None,
         (
-            "The sprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The sprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real sprintf.\n\nr0: str\nr1:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Strlen = Symbol(
+    strlen = Symbol(
         None,
         None,
         None,
         "The strlen(3) C library function.\n\nr0: s\nreturn: length of s",
     )
 
-    Strcpy = Symbol(
+    strcpy = Symbol(
         None,
         None,
         None,
         (
             "The strcpy(3) C library function.\n\nThis function is optimized to copy"
             " characters in aligned 4-byte chunks if possible, correctly handling any"
-            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src"
+            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src\nreturn: dest"
         ),
     )
 
-    Strncpy = Symbol(
+    strncpy = Symbol(
         None,
         None,
         None,
-        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcat = Symbol(
-        None, None, None, "The strcat(3) C library function.\n\nr0: dest\nr1: src"
+    strcat = Symbol(
+        None,
+        None,
+        None,
+        "The strcat(3) C library function.\n\nr0: dest\nr1: src\nreturn: dest",
     )
 
-    Strncat = Symbol(
+    strncat = Symbol(
         None,
         None,
         None,
-        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcmp = Symbol(
+    strcmp = Symbol(
         None,
         None,
         None,
         (
-            "The strcmp(3) C library function.\n\nSimilarly to Strcpy, this function is"
+            "The strcmp(3) C library function.\n\nSimilarly to strcpy, this function is"
             " optimized to compare characters in aligned 4-byte chunks if"
             " possible.\n\nr0: s1\nr1: s2\nreturn: comparison value"
         ),
     )
 
-    Strncmp = Symbol(
+    strncmp = Symbol(
         None,
         None,
         None,
         (
             "The strncmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    Strchr = Symbol(
+    strchr = Symbol(
         None,
         None,
         None,
         (
             "The strchr(3) C library function.\n\nr0: string\nr1: c\nreturn: pointer to"
             " the located byte c, or null pointer if no match"
         ),
     )
 
-    Strcspn = Symbol(
+    strcspn = Symbol(
         None,
         None,
         None,
         (
             "The strcspn(3) C library function.\n\nr0: string\nr1: stopset\nreturn:"
             " offset of the first character in string within stopset"
         ),
     )
 
-    Strstr = Symbol(
+    strstr = Symbol(
         None,
         None,
         None,
         (
             "The strstr(3) C library function.\n\nr0: haystack\nr1: needle\nreturn:"
             " pointer into haystack where needle starts, or null pointer if no match"
         ),
     )
 
-    Wcslen = Symbol(
+    wcslen = Symbol(
         None,
         None,
         None,
         "The wcslen(3) C library function.\n\nr0: ws\nreturn: length of ws",
     )
 
-    AddFloat = Symbol(
+    __addsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __addsf3 (not sure which"
             " gcc version), which implements the addition operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a + b"
         ),
     )
 
-    DivideFloat = Symbol(
+    __divsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __divsf3 (not sure which"
             " gcc version), which implements the division operator for IEEE 754"
             " floating-point numbers.\n\nr0: dividend\nr1: divisor\nreturn: dividend /"
             " divisor"
         ),
     )
 
-    FloatToDouble = Symbol(
+    __extendsfdf2 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __extendsfdf2 (not sure"
             " which gcc version), which implements the float to double cast operation"
             " for IEEE 754 floating-point numbers.\n\nr0: float\nreturn: (double)float"
         ),
     )
 
-    FloatToInt = Symbol(
+    __fixsfsi = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __fixsfsi (not sure which"
             " gcc version), which implements the float to int cast operation for IEEE"
             " 754 floating-point numbers. The output saturates if the input is out of"
             " the representable range for the int type.\n\nr0: float\nreturn:"
             " (int)float"
         ),
     )
 
-    IntToFloat = Symbol(
+    __floatsisf = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __floatsisf (not sure"
             " which gcc version), which implements the int to float cast operation for"
             " IEEE 754 floating-point numbers.\n\nr0: int\nreturn: (float)int"
         ),
     )
 
-    UIntToFloat = Symbol(
+    __floatunsisf = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __floatunsisf (not sure"
             " which gcc version), which implements the unsigned int to float cast"
             " operation for IEEE 754 floating-point numbers.\n\nr0: uint\nreturn:"
             " (float)uint"
         ),
     )
 
-    MultiplyFloat = Symbol(
+    __mulsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __mulsf3 (not sure which"
             " gcc version), which implements the multiplication operator for IEEE 754"
             " floating-point numbers."
         ),
     )
 
-    Sqrtf = Symbol(
+    sqrtf = Symbol(
         None, None, None, "The sqrtf(3) C library function.\n\nr0: x\nreturn: sqrt(x)"
     )
 
-    SubtractFloat = Symbol(
+    __subsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __subsf3 (not sure which"
             " gcc version), which implements the subtraction operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a - b"
         ),
     )
 
-    DivideInt = Symbol(
+    __divsi3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __divsi3 (not sure which"
             " gcc version), which implements the division operator for signed"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
@@ -6781,39 +6784,39 @@
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
             " (remainder << 32)"
         ),
     )
 
-    DivideUInt = Symbol(
+    __udivsi3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __udivsi3 (not sure which"
             " gcc version), which implements the division operator for unsigned"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
             " (dividend / divisor) in the lower 32 bits and the remainder (dividend %"
             " divisor) in the upper 32 bits. In accordance with the Procedure Call"
             " Standard for the Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nNote: This function falls through to"
-            " DivideUIntNoZeroCheck.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
-            " (remainder << 32)"
+            " __udivsi3_no_zero_check.\n\nr0: dividend\nr1: divisor\nreturn: (quotient)"
+            " | (remainder << 32)"
         ),
     )
 
-    DivideUIntNoZeroCheck = Symbol(
+    __udivsi3_no_zero_check = Symbol(
         None,
         None,
         None,
         (
-            "Subsidiary function to DivideUInt. Skips the initial check for divisor =="
+            "Subsidiary function to __udivsi3. Skips the initial check for divisor =="
             " 0.\n\nThe return value is a 64-bit integer, with the quotient (dividend /"
             " divisor) in the lower 32 bits and the remainder (dividend % divisor) in"
             " the upper 32 bits. In accordance with the Procedure Call Standard for the"
             " Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nThis function appears to only be called"
```

## pmdsky_debug_py/jp.py

```diff
@@ -563,15 +563,15 @@
 
     MemsetSimple = Symbol(
         [0x32A4],
         [0x20032A4],
         None,
         (
             "A simple implementation of the memset(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memset"
+            " function was probably manually implemented by the developers. See memset"
             " for what's probably the real libc function.\n\nr0: ptr\nr1: value\nr2:"
             " len (# bytes)"
         ),
     )
 
     Memset32 = Symbol(
         [0x32BC],
@@ -585,15 +585,15 @@
 
     MemcpySimple = Symbol(
         [0x32D4],
         [0x20032D4],
         None,
         (
             "A simple implementation of the memcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memcpy"
+            " function was probably manually implemented by the developers. See memcpy"
             " for what's probably the real libc function.\n\nThis function copies from"
             " src to dst in backwards byte order, so this is safe to call for"
             " overlapping src and dst if src <= dst.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     Memcpy16 = Symbol(
@@ -963,15 +963,15 @@
 
     DebugPrint0 = Symbol(
         [0xC1C8, 0xC1FC],
         [0x200C1C8, 0x200C1FC],
         None,
         (
             "Would log a printf format string in the debug binary.\n\nThis still"
-            " constructs the string with Vsprintf, but doesn't actually do anything"
+            " constructs the string with vsprintf, but doesn't actually do anything"
             " with it in the final binary.\n\nr0: format\n...: variadic"
         ),
     )
 
     GetDebugFlag2 = Symbol(
         [0xC234],
         [0x200C234],
@@ -1297,19 +1297,19 @@
             0x2041AB4,
             0x2042DF4,
             0x2052768,
             0x2054D98,
         ],
         None,
         (
-            "Functionally the same as Sprintf, just defined statically in many"
+            "Functionally the same as sprintf, just defined statically in many"
             " different places.\n\nSince this is essentially just a wrapper around"
             " vsprintf(3), this function was probably statically defined in a header"
             " somewhere and included in a bunch of different places. See the actual"
-            " Sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
+            " sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
             " variadic\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
     ItemZInit = Symbol(
         [0xD84C], [0x200D84C], None, "Zero-initializes an item struct.\n\nr0: item"
@@ -3108,26 +3108,26 @@
 
     StrcpySimple = Symbol(
         [0x25150],
         [0x2025150],
         None,
         (
             "A simple implementation of the strcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strcpy"
+            " function was probably manually implemented by the developers. See strcpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src"
         ),
     )
 
     StrncpySimple = Symbol(
         [0x2516C],
         [0x202516C],
         None,
         (
             "A simple implementation of the strncpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncpy"
+            " function was probably manually implemented by the developers. See strncpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     StrncpySimpleNoPad = Symbol(
         [0x251C0],
         [0x20251C0],
@@ -3140,15 +3140,15 @@
 
     StrncmpSimple = Symbol(
         [0x251FC],
         [0x20251FC],
         None,
         (
             "A simple implementation of the strncmp(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncmp"
+            " function was probably manually implemented by the developers. See strncmp"
             " for what's probably the real libc function.\n\nr0: s1\nr1: s2\nr2:"
             " n\nreturn: comparison value"
         ),
     )
 
     StrncpySimpleNoPadSafe = Symbol(
         [0x25268],
@@ -6583,22 +6583,22 @@
         None,
         (
             "Initializes a file_stream structure for file I/O.\n\nThis function must"
             " always be called before opening a file.\n\nr0: file_stream pointer"
         ),
     )
 
-    Abs = Symbol(
+    abs = Symbol(
         [0x86844],
         [0x2086844],
         None,
         "Takes the absolute value of an integer.\n\nr0: x\nreturn: abs(x)",
     )
 
-    Mbtowc = Symbol(
+    mbtowc = Symbol(
         [0x874A4],
         [0x20874A4],
         None,
         (
             "The mbtowc(3) C library function.\n\nr0: pwc\nr1: s\nr2: n\nreturn: number"
             " of consumed bytes, or -1 on failure"
         ),
@@ -6622,99 +6622,99 @@
         (
             "Wrapper around TryAssignByte.\n\nAccesses the TryAssignByte function with"
             " a weird chain of pointer dereferences.\n\nr0: pointer\nr1: value\nreturn:"
             " true on success, false on failure"
         ),
     )
 
-    Wcstombs = Symbol(
+    wcstombs = Symbol(
         [0x8750C],
         [0x208750C],
         None,
         (
             "The wcstombs(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn:"
             " characters converted"
         ),
     )
 
-    Memcpy = Symbol(
+    memcpy = Symbol(
         [0x87584],
         [0x2087584],
         None,
-        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Memmove = Symbol(
+    memmove = Symbol(
         [0x875A4],
         [0x20875A4],
         None,
         (
             "The memmove(3) C library function.\n\nThe implementation is nearly the"
-            " same as Memcpy, but it copies bytes from back to front if src <"
-            " dst.\n\nr0: dest\nr1: src\nr2: n"
+            " same as memcpy, but it copies bytes from back to front if src <"
+            " dst.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest"
         ),
     )
 
-    Memset = Symbol(
+    memset = Symbol(
         [0x875F0],
         [0x20875F0],
         None,
         (
             "The memset(3) C library function.\n\nThis is just a wrapper around"
-            " MemsetInternal that returns the pointer at the end.\n\nr0: s\nr1: c (int,"
-            " but must be a single-byte value)\nr2: n\nreturn: s"
+            " memset_internal that returns the pointer at the end.\n\nr0: s\nr1: c"
+            " (int, but must be a single-byte value)\nr2: n\nreturn: s"
         ),
     )
 
-    Memchr = Symbol(
+    memchr = Symbol(
         [0x87604],
         [0x2087604],
         None,
         (
             "The memchr(3) C library function.\n\nr0: s\nr1: c\nr2: n\nreturn: pointer"
             " to first occurrence of c in s, or a null pointer if no match"
         ),
     )
 
-    Memcmp = Symbol(
+    memcmp = Symbol(
         [0x87630],
         [0x2087630],
         None,
         (
             "The memcmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    MemsetInternal = Symbol(
+    memset_internal = Symbol(
         [0x87670],
         [0x2087670],
         None,
         (
             "The actual memory-setting implementation for the memset(3) C library"
             " function.\n\nThis function is optimized to set bytes in 4-byte chunks for"
             " n >= 32, correctly handling any unaligned bytes at the front/back. In"
             " this case, it also further optimizes by unrolling a for loop to set 8"
             " 4-byte values at once (effectively a 32-byte chunk).\n\nr0: s\nr1: c"
             " (int, but must be a single-byte value)\nr2: n"
         ),
     )
 
-    VsprintfInternalSlice = Symbol(
+    __vsprintf_internal_slice = Symbol(
         [0x88F5C],
         [0x2088F5C],
         None,
         (
-            "This is what implements the bulk of VsprintfInternal.\n\nThe"
+            "This is what implements the bulk of __vsprintf_internal.\n\nThe"
             " __vsprintf_internal in the modern-day version of glibc relies on"
             " __vfprintf_internal; this function has a slightly different interface,"
             " but it serves a similar role.\n\nr0: function pointer to append to the"
-            " string being built (VsprintfInternal uses TryAppendToSlice)\nr1: string"
-            " buffer slice\nr2: format\nr3: ap\nreturn: number of characters printed,"
-            " excluding the null-terminator"
+            " string being built (__vsprintf_internal uses TryAppendToSlice)\nr1:"
+            " string buffer slice\nr2: format\nr3: ap\nreturn: number of characters"
+            " printed, excluding the null-terminator"
         ),
     )
 
     TryAppendToSlice = Symbol(
         [0x89780],
         [0x2089780],
         None,
@@ -6722,258 +6722,258 @@
             "Best-effort append the given data to a slice. If the slice's capacity is"
             " reached, any remaining data will be truncated.\n\nr0: slice pointer\nr1:"
             " buffer of data to append\nr2: number of bytes in the data buffer\nreturn:"
             " true"
         ),
     )
 
-    VsprintfInternal = Symbol(
+    __vsprintf_internal = Symbol(
         [0x897C4],
         [0x20897C4],
         None,
         (
-            "This is what implements Vsprintf. It's akin to __vsprintf_internal in the"
+            "This is what implements vsprintf. It's akin to __vsprintf_internal in the"
             " modern-day version of glibc (in fact, it's probably an older version of"
-            " this).\n\nr0: str\nr1: maxlen (Vsprintf passes UINT32_MAX for this)\nr2:"
+            " this).\n\nr0: str\nr1: maxlen (vsprintf passes UINT32_MAX for this)\nr2:"
             " format\nr3: ap\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
-    Vsprintf = Symbol(
+    vsprintf = Symbol(
         [0x8982C],
         [0x208982C],
         None,
         (
             "The vsprintf(3) C library function.\n\nr0: str\nr1: format\nr2:"
             " ap\nreturn: number of characters printed, excluding the null-terminator"
         ),
     )
 
-    Snprintf = Symbol(
+    snprintf = Symbol(
         [0x89844],
         [0x2089844],
         None,
         (
-            "The snprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The snprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real snprintf.\n\nr0: str\nr1: n\nr2:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Sprintf = Symbol(
+    sprintf = Symbol(
         [0x8986C],
         [0x208986C],
         None,
         (
-            "The sprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The sprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real sprintf.\n\nr0: str\nr1:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Strlen = Symbol(
+    strlen = Symbol(
         [0x89960],
         [0x2089960],
         None,
         "The strlen(3) C library function.\n\nr0: s\nreturn: length of s",
     )
 
-    Strcpy = Symbol(
+    strcpy = Symbol(
         [0x8997C],
         [0x208997C],
         None,
         (
             "The strcpy(3) C library function.\n\nThis function is optimized to copy"
             " characters in aligned 4-byte chunks if possible, correctly handling any"
-            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src"
+            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src\nreturn: dest"
         ),
     )
 
-    Strncpy = Symbol(
+    strncpy = Symbol(
         [0x89A44],
         [0x2089A44],
         None,
-        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcat = Symbol(
+    strcat = Symbol(
         [0x89A94],
         [0x2089A94],
         None,
-        "The strcat(3) C library function.\n\nr0: dest\nr1: src",
+        "The strcat(3) C library function.\n\nr0: dest\nr1: src\nreturn: dest",
     )
 
-    Strncat = Symbol(
+    strncat = Symbol(
         [0x89AC4],
         [0x2089AC4],
         None,
-        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcmp = Symbol(
+    strcmp = Symbol(
         [0x89B14],
         [0x2089B14],
         None,
         (
-            "The strcmp(3) C library function.\n\nSimilarly to Strcpy, this function is"
+            "The strcmp(3) C library function.\n\nSimilarly to strcpy, this function is"
             " optimized to compare characters in aligned 4-byte chunks if"
             " possible.\n\nr0: s1\nr1: s2\nreturn: comparison value"
         ),
     )
 
-    Strncmp = Symbol(
+    strncmp = Symbol(
         [0x89C28],
         [0x2089C28],
         None,
         (
             "The strncmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    Strchr = Symbol(
+    strchr = Symbol(
         [0x89C5C],
         [0x2089C5C],
         None,
         (
             "The strchr(3) C library function.\n\nr0: string\nr1: c\nreturn: pointer to"
             " the located byte c, or null pointer if no match"
         ),
     )
 
-    Strcspn = Symbol(
+    strcspn = Symbol(
         [0x89C98],
         [0x2089C98],
         None,
         (
             "The strcspn(3) C library function.\n\nr0: string\nr1: stopset\nreturn:"
             " offset of the first character in string within stopset"
         ),
     )
 
-    Strstr = Symbol(
+    strstr = Symbol(
         [0x89D58],
         [0x2089D58],
         None,
         (
             "The strstr(3) C library function.\n\nr0: haystack\nr1: needle\nreturn:"
             " pointer into haystack where needle starts, or null pointer if no match"
         ),
     )
 
-    Wcslen = Symbol(
+    wcslen = Symbol(
         [0x8B6D0],
         [0x208B6D0],
         None,
         "The wcslen(3) C library function.\n\nr0: ws\nreturn: length of ws",
     )
 
-    AddFloat = Symbol(
+    __addsf3 = Symbol(
         [0x8EFA0],
         [0x208EFA0],
         None,
         (
             "This appears to be the libgcc implementation of __addsf3 (not sure which"
             " gcc version), which implements the addition operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a + b"
         ),
     )
 
-    DivideFloat = Symbol(
+    __divsf3 = Symbol(
         [0x8F51C],
         [0x208F51C],
         None,
         (
             "This appears to be the libgcc implementation of __divsf3 (not sure which"
             " gcc version), which implements the division operator for IEEE 754"
             " floating-point numbers.\n\nr0: dividend\nr1: divisor\nreturn: dividend /"
             " divisor"
         ),
     )
 
-    FloatToDouble = Symbol(
+    __extendsfdf2 = Symbol(
         [0x8F8D4],
         [0x208F8D4],
         None,
         (
             "This appears to be the libgcc implementation of __extendsfdf2 (not sure"
             " which gcc version), which implements the float to double cast operation"
             " for IEEE 754 floating-point numbers.\n\nr0: float\nreturn: (double)float"
         ),
     )
 
-    FloatToInt = Symbol(
+    __fixsfsi = Symbol(
         [0x8F958],
         [0x208F958],
         None,
         (
             "This appears to be the libgcc implementation of __fixsfsi (not sure which"
             " gcc version), which implements the float to int cast operation for IEEE"
             " 754 floating-point numbers. The output saturates if the input is out of"
             " the representable range for the int type.\n\nr0: float\nreturn:"
             " (int)float"
         ),
     )
 
-    IntToFloat = Symbol(
+    __floatsisf = Symbol(
         [0x8F98C],
         [0x208F98C],
         None,
         (
             "This appears to be the libgcc implementation of __floatsisf (not sure"
             " which gcc version), which implements the int to float cast operation for"
             " IEEE 754 floating-point numbers.\n\nr0: int\nreturn: (float)int"
         ),
     )
 
-    UIntToFloat = Symbol(
+    __floatunsisf = Symbol(
         [0x8F9D4],
         [0x208F9D4],
         None,
         (
             "This appears to be the libgcc implementation of __floatunsisf (not sure"
             " which gcc version), which implements the unsigned int to float cast"
             " operation for IEEE 754 floating-point numbers.\n\nr0: uint\nreturn:"
             " (float)uint"
         ),
     )
 
-    MultiplyFloat = Symbol(
+    __mulsf3 = Symbol(
         [0x8FA1C],
         [0x208FA1C],
         None,
         (
             "This appears to be the libgcc implementation of __mulsf3 (not sure which"
             " gcc version), which implements the multiplication operator for IEEE 754"
             " floating-point numbers."
         ),
     )
 
-    Sqrtf = Symbol(
+    sqrtf = Symbol(
         [0x8FBFC],
         [0x208FBFC],
         None,
         "The sqrtf(3) C library function.\n\nr0: x\nreturn: sqrt(x)",
     )
 
-    SubtractFloat = Symbol(
+    __subsf3 = Symbol(
         [0x8FCEC],
         [0x208FCEC],
         None,
         (
             "This appears to be the libgcc implementation of __subsf3 (not sure which"
             " gcc version), which implements the subtraction operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a - b"
         ),
     )
 
-    DivideInt = Symbol(
+    __divsi3 = Symbol(
         [0x9018C],
         [0x209018C],
         None,
         (
             "This appears to be the libgcc implementation of __divsi3 (not sure which"
             " gcc version), which implements the division operator for signed"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
@@ -6983,39 +6983,39 @@
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
             " (remainder << 32)"
         ),
     )
 
-    DivideUInt = Symbol(
+    __udivsi3 = Symbol(
         [0x90398],
         [0x2090398],
         None,
         (
             "This appears to be the libgcc implementation of __udivsi3 (not sure which"
             " gcc version), which implements the division operator for unsigned"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
             " (dividend / divisor) in the lower 32 bits and the remainder (dividend %"
             " divisor) in the upper 32 bits. In accordance with the Procedure Call"
             " Standard for the Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nNote: This function falls through to"
-            " DivideUIntNoZeroCheck.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
-            " (remainder << 32)"
+            " __udivsi3_no_zero_check.\n\nr0: dividend\nr1: divisor\nreturn: (quotient)"
+            " | (remainder << 32)"
         ),
     )
 
-    DivideUIntNoZeroCheck = Symbol(
+    __udivsi3_no_zero_check = Symbol(
         [0x903A0],
         [0x20903A0],
         None,
         (
-            "Subsidiary function to DivideUInt. Skips the initial check for divisor =="
+            "Subsidiary function to __udivsi3. Skips the initial check for divisor =="
             " 0.\n\nThe return value is a 64-bit integer, with the quotient (dividend /"
             " divisor) in the lower 32 bits and the remainder (dividend % divisor) in"
             " the upper 32 bits. In accordance with the Procedure Call Standard for the"
             " Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nThis function appears to only be called"
```

## pmdsky_debug_py/jp_itcm.py

```diff
@@ -556,15 +556,15 @@
 
     MemsetSimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the memset(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memset"
+            " function was probably manually implemented by the developers. See memset"
             " for what's probably the real libc function.\n\nr0: ptr\nr1: value\nr2:"
             " len (# bytes)"
         ),
     )
 
     Memset32 = Symbol(
         None,
@@ -578,15 +578,15 @@
 
     MemcpySimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the memcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memcpy"
+            " function was probably manually implemented by the developers. See memcpy"
             " for what's probably the real libc function.\n\nThis function copies from"
             " src to dst in backwards byte order, so this is safe to call for"
             " overlapping src and dst if src <= dst.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     Memcpy16 = Symbol(
@@ -953,15 +953,15 @@
 
     DebugPrint0 = Symbol(
         None,
         None,
         None,
         (
             "Would log a printf format string in the debug binary.\n\nThis still"
-            " constructs the string with Vsprintf, but doesn't actually do anything"
+            " constructs the string with vsprintf, but doesn't actually do anything"
             " with it in the final binary.\n\nr0: format\n...: variadic"
         ),
     )
 
     GetDebugFlag2 = Symbol(
         None,
         None,
@@ -1249,19 +1249,19 @@
     )
 
     SprintfStatic = Symbol(
         None,
         None,
         None,
         (
-            "Functionally the same as Sprintf, just defined statically in many"
+            "Functionally the same as sprintf, just defined statically in many"
             " different places.\n\nSince this is essentially just a wrapper around"
             " vsprintf(3), this function was probably statically defined in a header"
             " somewhere and included in a bunch of different places. See the actual"
-            " Sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
+            " sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
             " variadic\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
     ItemZInit = Symbol(None, None, None, "Zero-initializes an item struct.\n\nr0: item")
 
@@ -3020,26 +3020,26 @@
 
     StrcpySimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the strcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strcpy"
+            " function was probably manually implemented by the developers. See strcpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src"
         ),
     )
 
     StrncpySimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the strncpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncpy"
+            " function was probably manually implemented by the developers. See strncpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     StrncpySimpleNoPad = Symbol(
         None,
         None,
@@ -3052,15 +3052,15 @@
 
     StrncmpSimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the strncmp(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncmp"
+            " function was probably manually implemented by the developers. See strncmp"
             " for what's probably the real libc function.\n\nr0: s1\nr1: s2\nr2:"
             " n\nreturn: comparison value"
         ),
     )
 
     StrncpySimpleNoPadSafe = Symbol(
         None,
@@ -6387,22 +6387,22 @@
         None,
         (
             "Initializes a file_stream structure for file I/O.\n\nThis function must"
             " always be called before opening a file.\n\nr0: file_stream pointer"
         ),
     )
 
-    Abs = Symbol(
+    abs = Symbol(
         None,
         None,
         None,
         "Takes the absolute value of an integer.\n\nr0: x\nreturn: abs(x)",
     )
 
-    Mbtowc = Symbol(
+    mbtowc = Symbol(
         None,
         None,
         None,
         (
             "The mbtowc(3) C library function.\n\nr0: pwc\nr1: s\nr2: n\nreturn: number"
             " of consumed bytes, or -1 on failure"
         ),
@@ -6426,99 +6426,99 @@
         (
             "Wrapper around TryAssignByte.\n\nAccesses the TryAssignByte function with"
             " a weird chain of pointer dereferences.\n\nr0: pointer\nr1: value\nreturn:"
             " true on success, false on failure"
         ),
     )
 
-    Wcstombs = Symbol(
+    wcstombs = Symbol(
         None,
         None,
         None,
         (
             "The wcstombs(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn:"
             " characters converted"
         ),
     )
 
-    Memcpy = Symbol(
+    memcpy = Symbol(
         None,
         None,
         None,
-        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Memmove = Symbol(
+    memmove = Symbol(
         None,
         None,
         None,
         (
             "The memmove(3) C library function.\n\nThe implementation is nearly the"
-            " same as Memcpy, but it copies bytes from back to front if src <"
-            " dst.\n\nr0: dest\nr1: src\nr2: n"
+            " same as memcpy, but it copies bytes from back to front if src <"
+            " dst.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest"
         ),
     )
 
-    Memset = Symbol(
+    memset = Symbol(
         None,
         None,
         None,
         (
             "The memset(3) C library function.\n\nThis is just a wrapper around"
-            " MemsetInternal that returns the pointer at the end.\n\nr0: s\nr1: c (int,"
-            " but must be a single-byte value)\nr2: n\nreturn: s"
+            " memset_internal that returns the pointer at the end.\n\nr0: s\nr1: c"
+            " (int, but must be a single-byte value)\nr2: n\nreturn: s"
         ),
     )
 
-    Memchr = Symbol(
+    memchr = Symbol(
         None,
         None,
         None,
         (
             "The memchr(3) C library function.\n\nr0: s\nr1: c\nr2: n\nreturn: pointer"
             " to first occurrence of c in s, or a null pointer if no match"
         ),
     )
 
-    Memcmp = Symbol(
+    memcmp = Symbol(
         None,
         None,
         None,
         (
             "The memcmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    MemsetInternal = Symbol(
+    memset_internal = Symbol(
         None,
         None,
         None,
         (
             "The actual memory-setting implementation for the memset(3) C library"
             " function.\n\nThis function is optimized to set bytes in 4-byte chunks for"
             " n >= 32, correctly handling any unaligned bytes at the front/back. In"
             " this case, it also further optimizes by unrolling a for loop to set 8"
             " 4-byte values at once (effectively a 32-byte chunk).\n\nr0: s\nr1: c"
             " (int, but must be a single-byte value)\nr2: n"
         ),
     )
 
-    VsprintfInternalSlice = Symbol(
+    __vsprintf_internal_slice = Symbol(
         None,
         None,
         None,
         (
-            "This is what implements the bulk of VsprintfInternal.\n\nThe"
+            "This is what implements the bulk of __vsprintf_internal.\n\nThe"
             " __vsprintf_internal in the modern-day version of glibc relies on"
             " __vfprintf_internal; this function has a slightly different interface,"
             " but it serves a similar role.\n\nr0: function pointer to append to the"
-            " string being built (VsprintfInternal uses TryAppendToSlice)\nr1: string"
-            " buffer slice\nr2: format\nr3: ap\nreturn: number of characters printed,"
-            " excluding the null-terminator"
+            " string being built (__vsprintf_internal uses TryAppendToSlice)\nr1:"
+            " string buffer slice\nr2: format\nr3: ap\nreturn: number of characters"
+            " printed, excluding the null-terminator"
         ),
     )
 
     TryAppendToSlice = Symbol(
         None,
         None,
         None,
@@ -6526,252 +6526,255 @@
             "Best-effort append the given data to a slice. If the slice's capacity is"
             " reached, any remaining data will be truncated.\n\nr0: slice pointer\nr1:"
             " buffer of data to append\nr2: number of bytes in the data buffer\nreturn:"
             " true"
         ),
     )
 
-    VsprintfInternal = Symbol(
+    __vsprintf_internal = Symbol(
         None,
         None,
         None,
         (
-            "This is what implements Vsprintf. It's akin to __vsprintf_internal in the"
+            "This is what implements vsprintf. It's akin to __vsprintf_internal in the"
             " modern-day version of glibc (in fact, it's probably an older version of"
-            " this).\n\nr0: str\nr1: maxlen (Vsprintf passes UINT32_MAX for this)\nr2:"
+            " this).\n\nr0: str\nr1: maxlen (vsprintf passes UINT32_MAX for this)\nr2:"
             " format\nr3: ap\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
-    Vsprintf = Symbol(
+    vsprintf = Symbol(
         None,
         None,
         None,
         (
             "The vsprintf(3) C library function.\n\nr0: str\nr1: format\nr2:"
             " ap\nreturn: number of characters printed, excluding the null-terminator"
         ),
     )
 
-    Snprintf = Symbol(
+    snprintf = Symbol(
         None,
         None,
         None,
         (
-            "The snprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The snprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real snprintf.\n\nr0: str\nr1: n\nr2:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Sprintf = Symbol(
+    sprintf = Symbol(
         None,
         None,
         None,
         (
-            "The sprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The sprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real sprintf.\n\nr0: str\nr1:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Strlen = Symbol(
+    strlen = Symbol(
         None,
         None,
         None,
         "The strlen(3) C library function.\n\nr0: s\nreturn: length of s",
     )
 
-    Strcpy = Symbol(
+    strcpy = Symbol(
         None,
         None,
         None,
         (
             "The strcpy(3) C library function.\n\nThis function is optimized to copy"
             " characters in aligned 4-byte chunks if possible, correctly handling any"
-            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src"
+            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src\nreturn: dest"
         ),
     )
 
-    Strncpy = Symbol(
+    strncpy = Symbol(
         None,
         None,
         None,
-        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcat = Symbol(
-        None, None, None, "The strcat(3) C library function.\n\nr0: dest\nr1: src"
+    strcat = Symbol(
+        None,
+        None,
+        None,
+        "The strcat(3) C library function.\n\nr0: dest\nr1: src\nreturn: dest",
     )
 
-    Strncat = Symbol(
+    strncat = Symbol(
         None,
         None,
         None,
-        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcmp = Symbol(
+    strcmp = Symbol(
         None,
         None,
         None,
         (
-            "The strcmp(3) C library function.\n\nSimilarly to Strcpy, this function is"
+            "The strcmp(3) C library function.\n\nSimilarly to strcpy, this function is"
             " optimized to compare characters in aligned 4-byte chunks if"
             " possible.\n\nr0: s1\nr1: s2\nreturn: comparison value"
         ),
     )
 
-    Strncmp = Symbol(
+    strncmp = Symbol(
         None,
         None,
         None,
         (
             "The strncmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    Strchr = Symbol(
+    strchr = Symbol(
         None,
         None,
         None,
         (
             "The strchr(3) C library function.\n\nr0: string\nr1: c\nreturn: pointer to"
             " the located byte c, or null pointer if no match"
         ),
     )
 
-    Strcspn = Symbol(
+    strcspn = Symbol(
         None,
         None,
         None,
         (
             "The strcspn(3) C library function.\n\nr0: string\nr1: stopset\nreturn:"
             " offset of the first character in string within stopset"
         ),
     )
 
-    Strstr = Symbol(
+    strstr = Symbol(
         None,
         None,
         None,
         (
             "The strstr(3) C library function.\n\nr0: haystack\nr1: needle\nreturn:"
             " pointer into haystack where needle starts, or null pointer if no match"
         ),
     )
 
-    Wcslen = Symbol(
+    wcslen = Symbol(
         None,
         None,
         None,
         "The wcslen(3) C library function.\n\nr0: ws\nreturn: length of ws",
     )
 
-    AddFloat = Symbol(
+    __addsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __addsf3 (not sure which"
             " gcc version), which implements the addition operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a + b"
         ),
     )
 
-    DivideFloat = Symbol(
+    __divsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __divsf3 (not sure which"
             " gcc version), which implements the division operator for IEEE 754"
             " floating-point numbers.\n\nr0: dividend\nr1: divisor\nreturn: dividend /"
             " divisor"
         ),
     )
 
-    FloatToDouble = Symbol(
+    __extendsfdf2 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __extendsfdf2 (not sure"
             " which gcc version), which implements the float to double cast operation"
             " for IEEE 754 floating-point numbers.\n\nr0: float\nreturn: (double)float"
         ),
     )
 
-    FloatToInt = Symbol(
+    __fixsfsi = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __fixsfsi (not sure which"
             " gcc version), which implements the float to int cast operation for IEEE"
             " 754 floating-point numbers. The output saturates if the input is out of"
             " the representable range for the int type.\n\nr0: float\nreturn:"
             " (int)float"
         ),
     )
 
-    IntToFloat = Symbol(
+    __floatsisf = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __floatsisf (not sure"
             " which gcc version), which implements the int to float cast operation for"
             " IEEE 754 floating-point numbers.\n\nr0: int\nreturn: (float)int"
         ),
     )
 
-    UIntToFloat = Symbol(
+    __floatunsisf = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __floatunsisf (not sure"
             " which gcc version), which implements the unsigned int to float cast"
             " operation for IEEE 754 floating-point numbers.\n\nr0: uint\nreturn:"
             " (float)uint"
         ),
     )
 
-    MultiplyFloat = Symbol(
+    __mulsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __mulsf3 (not sure which"
             " gcc version), which implements the multiplication operator for IEEE 754"
             " floating-point numbers."
         ),
     )
 
-    Sqrtf = Symbol(
+    sqrtf = Symbol(
         None, None, None, "The sqrtf(3) C library function.\n\nr0: x\nreturn: sqrt(x)"
     )
 
-    SubtractFloat = Symbol(
+    __subsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __subsf3 (not sure which"
             " gcc version), which implements the subtraction operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a - b"
         ),
     )
 
-    DivideInt = Symbol(
+    __divsi3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __divsi3 (not sure which"
             " gcc version), which implements the division operator for signed"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
@@ -6781,39 +6784,39 @@
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
             " (remainder << 32)"
         ),
     )
 
-    DivideUInt = Symbol(
+    __udivsi3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __udivsi3 (not sure which"
             " gcc version), which implements the division operator for unsigned"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
             " (dividend / divisor) in the lower 32 bits and the remainder (dividend %"
             " divisor) in the upper 32 bits. In accordance with the Procedure Call"
             " Standard for the Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nNote: This function falls through to"
-            " DivideUIntNoZeroCheck.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
-            " (remainder << 32)"
+            " __udivsi3_no_zero_check.\n\nr0: dividend\nr1: divisor\nreturn: (quotient)"
+            " | (remainder << 32)"
         ),
     )
 
-    DivideUIntNoZeroCheck = Symbol(
+    __udivsi3_no_zero_check = Symbol(
         None,
         None,
         None,
         (
-            "Subsidiary function to DivideUInt. Skips the initial check for divisor =="
+            "Subsidiary function to __udivsi3. Skips the initial check for divisor =="
             " 0.\n\nThe return value is a 64-bit integer, with the quotient (dividend /"
             " divisor) in the lower 32 bits and the remainder (dividend % divisor) in"
             " the upper 32 bits. In accordance with the Procedure Call Standard for the"
             " Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nThis function appears to only be called"
```

## pmdsky_debug_py/na.py

```diff
@@ -563,15 +563,15 @@
 
     MemsetSimple = Symbol(
         [0x32A4],
         [0x20032A4],
         None,
         (
             "A simple implementation of the memset(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memset"
+            " function was probably manually implemented by the developers. See memset"
             " for what's probably the real libc function.\n\nr0: ptr\nr1: value\nr2:"
             " len (# bytes)"
         ),
     )
 
     Memset32 = Symbol(
         [0x32BC],
@@ -585,15 +585,15 @@
 
     MemcpySimple = Symbol(
         [0x32D4],
         [0x20032D4],
         None,
         (
             "A simple implementation of the memcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memcpy"
+            " function was probably manually implemented by the developers. See memcpy"
             " for what's probably the real libc function.\n\nThis function copies from"
             " src to dst in backwards byte order, so this is safe to call for"
             " overlapping src and dst if src <= dst.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     Memcpy16 = Symbol(
@@ -963,15 +963,15 @@
 
     DebugPrint0 = Symbol(
         [0xC1C8, 0xC1FC],
         [0x200C1C8, 0x200C1FC],
         None,
         (
             "Would log a printf format string in the debug binary.\n\nThis still"
-            " constructs the string with Vsprintf, but doesn't actually do anything"
+            " constructs the string with vsprintf, but doesn't actually do anything"
             " with it in the final binary.\n\nr0: format\n...: variadic"
         ),
     )
 
     GetDebugFlag2 = Symbol(
         [0xC234],
         [0x200C234],
@@ -1299,19 +1299,19 @@
             0x2042A84,
             0x2052418,
             0x2054A60,
             0x20609E8,
         ],
         None,
         (
-            "Functionally the same as Sprintf, just defined statically in many"
+            "Functionally the same as sprintf, just defined statically in many"
             " different places.\n\nSince this is essentially just a wrapper around"
             " vsprintf(3), this function was probably statically defined in a header"
             " somewhere and included in a bunch of different places. See the actual"
-            " Sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
+            " sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
             " variadic\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
     ItemZInit = Symbol(
         [0xD81C], [0x200D81C], None, "Zero-initializes an item struct.\n\nr0: item"
@@ -3110,26 +3110,26 @@
 
     StrcpySimple = Symbol(
         [0x25100],
         [0x2025100],
         None,
         (
             "A simple implementation of the strcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strcpy"
+            " function was probably manually implemented by the developers. See strcpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src"
         ),
     )
 
     StrncpySimple = Symbol(
         [0x2511C],
         [0x202511C],
         None,
         (
             "A simple implementation of the strncpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncpy"
+            " function was probably manually implemented by the developers. See strncpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     StrncpySimpleNoPad = Symbol(
         [0x25170],
         [0x2025170],
@@ -3142,15 +3142,15 @@
 
     StrncmpSimple = Symbol(
         [0x251AC],
         [0x20251AC],
         None,
         (
             "A simple implementation of the strncmp(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncmp"
+            " function was probably manually implemented by the developers. See strncmp"
             " for what's probably the real libc function.\n\nr0: s1\nr1: s2\nr2:"
             " n\nreturn: comparison value"
         ),
     )
 
     StrncpySimpleNoPadSafe = Symbol(
         [0x251F4],
@@ -6585,22 +6585,22 @@
         None,
         (
             "Initializes a file_stream structure for file I/O.\n\nThis function must"
             " always be called before opening a file.\n\nr0: file_stream pointer"
         ),
     )
 
-    Abs = Symbol(
+    abs = Symbol(
         [0x8655C],
         [0x208655C],
         None,
         "Takes the absolute value of an integer.\n\nr0: x\nreturn: abs(x)",
     )
 
-    Mbtowc = Symbol(
+    mbtowc = Symbol(
         [0x871BC],
         [0x20871BC],
         None,
         (
             "The mbtowc(3) C library function.\n\nr0: pwc\nr1: s\nr2: n\nreturn: number"
             " of consumed bytes, or -1 on failure"
         ),
@@ -6624,99 +6624,99 @@
         (
             "Wrapper around TryAssignByte.\n\nAccesses the TryAssignByte function with"
             " a weird chain of pointer dereferences.\n\nr0: pointer\nr1: value\nreturn:"
             " true on success, false on failure"
         ),
     )
 
-    Wcstombs = Symbol(
+    wcstombs = Symbol(
         [0x87224],
         [0x2087224],
         None,
         (
             "The wcstombs(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn:"
             " characters converted"
         ),
     )
 
-    Memcpy = Symbol(
+    memcpy = Symbol(
         [0x8729C],
         [0x208729C],
         None,
-        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Memmove = Symbol(
+    memmove = Symbol(
         [0x872BC],
         [0x20872BC],
         None,
         (
             "The memmove(3) C library function.\n\nThe implementation is nearly the"
-            " same as Memcpy, but it copies bytes from back to front if src <"
-            " dst.\n\nr0: dest\nr1: src\nr2: n"
+            " same as memcpy, but it copies bytes from back to front if src <"
+            " dst.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest"
         ),
     )
 
-    Memset = Symbol(
+    memset = Symbol(
         [0x87308],
         [0x2087308],
         None,
         (
             "The memset(3) C library function.\n\nThis is just a wrapper around"
-            " MemsetInternal that returns the pointer at the end.\n\nr0: s\nr1: c (int,"
-            " but must be a single-byte value)\nr2: n\nreturn: s"
+            " memset_internal that returns the pointer at the end.\n\nr0: s\nr1: c"
+            " (int, but must be a single-byte value)\nr2: n\nreturn: s"
         ),
     )
 
-    Memchr = Symbol(
+    memchr = Symbol(
         [0x8731C],
         [0x208731C],
         None,
         (
             "The memchr(3) C library function.\n\nr0: s\nr1: c\nr2: n\nreturn: pointer"
             " to first occurrence of c in s, or a null pointer if no match"
         ),
     )
 
-    Memcmp = Symbol(
+    memcmp = Symbol(
         [0x87348],
         [0x2087348],
         None,
         (
             "The memcmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    MemsetInternal = Symbol(
+    memset_internal = Symbol(
         [0x87388],
         [0x2087388],
         None,
         (
             "The actual memory-setting implementation for the memset(3) C library"
             " function.\n\nThis function is optimized to set bytes in 4-byte chunks for"
             " n >= 32, correctly handling any unaligned bytes at the front/back. In"
             " this case, it also further optimizes by unrolling a for loop to set 8"
             " 4-byte values at once (effectively a 32-byte chunk).\n\nr0: s\nr1: c"
             " (int, but must be a single-byte value)\nr2: n"
         ),
     )
 
-    VsprintfInternalSlice = Symbol(
+    __vsprintf_internal_slice = Symbol(
         [0x88C74],
         [0x2088C74],
         None,
         (
-            "This is what implements the bulk of VsprintfInternal.\n\nThe"
+            "This is what implements the bulk of __vsprintf_internal.\n\nThe"
             " __vsprintf_internal in the modern-day version of glibc relies on"
             " __vfprintf_internal; this function has a slightly different interface,"
             " but it serves a similar role.\n\nr0: function pointer to append to the"
-            " string being built (VsprintfInternal uses TryAppendToSlice)\nr1: string"
-            " buffer slice\nr2: format\nr3: ap\nreturn: number of characters printed,"
-            " excluding the null-terminator"
+            " string being built (__vsprintf_internal uses TryAppendToSlice)\nr1:"
+            " string buffer slice\nr2: format\nr3: ap\nreturn: number of characters"
+            " printed, excluding the null-terminator"
         ),
     )
 
     TryAppendToSlice = Symbol(
         [0x89498],
         [0x2089498],
         None,
@@ -6724,258 +6724,258 @@
             "Best-effort append the given data to a slice. If the slice's capacity is"
             " reached, any remaining data will be truncated.\n\nr0: slice pointer\nr1:"
             " buffer of data to append\nr2: number of bytes in the data buffer\nreturn:"
             " true"
         ),
     )
 
-    VsprintfInternal = Symbol(
+    __vsprintf_internal = Symbol(
         [0x894DC],
         [0x20894DC],
         None,
         (
-            "This is what implements Vsprintf. It's akin to __vsprintf_internal in the"
+            "This is what implements vsprintf. It's akin to __vsprintf_internal in the"
             " modern-day version of glibc (in fact, it's probably an older version of"
-            " this).\n\nr0: str\nr1: maxlen (Vsprintf passes UINT32_MAX for this)\nr2:"
+            " this).\n\nr0: str\nr1: maxlen (vsprintf passes UINT32_MAX for this)\nr2:"
             " format\nr3: ap\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
-    Vsprintf = Symbol(
+    vsprintf = Symbol(
         [0x89544],
         [0x2089544],
         None,
         (
             "The vsprintf(3) C library function.\n\nr0: str\nr1: format\nr2:"
             " ap\nreturn: number of characters printed, excluding the null-terminator"
         ),
     )
 
-    Snprintf = Symbol(
+    snprintf = Symbol(
         [0x8955C],
         [0x208955C],
         None,
         (
-            "The snprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The snprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real snprintf.\n\nr0: str\nr1: n\nr2:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Sprintf = Symbol(
+    sprintf = Symbol(
         [0x89584],
         [0x2089584],
         None,
         (
-            "The sprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The sprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real sprintf.\n\nr0: str\nr1:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Strlen = Symbol(
+    strlen = Symbol(
         [0x89678],
         [0x2089678],
         None,
         "The strlen(3) C library function.\n\nr0: s\nreturn: length of s",
     )
 
-    Strcpy = Symbol(
+    strcpy = Symbol(
         [0x89694],
         [0x2089694],
         None,
         (
             "The strcpy(3) C library function.\n\nThis function is optimized to copy"
             " characters in aligned 4-byte chunks if possible, correctly handling any"
-            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src"
+            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src\nreturn: dest"
         ),
     )
 
-    Strncpy = Symbol(
+    strncpy = Symbol(
         [0x8975C],
         [0x208975C],
         None,
-        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcat = Symbol(
+    strcat = Symbol(
         [0x897AC],
         [0x20897AC],
         None,
-        "The strcat(3) C library function.\n\nr0: dest\nr1: src",
+        "The strcat(3) C library function.\n\nr0: dest\nr1: src\nreturn: dest",
     )
 
-    Strncat = Symbol(
+    strncat = Symbol(
         [0x897DC],
         [0x20897DC],
         None,
-        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcmp = Symbol(
+    strcmp = Symbol(
         [0x8982C],
         [0x208982C],
         None,
         (
-            "The strcmp(3) C library function.\n\nSimilarly to Strcpy, this function is"
+            "The strcmp(3) C library function.\n\nSimilarly to strcpy, this function is"
             " optimized to compare characters in aligned 4-byte chunks if"
             " possible.\n\nr0: s1\nr1: s2\nreturn: comparison value"
         ),
     )
 
-    Strncmp = Symbol(
+    strncmp = Symbol(
         [0x89940],
         [0x2089940],
         None,
         (
             "The strncmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    Strchr = Symbol(
+    strchr = Symbol(
         [0x89974],
         [0x2089974],
         None,
         (
             "The strchr(3) C library function.\n\nr0: string\nr1: c\nreturn: pointer to"
             " the located byte c, or null pointer if no match"
         ),
     )
 
-    Strcspn = Symbol(
+    strcspn = Symbol(
         [0x899B0],
         [0x20899B0],
         None,
         (
             "The strcspn(3) C library function.\n\nr0: string\nr1: stopset\nreturn:"
             " offset of the first character in string within stopset"
         ),
     )
 
-    Strstr = Symbol(
+    strstr = Symbol(
         [0x89A70],
         [0x2089A70],
         None,
         (
             "The strstr(3) C library function.\n\nr0: haystack\nr1: needle\nreturn:"
             " pointer into haystack where needle starts, or null pointer if no match"
         ),
     )
 
-    Wcslen = Symbol(
+    wcslen = Symbol(
         [0x8B3E8],
         [0x208B3E8],
         None,
         "The wcslen(3) C library function.\n\nr0: ws\nreturn: length of ws",
     )
 
-    AddFloat = Symbol(
+    __addsf3 = Symbol(
         [0x8ECB8],
         [0x208ECB8],
         None,
         (
             "This appears to be the libgcc implementation of __addsf3 (not sure which"
             " gcc version), which implements the addition operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a + b"
         ),
     )
 
-    DivideFloat = Symbol(
+    __divsf3 = Symbol(
         [0x8F234],
         [0x208F234],
         None,
         (
             "This appears to be the libgcc implementation of __divsf3 (not sure which"
             " gcc version), which implements the division operator for IEEE 754"
             " floating-point numbers.\n\nr0: dividend\nr1: divisor\nreturn: dividend /"
             " divisor"
         ),
     )
 
-    FloatToDouble = Symbol(
+    __extendsfdf2 = Symbol(
         [0x8F5EC],
         [0x208F5EC],
         None,
         (
             "This appears to be the libgcc implementation of __extendsfdf2 (not sure"
             " which gcc version), which implements the float to double cast operation"
             " for IEEE 754 floating-point numbers.\n\nr0: float\nreturn: (double)float"
         ),
     )
 
-    FloatToInt = Symbol(
+    __fixsfsi = Symbol(
         [0x8F670],
         [0x208F670],
         None,
         (
             "This appears to be the libgcc implementation of __fixsfsi (not sure which"
             " gcc version), which implements the float to int cast operation for IEEE"
             " 754 floating-point numbers. The output saturates if the input is out of"
             " the representable range for the int type.\n\nr0: float\nreturn:"
             " (int)float"
         ),
     )
 
-    IntToFloat = Symbol(
+    __floatsisf = Symbol(
         [0x8F6A4],
         [0x208F6A4],
         None,
         (
             "This appears to be the libgcc implementation of __floatsisf (not sure"
             " which gcc version), which implements the int to float cast operation for"
             " IEEE 754 floating-point numbers.\n\nr0: int\nreturn: (float)int"
         ),
     )
 
-    UIntToFloat = Symbol(
+    __floatunsisf = Symbol(
         [0x8F6EC],
         [0x208F6EC],
         None,
         (
             "This appears to be the libgcc implementation of __floatunsisf (not sure"
             " which gcc version), which implements the unsigned int to float cast"
             " operation for IEEE 754 floating-point numbers.\n\nr0: uint\nreturn:"
             " (float)uint"
         ),
     )
 
-    MultiplyFloat = Symbol(
+    __mulsf3 = Symbol(
         [0x8F734],
         [0x208F734],
         None,
         (
             "This appears to be the libgcc implementation of __mulsf3 (not sure which"
             " gcc version), which implements the multiplication operator for IEEE 754"
             " floating-point numbers."
         ),
     )
 
-    Sqrtf = Symbol(
+    sqrtf = Symbol(
         [0x8F914],
         [0x208F914],
         None,
         "The sqrtf(3) C library function.\n\nr0: x\nreturn: sqrt(x)",
     )
 
-    SubtractFloat = Symbol(
+    __subsf3 = Symbol(
         [0x8FA04],
         [0x208FA04],
         None,
         (
             "This appears to be the libgcc implementation of __subsf3 (not sure which"
             " gcc version), which implements the subtraction operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a - b"
         ),
     )
 
-    DivideInt = Symbol(
+    __divsi3 = Symbol(
         [0x8FEA4],
         [0x208FEA4],
         None,
         (
             "This appears to be the libgcc implementation of __divsi3 (not sure which"
             " gcc version), which implements the division operator for signed"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
@@ -6985,39 +6985,39 @@
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
             " (remainder << 32)"
         ),
     )
 
-    DivideUInt = Symbol(
+    __udivsi3 = Symbol(
         [0x900B0],
         [0x20900B0],
         None,
         (
             "This appears to be the libgcc implementation of __udivsi3 (not sure which"
             " gcc version), which implements the division operator for unsigned"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
             " (dividend / divisor) in the lower 32 bits and the remainder (dividend %"
             " divisor) in the upper 32 bits. In accordance with the Procedure Call"
             " Standard for the Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nNote: This function falls through to"
-            " DivideUIntNoZeroCheck.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
-            " (remainder << 32)"
+            " __udivsi3_no_zero_check.\n\nr0: dividend\nr1: divisor\nreturn: (quotient)"
+            " | (remainder << 32)"
         ),
     )
 
-    DivideUIntNoZeroCheck = Symbol(
+    __udivsi3_no_zero_check = Symbol(
         [0x900B8],
         [0x20900B8],
         None,
         (
-            "Subsidiary function to DivideUInt. Skips the initial check for divisor =="
+            "Subsidiary function to __udivsi3. Skips the initial check for divisor =="
             " 0.\n\nThe return value is a 64-bit integer, with the quotient (dividend /"
             " divisor) in the lower 32 bits and the remainder (dividend % divisor) in"
             " the upper 32 bits. In accordance with the Procedure Call Standard for the"
             " Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nThis function appears to only be called"
```

## pmdsky_debug_py/na_itcm.py

```diff
@@ -556,15 +556,15 @@
 
     MemsetSimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the memset(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memset"
+            " function was probably manually implemented by the developers. See memset"
             " for what's probably the real libc function.\n\nr0: ptr\nr1: value\nr2:"
             " len (# bytes)"
         ),
     )
 
     Memset32 = Symbol(
         None,
@@ -578,15 +578,15 @@
 
     MemcpySimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the memcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Memcpy"
+            " function was probably manually implemented by the developers. See memcpy"
             " for what's probably the real libc function.\n\nThis function copies from"
             " src to dst in backwards byte order, so this is safe to call for"
             " overlapping src and dst if src <= dst.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     Memcpy16 = Symbol(
@@ -953,15 +953,15 @@
 
     DebugPrint0 = Symbol(
         None,
         None,
         None,
         (
             "Would log a printf format string in the debug binary.\n\nThis still"
-            " constructs the string with Vsprintf, but doesn't actually do anything"
+            " constructs the string with vsprintf, but doesn't actually do anything"
             " with it in the final binary.\n\nr0: format\n...: variadic"
         ),
     )
 
     GetDebugFlag2 = Symbol(
         None,
         None,
@@ -1249,19 +1249,19 @@
     )
 
     SprintfStatic = Symbol(
         None,
         None,
         None,
         (
-            "Functionally the same as Sprintf, just defined statically in many"
+            "Functionally the same as sprintf, just defined statically in many"
             " different places.\n\nSince this is essentially just a wrapper around"
             " vsprintf(3), this function was probably statically defined in a header"
             " somewhere and included in a bunch of different places. See the actual"
-            " Sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
+            " sprintf for the one in libc.\n\nr0: str\nr1: format\n...:"
             " variadic\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
     ItemZInit = Symbol(None, None, None, "Zero-initializes an item struct.\n\nr0: item")
 
@@ -3020,26 +3020,26 @@
 
     StrcpySimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the strcpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strcpy"
+            " function was probably manually implemented by the developers. See strcpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src"
         ),
     )
 
     StrncpySimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the strncpy(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncpy"
+            " function was probably manually implemented by the developers. See strncpy"
             " for what's probably the real libc function.\n\nr0: dest\nr1: src\nr2: n"
         ),
     )
 
     StrncpySimpleNoPad = Symbol(
         None,
         None,
@@ -3052,15 +3052,15 @@
 
     StrncmpSimple = Symbol(
         None,
         None,
         None,
         (
             "A simple implementation of the strncmp(3) C library function.\n\nThis"
-            " function was probably manually implemented by the developers. See Strncmp"
+            " function was probably manually implemented by the developers. See strncmp"
             " for what's probably the real libc function.\n\nr0: s1\nr1: s2\nr2:"
             " n\nreturn: comparison value"
         ),
     )
 
     StrncpySimpleNoPadSafe = Symbol(
         None,
@@ -6387,22 +6387,22 @@
         None,
         (
             "Initializes a file_stream structure for file I/O.\n\nThis function must"
             " always be called before opening a file.\n\nr0: file_stream pointer"
         ),
     )
 
-    Abs = Symbol(
+    abs = Symbol(
         None,
         None,
         None,
         "Takes the absolute value of an integer.\n\nr0: x\nreturn: abs(x)",
     )
 
-    Mbtowc = Symbol(
+    mbtowc = Symbol(
         None,
         None,
         None,
         (
             "The mbtowc(3) C library function.\n\nr0: pwc\nr1: s\nr2: n\nreturn: number"
             " of consumed bytes, or -1 on failure"
         ),
@@ -6426,99 +6426,99 @@
         (
             "Wrapper around TryAssignByte.\n\nAccesses the TryAssignByte function with"
             " a weird chain of pointer dereferences.\n\nr0: pointer\nr1: value\nreturn:"
             " true on success, false on failure"
         ),
     )
 
-    Wcstombs = Symbol(
+    wcstombs = Symbol(
         None,
         None,
         None,
         (
             "The wcstombs(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn:"
             " characters converted"
         ),
     )
 
-    Memcpy = Symbol(
+    memcpy = Symbol(
         None,
         None,
         None,
-        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The memcpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Memmove = Symbol(
+    memmove = Symbol(
         None,
         None,
         None,
         (
             "The memmove(3) C library function.\n\nThe implementation is nearly the"
-            " same as Memcpy, but it copies bytes from back to front if src <"
-            " dst.\n\nr0: dest\nr1: src\nr2: n"
+            " same as memcpy, but it copies bytes from back to front if src <"
+            " dst.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest"
         ),
     )
 
-    Memset = Symbol(
+    memset = Symbol(
         None,
         None,
         None,
         (
             "The memset(3) C library function.\n\nThis is just a wrapper around"
-            " MemsetInternal that returns the pointer at the end.\n\nr0: s\nr1: c (int,"
-            " but must be a single-byte value)\nr2: n\nreturn: s"
+            " memset_internal that returns the pointer at the end.\n\nr0: s\nr1: c"
+            " (int, but must be a single-byte value)\nr2: n\nreturn: s"
         ),
     )
 
-    Memchr = Symbol(
+    memchr = Symbol(
         None,
         None,
         None,
         (
             "The memchr(3) C library function.\n\nr0: s\nr1: c\nr2: n\nreturn: pointer"
             " to first occurrence of c in s, or a null pointer if no match"
         ),
     )
 
-    Memcmp = Symbol(
+    memcmp = Symbol(
         None,
         None,
         None,
         (
             "The memcmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    MemsetInternal = Symbol(
+    memset_internal = Symbol(
         None,
         None,
         None,
         (
             "The actual memory-setting implementation for the memset(3) C library"
             " function.\n\nThis function is optimized to set bytes in 4-byte chunks for"
             " n >= 32, correctly handling any unaligned bytes at the front/back. In"
             " this case, it also further optimizes by unrolling a for loop to set 8"
             " 4-byte values at once (effectively a 32-byte chunk).\n\nr0: s\nr1: c"
             " (int, but must be a single-byte value)\nr2: n"
         ),
     )
 
-    VsprintfInternalSlice = Symbol(
+    __vsprintf_internal_slice = Symbol(
         None,
         None,
         None,
         (
-            "This is what implements the bulk of VsprintfInternal.\n\nThe"
+            "This is what implements the bulk of __vsprintf_internal.\n\nThe"
             " __vsprintf_internal in the modern-day version of glibc relies on"
             " __vfprintf_internal; this function has a slightly different interface,"
             " but it serves a similar role.\n\nr0: function pointer to append to the"
-            " string being built (VsprintfInternal uses TryAppendToSlice)\nr1: string"
-            " buffer slice\nr2: format\nr3: ap\nreturn: number of characters printed,"
-            " excluding the null-terminator"
+            " string being built (__vsprintf_internal uses TryAppendToSlice)\nr1:"
+            " string buffer slice\nr2: format\nr3: ap\nreturn: number of characters"
+            " printed, excluding the null-terminator"
         ),
     )
 
     TryAppendToSlice = Symbol(
         None,
         None,
         None,
@@ -6526,252 +6526,255 @@
             "Best-effort append the given data to a slice. If the slice's capacity is"
             " reached, any remaining data will be truncated.\n\nr0: slice pointer\nr1:"
             " buffer of data to append\nr2: number of bytes in the data buffer\nreturn:"
             " true"
         ),
     )
 
-    VsprintfInternal = Symbol(
+    __vsprintf_internal = Symbol(
         None,
         None,
         None,
         (
-            "This is what implements Vsprintf. It's akin to __vsprintf_internal in the"
+            "This is what implements vsprintf. It's akin to __vsprintf_internal in the"
             " modern-day version of glibc (in fact, it's probably an older version of"
-            " this).\n\nr0: str\nr1: maxlen (Vsprintf passes UINT32_MAX for this)\nr2:"
+            " this).\n\nr0: str\nr1: maxlen (vsprintf passes UINT32_MAX for this)\nr2:"
             " format\nr3: ap\nreturn: number of characters printed, excluding the"
             " null-terminator"
         ),
     )
 
-    Vsprintf = Symbol(
+    vsprintf = Symbol(
         None,
         None,
         None,
         (
             "The vsprintf(3) C library function.\n\nr0: str\nr1: format\nr2:"
             " ap\nreturn: number of characters printed, excluding the null-terminator"
         ),
     )
 
-    Snprintf = Symbol(
+    snprintf = Symbol(
         None,
         None,
         None,
         (
-            "The snprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The snprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real snprintf.\n\nr0: str\nr1: n\nr2:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Sprintf = Symbol(
+    sprintf = Symbol(
         None,
         None,
         None,
         (
-            "The sprintf(3) C library function.\n\nThis calls VsprintfInternal"
+            "The sprintf(3) C library function.\n\nThis calls __vsprintf_internal"
             " directly, so it's presumably the real sprintf.\n\nr0: str\nr1:"
             " format\n...: variadic\nreturn: number of characters printed, excluding"
             " the null-terminator"
         ),
     )
 
-    Strlen = Symbol(
+    strlen = Symbol(
         None,
         None,
         None,
         "The strlen(3) C library function.\n\nr0: s\nreturn: length of s",
     )
 
-    Strcpy = Symbol(
+    strcpy = Symbol(
         None,
         None,
         None,
         (
             "The strcpy(3) C library function.\n\nThis function is optimized to copy"
             " characters in aligned 4-byte chunks if possible, correctly handling any"
-            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src"
+            " unaligned bytes at the front/back.\n\nr0: dest\nr1: src\nreturn: dest"
         ),
     )
 
-    Strncpy = Symbol(
+    strncpy = Symbol(
         None,
         None,
         None,
-        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncpy(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcat = Symbol(
-        None, None, None, "The strcat(3) C library function.\n\nr0: dest\nr1: src"
+    strcat = Symbol(
+        None,
+        None,
+        None,
+        "The strcat(3) C library function.\n\nr0: dest\nr1: src\nreturn: dest",
     )
 
-    Strncat = Symbol(
+    strncat = Symbol(
         None,
         None,
         None,
-        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n",
+        "The strncat(3) C library function.\n\nr0: dest\nr1: src\nr2: n\nreturn: dest",
     )
 
-    Strcmp = Symbol(
+    strcmp = Symbol(
         None,
         None,
         None,
         (
-            "The strcmp(3) C library function.\n\nSimilarly to Strcpy, this function is"
+            "The strcmp(3) C library function.\n\nSimilarly to strcpy, this function is"
             " optimized to compare characters in aligned 4-byte chunks if"
             " possible.\n\nr0: s1\nr1: s2\nreturn: comparison value"
         ),
     )
 
-    Strncmp = Symbol(
+    strncmp = Symbol(
         None,
         None,
         None,
         (
             "The strncmp(3) C library function.\n\nr0: s1\nr1: s2\nr2: n\nreturn:"
             " comparison value"
         ),
     )
 
-    Strchr = Symbol(
+    strchr = Symbol(
         None,
         None,
         None,
         (
             "The strchr(3) C library function.\n\nr0: string\nr1: c\nreturn: pointer to"
             " the located byte c, or null pointer if no match"
         ),
     )
 
-    Strcspn = Symbol(
+    strcspn = Symbol(
         None,
         None,
         None,
         (
             "The strcspn(3) C library function.\n\nr0: string\nr1: stopset\nreturn:"
             " offset of the first character in string within stopset"
         ),
     )
 
-    Strstr = Symbol(
+    strstr = Symbol(
         None,
         None,
         None,
         (
             "The strstr(3) C library function.\n\nr0: haystack\nr1: needle\nreturn:"
             " pointer into haystack where needle starts, or null pointer if no match"
         ),
     )
 
-    Wcslen = Symbol(
+    wcslen = Symbol(
         None,
         None,
         None,
         "The wcslen(3) C library function.\n\nr0: ws\nreturn: length of ws",
     )
 
-    AddFloat = Symbol(
+    __addsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __addsf3 (not sure which"
             " gcc version), which implements the addition operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a + b"
         ),
     )
 
-    DivideFloat = Symbol(
+    __divsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __divsf3 (not sure which"
             " gcc version), which implements the division operator for IEEE 754"
             " floating-point numbers.\n\nr0: dividend\nr1: divisor\nreturn: dividend /"
             " divisor"
         ),
     )
 
-    FloatToDouble = Symbol(
+    __extendsfdf2 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __extendsfdf2 (not sure"
             " which gcc version), which implements the float to double cast operation"
             " for IEEE 754 floating-point numbers.\n\nr0: float\nreturn: (double)float"
         ),
     )
 
-    FloatToInt = Symbol(
+    __fixsfsi = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __fixsfsi (not sure which"
             " gcc version), which implements the float to int cast operation for IEEE"
             " 754 floating-point numbers. The output saturates if the input is out of"
             " the representable range for the int type.\n\nr0: float\nreturn:"
             " (int)float"
         ),
     )
 
-    IntToFloat = Symbol(
+    __floatsisf = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __floatsisf (not sure"
             " which gcc version), which implements the int to float cast operation for"
             " IEEE 754 floating-point numbers.\n\nr0: int\nreturn: (float)int"
         ),
     )
 
-    UIntToFloat = Symbol(
+    __floatunsisf = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __floatunsisf (not sure"
             " which gcc version), which implements the unsigned int to float cast"
             " operation for IEEE 754 floating-point numbers.\n\nr0: uint\nreturn:"
             " (float)uint"
         ),
     )
 
-    MultiplyFloat = Symbol(
+    __mulsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __mulsf3 (not sure which"
             " gcc version), which implements the multiplication operator for IEEE 754"
             " floating-point numbers."
         ),
     )
 
-    Sqrtf = Symbol(
+    sqrtf = Symbol(
         None, None, None, "The sqrtf(3) C library function.\n\nr0: x\nreturn: sqrt(x)"
     )
 
-    SubtractFloat = Symbol(
+    __subsf3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __subsf3 (not sure which"
             " gcc version), which implements the subtraction operator for IEEE 754"
             " floating-point numbers.\n\nr0: a\nr1: b\nreturn: a - b"
         ),
     )
 
-    DivideInt = Symbol(
+    __divsi3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __divsi3 (not sure which"
             " gcc version), which implements the division operator for signed"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
@@ -6781,39 +6784,39 @@
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
             " (remainder << 32)"
         ),
     )
 
-    DivideUInt = Symbol(
+    __udivsi3 = Symbol(
         None,
         None,
         None,
         (
             "This appears to be the libgcc implementation of __udivsi3 (not sure which"
             " gcc version), which implements the division operator for unsigned"
             " ints.\n\nThe return value is a 64-bit integer, with the quotient"
             " (dividend / divisor) in the lower 32 bits and the remainder (dividend %"
             " divisor) in the upper 32 bits. In accordance with the Procedure Call"
             " Standard for the Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nNote: This function falls through to"
-            " DivideUIntNoZeroCheck.\n\nr0: dividend\nr1: divisor\nreturn: (quotient) |"
-            " (remainder << 32)"
+            " __udivsi3_no_zero_check.\n\nr0: dividend\nr1: divisor\nreturn: (quotient)"
+            " | (remainder << 32)"
         ),
     )
 
-    DivideUIntNoZeroCheck = Symbol(
+    __udivsi3_no_zero_check = Symbol(
         None,
         None,
         None,
         (
-            "Subsidiary function to DivideUInt. Skips the initial check for divisor =="
+            "Subsidiary function to __udivsi3. Skips the initial check for divisor =="
             " 0.\n\nThe return value is a 64-bit integer, with the quotient (dividend /"
             " divisor) in the lower 32 bits and the remainder (dividend % divisor) in"
             " the upper 32 bits. In accordance with the Procedure Call Standard for the"
             " Arm Architecture (see"
             " https://github.com/ARM-software/abi-aa/blob/60a8eb8c55e999d74dac5e368fc9d7e36e38dda4/aapcs32/aapcs32.rst#result-return),"
             " this means that the quotient is returned in r0 and the remainder is"
             " returned in r1.\nThis function appears to only be called"
```

## pmdsky_debug_py/protocol.py

```diff
@@ -3517,210 +3517,210 @@
     ]
 
     FileInit: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Abs: Symbol[
+    abs: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Mbtowc: Symbol[
+    mbtowc: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TryAssignByte: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TryAssignByteWrapper: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Wcstombs: Symbol[
+    wcstombs: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Memcpy: Symbol[
+    memcpy: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Memmove: Symbol[
+    memmove: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Memset: Symbol[
+    memset: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Memchr: Symbol[
+    memchr: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Memcmp: Symbol[
+    memcmp: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    MemsetInternal: Symbol[
+    memset_internal: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    VsprintfInternalSlice: Symbol[
+    __vsprintf_internal_slice: Symbol[
         Optional[List[int]],
         None,
     ]
 
     TryAppendToSlice: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    VsprintfInternal: Symbol[
+    __vsprintf_internal: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Vsprintf: Symbol[
+    vsprintf: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Snprintf: Symbol[
+    snprintf: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Sprintf: Symbol[
+    sprintf: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Strlen: Symbol[
+    strlen: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Strcpy: Symbol[
+    strcpy: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Strncpy: Symbol[
+    strncpy: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Strcat: Symbol[
+    strcat: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Strncat: Symbol[
+    strncat: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Strcmp: Symbol[
+    strcmp: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Strncmp: Symbol[
+    strncmp: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Strchr: Symbol[
+    strchr: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Strcspn: Symbol[
+    strcspn: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Strstr: Symbol[
+    strstr: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Wcslen: Symbol[
+    wcslen: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    AddFloat: Symbol[
+    __addsf3: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    DivideFloat: Symbol[
+    __divsf3: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    FloatToDouble: Symbol[
+    __extendsfdf2: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    FloatToInt: Symbol[
+    __fixsfsi: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    IntToFloat: Symbol[
+    __floatsisf: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    UIntToFloat: Symbol[
+    __floatunsisf: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    MultiplyFloat: Symbol[
+    __mulsf3: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    Sqrtf: Symbol[
+    sqrtf: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    SubtractFloat: Symbol[
+    __subsf3: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    DivideInt: Symbol[
+    __divsi3: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    DivideUInt: Symbol[
+    __udivsi3: Symbol[
         Optional[List[int]],
         None,
     ]
 
-    DivideUIntNoZeroCheck: Symbol[
+    __udivsi3_no_zero_check: Symbol[
         Optional[List[int]],
         None,
     ]
 
 
 class Arm9DataProtocol(Protocol):
     ARM9_HEADER: Symbol[
```

## Comparing `pmdsky_debug_py-6.0.0.dist-info/METADATA` & `pmdsky_debug_py-7.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmdsky-debug-py
-Version: 6.0.0
+Version: 7.0.0
 Summary: pmdsky-debug symbols for Python.
 Author-email: Marco 'Capypara' Köpcke <hello@capypara.de>
 License: MIT
 Project-URL: repository, https://github.com/SkyTemple/pmdsky-debug-py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

