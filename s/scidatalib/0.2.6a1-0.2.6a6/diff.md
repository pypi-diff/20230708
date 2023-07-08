# Comparing `tmp/SciDataLib-0.2.6a1.tar.gz` & `tmp/scidatalib-0.2.6a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SciDataLib-0.2.6a1.tar", max compression
+gzip compressed data, was "scidatalib-0.2.6a6.tar", max compression
```

## Comparing `SciDataLib-0.2.6a1.tar` & `scidatalib-0.2.6a6.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1087 2022-03-04 13:25:49.544908 SciDataLib-0.2.6a1/LICENSE.txt
--rw-r--r--   0        0        0     8159 2022-03-04 13:25:49.544908 SciDataLib-0.2.6a1/README.md
--rw-r--r--   0        0        0      900 2022-03-04 13:25:49.544908 SciDataLib-0.2.6a1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-03-04 13:25:49.544908 SciDataLib-0.2.6a1/scidatalib/__init__.py
--rw-r--r--   0        0        0     1133 2022-03-04 13:25:49.544908 SciDataLib-0.2.6a1/scidatalib/cli.py
--rw-r--r--   0        0        0       72 2022-03-04 13:25:49.544908 SciDataLib-0.2.6a1/scidatalib/io/__init__.py
--rw-r--r--   0        0        0     1272 2022-03-04 13:25:49.544908 SciDataLib-0.2.6a1/scidatalib/io/formats.py
--rw-r--r--   0        0        0    43307 2022-03-04 13:25:49.544908 SciDataLib-0.2.6a1/scidatalib/io/jcamp.py
--rw-r--r--   0        0        0    10286 2022-03-04 13:25:49.544908 SciDataLib-0.2.6a1/scidatalib/io/rruff.py
--rw-r--r--   0        0        0    31276 2022-03-04 13:25:49.544908 SciDataLib-0.2.6a1/scidatalib/scidata.py
--rw-r--r--   0        0        0     9299 2022-03-04 13:27:23.012989 SciDataLib-0.2.6a1/setup.py
--rw-r--r--   0        0        0     8986 2022-03-04 13:27:23.013704 SciDataLib-0.2.6a1/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-08 05:17:09.312753 scidatalib-0.2.6a6/LICENSE.txt
+-rw-r--r--   0        0        0     8738 2023-07-08 05:17:09.312753 scidatalib-0.2.6a6/README.md
+-rw-r--r--   0        0        0      928 2023-07-08 05:17:09.312753 scidatalib-0.2.6a6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-08 05:17:09.312753 scidatalib-0.2.6a6/scidatalib/__init__.py
+-rw-r--r--   0        0        0     1133 2023-07-08 05:17:09.312753 scidatalib-0.2.6a6/scidatalib/cli.py
+-rw-r--r--   0        0        0       72 2023-07-08 05:17:09.312753 scidatalib-0.2.6a6/scidatalib/io/__init__.py
+-rw-r--r--   0        0        0     1294 2023-07-08 05:17:09.312753 scidatalib-0.2.6a6/scidatalib/io/formats.py
+-rw-r--r--   0        0        0    43072 2023-07-08 05:17:09.312753 scidatalib-0.2.6a6/scidatalib/io/jcamp.py
+-rw-r--r--   0        0        0    10240 2023-07-08 05:17:09.312753 scidatalib-0.2.6a6/scidatalib/io/rruff.py
+-rw-r--r--   0        0        0    40747 2023-07-08 05:17:09.316753 scidatalib-0.2.6a6/scidatalib/scidata.py
+-rw-r--r--   0        0        0     9570 1970-01-01 00:00:00.000000 scidatalib-0.2.6a6/PKG-INFO
```

### Comparing `SciDataLib-0.2.6a1/LICENSE.txt` & `scidatalib-0.2.6a6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SciDataLib-0.2.6a1/README.md` & `scidatalib-0.2.6a6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SciDataLib
 
