# Comparing `tmp/task2a-1.0.2.tar.gz` & `tmp/task2a-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task2a-1.0.2.tar", max compression
+gzip compressed data, was "task2a-1.0.3.tar", max compression
```

## Comparing `task2a-1.0.2.tar` & `task2a-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      318 2023-07-06 22:19:40.173023 task2a-1.0.2/pwgen/__init__.py
--rw-r--r--   0        0        0      112 2023-07-06 22:19:40.173023 task2a-1.0.2/pwgen/__main__.py
--rw-r--r--   0        0        0       23 2023-07-07 02:46:06.969859 task2a-1.0.2/pwgen/__version__.py
--rw-r--r--   0        0        0       73 2023-07-06 22:19:40.174021 task2a-1.0.2/pwgen/cli/__init__.py
--rw-r--r--   0        0        0      112 2023-07-06 22:19:40.174021 task2a-1.0.2/pwgen/cli/__main__.py
--rw-r--r--   0        0        0     4614 2023-07-06 22:19:40.174021 task2a-1.0.2/pwgen/cli/cli.py
--rw-r--r--   0        0        0     8361 2023-07-06 22:19:40.175016 task2a-1.0.2/pwgen/pwgen.py
--rw-r--r--   0        0        0       93 2023-07-07 01:33:29.604917 task2a-1.0.2/pwgen/showcase/__init__.py
--rw-r--r--   0        0        0      132 2023-07-07 01:33:29.604917 task2a-1.0.2/pwgen/showcase/__main__.py
--rw-r--r--   0        0        0       99 2023-07-07 01:33:29.604917 task2a-1.0.2/pwgen/showcase/pattern-list-error.txt
--rw-r--r--   0        0        0      175 2023-07-07 01:33:29.605916 task2a-1.0.2/pwgen/showcase/pattern-list.txt
--rw-r--r--   0        0        0    19900 2023-07-07 01:33:29.605916 task2a-1.0.2/pwgen/showcase/showcase.py
--rw-r--r--   0        0        0      447 2023-07-07 02:45:55.874863 task2a-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    35645 2023-07-07 02:45:47.386179 task2a-1.0.2/README.md
--rw-r--r--   0        0        0    35395 1970-01-01 00:00:00.000000 task2a-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:00:47.124418 task2a-1.0.3/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-07 02:48:43.371622 task2a-1.0.3/pwgen/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.371622 task2a-1.0.3/pwgen/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-08 14:16:02.463794 task2a-1.0.3/pwgen/__version__.py
+-rw-r--r--   0        0        0       73 2023-07-07 02:48:43.372616 task2a-1.0.3/pwgen/cli/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-07 02:48:43.372616 task2a-1.0.3/pwgen/cli/__main__.py
+-rw-r--r--   0        0        0     4614 2023-07-07 02:48:43.373616 task2a-1.0.3/pwgen/cli/cli.py
+-rw-r--r--   0        0        0     8361 2023-07-07 02:48:43.373616 task2a-1.0.3/pwgen/pwgen.py
+-rw-r--r--   0        0        0       93 2023-07-07 02:48:43.374623 task2a-1.0.3/pwgen/showcase/__init__.py
+-rw-r--r--   0        0        0      132 2023-07-07 02:48:43.374623 task2a-1.0.3/pwgen/showcase/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-07 02:48:43.374623 task2a-1.0.3/pwgen/showcase/pattern-list-error.txt
+-rw-r--r--   0        0        0      175 2023-07-07 02:48:43.374623 task2a-1.0.3/pwgen/showcase/pattern-list.txt
+-rw-r--r--   0        0        0    19900 2023-07-07 02:48:43.375617 task2a-1.0.3/pwgen/showcase/showcase.py
+-rw-r--r--   0        0        0      464 2023-07-08 14:16:02.458793 task2a-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    36970 2023-07-08 14:11:17.636090 task2a-1.0.3/README.md
+-rw-r--r--   0        0        0    36772 1970-01-01 00:00:00.000000 task2a-1.0.3/PKG-INFO
```

### Comparing `task2a-1.0.2/pwgen/cli/cli.py` & `task2a-1.0.3/pwgen/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.2/pwgen/pwgen.py` & `task2a-1.0.3/pwgen/pwgen.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.2/pwgen/showcase/showcase.py` & `task2a-1.0.3/pwgen/showcase/showcase.py`

 * *Files identical despite different names*

### Comparing `task2a-1.0.2/README.md` & `task2a-1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 <p align="center">
   <a href="https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill">
-    <img src="assets/images/title-logo-origin.svg" alt="EPAM DevOps-7 Internal Lab title logo" width="100%" height="300px">
+    <img src="https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/ecd2eb07b44c03c4bcdf5493b45fe46238a12e14/shared/images/title-logo-origin.svg" alt="EPAM DevOps-7 Internal Lab title logo" width="100%" height="300px">
   </a>
 </p>
 
 <h1 align="center">
-  Password generator.
+  <div align="center" aria-colspan="0">Password generator.</div>
   <div align="center" aria-colspan="0">Module 2: Python. Task 2A.</div>
 </h1>
 
+<p align="center">
+  <a href="https://pypi.org/project/task2a/">
+    <img src="https://img.shields.io/pypi/v/task2a.svg?style=for-the-badge" alt="PYPI v." />
+  </a>&nbsp;
+  <a href="https://www.python.org/downloads/">
+    <img src="https://img.shields.io/pypi/pyversions/task2a?style=for-the-badge" alt="Python v." />
+  </a>&nbsp;
+  <a href="https://discord.gg/angular">
+    <img src="https://img.shields.io/pypi/l/task2a.svg?style=for-the-badge" alt="License" />
+  </a>
+</p>
+
 
 ## Preface
 
 This project contains a solution to one of the tasks of the EPAM DevOps Initial Internal Training Course #7 in 2023.