-| Health | Releases |
-|--------|----------|
-| [![GitHub Actions](https://github.com/ChalkLab/SciDataLib/actions/workflows/actions.yml/badge.svg?branch=master)](https://github.com/ChalkLab/SciDataLib/actions/workflows/actions.yml) | [![PyPI version](https://badge.fury.io/py/scidatalib.svg)](https://badge.fury.io/py/SciDataLib) |
-| [![codecov](https://codecov.io/gh/ChalkLab/SciDataLib/branch/master/graph/badge.svg)](https://codecov.io/gh/ChalkLab/SciDataLib) | [![DOI](https://zenodo.org/badge/219040010.svg)](https://zenodo.org/badge/latestdoi/219040010) |
+| Health                                                                                                                                                                                  | Releases                                                                                        |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
+| [![GitHub Actions](https://github.com/ChalkLab/SciDataLib/actions/workflows/actions.yml/badge.svg?branch=main)](https://github.com/ChalkLab/SciDataLib/actions/workflows/actions.yml) | [![PyPI version](https://badge.fury.io/py/scidatalib.svg)](https://badge.fury.io/py/SciDataLib) |
+| [![codecov](https://codecov.io/gh/ChalkLab/SciDataLib/branch/main/graph/badge.svg)](https://codecov.io/gh/ChalkLab/SciDataLib)                                                        | [![DOI](https://zenodo.org/badge/219040010.svg)](https://zenodo.org/badge/latestdoi/219040010)  |
 
 A Python library writing [SciData](http://stuchalk.github.io/scidata/) [JSON-LD](https://json-ld.org/) files.
 
 # SciData and JSON-LD
 
 JSON-LD is a convenient (human-readable) encoding of Resource
-Desctiption Framework (RDF) triples.  However, unlike traditional
+Description Framework (RDF) triples.  However, unlike traditional
 relational databases (e.g., MySQL), the graph has no schema. This
 is problematic as including data from different sources results
 in a system with no common way to search across the data.  The
 SciData framework is a structure for users to add data and its metadata
 that are organized in the graph through the associated SciData ontology.
 
 There are three main sections of the SciData framework:
@@ -53,16 +53,16 @@
     {
       "sci": "https://stuchalk.github.io/scidata/ontology/scidata.owl#"
     },
     {
       "@base": "https://my.research.edu/<uniqueid>/"
     }
   ],
-  "@id": "file_identifier",
-  "generatedAt": "<automatically added",
+  "@id": "graph name",
+  "generatedAt": "<automatically added>",
   "version": "1",
   "@graph": {
     "@id": "https://my.research.edu/<uniqueid>/",
     "@type": "sdo:scidataFramework",
     "uid": "<uniqueid>",
     "scidata": {
       "@type": "sdo:scientificData",
@@ -185,18 +185,18 @@
   "@context": [
     "https://stuchalk.github.io/scidata/contexts/scidata.jsonld",
     {
       "sci": "https://stuchalk.github.io/scidata/ontology/scidata.owl#",
       "sub": "https://stuchalk.github.io/scidata/ontology/substance.owl#",
       "chm": "https://stuchalk.github.io/scidata/ontology/chemical.owl#",
       "w3i": "https://w3id.org/skgo/modsci#",
-      "qudt": "http://qudt.org/vocab/unit/",
+      "qudt": "https://qudt.org/vocab/unit/",
       "obo": "http://purl.obolibrary.org/obo/",
-      "dc": "http://purl.org/dc/terms/",
-      "xsd": "http://www.w3.org/2001/XMLSchema#"
+      "dc": "https://purl.org/dc/terms/",
+      "xsd": "https://www.w3.org/2001/XMLSchema#"
     },
     {
       "@base": "https://scidata.unf.edu/chalk:example:jsonld/"
     }
   ],
   "@id": "",
   "generatedAt": "",
```

### Comparing `SciDataLib-0.2.6a1/pyproject.toml` & `scidatalib-0.2.6a6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SciDataLib"
-version = "0.2.6-alpha.1"
+version = "v0.2.6-alpha.6"
 description = "Python library for development of SciData JSON-LD files"
 authors = [
     "Stuart Chalk <schalk@unf.edu>",
     "Dylan Johnson <n01448636@unf.edu>",
     "Marshall McDonnell <mcdonnellmt@ornl.gov>"
 ]
 license = "MIT"
@@ -18,18 +18,19 @@
     "Operating System :: OS Independent"
 ]
 
 [tool.poetry.scripts]
 scidatalib = "scidatalib.cli:cli"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pytest-cov = "^2.11.1"
-numpy = "^1.20.2"
+python = "^3.8"
+numpy = "^1.22.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-flake8 = "^3.8.4"
+[tool.poetry.group.dev.dependencies]
+autopep8 = "^1.7.0"
+flake8 = "^5.0.4"
+pytest = "^7.2.0"
+pytest-cov = "^4.0.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `SciDataLib-0.2.6a1/scidatalib/cli.py` & `scidatalib-0.2.6a6/scidatalib/cli.py`

 * *Files identical despite different names*

### Comparing `SciDataLib-0.2.6a1/scidatalib/io/formats.py` & `scidatalib-0.2.6a6/scidatalib/io/formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 class UnknownFileTypeError(Exception):
     pass
 
 
 ioformats = {
     'jcamp': 'jcamp',
+    'rruff': 'rruff',
 }
 
 
 def _get_ioformat(name: str) -> types.ModuleType:
     if name not in ioformats:
         raise UnknownFileTypeError(name)
     module = _MODULE_BASE + ioformats[name]
```

### Comparing `SciDataLib-0.2.6a1/scidatalib/io/jcamp.py` & `scidatalib-0.2.6a6/scidatalib/io/jcamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 
 class MultiHeaderKeyException(Exception):
     """Exception for finding multiple header keys in a single line"""
 
 
 # Compression encoding dictionaries for JCAMP
-# Reference found on following site under "Compression Table"
+# Reference: found on following site under "Compression Table"
 #   - http://wwwchem.uwimona.edu.jm/software/jcampdx.html
 
 # Represents the value with a preceding space (compresses whitespace)
 SQZ_digits = {
     '@': '+0',
     'A': '+1',
     'B': '+2',
@@ -153,34 +153,34 @@
 
 def write_jcamp(filename: str, scidata: SciData):
     """
     Writer for SciData object to JCAMP-DX files.
     JCAMP-DX is Joint Committee on Atomic and Molecular Physical Data eXchange
     JCAMP-DX URL:  http://jcamp-dx.org/
 
-    :param filename: Filename for JCAMP-DX file
-    :param scidata: SciData object to write out
+    param filename: Filename for JCAMP-DX file
+    param scidata: SciData object to write out
     """
     _write_jcamp_header_section(filename, scidata, mode='w')
     _write_jcamp_data_section(filename, scidata, mode='a')
     with open(filename, 'a') as fileobj:
         fileobj.write('##END=\n')
 
 
 def _reader_is_float(strings: List[str]) -> bool:
-    '''
+    """
     Test if a string, or list of strings, contains a numeric value(s).
 
-    :param strings: The string or list of strings to test.
-    :return: Single boolean or list of boolean values indicating whether
-        each input can be converted into float.
-    :raises TypeError: If passing a list and elements are not strings or
-        single element is not a string
-    :raises ValueError: If passing empty list
-    '''
+    param strings: The string or list of strings to test.
+    return: Single boolean or list of boolean values indicating
+        whether each input can be converted into float.
+    raises TypeError: If passing a list and elements are not
+        strings or single element is not a string
+    raises ValueError: If passing empty list
+    """
     if isinstance(strings, tuple) or isinstance(strings, list):
         if not all(isinstance(i, str) for i in strings):
             raise TypeError("Input {} not a list of strings".format(strings))
 
         if not strings:
             raise ValueError('Input {} empty'.format(strings))
 
@@ -190,15 +190,15 @@
                 float(strings[i])
             except ValueError:
                 bool_list[i] = False
         return bool_list
 
     else:
         if not isinstance(strings, str):
-            raise TypeError("Input '%s' is not a string" % (strings))
+            raise TypeError("Input '%s' is not a string" % strings)
 
         try:
             float(strings)
             return True
         except ValueError:
             return False
 
@@ -207,23 +207,23 @@
     """
     Parse duplicate character compression for a line (i.e. DUP characters).
     Valid DUP characters are: [S, T, U, V, W, X, Y, Z]
 
     Example: Repeat 9 character 3 times with 'U'
         "9U" == "999"
 
-    Reference found on following site under "Compression Table"
+    Reference: found on following site under "Compression Table"
         - http://wwwchem.uwimona.edu.jm/software/jcampdx.html
 
     :param line: Line in JCAMP-DX file with duplicate characters (DUP)
     :return: Processed line with duplicates added in
     """
     new_line = ""
     for i, char in enumerate(line):
-        if (char in DUP_digits):
+        if char in DUP_digits:
             # Get number of duplicates to multiply by
             # NOTE: subtract one since we will already have one character from
             #       the original one we are duplicating from.
             nduplicates = DUP_digits[char] - 1
             new_line += line[i-1] * nduplicates
         else:
             new_line += char
@@ -233,95 +233,95 @@
 def _read_num_dif_factory(char: str, line: str) -> Tuple[str, bool]:
     """
     Helper utility factory function to
     :func:`_read_parse_dataset_line_single_x_multi_y` to use the current
     character to give the next numeric value  and flag if we are processing
     using DIF compression.
 
-    :param char: Character we are currently processing.
-    :param line: Line we are processing, used for raising exception.
-    :return: Tuple of updated values for numeric character (char)
+    param char: Character we are currently processing.
+    param line: Line we are processing, used for raising exception.
+    return: Tuple of updated values for numeric character (char)
         and DIF flag (bool). Example: ('+1', False)
-    :raises UnkownCharacterException: If we find a character that is neither
-            a valid compression character or number.
+    raises UnkownCharacterException: If we find a character that is
+        neither a valid compression character nor number.
     """
     if char == ' ':
         num = ''
-        DIF = False
+        dif = False
 
     elif char in SQZ_digits:
         num = SQZ_digits[char]
-        DIF = False
+        dif = False
 
     elif char in DIF_digits:
         num = str(DIF_digits[char])
-        DIF = True
+        dif = True
 
     else:
         msg = f"Unknown character {char} encountered in line {line}"
         raise UnknownCharacterException(msg)
 
-    return (num, DIF)
+    return num, dif
 
 
 def _read_parse_dataset_line_single_x_multi_y(line: str) -> List[float]:
     """
     Parse a JCAMP data line when using the format '(X++(Y..Y))',
     where we have one X column and multiple Y columns on one line.
     Handles decoding JCAMP compression encoding.
 
-    Reference found on following site under "Compression Table"
+    Reference: found on following site under "Compression Table"
         - http://wwwchem.uwimona.edu.jm/software/jcampdx.html
 
     :param line: Line from JCAMP for data of '(X++(Y..Y))' format
     :return: List of float values for the line
     :raises UnkownCharacterException: If we find a character that is neither
-        a valid compression character or number.
+        a valid compression character nor number.
     """
     # process the duplicate characters (DUP_digits)
-    DUP_set = set(DUP_digits)
-    if any(char in DUP_set for char in line):
+    dup_set = set(DUP_digits)
+    if any(char in dup_set for char in line):
         line = _read_parse_dataset_duplicate_characters(line)
 
-    DIF = False
+    dif = False
     num = ''
     values = []
     for char in line:
         if char.isdigit() or char == '.':
             num += char
             continue
 
         if num:
             value = float(num)
-            if DIF:
+            if dif:
                 value = float(num) + values[-1]
             values.append(value)
 
-        num, DIF = _read_num_dif_factory(char, line)
+        num, dif = _read_num_dif_factory(char, line)
 
     if num:
         value = float(num)
-        if DIF:
+        if dif:
             value = float(num) + values[-1]
         values.append(value)
     return values
 
 
 def _read_parse_dataset_line(line: str, data_format: str) -> List[float]:
     """
     Parse a data line of the JCAMP-DX file format for the given data format.
     Handles decoding JCAMP compression encoding.
 
-    Reference found on following site under "Compression Table"
+    Reference: found on following site under "Compression Table"
         - http://wwwchem.uwimona.edu.jm/software/jcampdx.html
 
-    :param line: Line in JCAMP-DX file to parse
-    :param data_format: Format of data. Choices: ['(XY..XY)', '(X++(Y..Y))']
+    param line: Line in JCAMP-DX file to parse
+    param data_format: Format of data. Choices: ['(XY..XY)', '(X++(Y..Y))']
 
-    :return: List of float values for the line
+    return: List of float values for the line
     """
     if data_format not in _DATA_FORMATS:
         msg = f'Data format {data_format} not supported type: {_DATA_FORMATS}'
         raise UnsupportedDataTypeConfigException(msg)
 
     if data_format == _DATA_FORMAT_XYXY:
         values = [float(v.strip()) for v in re.split(r"[,;\s]", line) if v]
@@ -334,18 +334,18 @@
 
 
 def _read_parse_header(line: str, datastart: bool) -> Tuple[dict, bool]:
     """
     Parse the header line, returning a dictionary for the key-value found
     and if we are starting into the data section.
 
-    :param line: Line to parse as a JCAMP header
-    :param datastart: Current boolean flag for if we are in a data section
+    param line: Line to parse as a JCAMP header
+    param datastart: Current boolean flag for if we are in a data section
 
-    :return: Tuple of a header dictionary and datastart boolean.
+    return: Tuple of a header dictionary and datastart boolean.
         Dictionary with header keys found.
         Will mostly return a single key-value pair but
         for some will return multiple pairs
 
         Example: A compound file will return the extra
             {'children': []} pair when detected.
 
@@ -374,42 +374,42 @@
             header_dict[key] = int(value)
         elif _reader_is_float(value):
             header_dict[key] = float(value)
         else:
             header_dict[key] = value
 
         # Figure out if we are starting a new data entry
-        if (key in _DATA_XY_TYPES):
+        if key in _DATA_XY_TYPES:
             datastart = True
             header_dict[_DATA_XY_TYPE_KEY] = value
-        elif (key == 'end'):
+        elif key == 'end':
             datastart = True
         elif datastart:
             datastart = False
 
     return header_dict, datastart
 
 
 def _read_parse_header_line(
     line: str, jcamp_dict: dict, datastart: bool = False, last_key: str = None
 ) -> Tuple[dict, bool, str]:
     """
     Parse the JCAMP header line and update the output JCAMP dictionary.
 
-    :param line: Header line to parse
-    :param jcamp_dict: Dictionary currently holding the JCAMP-DX file info
-    :param datastart: Boolean that is True if we are inside a data section,
+    param line: Header line to parse
+    param jcamp_dict: Dictionary currently holding the JCAMP-DX file info
+    param datastart: Boolean that is True if we are inside a data section,
         False if not
-    :param last_key: String to store the last key we parsed from the header
+    param last_key: String to store the last key we parsed from the header
 
-    :return: Tuple of the modified JCAMP dictionary, the updated flag for if
+    return: Tuple of the modified JCAMP dictionary, the updated flag for if
         in a data section and the last key entered used for updating a
         multiline comment in the header.
 
-    :raises MultiHeaderKeyException: If multiple header keys parsed
+    raises MultiHeaderKeyException: If multiple header keys parsed
     """
     output_dict = dict(jcamp_dict)
     header_dict, datastart = _read_parse_header(line, datastart)
 
     # Get the header key, stripping 'children' key if it is a compound file
     remove_keys = (_CHILDREN, _DATA_XY_TYPE_KEY)
     keys = [k for k in header_dict.keys() if k not in remove_keys]
@@ -435,31 +435,31 @@
     x: List[float],
     y: List[float],
     xstart: List[float],
     xnum: List[int]
 ) -> Tuple[List[float], List[float]]:
     """
     Utility function for _reader to format the XY data in a
-    post-process manner after we parse out this data from the file.
+    postprocess manner after we parse out this data from the file.
 
-    :param jcamp_dict: JCAMP dictionary parsed from file
-    :param x: X-axis data
-    :param y: Y-axis data
-    :param xstart: Starting X-axis values for multi-datasets
-    :param xnum: Number of starting X-axis value for multi-datasets
-    :return: Post-processed XY data
+    param jcamp_dict: JCAMP dictionary parsed from file
+    param x: X-axis data
+    param y: Y-axis data
+    param xstart: Starting X-axis values for multi-datasets
+    param xnum: Number of starting X-axis value for multi-datasets
+    return: Post-processed XY data
     """
     if jcamp_dict.get(_DATA_XY_TYPE_KEY) == _DATA_FORMAT_XYYY:
         xstart.append(jcamp_dict['lastx'])
         x = np.array([])
         for n in range(len(xnum)-1):
             dx = (xstart[n+1] - xstart[n]) / xnum[n]
             x = np.append(x, xstart[n]+(dx*np.arange(xnum[n])))
 
-        if (xnum[len(xnum)-1] > 1):
+        if xnum[len(xnum) - 1] > 1:
             numerator = (jcamp_dict['lastx'] - xstart[len(xnum)-1])
             denominator = (xnum[len(xnum)-1] - 1.0)
             dx = numerator / denominator
 
             xnext = xstart[len(xnum)-1]+(dx*np.arange(xnum[len(xnum)-1]))
             x = np.append(x, xnext)
         else:
@@ -467,28 +467,28 @@
 
         y = np.array([float(yval) for yval in y])
 
     else:
         x = np.array([float(xval) for xval in x])
         y = np.array([float(yval) for yval in y])
 
-    if ('xfactor' in jcamp_dict):
+    if 'xfactor' in jcamp_dict:
         x = x * jcamp_dict['xfactor']
-    if ('yfactor' in jcamp_dict):
+    if 'yfactor' in jcamp_dict:
         y = y * jcamp_dict['yfactor']
 
     return x, y
 
 
 def _reader(filehandle: str) -> dict:
     """
     File reader for JCAMP-DX file format
 
-    :param filehandle: JCAMP-DX file to read from
-    :return: Dictionary parsed from JCAMP-DX file
+    param filehandle: JCAMP-DX file to read from
+    return: Dictionary parsed from JCAMP-DX file
     """
     jcamp_dict = dict()
     xstart = []
     xnum = []
     y = []
     x = []
     datastart = False
@@ -507,15 +507,15 @@
         is_compound = _CHILDREN in jcamp_dict
         if is_compound and line.upper().startswith('##TITLE'):
             in_compound_block = True
             compound_block_contents = [line]
             continue
 
         # If we are reading a compound block, collect lines into an array to be
-        # processed by a recursive call this this function.
+        # processed by a recursive call to this function.
         if in_compound_block:
             compound_block_contents.append(line)
 
             # Detect the end of the compound block.
             if line.upper().startswith('##END'):
                 # Process the entire block and put it into the children array.
                 jcamp_dict[_CHILDREN].append(_reader(compound_block_contents))
@@ -556,16 +556,16 @@
 
 
 def _read_get_description(jcamp_dict: dict, keywords: List[str]) -> str:
     """
     Utility function to create a description string from the JCAMP
     dictionary
 
-    :param jcamp_dict: JCAMP-DX dictionary extracted from read
-    :return: String for the description for SciData object
+    param jcamp_dict: JCAMP-DX dictionary extracted from read
+    return: String for the description for SciData object
     """
     description_lines = []
     for key in keywords:
         if key in jcamp_dict:
             value = jcamp_dict.get(key)
             description_lines.append(f'{key.upper()}: {value}')
 
@@ -647,16 +647,16 @@
 
 
 def _read_get_aspects_section(jcamp_dict: dict) -> dict:
     """
     Extract and translate from the JCAMP-DX dictionary the SciData JSON-LD
     'aspects' sub-ection of the 'methodology' section
 
-    :param jcamp_dict: JCAMP-DX dictionary to extract aspects section from
-    :return: The 'aspects' section of SciData JSON-LD methodology
+    param jcamp_dict: JCAMP-DX dictionary to extract aspects section from
+    return: The 'aspects' section of SciData JSON-LD methodology
     """
     measurement = {}
     if "spectrometer/data system" in jcamp_dict:
         measurement = {
             "@id": "measurement/1",
             "@type": "sdo:measurement",
             "techniqueType": "cao:spectroscopy",
@@ -726,35 +726,33 @@
 
     return aspects
 
 
 def _read_get_facets_section(jcamp_dict: dict) -> dict:
     """
     Extract and translate from the JCAMP-DX dictionary the SciData JSON-LD
-    'facets' sub-section of the 'system' section
+    'facets' subsection of the 'system' section
 
-    :param jcamp_dict: JCAMP-DX dictionary to extract facets section from
-    :return: The 'facets' section of SciData JSON-LD from translation
+    param jcamp_dict: JCAMP-DX dictionary to extract facets section from
+    return: The 'facets' section of SciData JSON-LD from translation
     """
     facets = []
 
-    compound_dict = {}
     if "molform" in jcamp_dict or "cas registry no" in jcamp_dict:
         compound_dict = {
             "@id": "compound/1",
             "@type": ["sdo:facet", "sdo:material"],
             "name": jcamp_dict.get("title", "")
         }
         if "molform" in jcamp_dict:
             compound_dict.update({"formula": jcamp_dict.get("molform")})
         if "cas registry no" in jcamp_dict:
             compound_dict.update({"casrn": jcamp_dict.get("cas registry no")})
         facets.append(compound_dict)
 
-    substances_dict = {}
     if "state" in jcamp_dict:
         substances_dict = {
             "@id": "substance/1",
             "@type": ["sdo:constituent"],
             "name": jcamp_dict.get("title", ""),
             "phase": jcamp_dict.get("state", "")
         }
@@ -780,20 +778,20 @@
         facets.append(condition_dict)
 
     return facets
 
 
 def _read_get_datagroup_subsection(jcamp_dict: dict) -> List[dict]:
     """
-    Extract and translate from the JCAMP-DX dictionary the SciData JSON-LD
-    'dataset' section's datagroup
+    Extract and translate from the JCAMP-DX dictionary
+    the SciData JSON-LD 'dataset' section's datagroup
 
-    :param jcamp_dict: JCAMP-DX dictionary to extract
+    param jcamp_dict: JCAMP-DX dictionary to extract
         dataset section's datagroup from
-    :return: The 'dataset' section's datagroup of
+    return: The 'dataset' section's datagroup of
         SciData JSON-LD from translation
     """
     # Convert from JCAMP units -> SciData JSON-LD unitref
     xunits = jcamp_dict.get("xunits", "")
     xunitref = _XUNIT_MAP.get(xunits, "")
     yunitref = jcamp_dict.get("yunits", "")
 
@@ -905,17 +903,17 @@
 
 
 def _read_get_dataseries_subsection(jcamp_dict: dict) -> List[dict]:
     """
     Extract and translate from the JCAMP-DX dictionary the SciData JSON-LD
     'dataset' section's dataseries
 
-    :param jcamp_dict: JCAMP-DX dictionary to extract dataset section's
-        dataseries from
-    :return: The 'dataset' section's dataseries of SciData
+    param jcamp_dict: JCAMP-DX dictionary to extract
+        dataset section's dataseries from
+    return: The 'dataset' section's dataseries of SciData
     """
     xunits = jcamp_dict.get("xunits", "")
     xunitref = _XUNIT_MAP.get(xunits)
 
     dataseries = [
         {
             "@id": "dataseries",
@@ -945,16 +943,16 @@
     return dataseries
 
 
 def _read_translate_jcamp_to_scidata(jcamp_dict: dict) -> SciData:
     """
     Main translation of JCAMP-DX to SciData JSON-LD
 
-    :param jcamp_dict: JCAMP-DX dictionary extracted from read
-    :return: SciData object from translation
+    param jcamp_dict: JCAMP-DX dictionary extracted from read
+    return: SciData object from translation
     """
     scidata = SciData(_SCIDATA_UID)
 
     # Add champ namespace for aspect techniqueType
     cao = {"cao": "http://champ-project.org/images/ontology/cao.owl#"}
     scidata.namespaces(cao)
 
@@ -1019,17 +1017,17 @@
 
 
 def _write_extract_description_section(description: str, key: str) -> str:
     """
     Given a description string of the form "KEY1: VALUE1, KEY2: VALUE2, ..."
     extract the KEY that matches input key and extract the VALUE
 
-    :param desc: The description of form "KEY1: VALUE1, KEY2: VALUE2, ..."
-    :param key: The key used to extract value from the description
-    :return: String of the VALUE extracted from description for the key
+    param desc: The description of form "KEY1: VALUE1, KEY2: VALUE2, ..."
+    param key: The key used to extract value from the description
+    return: String of the VALUE extracted from description for the key
         provided. None is returned if key is not in the description.
     """
     desc_list = description.split(_DESCRIPTION_KEY_SPLIT_CHAR)
     results = [x for x in desc_list if x.strip().startswith(key)]
     if not results:
         return None
     element = results[0]
@@ -1038,22 +1036,21 @@
 
 
 def _write_add_header_lines_general(scidata: SciData) -> List[str]:
     """
     Get the general graph header lines from the SciData object
     used to write the JCAMP-DX header lines
 
-    :param scidata: SciData object to write as JCAMP-DX file
-    :return: List of header lines to write to the JCAMP-DX file
+    param scidata: SciData object to write as JCAMP-DX file
+    return: List of header lines to write to the JCAMP-DX file
     """
     graph = scidata.output.get("@graph")
     description = graph.get("description", "")
     jcamp_dx = _write_extract_description_section(description, "JCAMP-DX")
-    lines = []
-    lines.append(f'##JCAMP-DX={jcamp_dx}')
+    lines = [f'##JCAMP-DX={jcamp_dx}']
     if "property" in graph["scidata"]:
         lines.append(f'##DATA TYPE={graph["scidata"]["property"][0]}')
     if "publisher" in graph:
         lines.append(f'##ORIGIN={graph["publisher"]}')
     if "authors" in graph:
         lines.append(f'##OWNER={graph["authors"][0]["name"]}')
 
@@ -1097,16 +1094,16 @@
 
 
 def _write_add_header_lines_methodology(scidata: SciData) -> List[str]:
     """
     Get the methodology header lines from the SciData object
     used to write the JCAMP-DX header lines
 
-    :param scidata: SciData object to write as JCAMP-DX file
-    :return: List of header lines to write to the JCAMP-DX file
+    param scidata: SciData object to write as JCAMP-DX file
+    return: List of header lines to write to the JCAMP-DX file
     """
     lines = []
     graph = scidata.output.get("@graph")
     methodology = graph.get("scidata").get("methodology")
 
     # Aspects
     aspects = methodology.get("aspects")
@@ -1144,16 +1141,16 @@
 
 
 def _write_add_header_lines_system(scidata: SciData) -> List[str]:
     """
     Get the system header lines from the SciData object
     used to write the JCAMP-DX header lines
 
-    :param scidata: SciData object to write as JCAMP-DX file
-    :return: List of header lines to write to the JCAMP-DX file
+    param scidata: SciData object to write as JCAMP-DX file
+    return: List of header lines to write to the JCAMP-DX file
     """
     lines = []
     graph = scidata.output.get("@graph")
     system = graph.get("scidata").get("system", False)
 
     # Facets
     if system:
@@ -1184,34 +1181,31 @@
 
 
 def _write_add_header_lines_dataset(scidata: SciData) -> List[str]:
     """
     Get the dataset header lines from the SciData object
     used to write the JCAMP-DX header lines
 
-    :param scidata: SciData object to write as JCAMP-DX file
+    param scidata: SciData object to write as JCAMP-DX file
 
-    :return: List of header lines to write to the JCAMP-DX file
+    return: List of header lines to write to the JCAMP-DX file
     """
     lines = []
 
     graph = scidata.output.get("@graph")
     dataset = graph.get("scidata").get("dataset", False)
 
     if dataset:
         datagroup = dataset.get("datagroup")[0]
         attributes = datagroup.get("attribute", False)
 
         reverse_xunit_map = {v: k for k, v in _XUNIT_MAP.items()}
         scidata_xunits = attributes[0]["value"]["unitref"]
         xunits = reverse_xunit_map[scidata_xunits]
 
-        scidata_yunits = attributes[0]["value"]["unitref"]
-        yunits = scidata_yunits
-
         npoints = attributes[0]["value"]["number"]
 
         first_x = attributes[1]["value"]["number"]
         last_x = attributes[2]["value"]["number"]
         min_x = attributes[3]["value"]["number"]
         max_x = attributes[4]["value"]["number"]
         xfactor = attributes[5]["value"]["number"]
@@ -1248,17 +1242,17 @@
 def _write_jcamp_header_section(
     filename: str, scidata: SciData, mode: str = 'w'
 ):
     """
     Writes header of the JCAMP-DX file for given SciData object
     to the filename provided. Default mode is to overwrite the file.
 
-    :param filename: String name of file to write JCAMP header
-    :param scidata: SciData object to extract header info
-    :param mode: File mode to use (i.e. 'w' for overwrite, 'a' for append, ...)
+    param filename: String name of file to write JCAMP header
+    param scidata: SciData object to extract header info
+    param mode: File mode to use (i.e. 'w' for overwrite, 'a' for append, ...)
     """
     lines = []
 
     graph = scidata.output.get("@graph")
     lines.append(f'##TITLE={graph.get("title")}')
 
     headers = [
@@ -1284,18 +1278,18 @@
     precision: int = 3,
     trim: int = None,
 ):
     """
     Writes dataset section of the JCAMP-DX file for given SciData object
     to the filename provided. Default mode is to overwrite the file.
 
-    :param filename: String name of file to write JCAMP header
-    :param scidata: SciData object to extract dataset info
-    :param mode: File mode to use (i.e. 'w' for overwrite, 'a' for append, ...)
-    :param precision: Floating point number for formatting the output data
+    param filename: String name of file to write JCAMP header
+    param scidata: SciData object to extract dataset info
+    param mode: File mode to use (i.e. 'w' for overwrite, 'a' for append, ...)
+    param precision: Floating point number for formatting the output data
     """
 
     dataset = scidata.output.get("@graph").get("scidata").get("dataset")
     dataseries = dataset.get("dataseries")[0]
     parameters = dataseries.get("parameter")
     with open(filename, mode) as fileobj:
         xdata = []
```

### Comparing `SciDataLib-0.2.6a1/scidatalib/io/rruff.py` & `scidatalib-0.2.6a6/scidatalib/io/rruff.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 
 def read_rruff(filename: str) -> dict:
     """
     Reader for RRUFF database files to SciData object
     RRUFF file format is a modified version of JCAMP, so re-use jcamp module
 
-    :param filename: Filename to read from for RRUFF files
-    :return: SciData object read in from RRUFF file
+    param filename: Filename to read from for RRUFF files
+    return: SciData object read in from RRUFF file
     """
     with open(filename, "r") as fileobj:
         rruff_dict = _reader(fileobj)
     scidata = _read_translate_rruff_to_scidata(rruff_dict)
     return scidata
 
 
@@ -42,16 +42,16 @@
         fileobj.write('##END=\n')
 
 
 def _reader(filehandle: TextIO) -> dict:
     """
     File reader for  RRUFF file format
 
-    :param filehandle: RRUFF file to read from
-    :return: Dictionary parsed from RRUFF file
+    param filehandle: RRUFF file to read from
+    return: Dictionary parsed from RRUFF file
     """
     rruff_dict = {}
     y = []
     x = []
     for line in filehandle:
         # Skip blank or comment lines
         if not line.strip():
@@ -67,31 +67,31 @@
                 jcamp._DATA_FORMAT_XYXY)
             x.extend(datavals[0::2])
             y.extend(datavals[1::2])
 
     x = np.array([float(xval) for xval in x])
     y = np.array([float(yval) for yval in y])
 
-    if ("xfactor" in rruff_dict):
+    if "xfactor" in rruff_dict:
         x = x * rruff_dict["xfactor"]
-    if ("yfactor" in rruff_dict):
+    if "yfactor" in rruff_dict:
         y = y * rruff_dict["yfactor"]
 
     rruff_dict['x'] = x
     rruff_dict['y'] = y
     return rruff_dict
 
 
-def _read_get_aspects_section(rruff_dict: dict) -> dict:
+def _read_get_aspects_section(rruff_dict: dict) -> list:
     """
     Extract and translate from the RRUFF dictionary the SciData JSON-LD
-    'aspects' sub-ection of the 'methodology' section
+    'aspects' subsection of the 'methodology' section
 
-    :param rruff_dict: RRUFF dictionary to extract aspects section from
-    :return: The 'aspects' section of SciData JSON-LD methodology
+    param rruff_dict: RRUFF dictionary to extract aspects section from
+    return: The 'aspects' section of SciData JSON-LD methodology
     """
     aspects = []
 
     # Measurement
     measurement = {
         "@id": "measurement/1/",
         "@type": "cao:CAO_000152",
@@ -119,45 +119,45 @@
 
     measurement.update({"settings": settings})
 
     aspects.append(measurement)
     return aspects
 
 
-def _read_get_facets_section(rruff_dict: dict) -> dict:
+def _read_get_facets_section(rruff_dict: dict) -> list:
     """
     Extract and translate from the RRUFF dictionary the SciData JSON-LD
-    'facets' sub-section of the 'system' section
+    'facets' subsection of the 'system' section
 
-    :param rruff_dict: RRUFF dictionary to extract facets section from
-    :return: The 'facets' section of SciData JSON-LD from translation
+    param rruff_dict: RRUFF dictionary to extract facets section from
+    return: The 'facets' section of SciData JSON-LD from translation
     """
-
     facets = []
+
     material = {
         "@id": "material",
         "@type": "sdo:material",
         "name": rruff_dict.get("names", ""),
         "materialType": rruff_dict.get("ideal chemistry", ""),
     }
     facets.append(material)
     return facets
 
 
 def _read_translate_rruff_to_scidata(rruff_dict: dict) -> dict:
     """
     Main translation of RRUFF to SciData object
 
-    :param rruff_dict: RRUFF dictionary extracted from read
-    :return: SciData object from translation
+    param rruff_dict: RRUFF dictionary extracted from read
+    return: SciData object from translation
     """
     scidata = SciData(_SCIDATA_UID)
 
     # Add champ namespace for aspect techniqueType
-    cao = {"cao": "http://champ-project.org/images/ontology/cao.owl#"}
+    cao = {"cao": "https://champ-project.org/images/ontology/cao.owl#"}
     scidata.namespaces(cao)
 
     # Title
     scidata.title(rruff_dict.get("names", ""))
     scidata.publisher(rruff_dict.get("owner", ""))
 
     # Description
@@ -182,23 +182,22 @@
                 "@id": "author/{}".format(len(authors) + 1),
                 "@type": "dc:creator",
                 "name": rruff_dict[author_keyword]
             })
     scidata.author(authors)
 
     # Sources / references
-    sources = []
-    sources.append({
+    sources = [{
         "@id": "source/1/",
         "@type": "dc:source",
         "citation": "Highlights in Mineralogical Crystallography 2015 1-30",
         "reftype": "journal article",
         "doi": "10.1515/9783110417104-003",
         "url": "https://doi.org/10.1515/9783110417104-003"
-    })
+    }]
 
     if "url" in rruff_dict:
         sources.append({
                 "@id": f"source/{len(sources) + 1}",
                 "@type": "dc:source",
                 "citation": "RRUFF project database entry",
                 "url": f'https://{rruff_dict.get("url")}',
@@ -226,32 +225,32 @@
     return scidata
 
 
 def _write_get_ideal_chemistry(scidata: SciData) -> str:
     """
     Extract ideal chemistry from SciData object
 
-    :param scidata: SciData object
-    :return: The ideal chemistry if exists in SciData object, None otherwise
+    param scidata: SciData object
+    return: The ideal chemistry if exists in SciData object, None otherwise
     """
     chemistry = None
     graph = scidata.output.get("@graph")
     system = graph.get('scidata').get('system')
     for facet in system.get('facets'):
         if facet.get('@id').startswith('material'):
             chemistry = facet.get('materialType')
     return chemistry
 
 
 def _write_get_laser_wavelength(scidata: SciData) -> str:
     """
     Extract laser wavelength from SciData object
 
-    :param scidata: SciData object
-    :return: The laser wavelength if exists in SciData object, None otherwise
+    param scidata: SciData object
+    return: The laser wavelength if exists in SciData object, None otherwise
     """
     laser_wavelength = None
     graph = scidata.output.get("@graph")
     methodology = graph.get('scidata').get('methodology')
     for aspect in methodology.get('aspects'):
         if aspect.get('@id').startswith('measurement'):
             settings = aspect.get('settings')
@@ -262,32 +261,32 @@
     return laser_wavelength
 
 
 def _write_get_rruff_url(scidata: SciData) -> str:
     """
     Extract RRUFF URL from SciData object
 
-    :param scidata: SciData object
-    :return: The RRUFF URL if exists in SciData object, None otherwise
+    param scidata: SciData object
+    return: The RRUFF URL if exists in SciData object, None otherwise
     """
     url = None
     graph = scidata.output.get("@graph")
     sources = graph.get('sources')
     for source in sources:
         if source.get('url').startswith('https://rruff.info'):
             url = source.get('url').strip('https://')
     return url
 
 
 def _write_get_header_section(scidata: SciData) -> str:
     """
     Get the header lines section for RRUFF file from SciData object
 
-    :param scidata: SciData object
-    :return: List of lines to write for the RRUFF header section
+    param scidata: SciData object
+    return: List of lines to write for the RRUFF header section
     """
     lines = []
 
     graph = scidata.output.get("@graph")
     lines.append(f'##NAMES={graph.get("title")}')
 
     rruffid = graph.get("uid").strip("rruff:")
@@ -335,15 +334,15 @@
 def _write_rruff_header_section(
     filename: str, scidata: SciData, mode: str = 'w'
 ):
     """
     Writes RRUFF file header to filename using the SciData object.
     Can optionally change the mode of how to open the file.
 
-    :param filename: Name of the RRUFF file to write
-    :param scidata: SciData object to write as RRUFF file
-    :param mode: File mode. Default is 'w'.
+    param filename: Name of the RRUFF file to write
+    param scidata: SciData object to write as RRUFF file
+    param mode: File mode. Default is 'w'.
     """
     lines = _write_get_header_section(scidata)
     with open(filename, mode) as fileobj:
         for line in lines:
             fileobj.write(line)
```

### Comparing `SciDataLib-0.2.6a1/scidatalib/scidata.py` & `scidatalib-0.2.6a6/scidatalib/scidata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Python library for writing SciData JSON-LD files"""
 from datetime import datetime
 
 
+# noinspection PyTypeChecker
 class SciData:
     """
     This class is used to create and populate a SciData object, to be
     output as a SciData JSON-LD document
 
     A SciData object is created by calling the SciData class
     i.e. SciDataObject = SciData(<uid>)
@@ -14,195 +15,251 @@
     the JSON-LD document. Class methods are called to populate the meta keys
     """
 
     def __init__(self, uid: str):
         """Initialize the instance using a unique id"""
 
         self.meta = {
-            "@context": [],
-            "@id": "",
-            "generatedAt": "",
-            "version": "",
+            "@context": [
+                "https://stuchalk.github.io/scidata/contexts/scidata.jsonld",  # noqa
+                {"sdo": "https://stuchalk.github.io/scidata/ontology/scidata.owl#"},  # noqa
+                {}
+            ],  # def base
+            "@id": "",  # def docid
+            "generatedAt": "",  # autopopulated
+            "version": "",  # def version
             "@graph": {
-                "@id": "",
+                "@id": "",  # autopopulated
                 "@type": "sdo:scidataFramework",
-                "uid": "",
-                "title": "",
-                "authors": [],
-                "description": "",
-                "publisher": "",
-                "version": "",
-                "keywords": [],
-                "starttime": "",
-                "permalink": "",
-                "related": [],
-                "toc": [],
-                "ids": [],
+                "uid": "",  # def graph_uid
+                "title": "",  # def title
+                "authors": [],  # def author
+                "description": "",  # def description
+                "publisher": "",  # def publisher
+                "version": "",  # def graphversion
+                "keywords": [],  # def keywords
+                "starttime": "",  # def starttime
+                "permalink": "",  # def permalink
+                "related": [],  # def related
+                "toc": [],  # autopopulated
+                "ids": [],  # def ids
                 "scidata": {
                     "@id": "scidata/",
                     "@type": "sdo:scientificData",
-                    "discipline": "",
-                    "subdiscipline": "",
+                    "discipline": "",  # def discipline
+                    "subdiscipline": "",  # def subdiscipline
                     "methodology": {
                         "@id": "methodology/",
                         "@type": "sdo:methodology",
-                        "evaluation": "",
-                        "aspects": []},
+                        "evaluation": "",  # def evaluation
+                        "aspects": []},  # def aspects OR def scidatapacket
                     "system": {
                         "@id": "system/",
                         "@type": "sdo:system",
-                        "facets": []},
+                        "facets": []},  # def facets OR def scidatapacket
                     "dataset": {
                         "@id": "dataset/",
                         "@type": "sdo:dataset",
-                        "scope": ""},
+                        "datapoint": [],  # def datapoint OR def scidatapacket
+                        "scope": ""},  # def scope
                 },
-                "sources": [],
-                "rights": []
-            }
-        }
-        self.contexts = [
-            'https://stuchalk.github.io/scidata/contexts/scidata.jsonld']
-        self.nspaces = {
-            "sdo": "https://stuchalk.github.io/scidata/ontology/scidata.owl#",
-            "w3i": "https://w3id.org/skgo/modsci#",
-            "qudt": "http://qudt.org/vocab/unit/",
-            "obo": "http://purl.obolibrary.org/obo/",
-            "dc": "http://purl.org/dc/terms/",
-            "xsd": "http://www.w3.org/2001/XMLSchema#",
-            "sci": "https://stuchalk.github.io/scidata/ontology/scidata.owl#"
+                "sources": [],  # def sources
+                "rights": []  # def rights
+                }
         }
+        self.contexts = []
+        self.nspaces = {}
         self.baseurl = {}
         self.meta['@graph']['uid'] = uid
         self.uidindex = []
 
     # public class methods
     def context(self, context: [str, list], replace=False) -> list:
         """
         Add to or replace the list of external context files
-        :param context - context URL string or list of context URL strings
-        :param replace - boolean to replace or not the existing data
+
+        :param context: context URL string or list of context URL strings
+        :param replace: boolean to replace or not the existing data
 
         When called, the content URL content of the @context JSON object will
         be replaced or updated with the supplied list of context urls
+
         Example:
-        SciDataObject.context(
-            ['https://stuchalk.github.io/scidata/contexts/scidata.jsonld']
-        )
+
+        .. code-block:: python
+
+            SciDataObject.context(
+            ['https://stuchalk.github.io/scidata/contexts/scidata.jsonld'])
         """
+
         if replace:
+            self.meta['@context'][:-2] = []
             self.contexts = []
             if isinstance(context, str):
                 self.contexts = [context]
             if isinstance(context, list):
                 self.contexts = context
         if not replace:
+            self.contexts += self.meta['@context'][:-2]
             if isinstance(context, str):
                 self.contexts.append(context)
             if isinstance(context, list):
                 self.contexts += context
-        self.contexts = list(set(self.contexts))
+        self.contexts = sorted(list(set(self.contexts)))
         self.__make_context()
         return self.contexts
 
     def namespaces(self, namespaces: dict, replace=False) -> dict:
         """
         Add to or replace the dictionary of namespaces within @context.
         Namespaces are needed for values in a file that reference external
-        resources the define something (vocabulary/taxonomy/ontology entries).
-        :param namespaces - dictionary of namespaces (key->ns, val->URI start)
-        :param replace - boolean to replace or not the existing data
+        resources that define something (vocabulary/taxonomy/ontology entries).
+
+        :param namespaces: dictionary of namespaces (key->ns, val->URI start)
+        :param replace: boolean to replace or not the existing data
 
         When called, the dictionary of namespaces within the @context key
         of the meta variable will be replaced or updated with the supplied
         dictionary of namespaces
+
         Example:
-        SciDataObject.namespaces(
-            {"sci": "https://stuchalk.github.io/scidata/ontology/scidata.owl#"}
-        )
+
+        .. code-block:: python
+
+          SciDataObject.namespaces(
+            {
+              "sdo": "https://stuchalk.github.io/scidata/ontology/scidata.owl#"
+            }
+          )
         """
         if isinstance(namespaces, dict):
             if replace:
+                self.meta['@context'][-2] = {}
                 self.nspaces = {}
                 self.nspaces = namespaces
             if not replace:
+                self.nspaces.update(self.meta['@context'][-2])
                 self.nspaces.update(namespaces)
         self.__make_context()
         return self.nspaces
 
     def base(self, base: str) -> dict:
         """
         Assign the JSON-LD @base URL
         (also defines '@id' under '@graph' for consistency)
         See: https://www.w3.org/TR/json-ld/#base-iri
-        :param base - @base URL for a JSON-LD file
+
+        :param base: @base URL for a JSON-LD file
 
         Defines the base url for all internal unique identifiers
-        (define though '@id's). For consistency, the codes also
-        sets the '@id' field under '@graph' so that all triple
-        subjects are unique and associated with the same graph
+        (defined though '@id' keyword fields). For consistency, the
+        code also sets the '@id' field under '@graph' so that all
+        triple subjects are unique and associated with the same graph
+
         Example:
-        SciDataObject.graph_uid("<uniqueidentifier>")
+
+        .. code-block:: python
+
+            SciDataObject.graph_uid("<uniqueidentifier>")
         """
         if isinstance(base, str):
             if base == "":
                 base = "https://scidata.unf.edu/update_your_base_URL"
             self.baseurl = {"@base": base}
         self.__make_context()
         self.__graphid(base)
         return self.baseurl
 
+    def __make_context(self) -> dict:
+        """
+        Recreates the context when something is added to contexts,
+        namespaces or base. The method is called as part of
+        the contexts, namespaces and base methods.
+        """
+
+        self.contexts += self.meta['@context'][:-2]
+        self.contexts = sorted(list(set(self.contexts)))
+        c = self.contexts
+        self.nspaces.update(self.meta['@context'][-2])
+        n = self.nspaces
+        b = self.baseurl
+        self.meta["@context"] = c + [n, b]
+        return self.meta["@context"]
+
     def docid(self, docid: str) -> dict:
         """
         Assign the document identifier.  This will become the
         graph name if the file is uploaded to a graph database
-        :param docid - the root level @id value
+
+        :param docid: the root level @id value
         """
         if isinstance(docid, str):
             self.meta['@id'] = docid
         return self.meta['@id']
 
     def version(self, version: str) -> dict:
         """
         Assign the version of this file (not the version of the data)
-        :param version - the top level 'version' value
+
+        :param version: the top level 'version' value
         """
         if isinstance(version, str):
             self.meta['version'] = version
         return self.meta['version']
 
     def graph_uid(self, guid: str) -> dict:
         """
         Assign the uid value within the @graph JSON object
-        :param guid - the @graph uid value
+
+        :param guid: the @graph uid value
 
         Normally the same as the unique id used in the @graph @id
         value and used to easily find the data in a file system.
+
         Example:
-        SciDataObject.graph_uid("<uniqueidentifier>")
+
+        .. code-block:: python
+
+            SciDataObject.graph_uid("<uniqueidentifier>")
         """
         if isinstance(guid, str):
             self.meta['@graph']['uid'] = guid
         return self.meta['@graph']['uid']
 
     def author(self, authors: list, replace=False) -> list:
         """
         Add to or replace the list of authors within the @graph authors section
-        :param authors - list of names, or list of dicts with multiple fields
-        :param replace - boolean to replace or not the existing data
+
+        :param authors: list of names, or list of dicts with multiple fields
+        :param replace: boolean to replace or not the existing data
+
         Add the list of authors of a set of data with the following defined
         fields in the SciData context file: name, address, organization,
-        email, orcid. Expects either:
+        email, orcid.
+
+        Expects either:
+
         1)  a list of dictionaries where each dictionary contains
-            at minimum of a key that is 'name'
-            Example:
+        at minimum of a key that is 'name'
+
+        Example:
+
+        .. code-block:: python
+
+            SciDataObject.author(
             [{'name': 'George Washington', 'ORCID': 1},
-             {'name': 'John Adams', 'ORCID': 2}]
+            {'name': 'John Adams', 'ORCID': 2}])
+
         2)  a list of strings which are author names
-            Example: ['George Washington', 'John Adams']
+
+        Example:
+
+        .. code-block:: python
+
+            SciDataObject.author(['George Washington', 'John Adams'])
         """
         if isinstance(authors, list):
             a = []
             if not replace:
                 a += self.meta['@graph']['authors']
             for au in authors:
                 auth = {'@id': ('author/' + str(len(a) + 1) + '/')}
@@ -215,74 +272,97 @@
                 a.append(auth)
             self.meta['@graph']['authors'] = a
         return self.meta['@graph']['authors']
 
     def title(self, title: str) -> str:
         """
         Used to create or replace title key within @graph
-        :param title - descriptive title of the dataset
+
+        :param title: descriptive title of the dataset
 
         For a data source such as a journal article, this would
         typically be the title of the article
+
         Example:
-        SciDataObject.title("The Hitchhiker's Guide to the Galaxy")
+
+        .. code-block:: python
+
+            SciDataObject.title("The Hitchhiker's Guide to the Galaxy")
         """
         if isinstance(title, str):
             self.meta['@graph']['title'] = title
         return self.meta['@graph']['title']
 
     def description(self, description: str) -> str:
         """
         Assign the description field within @graph
-        :param description - textual description of the dataset
+
+        :param description: textual description of the dataset
 
         Used as a brief description of the type of data. For a
         journal article, this might house the abstract
+
         Example:
-        SciDataObject.description('a brief description')
+
+        .. code-block:: python
+
+            SciDataObject.description('a brief description')
         """
         if isinstance(description, str):
             self.meta['@graph']['description'] = description
         return self.meta['@graph']['description']
 
     def publisher(self, publisher: str) -> str:
         """
         Assign the publisher field within @graph
         :param publisher - the name or title of the publisher of the data
 
         This is a person, project, research group, organization etc.
+
         Example:
-        SciDataObject.publisher('The Daily Prophet')
+
+        .. code-block:: python
+
+            SciDataObject.publisher('The Daily Prophet')
         """
         if isinstance(publisher, str):
             self.meta['@graph']['publisher'] = publisher
         return self.meta['@graph']['publisher']
 
     def graphversion(self, version: str) -> str:
         """
         Assign the data version
-        :param version - the version assigned to the data
+
+        :param version: the version assigned to the data
 
         If a version is not available, the date it was accessed online
         can be used to indicate the 'state' of the data as downloaded
+
         Example:
-        SciDataObject.graphversion('ChEMBL database v28')
+
+        .. code-block:: python
+
+            SciDataObject.graphversion('ChEMBL database v28')
         """
         if isinstance(version, str):
             self.meta['@graph']['version'] = version
         return self.meta['@graph']['version']
 
     def keywords(self, keywords: [str, list], replace=False) -> list:
         """
         Add to or replace the keywords of the instance
-        :param keywords - important keywords to improve data findability
-        :param replace - boolean to replace or not the existing data
+
+        :param keywords: important keywords to improve data findability
+        :param replace: boolean to replace or not the existing data
 
         Example:
-        SciDataObject.keywords('important')
+
+        .. code-block:: python
+
+            SciDataObject.keywords('important')
         """
         keys = []
         if not replace:
             keys = self.meta['@graph']['keywords']
         if isinstance(keywords, str):
             keys.append(keywords)
         elif isinstance(keywords, list):
@@ -290,205 +370,318 @@
         keys.sort()
         self.meta['@graph']['keywords'] = keys
         return self.meta['@graph']['keywords']
 
     def starttime(self, stime: str) -> str:
         """
         Assign the start time
-        :param stime - datetime string
+
+        :param stime: datetime string
 
         Typically in "%m-%d-%y %H:%M:%S" format
+
         Example:
-        SciDataObject.starttime('04-05-21 06:14:53')
+
+        .. code-block:: python
+
+            SciDataObject.starttime('04-05-21 06:14:53')
         """
         if isinstance(stime, str):
             self.meta['@graph']['starttime'] = stime
         return self.meta['@graph']['starttime']
 
     def permalink(self, link: str) -> dict:
         """
         Assign the document permanent link
-        :param link - URL to the location where this document can be found
+
+        :param link: URL to the location where this document can be found
 
         Example:
-        SciDataObject.permalink('https://permanent.link.com/data1')
+
+        .. code-block:: python
+
+            SciDataObject.permalink('https://permanent.link.com/data1')
         """
         if isinstance(link, str):
             self.meta['@graph']['permalink'] = link
         return self.meta['@graph']['permalink']
 
     def related(self, related: [str, list], replace=False) -> list:
         """
         Add to or replace the related URLs
-        :param related - URLs to other data related to this dataset
-        :param replace - boolean to replace or not the existing data
+
+        :param related: URLs to other data related to this dataset
+        :param replace: boolean to replace or not the existing data
 
         Example:
-        SciDataObject.related('http://example.com/greatdata.jsonld')
+
+        .. code-block:: python
+
+            SciDataObject.related('https://example.com/greatdata.jsonld')
         """
         rels = []
         if not replace:
             rels = self.meta['@graph']['related']
         if isinstance(related, str):
             rels.append(related)
         elif isinstance(related, list):
             rels += related
         self.meta['@graph']['related'] = rels
         return self.meta['@graph']['related']
 
     def ids(self, ids: [str, list]) -> list:
         """
         Add to the ids list
-        :param ids - string or list of strings that are external
-        references to ontological concepts
+
+        :param ids: string or list of strings that are
+         external references to ontological concepts
 
         When called the contents of 'ids' is added to the ids list.
         Note that when the output function is called it iterates
         over instance content to find any values that are ontological
         references, in the format "<namespace>:<uniquevalue>", and
         adds them to ids. Only ids provided in this format will be added
         and duplicates are ignored. Remember to add namespaces for ids.
-        Example
-        SciDataObject.ids(['chebi:00001','qudt:GM'])
+
+        Example:
+
+        .. code-block:: python
+
+            SciDataObject.ids(['chebi:00001','qudt:GM'])
+
         (requires the addition of the 'chebi' namespace)
         """
         curr_ids = self.meta['@graph']['ids']
         if isinstance(ids, list):
             for idee in ids:
                 if ':' in idee:
                     if idee.split(':')[0] not in self.nspaces.keys():
-                        print('Namespace ' + idee.split(':')[0] + ' not set')
+                        print('Note: Namespace <'
+                              + idee.split(':')[0]
+                              + "> not set. A crosswalk "
+                                "url prefix is likely not "
+                                "matched with it's linked namespace")
                         # raise EnvironmentError
                     curr_ids.append(idee)
         elif isinstance(ids, str):
             if ':' in ids:
                 if ids.split(':')[0] not in self.nspaces.keys():
-                    print('Namespace ' + ids.split(':')[0] +
-                          ' not set ' + str(self.nspaces.keys()))
+                    print('Note: Namespace <' + ids.split(':')[0]
+                          + "> not set. A crosswalk url prefix is "
+                            "likely not matched with it's linked namespace")
                     # raise EnvironmentError
                 curr_ids.append(ids)
         self.meta['@graph']['ids'] = sorted(set(curr_ids))
         return self.meta['@graph']['ids']
 
     def discipline(self, disc: str) -> str:
         """
-        Assign the discipline area of the data
+        Assign the discipline area of the data'
+
         :param disc: a discipline name or identifier (preferred)
 
         Best practice is to use and entry in an ontology,
         i.e. the Modern Science Ontology (https://w3id.org/skgo/modsci#)
+
         Example:
-        SciDataObject.discipline('w3i:Chemistry')
+
+        .. code-block:: python
+
+            SciDataObject.discipline('w3i:Chemistry')
+
+        (requires the addition of the 'w3i' namespace)
         """
         if isinstance(disc, str):
-            self.__addid(disc)
+            if ":" in disc:
+                self.__addid(disc)
             self.meta['@graph']['scidata']['discipline'] = disc
         return self.meta['@graph']['scidata']['discipline']
 
     def subdiscipline(self, subdisc: str) -> str:
         """
         Assign the subdiscipline area of the data
+
         :param subdisc: a subdiscipline name or identifier (preferred)
 
         Best practice is to use and entry in an ontology,
         i.e. the Modern Science Ontology (https://w3id.org/skgo/modsci#)
+
         Example:
-        SciDataObject.subdiscipline('w3i:AnalyticalChemistry')
+
+        .. code-block:: python
+
+            SciDataObject.subdiscipline('w3i:AnalyticalChemistry')
         """
         if isinstance(subdisc, str):
-            self.__addid(subdisc)
+            if ":" in subdisc:
+                self.__addid(subdisc)
             self.meta['@graph']['scidata']['subdiscipline'] = subdisc
         return self.meta['@graph']['scidata']['subdiscipline']
 
     def evaluation(self, evaln: str) -> str:
         """
         Assign the evaluation field
+
         :param evaln: the method of evaluation of research data
 
         Recommended values of this field are:
         experimental, theoretical, computational
+
         Example:
-        SciDataObject.evaluation('experimental')
+
+        .. code-block:: python
+
+            SciDataObject.evaluation('experimental')
         """
         if isinstance(evaln, str):
-            self.__addid(evaln)
+            if ":" in evaln:
+                self.__addid(evaln)
             self.meta['@graph']['scidata']['methodology']['evaluation'] = evaln
         return self.meta['@graph']['scidata']['methodology']['evaluation']
 
     def aspects(self, aspects: list) -> list:
-        """Add to or replace the aspects of the file"""
+        """Add to or replace the aspects of the file
+
+        Example:
+
+        .. code-block:: python
+
+            SciDataObject.aspects(
+            [{"@id": "assay",
+             "@type": "sdo:assay",
+             "description": "Inhibition of human ERG "
+                            "by MK499 binding assay",
+             "assay_organism": "Homo sapiens"}])
+
+        Method also accepts keyword '#intlinks'.
+        See documentation for def scidatapackage.
+        """
         new_aspects = []
         scidata: dict = self.meta['@graph']['scidata']
-        meth: dict = scidata['methodology']
-        curr_aspects: list = meth['aspects']
+        methodology: dict = scidata['methodology']
+        curr_aspects: list = methodology['aspects']
         for listentry in aspects:
-            item = self.__iterate_function(listentry)
-            item_noid = {k: item[k] for k in set(list(item.keys())) - {'@id'}}
-            matched_aspect = 0
-            for aspectitem in curr_aspects:
-                aspect_item_noid = {
-                    k: aspectitem[k] for k in set(
-                        list(
-                            aspectitem.keys())) -
-                    {'@id'}}
-                if aspect_item_noid == item_noid:
-                    matched_aspect = aspectitem
-                    # matched_aspect_id = aspectitem['@id']
-            if matched_aspect:
-                new_aspects.append(matched_aspect)
-                self.uidindex.remove(item['@id'])
-            else:
-                new_aspects.append(item)
-                curr_aspects.append(item)
-
-        meth['aspects'] = curr_aspects
-        scidata['methodology'] = meth
+            intlinklist = None
+            if '#intlinks' in listentry.keys():
+                intlinklist = listentry.pop('#intlinks')
+            rootitem = self.__iterate_function(listentry)
+            rootitemid = rootitem['@id']
+            itemlist = [rootitem]
+            if intlinklist:
+                for intlinkentry in intlinklist:
+                    intitem = (self.__iterate_function(intlinkentry))
+                    intitem.update({'aspects#': [rootitemid]})
+                    itemlist.append(intitem)
+            for n, item in enumerate(itemlist):
+                item_noid = {k: item[k] for k in
+                             set(list(item.keys())) - {'@id'} - {'aspects#'}}
+                matched_aspect = 0
+                for aspectitem in curr_aspects:
+                    aspect_item_noid = {
+                        k: aspectitem[k] for k in
+                        set(list(aspectitem.keys())) - {'@id'} - {'aspects#'}}
+                    if aspect_item_noid == item_noid:
+                        if n == 0:
+                            rootitemid = aspectitem['@id']
+                        if aspectitem.get('aspects#', None):
+                            item['aspects#'] = [rootitemid]
+                            if item['aspects#'][0] not in \
+                                    aspectitem['aspects#']:
+                                aspectitem['aspects#'] \
+                                    .append(item['aspects#'][0])
+                        matched_aspect = aspectitem
+                if matched_aspect:
+                    self.uidindex.remove(item['@id'])
+                    new_aspects.append(matched_aspect)
+                else:
+                    new_aspects.append(item)
+                    curr_aspects.append(item)
+        methodology['aspects'] = curr_aspects
+        scidata['methodology'] = methodology
         self.meta['@graph']['scidata'] = scidata
         return new_aspects
 
     def facets(self, facets: list) -> list:
-        """Add to or replace the facets of the file"""
+        """Add to or replace the facets of the file
+
+        Example:
+
+        .. code-block:: python
+
+            SciDataObject.facets(
+            [{"@id": "compound",
+            "@type": "sdo:compound",
+            "mw_freebase": "491.52",
+            "full_molformula": "C26H26FN5O4"}])
+
+        Method also accepts keyword '#intlinks'.
+        See documentation for def scidatapackage.
+        """
         new_facets = []
         scidata: dict = self.meta['@graph']['scidata']
         system: dict = scidata['system']
         curr_facets: list = system['facets']
         for listentry in facets:
-            item = self.__iterate_function(listentry)
-            item_noid = {k: item[k] for k in set(list(item.keys())) - {'@id'}}
-            matched_facet = 0
-            for facetitem in curr_facets:
-                facet_item_noid = {
-                    k: facetitem[k] for k in set(
-                        list(
-                            facetitem.keys())) -
-                    {'@id'}}
-                if facet_item_noid == item_noid:
-                    matched_facet = facetitem
-            if matched_facet:
-                new_facets.append(matched_facet)
-                self.uidindex.remove(item['@id'])
-            else:
-                new_facets.append(item)
-                curr_facets.append(item)
+            intlinklist = None
+            if '#intlinks' in listentry.keys():
+                intlinklist = listentry.pop('#intlinks')
+            rootitem = self.__iterate_function(listentry)
+            rootitemid = rootitem['@id']
+            itemlist = [rootitem]
+            if intlinklist:
+                for intlinkentry in intlinklist:
+                    intitem = self.__iterate_function(intlinkentry)
+                    intitem.update({'facets#': [rootitemid]})
+                    itemlist.append(intitem)
+            for n, item in enumerate(itemlist):
+                item_keys = set(list(item.keys()))
+                item_noid = {
+                    k: item[k] for k in item_keys - {'@id'} - {'facets#'}
+                }
+                matched_facet = 0
+                for facetitem in curr_facets:
+                    facet_item_noid = {
+                        k: facetitem[k] for k in
+                        set(list(facetitem.keys())) - {'@id'} - {'facets#'}}
+                    if facet_item_noid == item_noid:
+                        if n == 0:
+                            rootitemid = facetitem['@id']
+                        if facetitem.get('facets#', None):
+                            item['facets#'] = [rootitemid]
+                            facetitem['facets#'].append(item['facets#'][0])
+                            facet_list = list(set(facetitem['facets#']))
+                            facetitem['facets#'] = facet_list
+                        matched_facet = facetitem
+                if matched_facet:
+                    self.uidindex.remove(item['@id'])
+                    new_facets.append(matched_facet)
+                else:
+                    new_facets.append(item)
+                    curr_facets.append(item)
         system['facets'] = curr_facets
         scidata['system'] = system
         self.meta['@graph']['scidata'] = scidata
         return new_facets
 
     def scope(self, scope: [str, list]) -> str:
         """
         Assign what thing(s) the dataset relates to
+
         :param scope: str or list of internal unique id()s of
-        entity(ies) in the system to which the data describes
+         entity(ies) in the system to which the data describes
 
         The scope of a datasets should be described in the 'system' 'facets'
         section, e.g. chemical system, organism, specimen, should be included
         as a scope using the defined unique '@id' for that section
-        Example
-        SciDataObject.scope('chemicalsystem/1/')
+
+        Example:
+
+        .. code-block:: python
+
+            SciDataObject.scope('chemicalsystem/1/')
         """
         if isinstance(scope, str) or isinstance(scope, list):
             self.meta['@graph']['scidata']['dataset']['scope'] = scope
         return self.meta['@graph']['scidata']['dataset']['scope']
 
     def attribute(self, attributes: list) -> list:
         """Add one or more attributes"""
@@ -503,16 +696,15 @@
             item = self.__iterate_function(listentry)
             item_noid = {k: item[k] for k in set(list(item.keys())) - {'@id'}}
             matched_attribute = 0
             for attributeitem in curr_attributes:
                 attribute_item_noid = {
                     k: attributeitem[k] for k in set(
                         list(
-                            attributeitem.keys())) -
-                    {'@id'}}
+                            attributeitem.keys())) - {'@id'}}
                 if attribute_item_noid == item_noid:
                     matched_attribute = attributeitem
             if matched_attribute:
                 new_attributes.append(matched_attribute)
                 self.uidindex.remove(item['@id'])
             else:
                 new_attributes.append(item)
@@ -520,36 +712,48 @@
 
         dataset['attribute'] = curr_attributes
         scidata['dataset'] = dataset
         self.meta['@graph']['scidata'] = scidata
         return new_attributes
 
     def datapoint(self, points: list) -> list:
-        """Add one or more datapoints"""
+        """Add one or more datapoints
+
+        Example:
+
+        .. code-block:: python
+
+            SciDataObject.datapoint(
+            [{"@id": "datapoint",
+             "@type": "sdo:datapoint",
+             "data": [{"@id": "datum",
+                       "@type": "sdo:exptdata",
+                       "type": "IC50",
+                       "value": "15.2",
+                       "units": "uM"}]}])
+
+        """
         new_points = []
         scidata: dict = self.meta['@graph']['scidata']
         dataset: dict = scidata['dataset']
 
-        if 'datapoint' in dataset.keys():
-            curr_points: list = dataset['datapoint']
-        else:
-            curr_points = []
+        curr_points: list = dataset['datapoint']
 
         for listentry in points:
             item = self.__iterate_function(listentry)
             new_points.append(item)
             curr_points.append(item)
 
         dataset['datapoint'] = curr_points
         scidata['dataset'] = dataset
         self.meta['@graph']['scidata'] = scidata
         return new_points
 
     def dataseries(self, series: list) -> list:
-        """Add one or more datapoints"""
+        """Add one or more dataseries"""
         new_series = []
         scidata: dict = self.meta['@graph']['scidata']
         dataset: dict = scidata['dataset']
         if 'dataseries' in dataset.keys():
             curr_series: list = dataset['dataseries']
         else:
             curr_series = []
@@ -557,16 +761,15 @@
             item = self.__iterate_function(listentry)
             item_noid = {k: item[k] for k in set(list(item.keys())) - {'@id'}}
             matched_serie = 0
             for serieitem in curr_series:
                 serie_item_noid = {
                     k: serieitem[k] for k in set(
                         list(
-                            serieitem.keys())) -
-                    {'@id'}}
+                            serieitem.keys())) - {'@id'}}
                 if serie_item_noid == item_noid:
                     matched_serie = serieitem
             if matched_serie:
                 new_series.append(matched_serie)
                 self.uidindex.remove(item['@id'])
             else:
                 new_series.append(item)
@@ -574,15 +777,15 @@
 
         dataset['dataseries'] = curr_series
         scidata['dataset'] = dataset
         self.meta['@graph']['scidata'] = scidata
         return new_series
 
     def datagroup(self, group: list) -> list:
-        """Add one or more datapoints"""
+        """Add one or more datagroups"""
         new_group = []
         scidata: dict = self.meta['@graph']['scidata']
         dataset: dict = scidata['dataset']
         if 'datagroup' in dataset.keys():
             curr_group: list = dataset['datagroup']
         else:
             curr_group = []
@@ -590,16 +793,15 @@
             item = self.__iterate_function(listentry)
             item_noid = {k: item[k] for k in set(list(item.keys())) - {'@id'}}
             matched_group = 0
             for groupitem in curr_group:
                 group_item_noid = {
                     k: groupitem[k] for k in set(
                         list(
-                            groupitem.keys())) -
-                    {'@id'}}
+                            groupitem.keys())) - {'@id'}}
                 if group_item_noid == item_noid:
                     matched_group = groupitem
             if matched_group:
                 new_group.append(matched_group)
                 self.uidindex.remove(item['@id'])
             else:
                 new_group.append(item)
@@ -607,18 +809,74 @@
 
         dataset['datagroup'] = curr_group
         scidata['dataset'] = dataset
         self.meta['@graph']['scidata'] = scidata
         return new_group
 
     def scidatapackage(self, package):
-        """Add a package of data where the datapoints are linked
-            with the associated aspects and facets
-        package = [{'aspects':{},'facets':{},'datapoint':{}},
-            {'aspects':{},'facets':{},'datapoint':{}}]"""
+        """
+        Add a package of data where the datapoints are linked with the
+        associated aspects and facets.
+        A package contains one or more 'packets' of associated aspects,
+        facets and datapoints.
+
+        Template:
+
+        .. code-block:: python
+
+            package = [
+                {'aspects':{},'facets':{},'datapoints':{}},
+                {'aspects':{},'facets':{},'datapoints':{}}
+                ]
+
+        Example:
+
+        .. code-block:: python
+
+          SciDataObject.scidatapackage([{
+            "aspects": [{
+              "@id": "assay/",
+              "@type": "sdo:assay",
+              "description": "Inhibition of human ERG by MK499 binding assay",
+              "assay_organism": "Homo sapiens"
+            }],
+            "facets": [
+              {
+                "@id": "compound/",
+                "@type": "sdo:compound",
+                "mw_freebase": "491.52",
+                "full_molformula": "C26H26FN5O4",
+                "#intlinks": [{
+                  "@id": "identifier/",
+                  "@type": "sdo:identifier",
+                  "standard_inchi_key": "OINHUVBCKUJZAG-UHFFFAOYSA-N"
+                }]
+              },
+              {
+                "@id": "target/",
+                "@type": "sdo:target",
+                "pref_name": "HERG",
+                "tax_id": 9606,
+                "organism": "Homo sapiens"
+              }
+            ],
+            "datapoints": [{
+              "@id": "datapoint/",
+              "@type": "sdo:datapoint",
+              "data":[{
+                "@id": "datum",
+                "@type": "sdo:exptdata",
+                "type": "IC50",
+                "value": "15.2",
+                "units": "uM"
+              }]
+            }]
+          }])
+
+        """
         for packet in package:
             packet['facets'] = self.facets(packet['facets'])
             packet['aspects'] = self.aspects(packet['aspects'])
             atfacet = [a_dict["@id"] for a_dict in packet['facets']]
             ataspect = [a_dict["@id"] for a_dict in packet['aspects']]
             for dp in packet['dataset']:
                 if atfacet:
@@ -626,79 +884,89 @@
                 if ataspect:
                     dp.update({'aspects#': ataspect})
             self.datapoint(packet['dataset'])
 
     def sources(self, sources: list, replace=False) -> dict:
         """
         Add to or replace the source reference list
-        :param sources - information about where the data came from
-        :param replace - boolean to replace or not the existing data
+
+        :param sources: information about where the data came from
+        :type sources: list
+        :param replace: replace (True) or add to the existing sources (False)
+        :type replace: bool (default: False)
 
         Add a list of sources with any of the available defined fields
         in the SciData context file: citation, reftype, url, doi
-        Example
-        SciDataObject.sources([
+
+        Example:
+
+        .. code-block:: python
+
+            SciDataObject.sources([
             {'citation': 'Chalk, S.J. SciData: a data model and
             ontology for semantic representation of scientific data.
             J Cheminform 8, 54 (2016)',
-            'doi': https://doi.org/10.1186/s13321-016-0168-9'}])
+            doi': https://doi.org/10.1186/s13321-016-0168-9'}])
         """
         srcs = []
         if not replace:
             srcs = self.meta['@graph']['sources']
         for x in sources:
             ld = {
                 '@id': 'source/' + str(len(srcs) + 1) + '/',
                 '@type': 'dc:source'
             }
             ld.update(x)
             srcs.append(ld)
         return self.meta['@graph']['sources']
 
-    def rights(self, holder: str, license: str) -> dict:
+    def rights(self, holder: str, lic: str) -> dict:
         """
         Add the rights section to the file (max: 1 entry)
-        :param holder - the entity that holds the license to this data
-        :param license - the assigned license
+
+        :param holder: the entity that holds the license to this data
+        :param lic: the assigned license
+
         """
         rights = []
-        if isinstance(holder, str) and isinstance(license, str):
+        if isinstance(holder, str) and isinstance(lic, str):
             rights = [{
                 '@id': 'rights/1/',
                 '@type': 'dc:rights',
                 'holder': holder,
-                'license': license,
+                'license': lic,
             }]
         self.meta['@graph']['rights'] = rights
         return self.meta['@graph']['rights']
 
     # private class functions
     def __addid(self, text: str) -> bool:
-        """ adds entry to ids list if string contains ':' """
+        """
+        Adds entry to ids list if string contains ':'
+        """
         if isinstance(text, str):
             if '://' in text:
                 return False
             elif len(text.split(':')) > 1:
                 return False
             elif ':' in text:
                 self.ids(text)
                 return True
         else:
             return False
 
     def __graphid(self, gid: str) -> bool:
         """
         Assigns the @id value within the @graph JSON object.
-        Automatically set as the value of the '@base'
         """
         self.meta['@graph']['@id'] = gid
         return True
 
     def __addtoc(self):
-        """ adds entries to the toc list """
+        """ adds entries to the toc list"""
 
         def tocdict(a):
             """ get the @type entry from a dictionary """
             for k, v in a.items():
                 if k == '@type':
                     if isinstance(v, list):
                         self.meta['@graph']['toc'].extend(v)
@@ -724,110 +992,164 @@
                 tocdict(value)
             if isinstance(value, list):
                 toclist(value)
 
         self.meta['@graph']['toc'] = sorted(set(self.meta['@graph']['toc']))
         return
 
-    def __make_context(self) -> dict:
-        """
-        Recreates the context when something is added to contexts,
-        namespaces or base. The method is called as part of
-        the contexts, namespaces and base methods.
-        """
-
-        c = self.contexts
-        n = self.nspaces
-        b = self.baseurl
-        self.meta["@context"] = c + [n, b]
-        return self.meta["@context"]
-
     def __iterate_function(self, it, uid=False):
-
         if isinstance(it, str):
             self.__addid(it)
             return it
+        if isinstance(it, list):
+            if not all(isinstance(item, dict) for item in it):
+                return it
         prev_uid = uid
 
         # Set the category
         if '@id' in it:
             category = it['@id']
-        elif 'descriptors' in it or 'identifiers' in it:
-            category = 'compound'
         else:
             category = 'undefined'
 
         if prev_uid:
             uid = prev_uid + category + '/1/'
         else:
             uid = category + '/1/'
 
-        def enumuid(uid):
-            uidsplit = uid.rsplit('/', 2)
-            uid = uidsplit[0] + '/' + str(int(uidsplit[1]) + 1) + '/'
-            return uid
+        def enumuid(uidstr):
+            """
+            function to create unique internal id ('@id')
+            for each section of the file.
+            """
+            uidsplit = uidstr.rsplit('/', 2)
+            uidstr = uidsplit[0] + '/' + str(int(uidsplit[1]) + 1) + '/'
+            return uidstr
 
         while uid in self.uidindex:
             uid = enumuid(uid)
         self.uidindex.append(uid)
 
         temp: dict = {'@id': uid, '@type': 'sdo:' + category}
-
         for key, value in it.items():
             if key != '@id':
-
                 if isinstance(value, list):
-                    listuid = uid
-                    for i, listentry in enumerate(value):
-                        value[i] = self.__iterate_function(
-                            listentry, listuid)
-                    temp[key] = value
+                    if not all(isinstance(item, dict) for item in value):
+                        temp[key] = value
+                    else:
+                        listuid = uid
+                        for i, listentry in enumerate(value):
+                            value[i] = self.__iterate_function(
+                                listentry, listuid)
+                        temp[key] = value
 
                 elif isinstance(value, dict):
                     temp[key] = self.__iterate_function(
                         value, uid)
 
                 else:
                     temp[key] = value
                     self.__addid(value)
-
         return temp
 
     @property
     def output(self) -> dict:
         """
-        Generates Scidata JSON-LD File
+        Completes and cleans a Scidata Object (instance of this class)
+        before its output.
         """
+
+        # add the generatedAt date
         today = datetime.today()
         self.meta['generatedAt'] = today.strftime("%m-%d-%y %H:%M:%S")
 
-        # clean top level
+        # clean @graph
         for key in list(self.meta['@graph']):
             if not self.meta['@graph'][key]:
                 if key != 'toc':
                     del self.meta['@graph'][key]
+
+        # clean scidata
         for key in list(self.meta['@graph']['scidata']):
-            if not self.meta['@graph']['scidata'][key]:
+            value = self.meta['@graph']['scidata'][key]
+            if not value or value == "":
                 del self.meta['@graph']['scidata'][key]
-        if self.meta['@graph']['scidata'].get('methodology'):
-            if not self.meta['@graph']['scidata'].get(
-                    'methodology',
-                    {}).get(
-                    'aspects',
-                    False):
-                del self.meta['@graph']['scidata']['methodology']
-        if self.meta['@graph']['scidata'].get('system'):
-            if not self.meta['@graph']['scidata'].get(
-                    'system',
-                    {}).get(
-                    'facets',
-                    False):
-                del self.meta['@graph']['scidata']['system']
-        if self.meta['@graph']['scidata'].get('dataset'):
-            if not self.meta['@graph']['scidata'].get(
-                    'dataset', {}).get('datapoint', False):
-                if not self.meta['@graph']['scidata'].get(
-                        'dataset', {}).get('dataseries', False):
-                    del self.meta['@graph']['scidata']['dataset']
+
+        # clean methodology, if exists
+        if 'methodology' in self.meta['@graph']['scidata']:
+            methodology = self.meta['@graph']['scidata']['methodology']
+
+            if methodology.get('aspects', False):
+                for key in list(methodology):
+                    if not methodology[key] or methodology[key] == "":
+                        del methodology[key]
+            else:
+                # as 'aspects' is empty, delete the methodology section
+                del methodology
+
+            # clean system, if exists
+        if 'system' in self.meta['@graph']['scidata']:
+            system = self.meta['@graph']['scidata']['system']
+            if system.get('facets', False):
+                for key in list(system):
+                    if not system[key] or system[key] == "":
+                        del system[key]
+            else:
+                # as 'facets' is empty, delete the system section
+                del system
+
+        # remove data set if not data
+        if 'dataset' in self.meta['@graph']['scidata']:
+            dataset = self.meta['@graph']['scidata']['dataset']
+            if not dataset.get('dataseries', False):
+                if not dataset.get('datagroups', False):
+                    if not dataset.get('datapoints', False):
+                        del dataset
+
+        # clean dataset, if exists
+        if 'dataset' in self.meta['@graph']['scidata']:
+            dataset = self.meta['@graph']['scidata']['dataset']
+            if dataset:
+                for key in list(dataset):
+                    if not dataset[key] or dataset[key] == "":
+                        del dataset[key]
+
+                # clean dataseries
+                if 'dataseries' in dataset.keys():
+                    if dataset.get('dataseries', False):
+                        dataseries = dataset["dataseries"]
+                        for seridx, series in enumerate(dataseries):
+                            for key in list(series):
+                                if not series[key]:
+                                    del dataseries[seridx][key]
+                    else:
+                        # delete if present but empty
+                        del dataseries
+
+                # clean datagroups
+                if 'datagroups' in dataset.keys():
+                    if dataset.get('datagroups', False):
+                        datagroups = dataset["datagroups"]
+                        for grpidx, series in enumerate(datagroups):
+                            for key in list(series):
+                                if not series[key]:
+                                    del datagroups[grpidx][key]
+                    else:
+                        # delete if present but empty
+                        del datagroups
+
+                # clean datapoints
+                if 'datapoints' in dataset.keys():
+                    if dataset.get('datapoints', False):
+                        datapoints = dataset["datapoints"]
+                        for pntidx, series in enumerate(datapoints):
+                            for key in list(series):
+                                if not series[key]:
+                                    del datapoints[pntidx][key]
+                    else:
+                        # delete if present but empty
+                        del datapoints
+
+        # add the toc to the output
         self.__addtoc()
 
         return self.meta
```

### Comparing `SciDataLib-0.2.6a1/setup.py` & `scidatalib-0.2.6a6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,301 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: scidatalib
+Version: 0.2.6a6
+Summary: Python library for development of SciData JSON-LD files
+Home-page: https://github.com/ChalkLab/SciDataLib
+License: MIT
+Keywords: scidata,scidatalib
+Author: Stuart Chalk
+Author-email: schalk@unf.edu
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: numpy (>=1.22.0,<2.0.0)
+Project-URL: Repository, https://github.com/ChalkLab/SciDataLib
+Description-Content-Type: text/markdown
 
-packages = \
-['scidatalib', 'scidatalib.io']
+# SciDataLib
 
-package_data = \
-{'': ['*']}
+| Health                                                                                                                                                                                  | Releases                                                                                        |
+|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
+| [![GitHub Actions](https://github.com/ChalkLab/SciDataLib/actions/workflows/actions.yml/badge.svg?branch=main)](https://github.com/ChalkLab/SciDataLib/actions/workflows/actions.yml) | [![PyPI version](https://badge.fury.io/py/scidatalib.svg)](https://badge.fury.io/py/SciDataLib) |
+| [![codecov](https://codecov.io/gh/ChalkLab/SciDataLib/branch/main/graph/badge.svg)](https://codecov.io/gh/ChalkLab/SciDataLib)                                                        | [![DOI](https://zenodo.org/badge/219040010.svg)](https://zenodo.org/badge/latestdoi/219040010)  |
 
-install_requires = \
-['numpy>=1.20.2,<2.0.0', 'pytest-cov>=2.11.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['scidatalib = scidatalib.cli:cli']}
-
-setup_kwargs = {
-    'name': 'scidatalib',
-    'version': '0.2.6a1',
-    'description': 'Python library for development of SciData JSON-LD files',
-    'long_description': '# SciDataLib\n\n| Health | Releases |\n|--------|----------|\n| [![GitHub Actions](https://github.com/ChalkLab/SciDataLib/actions/workflows/actions.yml/badge.svg?branch=master)](https://github.com/ChalkLab/SciDataLib/actions/workflows/actions.yml) | [![PyPI version](https://badge.fury.io/py/scidatalib.svg)](https://badge.fury.io/py/SciDataLib) |\n| [![codecov](https://codecov.io/gh/ChalkLab/SciDataLib/branch/master/graph/badge.svg)](https://codecov.io/gh/ChalkLab/SciDataLib) | [![DOI](https://zenodo.org/badge/219040010.svg)](https://zenodo.org/badge/latestdoi/219040010) |\n\nA Python library writing [SciData](http://stuchalk.github.io/scidata/) [JSON-LD](https://json-ld.org/) files.\n\n# SciData and JSON-LD\n\nJSON-LD is a convenient (human-readable) encoding of Resource\nDesctiption Framework (RDF) triples.  However, unlike traditional\nrelational databases (e.g., MySQL), the graph has no schema. This\nis problematic as including data from different sources results\nin a system with no common way to search across the data.  The\nSciData framework is a structure for users to add data and its metadata\nthat are organized in the graph through the associated SciData ontology.\n\nThere are three main sections of the SciData framework:\n- the methodology section (describing how the research was done)\n- the system section (describing what the research studied and the conditions)\n- the dataset section (the experimental data, plus any derived or supplemental data)\n\nThe methodology and system sections are generic and users can add any data\nthey need to contextualize the dataset.  However, in addition they must\nprovide a JSON-LD context file to semantically describe the data elements\nincluded.  The dataset section has predefined data structures (dataseries,\ndatagroup, and datapoint) although other strudtures can be included\nif needed.\n\nTranslating the content in JSON-LD.  Referencing the JSON-LD below:\n- \'@context\': provides resources that define the context (meaning) of \n  data elements in the document (as a JSON array). It consists of three sections:\n    - a list of one or more \'context\' files\n    - a JSON object containing one or more definitions of namespaces\n    used in the document\n    - a JSON object with one entry \'@base\' that defines the base URL\n    to be prepended to all internal references (i.e. \'@id\' entries)\n- root level \'@id\': the \'name\' of the file and where ingested into a\ngraph database, the graph name\n- \'@graph\': the definition of content that will be represented as triples\nand identified by the graph name (this is therfore a \'quad\')\n- \'@id\' under \'@graph\': the identifier for the graph.  The scidatalib\ncode uses the \'@base\' to populate this, so they are consistent. As a result,\n  all node identifiers \'@id\'s in the document are globally unique because the\n  \'@base\' is unique.\n\n```json\n{\n  "@context": [\n    "https://stuchalk.github.io/scidata/contexts/scidata.jsonld",\n    {\n      "sci": "https://stuchalk.github.io/scidata/ontology/scidata.owl#"\n    },\n    {\n      "@base": "https://my.research.edu/<uniqueid>/"\n    }\n  ],\n  "@id": "file_identifier",\n  "generatedAt": "<automatically added",\n  "version": "1",\n  "@graph": {\n    "@id": "https://my.research.edu/<uniqueid>/",\n    "@type": "sdo:scidataFramework",\n    "uid": "<uniqueid>",\n    "scidata": {\n      "@type": "sdo:scientificData",\n      "methodology": {\n        "@id": "methodology/",\n        "@type": "sdo:methodology",\n        "aspects": []\n      },\n      "system": {\n        "@id": "system/",\n        "@type": "sdo:system",\n        "facets": []\n      },\n      "dataset": {\n        "@id": "dataset/",\n        "@type": "sdo:dataset",\n        "dataseries": [],\n        "datagroup": [],\n        "datapoint": []\n      }\n    }\n  }\n}\n```\n\n\n# Installation\n\n### Using pip\n```\npip install scidatalib\n```\n\n### Manual (from source)\nClone the repository either via:\n - HTTP:\n```\ngit clone https://github.com/ChalkLab/SciDataLib.git\n```\n - SSH:\n```\ngit clone git@github.com:ChalkLab/SciDataLib.git\n```\n\nCreate a virtual environment and activate to install the package in the isolated environment:\n```\npython -m venv <name of env>\nsource <env>/bin/activate\n```\n\nTo [install the package from the local source tree into the environment](\nhttps://packaging.python.org/tutorials/installing-packages/#installing-from-a-local-src-tree), run:\n```\npython -m pip install .\n```\n\nOr to do so in ["Development Mode"](https://setuptools.readthedocs.io/en/latest/setuptools.html#development-mode), \nyou can run:\n```\npython -m pip install -e .\n```\n\nTo deactivate the virtual environment\n```\ndeactivate\n```\n\nWhen finished, remove the virtual environment by deleting the directory:\n```\nrm -rf <name of env>\n```\n\n# Usage\n\nSciDataLib consists of both a command line interface (CLI)\nand a library for constructing and modifying SciData JSON-LD files\n\n### Command Line Interface\n\nThe CLI tool is `scidatalib`.\nYou can use it to create SciData JSON-LD files\nvia specifying an output JSON-LD filename\nand additional options to create the content of the file.\n\nExample to create "bare" SciData JSON-LD file:\n```\nscidatalib output.jsonld\n```\n\nYou can access the additional functionality via the `--help` option:\n```\nscidatalib --help\n```\n\n### SciDataLib library\nAfter installation, import the `SciData` class to start creating SciData JSON-LD:\n```python\nfrom scidatalib.scidata import SciData\n```\n\nExample:\n```python\nfrom scidatalib.scidata import SciData\nimport json\n\nuid = \'chalk:example:jsonld\'\nexample = SciData(uid)\n\n# context parameters\nbase = \'https://scidata.unf.edu/\' + uid + \'/\'\nexample.base(base)\n\n# print out the SciData JSON-LD for example\nprint(json.dumps(example.output, indent=2))\n```\n\n**Output**:\n```json\n{\n  "@context": [\n    "https://stuchalk.github.io/scidata/contexts/scidata.jsonld",\n    {\n      "sci": "https://stuchalk.github.io/scidata/ontology/scidata.owl#",\n      "sub": "https://stuchalk.github.io/scidata/ontology/substance.owl#",\n      "chm": "https://stuchalk.github.io/scidata/ontology/chemical.owl#",\n      "w3i": "https://w3id.org/skgo/modsci#",\n      "qudt": "http://qudt.org/vocab/unit/",\n      "obo": "http://purl.obolibrary.org/obo/",\n      "dc": "http://purl.org/dc/terms/",\n      "xsd": "http://www.w3.org/2001/XMLSchema#"\n    },\n    {\n      "@base": "https://scidata.unf.edu/chalk:example:jsonld/"\n    }\n  ],\n  "@id": "",\n  "generatedAt": "",\n  "version": "",\n  "@graph": {\n    "@id": "",\n    "@type": "sdo:scidataFramework",\n    "uid": "chalk:example:jsonld",\n    "scidata": {\n      "@type": "sdo:scientificData",\n      "discipline": "",\n      "subdiscipline": "",\n      "dataset": {\n        "@id": "dataset/",\n        "@type": "sdo:dataset"\n      }\n    }\n  }\n}\n```\n\n# Development\n\n### Install using poetry\nInstall via [poetry](https://python-poetry.org/) with dev dependencies:\n```\npoetry install\n```\n\nThen, run commands via poetry:\n```\npoetry run python -c "import scidatalib"\n```\n\n### CLI\n\nRun the CLI in using poetry via:\n```\npoetry install\npoetry run scidatalib --help\n```\n\n### Tests / Linting\n\n#### Flake8 linting\nRun linting over the package with [flake8](https://flake8.pycqa.org/en/latest/) via:\n```\npoetry run flake8 --count\n```\n\n#### Pytest testing\nRun tests using [pytest](https://docs.pytest.org/en/stable/):\n```\npoetry run pytest tests/\n```\n\n#### Code coverage\n\nGet code coverage reporting using the [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/) plugin:\n```\npoetry run pytest --cov=scidatalib --cov-report=term-missing tests/\n```\n\n# Release\n\nFor developers, please see [Release Workflow](https://github.com/ChalkLab/SciDataLib/wiki/Release-Workflow).\n\n# Contributing\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n# Links\n* SciData Research Paper: [https://doi.org/10.1186/s13321-016-0168-9](https://doi.org/10.1186/s13321-016-0168-9)\n* SciData Project Website: [http://stuchalk.github.io/scidata/](http://stuchalk.github.io/scidata/) \n* SciData Project GitHub Repository: [https://github.com/stuchalk/scidata](https://github.com/stuchalk/scidata)\n\n# Licensing\n[MIT](https://choosealicense.com/licenses/mit/)\n',
-    'author': 'Stuart Chalk',
-    'author_email': 'schalk@unf.edu',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ChalkLab/SciDataLib',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+A Python library writing [SciData](http://stuchalk.github.io/scidata/) [JSON-LD](https://json-ld.org/) files.
+
+# SciData and JSON-LD
+
+JSON-LD is a convenient (human-readable) encoding of Resource
+Description Framework (RDF) triples.  However, unlike traditional
+relational databases (e.g., MySQL), the graph has no schema. This
+is problematic as including data from different sources results
+in a system with no common way to search across the data.  The
+SciData framework is a structure for users to add data and its metadata
+that are organized in the graph through the associated SciData ontology.
+
+There are three main sections of the SciData framework:
+- the methodology section (describing how the research was done)
+- the system section (describing what the research studied and the conditions)
+- the dataset section (the experimental data, plus any derived or supplemental data)
+
+The methodology and system sections are generic and users can add any data
+they need to contextualize the dataset.  However, in addition they must
+provide a JSON-LD context file to semantically describe the data elements
+included.  The dataset section has predefined data structures (dataseries,
+datagroup, and datapoint) although other strudtures can be included
+if needed.
+
+Translating the content in JSON-LD.  Referencing the JSON-LD below:
+- '@context': provides resources that define the context (meaning) of 
+  data elements in the document (as a JSON array). It consists of three sections:
+    - a list of one or more 'context' files
+    - a JSON object containing one or more definitions of namespaces
+    used in the document
+    - a JSON object with one entry '@base' that defines the base URL
+    to be prepended to all internal references (i.e. '@id' entries)
+- root level '@id': the 'name' of the file and where ingested into a
+graph database, the graph name
+- '@graph': the definition of content that will be represented as triples
+and identified by the graph name (this is therfore a 'quad')
+- '@id' under '@graph': the identifier for the graph.  The scidatalib
+code uses the '@base' to populate this, so they are consistent. As a result,
+  all node identifiers '@id's in the document are globally unique because the
+  '@base' is unique.
+
+```json
+{
+  "@context": [
+    "https://stuchalk.github.io/scidata/contexts/scidata.jsonld",
+    {
+      "sci": "https://stuchalk.github.io/scidata/ontology/scidata.owl#"
+    },
+    {
+      "@base": "https://my.research.edu/<uniqueid>/"
+    }
+  ],
+  "@id": "graph name",
+  "generatedAt": "<automatically added>",
+  "version": "1",
+  "@graph": {
+    "@id": "https://my.research.edu/<uniqueid>/",
+    "@type": "sdo:scidataFramework",
+    "uid": "<uniqueid>",
+    "scidata": {
+      "@type": "sdo:scientificData",
+      "methodology": {
+        "@id": "methodology/",
+        "@type": "sdo:methodology",
+        "aspects": []
+      },
+      "system": {
+        "@id": "system/",
+        "@type": "sdo:system",
+        "facets": []
+      },
+      "dataset": {
+        "@id": "dataset/",
+        "@type": "sdo:dataset",
+        "dataseries": [],
+        "datagroup": [],
+        "datapoint": []
+      }
+    }
+  }
 }
+```
+
+
+# Installation
+
+### Using pip
+```
+pip install scidatalib
+```
+
+### Manual (from source)
+Clone the repository either via:
+ - HTTP:
+```
+git clone https://github.com/ChalkLab/SciDataLib.git
+```
+ - SSH:
+```
+git clone git@github.com:ChalkLab/SciDataLib.git
+```
+
+Create a virtual environment and activate to install the package in the isolated environment:
+```
+python -m venv <name of env>
+source <env>/bin/activate
+```
+
+To [install the package from the local source tree into the environment](
+https://packaging.python.org/tutorials/installing-packages/#installing-from-a-local-src-tree), run:
+```
+python -m pip install .
+```
+
+Or to do so in ["Development Mode"](https://setuptools.readthedocs.io/en/latest/setuptools.html#development-mode), 
+you can run:
+```
+python -m pip install -e .
+```
+
+To deactivate the virtual environment
+```
+deactivate
+```
+
+When finished, remove the virtual environment by deleting the directory:
+```
+rm -rf <name of env>
+```
+
+# Usage
+
+SciDataLib consists of both a command line interface (CLI)
+and a library for constructing and modifying SciData JSON-LD files
+
+### Command Line Interface
+
+The CLI tool is `scidatalib`.
+You can use it to create SciData JSON-LD files
+via specifying an output JSON-LD filename
+and additional options to create the content of the file.
+
+Example to create "bare" SciData JSON-LD file:
+```
+scidatalib output.jsonld
+```
+
+You can access the additional functionality via the `--help` option:
+```
+scidatalib --help
+```
+
+### SciDataLib library
+After installation, import the `SciData` class to start creating SciData JSON-LD:
+```python
+from scidatalib.scidata import SciData
+```
+
+Example:
+```python
+from scidatalib.scidata import SciData
+import json
+
+uid = 'chalk:example:jsonld'
+example = SciData(uid)
+
+# context parameters
+base = 'https://scidata.unf.edu/' + uid + '/'
+example.base(base)
+
+# print out the SciData JSON-LD for example
+print(json.dumps(example.output, indent=2))
+```
+
+**Output**:
+```json
+{
+  "@context": [
+    "https://stuchalk.github.io/scidata/contexts/scidata.jsonld",
+    {
+      "sci": "https://stuchalk.github.io/scidata/ontology/scidata.owl#",
+      "sub": "https://stuchalk.github.io/scidata/ontology/substance.owl#",
+      "chm": "https://stuchalk.github.io/scidata/ontology/chemical.owl#",
+      "w3i": "https://w3id.org/skgo/modsci#",
+      "qudt": "https://qudt.org/vocab/unit/",
+      "obo": "http://purl.obolibrary.org/obo/",
+      "dc": "https://purl.org/dc/terms/",
+      "xsd": "https://www.w3.org/2001/XMLSchema#"
+    },
+    {
+      "@base": "https://scidata.unf.edu/chalk:example:jsonld/"
+    }
+  ],
+  "@id": "",
+  "generatedAt": "",
+  "version": "",
+  "@graph": {
+    "@id": "",
+    "@type": "sdo:scidataFramework",
+    "uid": "chalk:example:jsonld",
+    "scidata": {
+      "@type": "sdo:scientificData",
+      "discipline": "",
+      "subdiscipline": "",
+      "dataset": {
+        "@id": "dataset/",
+        "@type": "sdo:dataset"
+      }
+    }
+  }
+}
+```
+
+# Development
+
+### Install using poetry
+Install via [poetry](https://python-poetry.org/) with dev dependencies:
+```
+poetry install
+```
+
+Then, run commands via poetry:
+```
+poetry run python -c "import scidatalib"
+```
+
+### CLI
+
+Run the CLI in using poetry via:
+```
+poetry install
+poetry run scidatalib --help
+```
+
+### Tests / Linting
+
+#### Flake8 linting
+Run linting over the package with [flake8](https://flake8.pycqa.org/en/latest/) via:
+```
+poetry run flake8 --count
+```
+
+#### Pytest testing
+Run tests using [pytest](https://docs.pytest.org/en/stable/):
+```
+poetry run pytest tests/
+```
+
+#### Code coverage
+
+Get code coverage reporting using the [pytest-cov](https://pytest-cov.readthedocs.io/en/latest/) plugin:
+```
+poetry run pytest --cov=scidatalib --cov-report=term-missing tests/
+```
+
+# Release
+
+For developers, please see [Release Workflow](https://github.com/ChalkLab/SciDataLib/wiki/Release-Workflow).
+
+# Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+# Links
+* SciData Research Paper: [https://doi.org/10.1186/s13321-016-0168-9](https://doi.org/10.1186/s13321-016-0168-9)
+* SciData Project Website: [http://stuchalk.github.io/scidata/](http://stuchalk.github.io/scidata/) 
+* SciData Project GitHub Repository: [https://github.com/stuchalk/scidata](https://github.com/stuchalk/scidata)
 
+# Licensing
+[MIT](https://choosealicense.com/licenses/mit/)
 
-setup(**setup_kwargs)
```