-Detailed information about the course, as well as reports on each of the completed tasks (including this one) can be found [here](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill) [![/^](/assets/images/external-link-blue-12.png)](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
+Detailed information about the course, as well as reports on each of the completed tasks (including this one) can be found [here](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill) [![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
 <br>
 As mentioned above, the project contains a solution to task #2A as part of module #2 of learning the Python programming language.
 Below you will find a detailed description of the task, as well as a brief description of the implementation.
 
 ## Table of Contents
 
 - [Task description](#task-description)
@@ -357,24 +369,24 @@
 }
 
 ''.join(str(c) for c in character_set)  # 'ABCDEFGHIJKLMNOPQRSTUVWXYZ012349@$%&#*!'
 ```
 
 ## Implementation
 
-[Pwgen](https://pypi.org/project/testpoetry2/)[![/^](/assets/images/external-link-blue-12.png)](https://pypi.org/project/testpoetry2/)
+[Pwgen](https://pypi.org/project/task2a/)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://pypi.org/project/task2a/)
 is a Python package that could be added to your global or virtual environment by preferable package manager pip, pipenv, poetry, etc.
-The project itself was managed and built using the [Poetry library](https://python-poetry.org/)[![/^](/assets/images/external-link-blue-12.png)](https://python-poetry.org/),
-so if you intend to clone this repo and make some changes for your own purposes, please install [Poetry](https://python-poetry.org/docs/#installation)[![/^](/assets/images/external-link-blue-12.png)](https://python-poetry.org/docs/#installation)
+The project itself was managed and built using the [Poetry library](https://python-poetry.org/)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://python-poetry.org/),
+so if you intend to clone this repo and make some changes for your own purposes, please install [Poetry](https://python-poetry.org/docs/#installation)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://python-poetry.org/docs/#installation)
 or migrate to your preferred package management library.
 
 Based on the need to build and the possibility of using both the library and the CLI, the code was split into a library for importing and a script for execution
 via the command line. Additionally, the package contains a showcase that demonstrates all use cases when run through the command line.
 
-To enhance the command line's functionality and expand showcase capabilities, the [Questionary](https://questionary.readthedocs.io/en/stable/)[![/^](/assets/images/external-link-blue-12.png)](https://questionary.readthedocs.io/en/stable/)
+To enhance the command line's functionality and expand showcase capabilities, the [Questionary](https://questionary.readthedocs.io/en/stable/)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://questionary.readthedocs.io/en/stable/)
 library is used and will be installed through a dependency link upon package installation.
 
 ### Structure
 
 ```markdown
 task_2a/
 ├── README.md (You are here now)
@@ -403,20 +415,20 @@
 
 ###### Pip
 
 To install Pwgen packet to your environment using pip manager invoke `pip install task2a`.
 
 ```bash
 $ pip install task2a
-Collecting testpoetry2
+Collecting task2a
   Using cached task2a-0.1.N-py3-none-any.whl (10 kB)
 Collecting questionary<2.0.0,>=1.10.0 (from task2a)
   Downloading questionary-1.10.0-py3-none-any.whl (31 kB)
      ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 31.1/31.1 kB N.N MB/s eta 0:00:00
-Collecting prompt_toolkit<4.0,>=2.0 (from questionary<2.0.0,>=1.10.0->testpoetry2)
+Collecting prompt_toolkit<4.0,>=2.0 (from questionary<2.0.0,>=1.10.0->task2a)
   Downloading prompt_toolkit-3.0.39-py3-none-any.whl (385 kB)
      ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 385.2/385.2 kB N.N MB/s eta 0:00:00
 Requirement already satisfied: wcwidth in <your environment folder>\.venv\lib\site-packages (from prompt_toolkit<4.0,>=2.0->questionary<2.0.0,>=1.10.0->task2a) (0.2.6)
 Installing collected packages: prompt_toolkit, questionary, task2a
 Successfully installed prompt_toolkit-3.0.39 questionary-1.10.0 task2a-0.1.N
 ```
 
@@ -572,15 +584,15 @@
 - if you pass argument -f, the -t and -S arguments will be ignored
 - if you pass argument -t, the -S arguments will be ignored
 - if no -f, -t, -S arguments are passed, passwords are generated based on the default character set
 
 When using input files or stdin via the pipe, it's important to pass patterns or lists of patterns only (avoid character sets and other variations).
 Each line in the file will be treated as one pattern.
 
-To handle the arguments, the [argparse](https://docs.python.org/3/library/argparse.html)[![/^](/assets/images/external-link-blue-12.png)](https://docs.python.org/3/library/argparse.html)
+To handle the arguments, the [argparse](https://docs.python.org/3/library/argparse.html)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://docs.python.org/3/library/argparse.html)
 module is used. If you are already acquainted with it, you will have no difficulty in passing the arguments along with their values and comprehending their behavior.
 
 Here is an example list of CLI using, more examples in a more convenient form you could find in the [showcase](#showcase):
 
 | Call example                                                             | Outcome explanation                                                                                                                                                                             |
 |--------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `pwgen` or `python -m pwgen`                                             | One eight-character (default value) password will be generated based on the default character set.                                                                                              |
@@ -618,15 +630,15 @@
 #### Showcase
 
 To showcase the behavior of the pwgen library, an interactive command called "pwgen_showcase" has been created.
 This command utilizes both the pwgen CLI and the pwgen library. It's an interactive command you can invoke via `pwgen_showcase` or `python -m pwgen.showcase`.
 It has an optional flag that allows you to view all use cases at once without any interaction.
 You can use the command `pwgen_showcase --all` to activate this feature.
 
-![showcase_demo.gif](assets/images/showcase_demo.gif)
+![showcase_demo.gif](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/m2-python/task-2a/images/showcase_demo.gif)
 
 ## General provisions
 
 All materials provided and/or made available contain EPAM’s proprietary and confidential information and must not to be copied,
 reproduced or disclosed to any third party or to any other person, other than those persons who have a bona fide need to review it
 for the purpose of participation in the online courses being provided by EPAM.
 The intellectual property rights in all materials (including any trademarks) are owned by EPAM Systems Inc or its associated companies,
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                               Password generator.
                           Module 2: Python. Task 2A.
+                       [PYPI_v.]  [Python_v.]  [License]
 ## Preface This project contains a solution to one of the tasks of the EPAM
 DevOps Initial Internal Training Course #7 in 2023. Detailed information about
 the course, as well as reports on each of the completed tasks (including this
 one) can be found [here](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-
-avramenko-bill) [![/^](/assets/images/external-link-blue-12.png)](https://
-gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
+avramenko-bill) [![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/
+raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-
+12.png)](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
 As mentioned above, the project contains a solution to task #2A as part of
 module #2 of learning the Python programming language. Below you will find a
 detailed description of the task, as well as a brief description of the
 implementation. ## Table of Contents - [Task description](#task-description) -
 [Detailed conditions](#detailed-conditions) - [Generation Based on Character
 Sets](#generation-based-on-character-sets) - [Generation Based on Patterns]
 (#generation-based-on-patterns) - [CLI interface arguments](#cli-interface-can-
@@ -200,30 +202,36 @@
 differences of them and join it to the string. ```python character_set -
 = excluded_character_set return ''.join(str(c) for c in character_set) ``` The
 differences and the final string will be ```python { 'A', 'B', 'C', 'D', 'E',
 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U',
 'V', 'W', 'X', 'Y', 'Z', '0', '1', '2', '3', '4', '9', '@', '$', '%', '&', '#',
 '*', '!', } ''.join(str(c) for c in character_set) #
 'ABCDEFGHIJKLMNOPQRSTUVWXYZ012349@$%&#*!' ``` ## Implementation [Pwgen](https:/
-/pypi.org/project/testpoetry2/)[![/^](/assets/images/external-link-blue-
-12.png)](https://pypi.org/project/testpoetry2/) is a Python package that could
-be added to your global or virtual environment by preferable package manager
-pip, pipenv, poetry, etc. The project itself was managed and built using the
-[Poetry library](https://python-poetry.org/)[![/^](/assets/images/external-
-link-blue-12.png)](https://python-poetry.org/), so if you intend to clone this
-repo and make some changes for your own purposes, please install [Poetry]
-(https://python-poetry.org/docs/#installation)[![/^](/assets/images/external-
-link-blue-12.png)](https://python-poetry.org/docs/#installation) or migrate to
-your preferred package management library. Based on the need to build and the
-possibility of using both the library and the CLI, the code was split into a
-library for importing and a script for execution via the command line.
-Additionally, the package contains a showcase that demonstrates all use cases
-when run through the command line. To enhance the command line's functionality
-and expand showcase capabilities, the [Questionary](https://
-questionary.readthedocs.io/en/stable/)[![/^](/assets/images/external-link-blue-
+/pypi.org/project/task2a/)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-
+7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-
+link-blue-12.png)](https://pypi.org/project/task2a/) is a Python package that
+could be added to your global or virtual environment by preferable package
+manager pip, pipenv, poetry, etc. The project itself was managed and built
+using the [Poetry library](https://python-poetry.org/)[![/^](https://
+gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/
+45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-
+12.png)](https://python-poetry.org/), so if you intend to clone this repo and
+make some changes for your own purposes, please install [Poetry](https://
+python-poetry.org/docs/#installation)[![/^](https://gitlab.com/EPAM-
+DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/
+shared/images/external-link-blue-12.png)](https://python-poetry.org/docs/
+#installation) or migrate to your preferred package management library. Based
+on the need to build and the possibility of using both the library and the CLI,
+the code was split into a library for importing and a script for execution via
+the command line. Additionally, the package contains a showcase that
+demonstrates all use cases when run through the command line. To enhance the
+command line's functionality and expand showcase capabilities, the
+[Questionary](https://questionary.readthedocs.io/en/stable/)[![/^](https://
+gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/
+45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-
 12.png)](https://questionary.readthedocs.io/en/stable/) library is used and
 will be installed through a dependency link upon package installation. ###
 Structure ```markdown task_2a/ âââ README.md (You are here now) âââ
 task_2a.toml # Poetry package management file âââ pwgen/ (Module 1. Git)
 âââ __init__.py # library entry point âââ __main__.py # CLI entry
 point âââ __version__.py âââ pwgen.py # library implementation
 âââ cli/ â âââ __init__.py â âââ __main__.py â
@@ -231,21 +239,21 @@
 __init__.py âââ __main__.py # showcase entry point when using python -
 m showcase âââ pattern-list.txt # input pattern examples file âââ
 pattern-list-error.txt # input pattern examples file with intentional errors
 âââ showcase.py # showcase implementation ``` ## Installation Use your
 preferred installation method via different package installation managers to
 install Pwgen. ###### Pip To install Pwgen packet to your environment using pip
 manager invoke `pip install task2a`. ```bash $ pip install task2a Collecting
-testpoetry2 Using cached task2a-0.1.N-py3-none-any.whl (10 kB) Collecting
+task2a Using cached task2a-0.1.N-py3-none-any.whl (10 kB) Collecting
 questionary<2.0.0,>=1.10.0 (from task2a) Downloading questionary-1.10.0-py3-
 none-any.whl (31 kB)
 ââââââââââââââââââââââââââââââââââââââââ
 31.1/31.1 kB N.N MB/s eta 0:00:00 Collecting prompt_toolkit<4.0,>=2.0 (from
-questionary<2.0.0,>=1.10.0->testpoetry2) Downloading prompt_toolkit-3.0.39-py3-
-none-any.whl (385 kB)
+questionary<2.0.0,>=1.10.0->task2a) Downloading prompt_toolkit-3.0.39-py3-none-
+any.whl (385 kB)
 ââââââââââââââââââââââââââââââââââââââââ
 385.2/385.2 kB N.N MB/s eta 0:00:00 Requirement already satisfied: wcwidth in
 \.venv\lib\site-packages (from prompt_toolkit<4.0,>=2.0-
 >questionary<2.0.0,>=1.10.0->task2a) (0.2.6) Installing collected packages:
 prompt_toolkit, questionary, task2a Successfully installed prompt_toolkit-
 3.0.39 questionary-1.10.0 task2a-0.1.N ``` To uninstall Pwgen from your
 environment invoke `pip uninstall task2a`. ```bash $ pip uninstall task2a Found
@@ -317,66 +325,67 @@
 argument handling: - if you pass argument -f, the -t and -S arguments will be
 ignored - if you pass argument -t, the -S arguments will be ignored - if no -f,
 -t, -S arguments are passed, passwords are generated based on the default
 character set When using input files or stdin via the pipe, it's important to
 pass patterns or lists of patterns only (avoid character sets and other
 variations). Each line in the file will be treated as one pattern. To handle
 the arguments, the [argparse](https://docs.python.org/3/library/argparse.html)
-[![/^](/assets/images/external-link-blue-12.png)](https://docs.python.org/3/
-library/argparse.html) module is used. If you are already acquainted with it,
-you will have no difficulty in passing the arguments along with their values
-and comprehending their behavior. Here is an example list of CLI using, more
-examples in a more convenient form you could find in the [showcase](#showcase):
-| Call example | Outcome explanation | |---------------------------------------
------------------------------------|-------------------------------------------
+[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/
+45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-
+12.png)](https://docs.python.org/3/library/argparse.html) module is used. If
+you are already acquainted with it, you will have no difficulty in passing the
+arguments along with their values and comprehending their behavior. Here is an
+example list of CLI using, more examples in a more convenient form you could
+find in the [showcase](#showcase): | Call example | Outcome explanation | |----
+----------------------------------------------------------------------|--------
 -------------------------------------------------------------------------------
------------------------------------------------------------------------| |
-`pwgen` or `python -m pwgen` | One eight-character (default value) password
-will be generated based on the default character set. | | `pwgen -n5` or `pwgen
--n 5` | One five-character password will be generated based on the default
-character set. | | `pwgen -c3` | Three eight-character passwords will be
-generated based on the default character set. | | `pwgen -n5 -c3 -p` | Three
-five-character passwords will be generated based on the default character set
-and permutate. | | `pwgen -n5 -c3 -v` | Three five-character passwords will be
-generated based on the default character set. Warning messages will also be
-displayed during the generation. | | `pwgen -n5 -c3 -vv` | Three five-character
-passwords will be generated based on the default character set. Warning and
-info messages will also be displayed during the generation. | | `pwgen -n5 -c3
--vvv` | Three five-character passwords will be generated based on the default
-character set. All types of messages will be displayed during the generation. |
-| `pwgen -f .venv/Lib/site-packages/pwgen/test/pattern-list.txt` | N passwords
-(based on text lines in the file) will be generated based on each line given
-template. Pattern length sets the password length. | | `pwgen -f .venv/Lib/
-site-packages/pwgen/test/pattern-list.txt -n5 -c3` | N * 3 passwords will be
-generated based on each line given template. The -n flag will be ignored. | |
-`pwgen -t u{2}p{5}l{2}d{2}L -n5 -c3 -p` | Three passwords will be generated
-based on a given template and will be permutate after the generation. The -
-n flag will be ignored. | | `pwgen -S Ld^l^\\4^\\5^\\6^\\7^\\8 -n5 -c3` | Three
-five-character passwords will be generated based on the given character set.
-(Please note that in certain cases, you may need to double the \ symbol to
-prevent any errors in execution). | | `pwgen -t u{2}p{5}l{2}d{2}L -
-S Ld^l^\\4^\\5^\\6^\\7^\\8 -n5 -c3` | N * 3 passwords will be generated based
-on each line given template. The -n and -s flags will be ignored. | #### Pipes
-and files The pwgen command could be used inside the pipe of the BASH commands.
-It can be used in various ways within a pipeline: - receiving input - direct
-output to a file - direct logging also to a file - direct output to the next
-command in the pipeline Here is an example list of pipeline using, more
-examples in a more convenient form you could find in the [showcase](#showcase):
-| Call example | Outcome explanation | |---------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------|--------------------------------
+---------------------------| | `pwgen` or `python -m pwgen` | One eight-
+character (default value) password will be generated based on the default
+character set. | | `pwgen -n5` or `pwgen -n 5` | One five-character password
+will be generated based on the default character set. | | `pwgen -c3` | Three
+eight-character passwords will be generated based on the default character set.
+| | `pwgen -n5 -c3 -p` | Three five-character passwords will be generated based
+on the default character set and permutate. | | `pwgen -n5 -c3 -v` | Three
+five-character passwords will be generated based on the default character set.
+Warning messages will also be displayed during the generation. | | `pwgen -n5 -
+c3 -vv` | Three five-character passwords will be generated based on the default
+character set. Warning and info messages will also be displayed during the
+generation. | | `pwgen -n5 -c3 -vvv` | Three five-character passwords will be
+generated based on the default character set. All types of messages will be
+displayed during the generation. | | `pwgen -f .venv/Lib/site-packages/pwgen/
+test/pattern-list.txt` | N passwords (based on text lines in the file) will be
+generated based on each line given template. Pattern length sets the password
+length. | | `pwgen -f .venv/Lib/site-packages/pwgen/test/pattern-list.txt -n5 -
+c3` | N * 3 passwords will be generated based on each line given template. The
+-n flag will be ignored. | | `pwgen -t u{2}p{5}l{2}d{2}L -n5 -c3 -p` | Three
+passwords will be generated based on a given template and will be permutate
+after the generation. The -n flag will be ignored. | | `pwgen -
+S Ld^l^\\4^\\5^\\6^\\7^\\8 -n5 -c3` | Three five-character passwords will be
+generated based on the given character set. (Please note that in certain cases,
+you may need to double the \ symbol to prevent any errors in execution). | |
+`pwgen -t u{2}p{5}l{2}d{2}L -S Ld^l^\\4^\\5^\\6^\\7^\\8 -n5 -c3` | N * 3
+passwords will be generated based on each line given template. The -n and -
+s flags will be ignored. | #### Pipes and files The pwgen command could be used
+inside the pipe of the BASH commands. It can be used in various ways within a
+pipeline: - receiving input - direct output to a file - direct logging also to
+a file - direct output to the next command in the pipeline Here is an example
+list of pipeline using, more examples in a more convenient form you could find
+in the [showcase](#showcase): | Call example | Outcome explanation | |---------
+-------------------------------------------------------------------------------
+----------------------------------------------------------------------------|--
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------------------| | `cat .venv/Lib/site-packages/pwgen/test/
-pattern-list.txt \| pwgen -n5 -c3` or `cat .venv/Lib/site-packages/pwgen/test/
-pattern-list.txt \| python -m pwgen -n5 -c3` | A template list is taken from a
-file and passed as input to pwgen. Three passwords on each template will be
-generated. The -n flag will be ignored. | | `pwgen -
-S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n5 -c3 -vv > ./pwd-lst.txt` | Three five-
+-----------------------------------------------------------| | `cat .venv/Lib/
+site-packages/pwgen/test/pattern-list.txt \| pwgen -n5 -c3` or `cat .venv/Lib/
+site-packages/pwgen/test/pattern-list.txt \| python -m pwgen -n5 -c3` | A
+template list is taken from a file and passed as input to pwgen. Three
+passwords on each template will be generated. The -n flag will be ignored. | |
+`pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n5 -c3 -vv > ./pwd-lst.txt` | Three five-
 character passwords will be generated based on the given character set. The
 generated passwords will not be displayed on the screen and will be saved to a
 file. Warning and info messages will also be displayed during the generation. |
 | `pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n5 -c3 -vvv 2> ./pwgen.log` | Three
 five-character passwords will be generated based on the given character set.
 The generated passwords will be displayed. All types of messages will not be
 displayed during the generation and will be saved to a file. | | `echo u{4}
@@ -387,19 +396,20 @@
 order and print them out. The -n flag will be ignored. | #### Showcase To
 showcase the behavior of the pwgen library, an interactive command called
 "pwgen_showcase" has been created. This command utilizes both the pwgen CLI and
 the pwgen library. It's an interactive command you can invoke via
 `pwgen_showcase` or `python -m pwgen.showcase`. It has an optional flag that
 allows you to view all use cases at once without any interaction. You can use
 the command `pwgen_showcase --all` to activate this feature. !
-[showcase_demo.gif](assets/images/showcase_demo.gif) ## General provisions All
-materials provided and/or made available contain EPAMâs proprietary and
-confidential information and must not to be copied, reproduced or disclosed to
-any third party or to any other person, other than those persons who have a
-bona fide need to review it for the purpose of participation in the online
-courses being provided by EPAM. The intellectual property rights in all
-materials (including any trademarks) are owned by EPAM Systems Inc or its
-associated companies, and a limited license, terminable at the discretion of
-EPAM without notice, is hereby granted to you solely for the purpose of
-participating in the online courses being provided by EPAM. Neither you nor any
-other party shall acquire any intellectual property rights of any kind in such
-materials.
+[showcase_demo.gif](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/
+raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/m2-python/task-2a/images/
+showcase_demo.gif) ## General provisions All materials provided and/or made
+available contain EPAMâs proprietary and confidential information and must
+not to be copied, reproduced or disclosed to any third party or to any other
+person, other than those persons who have a bona fide need to review it for the
+purpose of participation in the online courses being provided by EPAM. The
+intellectual property rights in all materials (including any trademarks) are
+owned by EPAM Systems Inc or its associated companies, and a limited license,
+terminable at the discretion of EPAM without notice, is hereby granted to you
+solely for the purpose of participating in the online courses being provided by
+EPAM. Neither you nor any other party shall acquire any intellectual property
+rights of any kind in such materials.
```

### Comparing `task2a-1.0.2/PKG-INFO` & `task2a-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 Metadata-Version: 2.1
 Name: task2a
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
+License: MIT
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill">
-    <img src="assets/images/title-logo-origin.svg" alt="EPAM DevOps-7 Internal Lab title logo" width="100%" height="300px">
+    <img src="https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/ecd2eb07b44c03c4bcdf5493b45fe46238a12e14/shared/images/title-logo-origin.svg" alt="EPAM DevOps-7 Internal Lab title logo" width="100%" height="300px">
   </a>
 </p>
 
 <h1 align="center">
-  Password generator.
+  <div align="center" aria-colspan="0">Password generator.</div>
   <div align="center" aria-colspan="0">Module 2: Python. Task 2A.</div>
 </h1>
 
+<p align="center">
+  <a href="https://pypi.org/project/task2a/">
+    <img src="https://img.shields.io/pypi/v/task2a.svg?style=for-the-badge" alt="PYPI v." />
+  </a>&nbsp;
+  <a href="https://www.python.org/downloads/">
+    <img src="https://img.shields.io/pypi/pyversions/task2a?style=for-the-badge" alt="Python v." />
+  </a>&nbsp;
+  <a href="https://discord.gg/angular">
+    <img src="https://img.shields.io/pypi/l/task2a.svg?style=for-the-badge" alt="License" />
+  </a>
+</p>
+
 
 ## Preface
 
 This project contains a solution to one of the tasks of the EPAM DevOps Initial Internal Training Course #7 in 2023.
-Detailed information about the course, as well as reports on each of the completed tasks (including this one) can be found [here](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill) [![/^](/assets/images/external-link-blue-12.png)](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
+Detailed information about the course, as well as reports on each of the completed tasks (including this one) can be found [here](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill) [![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
 <br>
 As mentioned above, the project contains a solution to task #2A as part of module #2 of learning the Python programming language.
 Below you will find a detailed description of the task, as well as a brief description of the implementation.
 
 ## Table of Contents
 
 - [Task description](#task-description)
@@ -370,24 +384,24 @@
 }
 
 ''.join(str(c) for c in character_set)  # 'ABCDEFGHIJKLMNOPQRSTUVWXYZ012349@$%&#*!'
 ```
 
 ## Implementation
 
-[Pwgen](https://pypi.org/project/testpoetry2/)[![/^](/assets/images/external-link-blue-12.png)](https://pypi.org/project/testpoetry2/)
+[Pwgen](https://pypi.org/project/task2a/)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://pypi.org/project/task2a/)
 is a Python package that could be added to your global or virtual environment by preferable package manager pip, pipenv, poetry, etc.
-The project itself was managed and built using the [Poetry library](https://python-poetry.org/)[![/^](/assets/images/external-link-blue-12.png)](https://python-poetry.org/),
-so if you intend to clone this repo and make some changes for your own purposes, please install [Poetry](https://python-poetry.org/docs/#installation)[![/^](/assets/images/external-link-blue-12.png)](https://python-poetry.org/docs/#installation)
+The project itself was managed and built using the [Poetry library](https://python-poetry.org/)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://python-poetry.org/),
+so if you intend to clone this repo and make some changes for your own purposes, please install [Poetry](https://python-poetry.org/docs/#installation)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://python-poetry.org/docs/#installation)
 or migrate to your preferred package management library.
 
 Based on the need to build and the possibility of using both the library and the CLI, the code was split into a library for importing and a script for execution
 via the command line. Additionally, the package contains a showcase that demonstrates all use cases when run through the command line.
 
-To enhance the command line's functionality and expand showcase capabilities, the [Questionary](https://questionary.readthedocs.io/en/stable/)[![/^](/assets/images/external-link-blue-12.png)](https://questionary.readthedocs.io/en/stable/)
+To enhance the command line's functionality and expand showcase capabilities, the [Questionary](https://questionary.readthedocs.io/en/stable/)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://questionary.readthedocs.io/en/stable/)
 library is used and will be installed through a dependency link upon package installation.
 
 ### Structure
 
 ```markdown
 task_2a/
 ├── README.md (You are here now)
@@ -416,20 +430,20 @@
 
 ###### Pip
 
 To install Pwgen packet to your environment using pip manager invoke `pip install task2a`.
 
 ```bash
 $ pip install task2a
-Collecting testpoetry2
+Collecting task2a
   Using cached task2a-0.1.N-py3-none-any.whl (10 kB)
 Collecting questionary<2.0.0,>=1.10.0 (from task2a)
   Downloading questionary-1.10.0-py3-none-any.whl (31 kB)
      ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 31.1/31.1 kB N.N MB/s eta 0:00:00
-Collecting prompt_toolkit<4.0,>=2.0 (from questionary<2.0.0,>=1.10.0->testpoetry2)
+Collecting prompt_toolkit<4.0,>=2.0 (from questionary<2.0.0,>=1.10.0->task2a)
   Downloading prompt_toolkit-3.0.39-py3-none-any.whl (385 kB)
      ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 385.2/385.2 kB N.N MB/s eta 0:00:00
 Requirement already satisfied: wcwidth in <your environment folder>\.venv\lib\site-packages (from prompt_toolkit<4.0,>=2.0->questionary<2.0.0,>=1.10.0->task2a) (0.2.6)
 Installing collected packages: prompt_toolkit, questionary, task2a
 Successfully installed prompt_toolkit-3.0.39 questionary-1.10.0 task2a-0.1.N
 ```
 
@@ -585,15 +599,15 @@
 - if you pass argument -f, the -t and -S arguments will be ignored
 - if you pass argument -t, the -S arguments will be ignored
 - if no -f, -t, -S arguments are passed, passwords are generated based on the default character set
 
 When using input files or stdin via the pipe, it's important to pass patterns or lists of patterns only (avoid character sets and other variations).
 Each line in the file will be treated as one pattern.
 
-To handle the arguments, the [argparse](https://docs.python.org/3/library/argparse.html)[![/^](/assets/images/external-link-blue-12.png)](https://docs.python.org/3/library/argparse.html)
+To handle the arguments, the [argparse](https://docs.python.org/3/library/argparse.html)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-12.png)](https://docs.python.org/3/library/argparse.html)
 module is used. If you are already acquainted with it, you will have no difficulty in passing the arguments along with their values and comprehending their behavior.
 
 Here is an example list of CLI using, more examples in a more convenient form you could find in the [showcase](#showcase):
 
 | Call example                                                             | Outcome explanation                                                                                                                                                                             |
 |--------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `pwgen` or `python -m pwgen`                                             | One eight-character (default value) password will be generated based on the default character set.                                                                                              |
@@ -631,15 +645,15 @@
 #### Showcase
 
 To showcase the behavior of the pwgen library, an interactive command called "pwgen_showcase" has been created.
 This command utilizes both the pwgen CLI and the pwgen library. It's an interactive command you can invoke via `pwgen_showcase` or `python -m pwgen.showcase`.
 It has an optional flag that allows you to view all use cases at once without any interaction.
 You can use the command `pwgen_showcase --all` to activate this feature.
 
-![showcase_demo.gif](assets/images/showcase_demo.gif)
+![showcase_demo.gif](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/m2-python/task-2a/images/showcase_demo.gif)
 
 ## General provisions
 
 All materials provided and/or made available contain EPAM’s proprietary and confidential information and must not to be copied,
 reproduced or disclosed to any third party or to any other person, other than those persons who have a bona fide need to review it
 for the purpose of participation in the online courses being provided by EPAM.
 The intellectual property rights in all materials (including any trademarks) are owned by EPAM Systems Inc or its associated companies,
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: task2a Version: 1.0.2 Summary: Author:
+Metadata-Version: 2.1 Name: task2a Version: 1.0.3 Summary: License: MIT Author:
 Bill.Avramenko Author-email: billavramenko@gmail.com Requires-Python:
->=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Dist: questionary (>=1.10.0,<2.0.0) Description-
-Content-Type: text/markdown
+>=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
+questionary (>=1.10.0,<2.0.0) Description-Content-Type: text/markdown
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                               Password generator.
                           Module 2: Python. Task 2A.
+                       [PYPI_v.]  [Python_v.]  [License]
 ## Preface This project contains a solution to one of the tasks of the EPAM
 DevOps Initial Internal Training Course #7 in 2023. Detailed information about
 the course, as well as reports on each of the completed tasks (including this
 one) can be found [here](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-
-avramenko-bill) [![/^](/assets/images/external-link-blue-12.png)](https://
-gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
+avramenko-bill) [![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/
+raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-
+12.png)](https://gitlab.com/Bill-EPAM-DevOpsInt2023/devops-7-avramenko-bill).
 As mentioned above, the project contains a solution to task #2A as part of
 module #2 of learning the Python programming language. Below you will find a
 detailed description of the task, as well as a brief description of the
 implementation. ## Table of Contents - [Task description](#task-description) -
 [Detailed conditions](#detailed-conditions) - [Generation Based on Character
 Sets](#generation-based-on-character-sets) - [Generation Based on Patterns]
 (#generation-based-on-patterns) - [CLI interface arguments](#cli-interface-can-
@@ -206,30 +208,36 @@
 differences of them and join it to the string. ```python character_set -
 = excluded_character_set return ''.join(str(c) for c in character_set) ``` The
 differences and the final string will be ```python { 'A', 'B', 'C', 'D', 'E',
 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U',
 'V', 'W', 'X', 'Y', 'Z', '0', '1', '2', '3', '4', '9', '@', '$', '%', '&', '#',
 '*', '!', } ''.join(str(c) for c in character_set) #
 'ABCDEFGHIJKLMNOPQRSTUVWXYZ012349@$%&#*!' ``` ## Implementation [Pwgen](https:/
-/pypi.org/project/testpoetry2/)[![/^](/assets/images/external-link-blue-
-12.png)](https://pypi.org/project/testpoetry2/) is a Python package that could
-be added to your global or virtual environment by preferable package manager
-pip, pipenv, poetry, etc. The project itself was managed and built using the
-[Poetry library](https://python-poetry.org/)[![/^](/assets/images/external-
-link-blue-12.png)](https://python-poetry.org/), so if you intend to clone this
-repo and make some changes for your own purposes, please install [Poetry]
-(https://python-poetry.org/docs/#installation)[![/^](/assets/images/external-
-link-blue-12.png)](https://python-poetry.org/docs/#installation) or migrate to
-your preferred package management library. Based on the need to build and the
-possibility of using both the library and the CLI, the code was split into a
-library for importing and a script for execution via the command line.
-Additionally, the package contains a showcase that demonstrates all use cases
-when run through the command line. To enhance the command line's functionality
-and expand showcase capabilities, the [Questionary](https://
-questionary.readthedocs.io/en/stable/)[![/^](/assets/images/external-link-blue-
+/pypi.org/project/task2a/)[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-
+7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-
+link-blue-12.png)](https://pypi.org/project/task2a/) is a Python package that
+could be added to your global or virtual environment by preferable package
+manager pip, pipenv, poetry, etc. The project itself was managed and built
+using the [Poetry library](https://python-poetry.org/)[![/^](https://
+gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/
+45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-
+12.png)](https://python-poetry.org/), so if you intend to clone this repo and
+make some changes for your own purposes, please install [Poetry](https://
+python-poetry.org/docs/#installation)[![/^](https://gitlab.com/EPAM-
+DevOpsInt2023/devops-7-assets/-/raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/
+shared/images/external-link-blue-12.png)](https://python-poetry.org/docs/
+#installation) or migrate to your preferred package management library. Based
+on the need to build and the possibility of using both the library and the CLI,
+the code was split into a library for importing and a script for execution via
+the command line. Additionally, the package contains a showcase that
+demonstrates all use cases when run through the command line. To enhance the
+command line's functionality and expand showcase capabilities, the
+[Questionary](https://questionary.readthedocs.io/en/stable/)[![/^](https://
+gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/
+45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-
 12.png)](https://questionary.readthedocs.io/en/stable/) library is used and
 will be installed through a dependency link upon package installation. ###
 Structure ```markdown task_2a/ âââ README.md (You are here now) âââ
 task_2a.toml # Poetry package management file âââ pwgen/ (Module 1. Git)
 âââ __init__.py # library entry point âââ __main__.py # CLI entry
 point âââ __version__.py âââ pwgen.py # library implementation
 âââ cli/ â âââ __init__.py â âââ __main__.py â
@@ -237,21 +245,21 @@
 __init__.py âââ __main__.py # showcase entry point when using python -
 m showcase âââ pattern-list.txt # input pattern examples file âââ
 pattern-list-error.txt # input pattern examples file with intentional errors
 âââ showcase.py # showcase implementation ``` ## Installation Use your
 preferred installation method via different package installation managers to
 install Pwgen. ###### Pip To install Pwgen packet to your environment using pip
 manager invoke `pip install task2a`. ```bash $ pip install task2a Collecting
-testpoetry2 Using cached task2a-0.1.N-py3-none-any.whl (10 kB) Collecting
+task2a Using cached task2a-0.1.N-py3-none-any.whl (10 kB) Collecting
 questionary<2.0.0,>=1.10.0 (from task2a) Downloading questionary-1.10.0-py3-
 none-any.whl (31 kB)
 ââââââââââââââââââââââââââââââââââââââââ
 31.1/31.1 kB N.N MB/s eta 0:00:00 Collecting prompt_toolkit<4.0,>=2.0 (from
-questionary<2.0.0,>=1.10.0->testpoetry2) Downloading prompt_toolkit-3.0.39-py3-
-none-any.whl (385 kB)
+questionary<2.0.0,>=1.10.0->task2a) Downloading prompt_toolkit-3.0.39-py3-none-
+any.whl (385 kB)
 ââââââââââââââââââââââââââââââââââââââââ
 385.2/385.2 kB N.N MB/s eta 0:00:00 Requirement already satisfied: wcwidth in
 \.venv\lib\site-packages (from prompt_toolkit<4.0,>=2.0-
 >questionary<2.0.0,>=1.10.0->task2a) (0.2.6) Installing collected packages:
 prompt_toolkit, questionary, task2a Successfully installed prompt_toolkit-
 3.0.39 questionary-1.10.0 task2a-0.1.N ``` To uninstall Pwgen from your
 environment invoke `pip uninstall task2a`. ```bash $ pip uninstall task2a Found
@@ -323,66 +331,67 @@
 argument handling: - if you pass argument -f, the -t and -S arguments will be
 ignored - if you pass argument -t, the -S arguments will be ignored - if no -f,
 -t, -S arguments are passed, passwords are generated based on the default
 character set When using input files or stdin via the pipe, it's important to
 pass patterns or lists of patterns only (avoid character sets and other
 variations). Each line in the file will be treated as one pattern. To handle
 the arguments, the [argparse](https://docs.python.org/3/library/argparse.html)
-[![/^](/assets/images/external-link-blue-12.png)](https://docs.python.org/3/
-library/argparse.html) module is used. If you are already acquainted with it,
-you will have no difficulty in passing the arguments along with their values
-and comprehending their behavior. Here is an example list of CLI using, more
-examples in a more convenient form you could find in the [showcase](#showcase):
-| Call example | Outcome explanation | |---------------------------------------
------------------------------------|-------------------------------------------
+[![/^](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/
+45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/shared/images/external-link-blue-
+12.png)](https://docs.python.org/3/library/argparse.html) module is used. If
+you are already acquainted with it, you will have no difficulty in passing the
+arguments along with their values and comprehending their behavior. Here is an
+example list of CLI using, more examples in a more convenient form you could
+find in the [showcase](#showcase): | Call example | Outcome explanation | |----
+----------------------------------------------------------------------|--------
 -------------------------------------------------------------------------------
------------------------------------------------------------------------| |
-`pwgen` or `python -m pwgen` | One eight-character (default value) password
-will be generated based on the default character set. | | `pwgen -n5` or `pwgen
--n 5` | One five-character password will be generated based on the default
-character set. | | `pwgen -c3` | Three eight-character passwords will be
-generated based on the default character set. | | `pwgen -n5 -c3 -p` | Three
-five-character passwords will be generated based on the default character set
-and permutate. | | `pwgen -n5 -c3 -v` | Three five-character passwords will be
-generated based on the default character set. Warning messages will also be
-displayed during the generation. | | `pwgen -n5 -c3 -vv` | Three five-character
-passwords will be generated based on the default character set. Warning and
-info messages will also be displayed during the generation. | | `pwgen -n5 -c3
--vvv` | Three five-character passwords will be generated based on the default
-character set. All types of messages will be displayed during the generation. |
-| `pwgen -f .venv/Lib/site-packages/pwgen/test/pattern-list.txt` | N passwords
-(based on text lines in the file) will be generated based on each line given
-template. Pattern length sets the password length. | | `pwgen -f .venv/Lib/
-site-packages/pwgen/test/pattern-list.txt -n5 -c3` | N * 3 passwords will be
-generated based on each line given template. The -n flag will be ignored. | |
-`pwgen -t u{2}p{5}l{2}d{2}L -n5 -c3 -p` | Three passwords will be generated
-based on a given template and will be permutate after the generation. The -
-n flag will be ignored. | | `pwgen -S Ld^l^\\4^\\5^\\6^\\7^\\8 -n5 -c3` | Three
-five-character passwords will be generated based on the given character set.
-(Please note that in certain cases, you may need to double the \ symbol to
-prevent any errors in execution). | | `pwgen -t u{2}p{5}l{2}d{2}L -
-S Ld^l^\\4^\\5^\\6^\\7^\\8 -n5 -c3` | N * 3 passwords will be generated based
-on each line given template. The -n and -s flags will be ignored. | #### Pipes
-and files The pwgen command could be used inside the pipe of the BASH commands.
-It can be used in various ways within a pipeline: - receiving input - direct
-output to a file - direct logging also to a file - direct output to the next
-command in the pipeline Here is an example list of pipeline using, more
-examples in a more convenient form you could find in the [showcase](#showcase):
-| Call example | Outcome explanation | |---------------------------------------
 -------------------------------------------------------------------------------
-----------------------------------------------|--------------------------------
+---------------------------| | `pwgen` or `python -m pwgen` | One eight-
+character (default value) password will be generated based on the default
+character set. | | `pwgen -n5` or `pwgen -n 5` | One five-character password
+will be generated based on the default character set. | | `pwgen -c3` | Three
+eight-character passwords will be generated based on the default character set.
+| | `pwgen -n5 -c3 -p` | Three five-character passwords will be generated based
+on the default character set and permutate. | | `pwgen -n5 -c3 -v` | Three
+five-character passwords will be generated based on the default character set.
+Warning messages will also be displayed during the generation. | | `pwgen -n5 -
+c3 -vv` | Three five-character passwords will be generated based on the default
+character set. Warning and info messages will also be displayed during the
+generation. | | `pwgen -n5 -c3 -vvv` | Three five-character passwords will be
+generated based on the default character set. All types of messages will be
+displayed during the generation. | | `pwgen -f .venv/Lib/site-packages/pwgen/
+test/pattern-list.txt` | N passwords (based on text lines in the file) will be
+generated based on each line given template. Pattern length sets the password
+length. | | `pwgen -f .venv/Lib/site-packages/pwgen/test/pattern-list.txt -n5 -
+c3` | N * 3 passwords will be generated based on each line given template. The
+-n flag will be ignored. | | `pwgen -t u{2}p{5}l{2}d{2}L -n5 -c3 -p` | Three
+passwords will be generated based on a given template and will be permutate
+after the generation. The -n flag will be ignored. | | `pwgen -
+S Ld^l^\\4^\\5^\\6^\\7^\\8 -n5 -c3` | Three five-character passwords will be
+generated based on the given character set. (Please note that in certain cases,
+you may need to double the \ symbol to prevent any errors in execution). | |
+`pwgen -t u{2}p{5}l{2}d{2}L -S Ld^l^\\4^\\5^\\6^\\7^\\8 -n5 -c3` | N * 3
+passwords will be generated based on each line given template. The -n and -
+s flags will be ignored. | #### Pipes and files The pwgen command could be used
+inside the pipe of the BASH commands. It can be used in various ways within a
+pipeline: - receiving input - direct output to a file - direct logging also to
+a file - direct output to the next command in the pipeline Here is an example
+list of pipeline using, more examples in a more convenient form you could find
+in the [showcase](#showcase): | Call example | Outcome explanation | |---------
+-------------------------------------------------------------------------------
+----------------------------------------------------------------------------|--
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------------------| | `cat .venv/Lib/site-packages/pwgen/test/
-pattern-list.txt \| pwgen -n5 -c3` or `cat .venv/Lib/site-packages/pwgen/test/
-pattern-list.txt \| python -m pwgen -n5 -c3` | A template list is taken from a
-file and passed as input to pwgen. Three passwords on each template will be
-generated. The -n flag will be ignored. | | `pwgen -
-S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n5 -c3 -vv > ./pwd-lst.txt` | Three five-
+-----------------------------------------------------------| | `cat .venv/Lib/
+site-packages/pwgen/test/pattern-list.txt \| pwgen -n5 -c3` or `cat .venv/Lib/
+site-packages/pwgen/test/pattern-list.txt \| python -m pwgen -n5 -c3` | A
+template list is taken from a file and passed as input to pwgen. Three
+passwords on each template will be generated. The -n flag will be ignored. | |
+`pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n5 -c3 -vv > ./pwd-lst.txt` | Three five-
 character passwords will be generated based on the given character set. The
 generated passwords will not be displayed on the screen and will be saved to a
 file. Warning and info messages will also be displayed during the generation. |
 | `pwgen -S "Ld^l^\\4^\\5^\\6^\\7^\\8" -n5 -c3 -vvv 2> ./pwgen.log` | Three
 five-character passwords will be generated based on the given character set.
 The generated passwords will be displayed. All types of messages will not be
 displayed during the generation and will be saved to a file. | | `echo u{4}
@@ -393,19 +402,20 @@
 order and print them out. The -n flag will be ignored. | #### Showcase To
 showcase the behavior of the pwgen library, an interactive command called
 "pwgen_showcase" has been created. This command utilizes both the pwgen CLI and
 the pwgen library. It's an interactive command you can invoke via
 `pwgen_showcase` or `python -m pwgen.showcase`. It has an optional flag that
 allows you to view all use cases at once without any interaction. You can use
 the command `pwgen_showcase --all` to activate this feature. !
-[showcase_demo.gif](assets/images/showcase_demo.gif) ## General provisions All
-materials provided and/or made available contain EPAMâs proprietary and
-confidential information and must not to be copied, reproduced or disclosed to
-any third party or to any other person, other than those persons who have a
-bona fide need to review it for the purpose of participation in the online
-courses being provided by EPAM. The intellectual property rights in all
-materials (including any trademarks) are owned by EPAM Systems Inc or its
-associated companies, and a limited license, terminable at the discretion of
-EPAM without notice, is hereby granted to you solely for the purpose of
-participating in the online courses being provided by EPAM. Neither you nor any
-other party shall acquire any intellectual property rights of any kind in such
-materials.
+[showcase_demo.gif](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/
+raw/45ed5458fe7cf837b62a423fcdff6a52b8db3cdb/m2-python/task-2a/images/
+showcase_demo.gif) ## General provisions All materials provided and/or made
+available contain EPAMâs proprietary and confidential information and must
+not to be copied, reproduced or disclosed to any third party or to any other
+person, other than those persons who have a bona fide need to review it for the
+purpose of participation in the online courses being provided by EPAM. The
+intellectual property rights in all materials (including any trademarks) are
+owned by EPAM Systems Inc or its associated companies, and a limited license,
+terminable at the discretion of EPAM without notice, is hereby granted to you
+solely for the purpose of participating in the online courses being provided by
+EPAM. Neither you nor any other party shall acquire any intellectual property
+rights of any kind in such materials.
```

