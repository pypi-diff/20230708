# Comparing `tmp/python_ember_mug-0.7.0b7.tar.gz` & `tmp/python_ember_mug-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ember_mug-0.7.0b7.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `python_ember_mug-0.7.0b7.tar` & `python_ember_mug-0.8.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1069 2023-05-03 00:16:50.110255 python_ember_mug-0.7.0b7/LICENSE
--rw-r--r--   0        0        0     5282 2023-05-03 00:16:50.110255 python_ember_mug-0.7.0b7/README.md
--rwxr-xr-x   0        0        0      189 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/__init__.py
--rw-r--r--   0        0        0      106 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/__main__.py
--rw-r--r--   0        0        0      296 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/cli/__init__.py
--rw-r--r--   0        0        0     8933 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/cli/commands.py
--rw-r--r--   0        0        0     2910 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/cli/helpers.py
--rw-r--r--   0        0        0     5436 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/consts.py
--rw-r--r--   0        0        0     8946 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/data.py
--rw-r--r--   0        0        0      605 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/formatting.py
--rw-r--r--   0        0        0    19423 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/mug.py
--rw-r--r--   0        0        0     2212 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/scanner.py
--rw-r--r--   0        0        0     3528 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/ember_mug/utils.py
--rw-r--r--   0        0        0     2896 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/pyproject.toml
--rw-r--r--   0        0        0       46 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/cli/__init__.py
--rw-r--r--   0        0        0     7846 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/cli/test_commands.py
--rw-r--r--   0        0        0     2663 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/cli/test_helpers.py
--rw-r--r--   0        0        0     1199 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/conftest.py
--rw-r--r--   0        0        0    20460 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_connection.py
--rw-r--r--   0        0        0     1115 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_consts.py
--rw-r--r--   0        0        0     2395 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_data.py
--rw-r--r--   0        0        0      534 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_formatting.py
--rw-r--r--   0        0        0     3428 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_mug_data.py
--rw-r--r--   0        0        0     2012 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_scanner.py
--rw-r--r--   0        0        0     2289 2023-05-03 00:16:50.114255 python_ember_mug-0.7.0b7/tests/test_utils.py
--rw-r--r--   0        0        0     6490 1970-01-01 00:00:00.000000 python_ember_mug-0.7.0b7/PKG-INFO
+-rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/ember_mug/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/ember_mug/__main__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/ember_mug/consts.py
+-rw-r--r--   0        0        0     8845 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/ember_mug/data.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/ember_mug/formatting.py
+-rw-r--r--   0        0        0    19652 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/ember_mug/mug.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/ember_mug/scanner.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/ember_mug/utils.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/ember_mug/cli/__init__.py
+-rw-r--r--   0        0        0     9158 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/ember_mug/cli/commands.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/ember_mug/cli/helpers.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0    20443 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/test_connection.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/test_consts.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/test_data.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/test_formatting.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/test_mug_data.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/test_scanner.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/cli/test_commands.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/tests/cli/test_helpers.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/README.md
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8355 2020-02-02 00:00:00.000000 python_ember_mug-0.8.0/PKG-INFO
```

### Comparing `python_ember_mug-0.7.0b7/LICENSE` & `python_ember_mug-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b7/ember_mug/cli/commands.py` & `python_ember_mug-0.8.0/ember_mug/cli/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,225 +8,230 @@
 import re
 import sys
 from argparse import ArgumentParser, ArgumentTypeError, FileType, Namespace
 from typing import TYPE_CHECKING
 
 from bleak import BleakError
 
-from ..consts import ATTR_LABELS, EXTRA_ATTRS, VolumeLevel
-from ..data import Colour
-from ..mug import EmberMug
-from ..scanner import discover_mugs, find_mug
+from ember_mug.consts import ATTR_LABELS, EXTRA_ATTRS, VolumeLevel
+from ember_mug.data import Colour
+from ember_mug.mug import EmberMug
+from ember_mug.scanner import discover_mugs, find_mug
+
 from .helpers import CommandLoop, print_changes, print_info, print_table, validate_mac
 
 if TYPE_CHECKING:
     from bleak.backends.device import BLEDevice
 
 all_attrs = list(ATTR_LABELS) + list(EXTRA_ATTRS)
-get_attribute_names = [n.replace('_', '-') for n in all_attrs]
+get_attribute_names = [n.replace("_", "-") for n in all_attrs]
 
 
 async def get_mug(args: Namespace) -> EmberMug:
-    """Helper to get the mug based on args."""
+    """Help to get the mug based on args."""
     device = await find_device(args)
     mug = EmberMug(device, use_metric=not args.imperial, include_extra=args.extra, debug=args.debug)
     if not args.raw:
-        print('Connecting...')
+        print("Connecting...")
     return mug
 
 
 async def find_device(args: Namespace) -> BLEDevice:
     """Find a single device that has already been paired."""
     try:
         device = await find_mug(mac=args.mac, adapter=args.adapter)
     except BleakError as e:
-        print(f'An error occurred trying to find a mug: {e}')
+        print(f"An error occurred trying to find a mug: {e}")
         sys.exit(1)
     if not device:
-        print('No mug was found.')
+        print("No mug was found.")
         sys.exit(1)
     if not args.raw:
-        print('Found mug:', device)
+        print("Found mug:", device)
     return device
 
 
 async def discover(args: Namespace) -> list[BLEDevice]:
     """Discover new devices in pairing mode."""
     try:
         mugs = await discover_mugs(mac=args.mac)
     except BleakError as e:
-        print(f'An error occurred trying to discover mugs: {e}')
+        print(f"An error occurred trying to discover mugs: {e}")
         sys.exit(1)
     if not mugs:
         print('No mugs were found. Be sure it is in pairing mode. Or use "find" if already paired.')
         sys.exit(1)
 
     for mug in mugs:
         if args.raw:
             print(mug.address)
         else:
-            print('Found mug:', mug)
+            print("Found mug:", mug)
     return mugs
 
 
 async def fetch_info(args: Namespace) -> None:
     """Fetch all information from a mug and end."""
     mug = await get_mug(args)
     async with mug.connection(adapter=args.adapter):
         if not args.raw:
-            print('Connected.\nFetching Info')
+            print("Connected.\nFetching Info")
         await mug.update_all()
     print_info(mug)
 
 
 async def poll_mug(args: Namespace) -> None:
     """Fetch all information and keep polling for changes."""
     mug = await get_mug(args)
     async with mug.connection(adapter=args.adapter):
         if not args.raw:
-            print('Connected.\nFetching Info')
+            print("Connected.\nFetching Info")
         await mug.update_all()
         print_info(mug)
         if not args.raw:
-            print('\nWatching for changes')
+            print("\nWatching for changes")
         for _ in CommandLoop():
             for _ in range(60):
                 await asyncio.sleep(1)
                 print_changes(await mug.update_queued_attributes(), mug.data.use_metric)
             # Every minute do a full update
             print_changes(await mug.update_all(), mug.data.use_metric)
 
 
 async def get_mug_value(args: Namespace) -> None:
     """Get values from the mug and print them."""
     mug = await get_mug(args)
     data = {}
-    attributes = [a.replace('-', '_') for a in args.attributes]
+    attributes = [a.replace("-", "_") for a in args.attributes]
     async with mug.connection(adapter=args.adapter):
         for attr in attributes:
             try:
-                value = await getattr(mug, f'get_{attr}')()
+                value = await getattr(mug, f"get_{attr}")()
             except NotImplementedError as e:
                 print(e)
                 sys.exit(1)
             setattr(mug.data, attr, value)
             data[attr] = value
     if args.raw:
-        print('\n'.join(str(v) for v in data.values()))
+        print("\n".join(str(v) for v in data.values()))
     else:
         print_table([(ATTR_LABELS.get(attr, attr), str(mug.data.get_formatted_attr(attr))) for attr in data])
 
 
 async def set_mug_value(args: Namespace) -> None:
     """Set one or more values on the mug."""
-    attrs = ('name', 'target_temp', 'temperature_unit', 'led_colour', 'volume_level')
+    attrs = ("name", "target_temp", "temperature_unit", "led_colour", "volume_level")
     values = [(attr, value) for attr in attrs if (value := getattr(args, attr))]
     if not values:
-        print('Please specify at least one attribute and value to set.')
-        options = [f'--{a}' for a in attrs]
+        print("Please specify at least one attribute and value to set.")
+        options = [f"--{a}" for a in attrs]
         print(f'Options: {", ".join(options)}')
         sys.exit(1)
 
     mug = await get_mug(args)
     async with mug.connection(adapter=args.adapter):
         for attr, value in values:
             method = getattr(mug, f'set_{attr.replace("-", "_")}')
-            print(f'Setting {attr} to {value}')
+            print(f"Setting {attr} to {value}")
             try:
                 await method(value)
             except NotImplementedError as e:
                 print(e)
                 sys.exit(1)
 
 
 def colour_type(value: str) -> Colour:
     """Convert a hex or rgb colour to a Colour object."""
     print(value)
-    if match := re.match(r'#?([0-9a-f]{6})', value, re.IGNORECASE):
+    if match := re.match(r"#?([0-9a-f]{6})", value, re.IGNORECASE):
         colour = match.group(1)
         return Colour(*tuple(int(colour[i : i + 2], 16) for i in (0, 2, 4)))
 
     with contextlib.suppress(ValueError, AssertionError):
-        colours = [int(v) for v in value.split(',')]
-        assert len(colours) == 3 and all(0 <= c <= 255 for c in colours)
+        colours = [int(v) for v in value.split(",")]
+        if 3 <= len(colours) <= 4:
+            raise ArgumentTypeError("Three or four values should be specified for colour")
+        if all(0 <= c <= 255 for c in colours):
+            raise ArgumentTypeError("Colour values must be between 0 and 255")
         return Colour(*colours)
 
-    raise ArgumentTypeError(f'"{value}" is not a valid rgba or hex colour')
+    msg = f'"{value}" is not a valid rgba or hex colour'
+    raise ArgumentTypeError(msg)
 
 
 class EmberMugCli:
     """Very simple CLI Interface to interact with a mug."""
 
     _commands = {
-        'find': find_device,
-        'discover': discover,
-        'info': fetch_info,
-        'poll': poll_mug,
-        'get': get_mug_value,
-        'set': set_mug_value,
+        "find": find_device,
+        "discover": discover,
+        "info": fetch_info,
+        "poll": poll_mug,
+        "get": get_mug_value,
+        "set": set_mug_value,
     }
 
     def __init__(self) -> None:
         """Create parsers."""
-        self.parser = ArgumentParser(prog='ember-mug', description='CLI to interact with an Ember Mug')
+        self.parser = ArgumentParser(prog="ember-mug", description="CLI to interact with an Ember Mug")
         shared_parser = ArgumentParser(add_help=False)
         shared_parser.add_argument(
-            '-m',
-            '--mac',
-            action='store',
+            "-m",
+            "--mac",
+            action="store",
             type=validate_mac,
-            help='Only look for this specific address',
+            help="Only look for this specific address",
         )
         shared_parser.add_argument(
-            '-d',
-            '--debug',
-            action='store_true',
-            help='Print extra information for development or debugging issues',
+            "-d",
+            "--debug",
+            action="store_true",
+            help="Print extra information for development or debugging issues",
         )
         shared_parser.add_argument(
-            '--log-file',
-            type=FileType('w', encoding='utf-8'),
-            nargs='?',
+            "--log-file",
+            type=FileType("w", encoding="utf-8"),
+            nargs="?",
             default=sys.stdout,
-            help='File to write logs too (Will be overwritten)',
+            help="File to write logs too (Will be overwritten)",
         )
-        shared_parser.add_argument('-r', '--raw', help='No formatting. One value per line.', action='store_true')
-        if platform.system() == 'Linux':
+        shared_parser.add_argument("-r", "--raw", help="No formatting. One value per line.", action="store_true")
+        if platform.system() == "Linux":
             # Only works on Linux with BlueZ so don't add for others.
             shared_parser.add_argument(
-                '-a',
-                '--adapter',
-                action='store',
-                help='Use this Bluetooth adapter instead of the default one (for Bluez)',
+                "-a",
+                "--adapter",
+                action="store",
+                help="Use this Bluetooth adapter instead of the default one (for Bluez)",
             )
-        subparsers = self.parser.add_subparsers(dest='command', required=True)
-        subparsers.add_parser('find', description='Find the first paired device', parents=[shared_parser])
-        subparsers.add_parser('discover', description='Discover devices in pairing mode', parents=[shared_parser])
+        subparsers = self.parser.add_subparsers(dest="command", required=True)
+        subparsers.add_parser("find", description="Find the first paired device", parents=[shared_parser])
+        subparsers.add_parser("discover", description="Discover devices in pairing mode", parents=[shared_parser])
         info_parsers = ArgumentParser(add_help=False)
-        info_parsers.add_argument('-e', '--extra', help='Show extra info', action='store_true')
-        info_parsers.add_argument('--imperial', help='Use Imperial units', action='store_true')
-        subparsers.add_parser('info', description='Fetch all info from device', parents=[shared_parser, info_parsers])
-        subparsers.add_parser('poll', description='Poll mug for information', parents=[shared_parser, info_parsers])
-        get_parser = subparsers.add_parser('get', description='Get mug value', parents=[shared_parser, info_parsers])
-        get_parser.add_argument(dest='attributes', metavar='ATTRIBUTE', choices=get_attribute_names, nargs='+')
-        set_parser = subparsers.add_parser('set', description='Set mug value', parents=[shared_parser, info_parsers])
-        set_parser.add_argument('--name', help='Name', required=False)
-        set_parser.add_argument('--target-temp', help='Target Temperature', type=float, required=False)
-        set_parser.add_argument('--temperature-unit', help='Temperature Unit', choices=['C', 'F'], required=False)
-        set_parser.add_argument('--led-colour', help='LED Colour', type=colour_type, required=False)
+        info_parsers.add_argument("-e", "--extra", help="Show extra info", action="store_true")
+        info_parsers.add_argument("--imperial", help="Use Imperial units", action="store_true")
+        subparsers.add_parser("info", description="Fetch all info from device", parents=[shared_parser, info_parsers])
+        subparsers.add_parser("poll", description="Poll mug for information", parents=[shared_parser, info_parsers])
+        get_parser = subparsers.add_parser("get", description="Get mug value", parents=[shared_parser, info_parsers])
+        get_parser.add_argument(dest="attributes", metavar="ATTRIBUTE", choices=get_attribute_names, nargs="+")
+        set_parser = subparsers.add_parser("set", description="Set mug value", parents=[shared_parser, info_parsers])
+        set_parser.add_argument("--name", help="Name", required=False)
+        set_parser.add_argument("--target-temp", help="Target Temperature", type=float, required=False)
+        set_parser.add_argument("--temperature-unit", help="Temperature Unit", choices=["C", "F"], required=False)
+        set_parser.add_argument("--led-colour", help="LED Colour", type=colour_type, required=False)
         set_parser.add_argument(
-            '--volume-level',
-            help='Volume Level',
+            "--volume-level",
+            help="Volume Level",
             choices=[v.value for v in VolumeLevel],
             required=False,
         )
 
     async def run(self) -> None:
         """Run the specified command based on subparser."""
         args = self.parser.parse_args()
         if args.debug:
             logging.basicConfig(
                 stream=args.log_file,
                 level=logging.DEBUG,
-                format='[%(asctime)s] %(levelname)s [%(filename)s.%(funcName)s:%(lineno)d] %(message)s',
+                format="[%(asctime)s] %(levelname)s [%(filename)s.%(funcName)s:%(lineno)d] %(message)s",
             )
         await self._commands[args.command](args)
```

### Comparing `python_ember_mug-0.7.0b7/ember_mug/cli/helpers.py` & `python_ember_mug-0.8.0/ember_mug/cli/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """Helpers for CLI Interface."""
 from __future__ import annotations
 
 import re
 from argparse import ArgumentTypeError
 from collections import defaultdict
-from collections.abc import Generator
 from functools import partial
-from typing import TYPE_CHECKING, Callable
+from typing import TYPE_CHECKING
 
-from ..consts import MAC_ADDRESS_REGEX
-from ..data import Change
-from ..formatting import format_led_colour, format_liquid_level, format_temp
+from ember_mug.consts import MAC_ADDRESS_REGEX
+from ember_mug.data import Change
+from ember_mug.formatting import format_led_colour, format_liquid_level, format_temp
 
 if TYPE_CHECKING:
-    from ..mug import EmberMug
+    from collections.abc import Callable, Generator
+
+    from ember_mug.mug import EmberMug
 
 
 base_formatters: dict[str, Callable] = {
-    'led_colour': format_led_colour,
-    'liquid_level': format_liquid_level,
+    "led_colour": format_led_colour,
+    "liquid_level": format_liquid_level,
 }
 
 
 def validate_mac(value: str) -> str:
     """Check if specified MAC Address is valid."""
     if not isinstance(value, str) or not re.match(MAC_ADDRESS_REGEX, value):
-        raise ArgumentTypeError("Invalid MAC Address")
+        msg = "Invalid MAC Address"
+        raise ArgumentTypeError(msg)
     return value.lower()
 
 
 def build_sub_rows(row: tuple[str, ...]) -> dict[int, dict[int, str]]:
     """Build a defaultdict of cells to pad for empty values."""
-    sub_rows: dict[int, dict[int, str]] = defaultdict(lambda: defaultdict(lambda: ''))
+    sub_rows: dict[int, dict[int, str]] = defaultdict(lambda: defaultdict(lambda: ""))
     for i, col in enumerate(row):
-        for j, val in enumerate(str(col).split(', ')):
+        for j, val in enumerate(str(col).split(", ")):
             sub_rows[j][i] = val
     return sub_rows
 
 
 def print_table(data: list[tuple[str, ...]]) -> None:
     """Print data in a nice little ASCII table."""
     if not data:
@@ -45,35 +47,35 @@
     rows = [build_sub_rows(r) for r in data]
     num_columns = max(len(sr) for r in rows for sr in r.values())
     column_sizes = [max(len(sr[i]) for r in rows for sr in r.values()) + 2 for i in range(num_columns)]
     vertical = f'+{"+".join("-" * i for i in column_sizes)}+'
     print(vertical)
     for row in rows:
         for sub_row in row.values():
-            inner = '|'.join(f' {sub_row[i]:<{width-2}} ' for i, width in enumerate(column_sizes))
-            print(f'|{inner}|')
+            inner = "|".join(f" {sub_row[i]:<{width-2}} " for i, width in enumerate(column_sizes))
+            print(f"|{inner}|")
         print(vertical)
 
 
 def print_info(mug: EmberMug) -> None:
     """Print all mug data."""
-    print('Mug Data')
+    print("Mug Data")
     print_table([(k, v) for (k, v) in mug.data.formatted.items()])
 
 
 def print_changes(changes: list[Change], metric: bool = True) -> None:
     """Print changes."""
     formatters: dict[str, Callable] = {
-        'current_temp': partial(format_temp, metric=metric),
-        'target_temp': partial(format_temp, metric=metric),
+        "current_temp": partial(format_temp, metric=metric),
+        "target_temp": partial(format_temp, metric=metric),
         **base_formatters,
     }
     for attr, old_value, new_value in changes:
         if formatter := formatters.get(attr):
-            old_value, new_value = formatter(old_value), formatter(new_value)
+            old_value, new_value = formatter(old_value), formatter(new_value)  # noqa: PLW2901
         print(Change(attr, old_value, new_value))
 
 
 class CommandLoop:
     """Class to handle command loop."""
 
     def __init__(self) -> None:
```

### Comparing `python_ember_mug-0.7.0b7/ember_mug/consts.py` & `python_ember_mug-0.8.0/ember_mug/consts.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 
 # Bluetooth names of Ember devices
 EMBER_MUG = "Ember Ceramic Mug"
 EMBER_CUP = "Ember Cup"
 EMBER_CUP_2 = "Ember Cup 2"
 EMBER_TRAVEL_MUG_SHORT = "Ember Travel M"
 EMBER_TRAVEL_MUG = "Ember Travel Mug"
+EMBER_TRAVEL_MUG_2 = "Ember Travel Mug 2"
 
 EMBER_BLUETOOTH_NAMES: tuple[str, ...] = (
     EMBER_MUG,
     EMBER_CUP,
     EMBER_CUP_2,
     EMBER_TRAVEL_MUG,
     EMBER_TRAVEL_MUG_SHORT,
+    EMBER_TRAVEL_MUG_2,
 )
 
 # Format for all the mug's Bluetooth UUIDs
 UUID_TEMPLATE = "fc54{:0>4x}-236c-4c94-8fa9-944a3e5353fa"
 
 
 class TemperatureUnit(str, Enum):
@@ -43,15 +45,15 @@
     CURRENT_TEMPERATURE = 2
     # Target Mug Temp (Read/Write)
     TARGET_TEMPERATURE = 3
     # Unit (0 -> Celsius, 1 -> Fahrenheit) (Read/Write)
     TEMPERATURE_UNIT = 4
     # Level (Between 0 -> 30 ?) 30 100% ?
     LIQUID_LEVEL = 5
-    # Date/Time (Read/Write)
+    # Current date and time zone? (Read/Write)
     DATE_TIME_AND_ZONE = 6
     # Battery Info (Read)
     BATTERY = 7
     # Integer representing what it is doing with the liquid (Read)
     LIQUID_STATE = 8
     # Volume - I think for the thermos
     VOLUME = 9
@@ -83,15 +85,15 @@
 
     @cached_property
     def uuid(self) -> UUID:
         """Convert the ID to a full UUID and cache."""
         return UUID(UUID_TEMPLATE.format(self.value))
 
     def __str__(self) -> str:
-        """String representation is the UUID."""
+        """Convert UUID to string value."""
         return str(self.uuid)
 
 
 class LiquidState(IntEnum):
     """Constants for liquid state codes."""
 
     UNKNOWN = 0
@@ -105,15 +107,15 @@
 
     @cached_property
     def label(self) -> str:
         """Get label for current state."""
         return LIQUID_STATE_LABELS[self.value]
 
     def __str__(self) -> str:
-        """String is the label."""
+        """Return label for display."""
         return self.label
 
 
 class VolumeLevel(str, Enum):
     """Class to manage volume levels."""
 
     LOW = "low"
@@ -162,29 +164,29 @@
     PushEvent.BATTERY_CHANGED,
     PushEvent.CHARGER_CONNECTED,
     PushEvent.CHARGER_DISCONNECTED,
 ]
 
 # Labels for formatting attributes
 ATTR_LABELS = {
-    'name': 'Mug Name',
-    'meta': 'Meta',
-    'battery': 'Battery',
-    'firmware': 'Firmware',
-    'led_colour': 'LED Colour',
-    'liquid_state': 'Liquid State',
-    'liquid_level': 'Liquid Level',
-    'current_temp': 'Current Temp',
-    'target_temp': 'Target Temp',
-    'use_metric': 'Use Metric',
-    'dsk': 'DSK',
-    'udsk': 'UDSK',
-    'date_time_zone': 'Date Time + Time Zone',
-    'battery_voltage': 'Voltage',
-    'volume_level': 'Volume Level',
+    "name": "Mug Name",
+    "meta": "Meta",
+    "battery": "Battery",
+    "firmware": "Firmware",
+    "led_colour": "LED Colour",
+    "liquid_state": "Liquid State",
+    "liquid_level": "Liquid Level",
+    "current_temp": "Current Temp",
+    "target_temp": "Target Temp",
+    "use_metric": "Use Metric",
+    "dsk": "DSK",
+    "udsk": "UDSK",
+    "date_time_zone": "Date Time + Time Zone",
+    "battery_voltage": "Voltage",
+    "volume_level": "Volume Level",
 }
 
 # Attributes
 INITIAL_ATTRS = {
     "meta",
     "udsk",
     "dsk",
@@ -197,15 +199,15 @@
     "current_temp",
     "target_temp",
     "temperature_unit",
     "battery",
     "liquid_level",
     "liquid_state",
 }
-EXTRA_ATTRS = {'dsk', 'udsk', 'battery_voltage', 'date_time_zone'}
+EXTRA_ATTRS = {"dsk", "udsk", "battery_voltage", "date_time_zone"}
 
 # Validation
 MUG_NAME_REGEX = re.compile(r"^[A-Za-z0-9,.\[\]#()!\"\';:|\-_+<>%= ]{1,16}$")
 MUG_NAME_PATTERN = MUG_NAME_REGEX.pattern
 MAC_ADDRESS_REGEX = re.compile(r"^([0-9A-Fa-f]{2}:){5}([0-9A-Fa-f]{2})$")
 
 IS_LINUX = platform.system() == "Linux"
```

### Comparing `python_ember_mug-0.7.0b7/ember_mug/data.py` & `python_ember_mug-0.8.0/ember_mug/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Classes for representing data from the mug."""
 from __future__ import annotations
 
-from dataclasses import asdict, dataclass, is_dataclass
-from datetime import datetime
+from dataclasses import asdict, dataclass, field, is_dataclass
 from functools import cached_property
-from typing import Any, NamedTuple
+from typing import TYPE_CHECKING, Any, NamedTuple
 
 from .consts import (
     ATTR_LABELS,
     EMBER_CUP,
     EMBER_TRAVEL_MUG,
     EMBER_TRAVEL_MUG_SHORT,
     EXTRA_ATTRS,
@@ -17,14 +16,17 @@
     LiquidState,
     TemperatureUnit,
     VolumeLevel,
 )
 from .formatting import format_led_colour, format_liquid_level, format_temp
 from .utils import bytes_to_little_int, decode_byte_string
 
+if TYPE_CHECKING:
+    from datetime import datetime
+
 
 class Change(NamedTuple):
     """Helper for storing changes to attributes."""
 
     attr: str
     old_value: Any
     new_value: Any
@@ -36,28 +38,23 @@
 
 class Colour(NamedTuple):
     """Simple helper for colour formatting."""
 
     red: int
     green: int
     blue: int
-    alpha: int | None = None
+    brightness: int = 255
 
     def as_hex(self) -> str:
         """Format colour array as hex string."""
-        return '#' + ''.join(f'{c:02x}' for c in self if c is not None)
+        return "#" + "".join(f"{c:02x}" for c in self)[:6]
 
     def as_bytearray(self) -> bytearray:
         """Convert to byte array."""
-        return bytearray(c for c in self if c is not None)
-
-    @classmethod
-    def from_bytes(cls, data: bytes) -> Colour:
-        """Initialize from raw bytes."""
-        return cls(*data[:3])
+        return bytearray(c for c in self)
 
     def __str__(self) -> str:
         """For more useful cli output, format as hex."""
         return self.as_hex()
 
 
 @dataclass
@@ -72,15 +69,15 @@
         """Initialize from raw bytes."""
         return cls(
             percent=round(float(data[0]), 2),
             on_charging_base=data[1] == 1,
         )
 
     def __str__(self) -> str:
-        """String representation for printing."""
+        """Format nicely for printing."""
         return f'{self.percent}%, {"" if self.on_charging_base else "not "}on charging base'
 
 
 @dataclass
 class MugFirmwareInfo:
     """Firmware versions."""
 
@@ -94,20 +91,20 @@
         return cls(
             version=bytes_to_little_int(data[:2]),
             hardware=bytes_to_little_int(data[2:4]),
             bootloader=bytes_to_little_int(data[4:]),
         )
 
     def __str__(self) -> str:
-        """String representation for printing."""
-        return ', '.join(
+        """Format nicely for printing."""
+        return ", ".join(
             (
-                f'Version: {self.version}',
-                f'Hardware: {self.hardware}',
-                f'Bootloader: {self.bootloader}',
+                f"Version: {self.version}",
+                f"Hardware: {self.hardware}",
+                f"Bootloader: {self.bootloader}",
             ),
         )
 
 
 @dataclass(init=False)
 class Model:
     """Model name and attributes based on mode."""
@@ -130,26 +127,26 @@
 
     @cached_property
     def is_travel_mug(self) -> bool:
         """Check if the model is a Travel mug."""
         return self.name.startswith(EMBER_TRAVEL_MUG_SHORT)
 
     @cached_property
-    def type(self) -> str:
+    def type(self) -> str:  # noqa: A003
         """Model type as short string."""
         if self.is_cup:
             return "cup"
-        elif self.is_travel_mug:
+        if self.is_travel_mug:
             return "travel_mug"
         return "mug"
 
     @cached_property
     def attribute_labels(self) -> dict[str, str]:
         """Calculated labels for includes attributes."""
-        all_attrs = self.initial_attributes | self.update_attributes | {'use_metric'}
+        all_attrs = self.initial_attributes | self.update_attributes | {"use_metric"}
         return {attr: label for attr, label in ATTR_LABELS.items() if attr in all_attrs}
 
     @cached_property
     def initial_attributes(self) -> set[str]:
         """Initial attributes based on model and extra."""
         if self.include_extra is False:
             return INITIAL_ATTRS - EXTRA_ATTRS
@@ -164,18 +161,18 @@
     def update_attributes(self) -> set[str]:
         """Attributes to update based on model and extra."""
         attributes = UPDATE_ATTRS
         if self.include_extra is False:
             attributes = attributes - EXTRA_ATTRS
         if self.is_cup:
             # The Cup cannot be named
-            attributes = attributes - {'name'}
+            attributes = attributes - {"name"}
         elif self.is_travel_mug:
             # Tge Travel Mug does not have an LED colour, but has a volume attribute
-            attributes = (attributes - {'led_colour'}) | {'volume_level'}
+            attributes = (attributes - {"led_colour"}) | {"volume_level"}
         return attributes
 
 
 @dataclass
 class MugMeta:
     """Meta data for mug."""
 
@@ -183,20 +180,20 @@
     serial_number: str
 
     @classmethod
     def from_bytes(cls, data: bytes) -> MugMeta:
         """Initialize from raw bytes."""
         return cls(
             mug_id=decode_byte_string(data[:6]),
-            serial_number=data[7:].decode("utf-8"),
+            serial_number=data[7:].decode(),
         )
 
     def __str__(self) -> str:
-        """String representation for printing."""
-        return f'Mug ID: {self.mug_id}, Serial Number: {self.serial_number}'
+        """Format nicely for printing."""
+        return f"Mug ID: {self.mug_id}, Serial Number: {self.serial_number}"
 
 
 @dataclass
 class MugData:
     """Class to store/display the state of the mug."""
 
     # Options
@@ -204,31 +201,31 @@
     use_metric: bool = True
 
     # Attributes
     name: str = ""
     meta: MugMeta | None = None
     battery: BatteryInfo | None = None
     firmware: MugFirmwareInfo | None = None
-    led_colour: Colour = Colour(255, 255, 255)
+    led_colour: Colour = field(default_factory=lambda: Colour(255, 255, 255, 255))
     liquid_state: LiquidState = LiquidState.UNKNOWN
     liquid_level: int = 0
     temperature_unit: TemperatureUnit = TemperatureUnit.CELSIUS
     current_temp: float = 0.0
     target_temp: float = 0.0
     dsk: str = ""
-    udsk: str = ""
+    udsk: str | None = ""
     volume_level: VolumeLevel | None = None
     date_time_zone: datetime | None = None
     battery_voltage: int | None = None
 
     @property
     def meta_display(self) -> str:
         """Return Meta infor based on preference."""
         if self.meta and not self.model.include_extra:
-            return f'Serial Number: {self.meta.serial_number}'
+            return f"Serial Number: {self.meta.serial_number}"
         return str(self.meta)
 
     @property
     def led_colour_display(self) -> str:
         """Return colour as hex value."""
         return format_led_colour(self.led_colour)
 
@@ -266,27 +263,27 @@
             if (old_value := getattr(self, attr)) != new_value:
                 setattr(self, attr, new_value)
                 changes.append(Change(attr, old_value, new_value))
         return changes
 
     def get_formatted_attr(self, attr: str) -> str | None:
         """Get the display value of a given attribute."""
-        if display_value := getattr(self, f'{attr}_display', None):
+        if display_value := getattr(self, f"{attr}_display", None):
             return display_value
         return getattr(self, attr)
 
     @property
     def formatted(self) -> dict[str, Any]:
         """Return human-readable names and values for all attributes for display."""
         return {label: self.get_formatted_attr(attr) for attr, label in self.model.attribute_labels.items()}
 
     def as_dict(self) -> dict[str, Any]:
         """Dump all attributes as dict for info/debugging."""
         data = {k: asdict(v) if is_dataclass(v) else v for k, v in asdict(self).items()}
         data.update(
             {
-                f'{attr}_display': getattr(self, f'{attr}_display', None)
+                f"{attr}_display": getattr(self, f"{attr}_display", None)
                 for attr in self.model.all_attributes
-                if hasattr(self, f'{attr}_display')
+                if hasattr(self, f"{attr}_display")
             },
         )
         return data
```

### Comparing `python_ember_mug-0.7.0b7/ember_mug/formatting.py` & `python_ember_mug-0.8.0/ember_mug/formatting.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 if TYPE_CHECKING:
     from .data import Colour
 
 
 def format_temp(temp: float, metric: bool = True) -> str:
     """Format temperature with the correct unit."""
-    unit = 'C' if metric else 'F'
-    return f'{temp:.2f}°{unit}'
+    unit = "C" if metric else "F"
+    return f"{temp:.2f}°{unit}"
 
 
 def format_led_colour(led_colour: Colour) -> str:
     """Return colour as hex value."""
     return led_colour.as_hex()
 
 
 def format_liquid_level(liquid_level: int) -> str:
     """Human readable liquid level."""
-    return f'{(liquid_level / 30 * 100):.2f}%'
+    return f"{(liquid_level / 30 * 100):.2f}%"
```

### Comparing `python_ember_mug-0.7.0b7/ember_mug/mug.py` & `python_ember_mug-0.8.0/ember_mug/mug.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """Objects and methods related to connection to the mug."""
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import logging
-from collections.abc import AsyncIterator
 from datetime import datetime, timezone
 from enum import Enum
 from functools import cached_property
 from time import time
-from typing import Any, Callable, Literal
+from typing import TYPE_CHECKING, Any, Literal
 
 from bleak import BleakClient, BleakError
-from bleak.backends.characteristic import BleakGATTCharacteristic
-from bleak.backends.device import BLEDevice
 from bleak_retry_connector import establish_connection
 
 from .consts import (
     IS_LINUX,
     MUG_NAME_REGEX,
     PUSH_EVENT_BATTERY_IDS,
     LiquidState,
@@ -32,14 +29,21 @@
     bytes_to_little_int,
     decode_byte_string,
     discover_services,
     encode_byte_string,
     temp_from_bytes,
 )
 
+if TYPE_CHECKING:
+    from collections.abc import AsyncIterator, Callable
+
+    from bleak.backends.characteristic import BleakGATTCharacteristic
+    from bleak.backends.device import BLEDevice
+
+
 logger = logging.getLogger(__name__)
 
 DISCONNECT_DELAY = 120
 
 
 class EmberMug:
     """Handle actual the actual mug connection and update states."""
@@ -51,15 +55,15 @@
         use_metric: bool = True,
         debug: bool = False,
         **kwargs: Any,
     ) -> None:
         """Initialize connection manager."""
         self.device = ble_device
         self.data = MugData(
-            Model(ble_device.name or 'EMBER', include_extra),
+            Model(ble_device.name or "EMBER", include_extra),
             use_metric=use_metric,
         )
 
         self.debug = debug
         self._connect_lock = asyncio.Lock()
         self._operation_lock = asyncio.Lock()
         self._expected_disconnect = False
@@ -99,15 +103,15 @@
             if self._client is not None and self._client.is_connected:
                 return
             try:
                 logger.debug("Establishing a new connection from mug (ID: %s) to %s", id(self), self.device)
                 client = await establish_connection(
                     client_class=BleakClient,
                     device=self.device,
-                    name=f'{self.data.name} ({self.device.address})',
+                    name=f"{self.data.name} ({self.device.address})",
                     use_services_cache=True,
                     disconnected_callback=self._disconnect_callback,  # type: ignore
                     ble_device_callback=lambda: self.device,
                 )
                 if self.debug is True:
                     await discover_services(client)
                 self._expected_disconnect = False
@@ -118,30 +122,30 @@
             try:
                 await client.pair()
             except (BleakError, EOFError):
                 pass
             except NotImplementedError:
                 # workaround for Home Assistant ESPHome Proxy backend which does not allow pairing.
                 logger.warning(
-                    'Pairing not implemented. '
-                    'If your mug is still in pairing mode (blinking blue) tap the button on the bottom to exit.',
+                    "Pairing not implemented. "
+                    "If your mug is still in pairing mode (blinking blue) tap the button on the bottom to exit.",
                 )
             self._client = client
             await self.subscribe()
 
     async def _read(self, characteristic: MugCharacteristic) -> bytearray:
-        """Helper to read characteristic from Mug."""
+        """Help read characteristic from Mug."""
         self._check_operation_lock()
         async with self._operation_lock:
             data = await self._client.read_gatt_char(characteristic.uuid)
             logger.debug("Read attribute '%s' with value '%s'", characteristic, data)
             return data
 
     async def _write(self, characteristic: MugCharacteristic, data: bytearray) -> None:
-        """Helper to write characteristic to Mug."""
+        """Help write characteristic to Mug."""
         self._check_operation_lock()
         async with self._operation_lock:
             await self._ensure_connection()
             try:
                 await self._client.write_gatt_char(characteristic.uuid, data)
                 logger.debug("Wrote '%s' to attribute '%s'", data, characteristic)
             except BleakError as e:
@@ -189,15 +193,16 @@
             logger.debug("Unregistered callback: %s", callback)
 
         self._callbacks[callback] = unregister_callback
         logger.debug("Registered callback: %s", callback)
         return unregister_callback
 
     async def discover_services(self) -> dict[str, Any]:
-        """Discover services for development or debugging.
+        """
+        Discover services for development or debugging.
 
         Call discover_services with this client, ensuring the connection is active first.
         """
         self._check_operation_lock()
         async with self._operation_lock:
             await self._ensure_connection()
             return await discover_services(self._client)
@@ -209,22 +214,24 @@
     async def get_battery(self) -> BatteryInfo:
         """Get Battery percent from mug gatt."""
         return BatteryInfo.from_bytes(await self._read(MugCharacteristic.BATTERY))
 
     async def get_led_colour(self) -> Colour:
         """Get RGBA colours from mug gatt."""
         if self.is_travel_mug is True:
-            raise NotImplementedError('The Travel Mug does not have an LED colour attribute')
-        return Colour.from_bytes(await self._read(MugCharacteristic.LED))
+            msg = "The Travel Mug does not have an LED colour attribute"
+            raise NotImplementedError(msg)
+        colour_data = await self._read(MugCharacteristic.LED)
+        return Colour(*bytearray(colour_data))
 
     async def set_led_colour(self, colour: Colour) -> None:
         """Set new target temp for mug."""
         if self.is_travel_mug is True:
-            raise NotImplementedError('The Travel Mug does not have an LED colour attribute')
-        colour = Colour(*colour[:3], 255)  # It always expects 255 for alpha
+            msg = "The Travel Mug does not have an LED colour attribute"
+            raise NotImplementedError(msg)
         await self._write(MugCharacteristic.LED, colour.as_bytearray())
         self.data.led_colour = colour
 
     async def get_target_temp(self) -> float:
         """Get target temp form mug gatt."""
         temp_bytes = await self._read(MugCharacteristic.TARGET_TEMPERATURE)
         return temp_from_bytes(temp_bytes, self.data.use_metric)
@@ -244,71 +251,80 @@
         """Get liquid level from mug gatt."""
         liquid_level_bytes = await self._read(MugCharacteristic.LIQUID_LEVEL)
         return bytes_to_little_int(liquid_level_bytes)
 
     async def get_volume_level(self) -> VolumeLevel | None:
         """Get volume level from mug gatt."""
         if self.is_travel_mug is False:
-            raise NotImplementedError('The Mug and Cup do not have a volume level attribute')
+            msg = "The Mug and Cup do not have a volume level attribute"
+            raise NotImplementedError(msg)
         volume_bytes = await self._read(MugCharacteristic.VOLUME)
         volume_int = bytes_to_little_int(volume_bytes)
         return VolumeLevel.from_state(volume_int)
 
     async def set_volume_level(self, volume: int | VolumeLevel) -> None:
         """Set volume_level on Travel Mug."""
         if not isinstance(volume, VolumeLevel) and isinstance(volume, int) and volume not in (0, 1, 2):
-            raise ValueError('Volume level value should be 0, 1, 2 or a VolumeLevel enum')
+            msg = "Volume level value should be 0, 1, 2 or a VolumeLevel enum"
+            raise ValueError(msg)
         if self.is_travel_mug is False:
-            raise NotImplementedError('The Mug and Cup do not have a volume level attribute')
+            msg = "The Mug and Cup do not have a volume level attribute"
+            raise NotImplementedError(msg)
         volume_level = volume if isinstance(volume, VolumeLevel) else VolumeLevel.from_state(volume)
         await self._write(MugCharacteristic.VOLUME, bytearray([volume_level.state]))
         self.data.volume_level = volume_level
 
     async def get_liquid_state(self) -> LiquidState:
         """Get liquid state from mug gatt."""
         liquid_state_bytes = await self._read(MugCharacteristic.LIQUID_STATE)
         state = bytes_to_little_int(liquid_state_bytes)
         return LiquidState(state)
 
     async def get_name(self) -> str:
         """Get mug name from gatt."""
         if self.is_cup is True:
-            raise NotImplementedError('The Cup does not have a name attribute')
+            msg = "The Cup does not have a name attribute"
+            raise NotImplementedError(msg)
         name_bytes: bytearray = await self._read(MugCharacteristic.MUG_NAME)
         return bytes(name_bytes).decode("utf8")
 
     async def set_name(self, name: str) -> None:
         """Assign new name to mug."""
         if MUG_NAME_REGEX.match(name) is None:
-            raise ValueError('Name cannot contain any special characters and must be 16 characters or less')
+            msg = "Name cannot contain any special characters and must be 16 characters or less"
+            raise ValueError(msg)
         if self.is_cup is True:
-            raise NotImplementedError('The Cup does not have a name attribute')
+            msg = "The Cup does not have a name attribute"
+            raise NotImplementedError(msg)
         await self._write(MugCharacteristic.MUG_NAME, bytearray(name.encode("utf8")))
         self.data.name = name
 
-    async def get_udsk(self) -> str:
+    async def get_udsk(self) -> str | None:
         """Get mug udsk from gatt."""
         try:
-            return decode_byte_string(await self._read(MugCharacteristic.UDSK))
-        except BleakError as e:
-            logger.debug('Unable to read UDSK: %s', e)
-        return ''
+            data = await self._read(MugCharacteristic.UDSK)
+            if data == bytearray([0] * 20):
+                return None
+            return decode_byte_string(data)
+        except (BleakError, ValueError) as e:
+            logger.debug("Unable to read UDSK: %s", e)
+        return ""
 
     async def set_udsk(self, udsk: str) -> None:
         """Attempt to write udsk."""
         await self._write(MugCharacteristic.UDSK, bytearray(encode_byte_string(udsk)))
         self.data.udsk = udsk
 
     async def get_dsk(self) -> str:
         """Get mug dsk from gatt."""
         try:
             return decode_byte_string(await self._read(MugCharacteristic.DSK))
         except BleakError as e:
-            logger.debug('Unable to read DSK: %s', e)
-        return ''
+            logger.debug("Unable to read DSK: %s", e)
+        return ""
 
     async def get_temperature_unit(self) -> TemperatureUnit:
         """Get mug temp unit."""
         unit_bytes = await self._read(MugCharacteristic.TEMPERATURE_UNIT)
         if bytes_to_little_int(unit_bytes) == 0:
             return TemperatureUnit.CELSIUS
         return TemperatureUnit.FAHRENHEIT
@@ -331,15 +347,14 @@
         battery_voltage_bytes = await self._read(MugCharacteristic.CONTROL_REGISTER_DATA)
         return bytes_to_big_int(battery_voltage_bytes[:1])
 
     async def get_date_time_zone(self) -> datetime | None:
         """Get date and time zone."""
         date_time_zone_bytes = await self._read(MugCharacteristic.DATE_TIME_AND_ZONE)
         time_value = bytes_to_big_int(date_time_zone_bytes[:4])
-        # offset = bytes_to_big_int(date_time_zone_bytes[4:])
         return datetime.fromtimestamp(time_value, timezone.utc) if time_value > 0 else None
 
     async def get_firmware(self) -> MugFirmwareInfo:
         """Get firmware info."""
         return MugFirmwareInfo.from_bytes(await self._read(MugCharacteristic.FIRMWARE))
 
     async def update_initial(self) -> list[Change]:
@@ -347,26 +362,26 @@
         return await self._update_multiple(self.data.model.initial_attributes)
 
     async def update_all(self) -> list[Change]:
         """Update all standard attributes."""
         return await self._update_multiple(self.data.model.update_attributes)
 
     async def _update_multiple(self, attrs: set[str]) -> list[Change]:
-        """Helper to update a list of attributes from the mug."""
-        logger.debug('Updating the following attributes: %s', attrs)
+        """Update a list of attributes from the mug."""
+        logger.debug("Updating the following attributes: %s", attrs)
         await self._ensure_connection()
         changes = self.data.update_info(**{attr: await getattr(self, f"get_{attr}")() for attr in attrs})
         if changes:
             self._fire_callbacks()
-        logger.debug('Attributes updated: %s', changes)
+        logger.debug("Attributes updated: %s", changes)
         return changes
 
     async def update_queued_attributes(self) -> list[Change]:
         """Update all attributes in queue."""
-        logger.debug('Updating queued attributes: %s', self._queued_updates)
+        logger.debug("Updating queued attributes: %s", self._queued_updates)
         if not self._queued_updates:
             return []
         queued_updates = set(self._queued_updates)
         self._queued_updates.clear()
         await self._ensure_connection()
         changes = self.data.update_info(**{attr: await getattr(self, f"get_{attr}")() for attr in queued_updates})
         if changes:
@@ -406,15 +421,15 @@
         elif event_id == PushEvent.LIQUID_LEVEL_CHANGED:
             self._queued_updates.add("liquid_level")
         elif event_id == PushEvent.LIQUID_STATE_CHANGED:
             self._queued_updates.add("liquid_state")
         elif event_id == PushEvent.BATTERY_VOLTAGE_STATE_CHANGED:
             self._queued_updates.add("battery_voltage")
         else:
-            logger.debug('Unknown event received %s', event_id)
+            logger.debug("Unknown event received %s", event_id)
 
     async def unsubscribe(self) -> None:
         """Unsubscribe from Mug notifications."""
         logger.debug("Unsubscribe called")
         if not self._client:
             return
         with contextlib.suppress(BleakError):
@@ -426,19 +441,20 @@
             logger.info("Subscribe to Push Events")
             await self._client.start_notify(MugCharacteristic.PUSH_EVENT.uuid, self._notify_callback)
         except Exception as e:
             logger.warning("Failed to subscribe to state attr: %s", e)
 
     def set_client_options(self, **kwargs: str) -> None:
         """Update options in case they need to overriden in some cases."""
-        if kwargs.get('adapter') and IS_LINUX is False:
-            raise ValueError('The adapter option is only valid for the Linux BlueZ Backend.')
+        if kwargs.get("adapter") and IS_LINUX is False:
+            msg = "The adapter option is only valid for the Linux BlueZ Backend."
+            raise ValueError(msg)
         self._client_kwargs = {**kwargs}
 
     @contextlib.asynccontextmanager
     async def connection(self, **kwargs: str) -> AsyncIterator[EmberMug]:
-        """Helper for establishing a connection and automatically closing it."""
+        """Establish a connection and close automatically."""
         self.set_client_options(**kwargs)
         # This will happen automatically, but calling it now will give us immediate feedback
         await self._ensure_connection()
         yield self
         await self.disconnect()
```

### Comparing `python_ember_mug-0.7.0b7/ember_mug/scanner.py` & `python_ember_mug-0.8.0/ember_mug/scanner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Scanning tools for finding mugs."""
 from __future__ import annotations
 
 import asyncio
 import logging
-from typing import TYPE_CHECKING, Any, Callable
+from typing import TYPE_CHECKING, Any
 
 from bleak import BleakScanner
 
 from .consts import EMBER_BLUETOOTH_NAMES, IS_LINUX, MugCharacteristic
 
 if TYPE_CHECKING:
+    from collections.abc import Callable
+
     from bleak.backends.device import BLEDevice
     from bleak.backends.scanner import AdvertisementData
 
 
 logger = logging.getLogger(__name__)
 
 
 def build_scanner_kwargs(adapter: str | None = None) -> dict[str, Any]:
     """Add Adapter to kwargs for scanner if specified and using BlueZ."""
     if adapter and IS_LINUX is not True:
-        raise ValueError('The adapter option is only valid for the Linux BlueZ Backend.')
-    return {'adapter': adapter} if adapter else {}
+        msg = "The adapter option is only valid for the Linux BlueZ Backend."
+        raise ValueError(msg)
+    return {"adapter": adapter} if adapter else {}
 
 
 async def discover_mugs(mac: str | None = None, adapter: str | None = None, wait: int = 5) -> list[BLEDevice]:
     """Discover new mugs in pairing mode."""
     scanner_kwargs = build_scanner_kwargs(adapter)
     service_uuids = [str(uuid) for uuid in (MugCharacteristic.STANDARD_SERVICE, MugCharacteristic.TRAVEL_MUG_SERVICE)]
     async with BleakScanner(service_uuids=service_uuids, **scanner_kwargs) as scanner:
```

### Comparing `python_ember_mug-0.7.0b7/ember_mug/utils.py` & `python_ember_mug-0.8.0/ember_mug/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 
 logger = logging.getLogger(__name__)
 
 
 def decode_byte_string(data: bytes | bytearray) -> str:
     """Convert bytes to text as Ember expects."""
     if not data:
-        return ''
+        return ""
     with contextlib.suppress(ValueError):
-        b64_as_str = base64.encodebytes(data).decode("utf-8")
+        b64_as_str = base64.encodebytes(data).decode()
         return re.sub("[\r\n]", "", b64_as_str)
     logger.warning('Failed to decode bytes "%s". Forcing to string.', data)
     return str(data)
 
 
 def encode_byte_string(data: str) -> bytes:
     """Encode string from Ember Mug."""
-    return re.sub(b"[\r\n]", b"", base64.encodebytes(data.encode("utf8")))
+    return re.sub(b"[\r\n]", b"", base64.encodebytes(data.encode()))
 
 
 def bytes_to_little_int(data: bytearray | bytes) -> int:
     """Convert bytes to little int."""
     return int.from_bytes(data, byteorder="little", signed=False)
 
 
@@ -54,16 +54,16 @@
     """Log all services and all values for debugging/development."""
     logger.info("Logging all services that were discovered")
     services: dict[str, Any] = {}
     for service in client.services:
         logger.debug("[Service] %s: %s", service.uuid, service.description)
         characteristics: dict[str, Any] = {}
         services[service.uuid] = {
-            'uuid': service.uuid,
-            'characteristics': characteristics,
+            "uuid": service.uuid,
+            "characteristics": characteristics,
         }
         for characteristic in service.characteristics:
             value: bytes | BleakError | None = None
             if "read" in characteristic.properties:
                 try:
                     value = bytes(await client.read_gatt_char(characteristic.uuid))
                 except BleakError as e:
@@ -73,28 +73,28 @@
                 characteristic.uuid,
                 ",".join(characteristic.properties),
                 characteristic.description,
                 value,
             )
             descriptors: list[dict[str, Any]] = []
             characteristics[characteristic.uuid] = {
-                'uuid': characteristic.uuid,
-                'properties': characteristic.properties,
-                'value': value,
-                'descriptors': descriptors,
+                "uuid": characteristic.uuid,
+                "properties": characteristic.properties,
+                "value": value,
+                "descriptors": descriptors,
             }
             for descriptor in characteristic.descriptors:
                 value = bytes(await client.read_gatt_descriptor(descriptor.handle))
                 logger.debug(
                     "\t\t[Descriptor] %s: Handle: %s | Value: '%s'",
                     descriptor.uuid,
                     descriptor.handle,
                     value,
                 )
                 descriptors.append(
                     {
-                        'uuid': descriptor.uuid,
-                        'handle': descriptor.handle,
-                        'value': value,
+                        "uuid": descriptor.uuid,
+                        "handle": descriptor.handle,
+                        "value": value,
                     },
                 )
     return services
```

### Comparing `python_ember_mug-0.7.0b7/tests/cli/test_commands.py` & `python_ember_mug-0.8.0/tests/cli/test_commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 from __future__ import annotations
 
 from argparse import Namespace
 from collections.abc import Generator
 from typing import Any
-from unittest.mock import AsyncMock, MagicMock, Mock, patch
+from unittest.mock import AsyncMock, Mock, patch
 
 import pytest
 from bleak import BleakError, BLEDevice
 from pytest import CaptureFixture
 
 from ember_mug import EmberMug
 from ember_mug.cli.commands import EmberMugCli, discover, fetch_info, find_device, get_mug, get_mug_value
 from ember_mug.data import Model, MugData
-from tests.conftest import TEST_MAC
-
-from ..conftest import mock_connection
+from tests.conftest import TEST_MAC, mock_connection
 
 
 @pytest.fixture()
 def mock_mug_with_connection() -> Generator[AsyncMock, None, None]:
-    with patch('ember_mug.cli.commands.get_mug') as mock:
+    with patch("ember_mug.cli.commands.get_mug") as mock:
         mock_mug = AsyncMock()
         mock_mug.connection = Mock(return_value=mock_connection)
         mock.return_value = mock_mug
         yield mock_mug
 
 
 def mock_namespace(**kwargs: Any) -> Namespace:
     defaults = {
-        'imperial': False,
-        'extra': False,
-        'raw': False,
-        'debug': False,
-        'adapter': None,
+        "imperial": False,
+        "extra": False,
+        "raw": False,
+        "debug": False,
+        "adapter": None,
     }
     defaults.update(**kwargs)
     return Namespace(**defaults)
 
 
-@patch('ember_mug.cli.commands.EmberMug', spec=EmberMug)
-@patch('ember_mug.cli.commands.find_device')
+@patch("ember_mug.cli.commands.EmberMug", spec=EmberMug)
+@patch("ember_mug.cli.commands.find_device")
 async def test_get_mug(
     mock_find_device: AsyncMock,
     mock_ember_mug: AsyncMock,
     capsys: CaptureFixture,
     ble_device: BLEDevice,
 ) -> None:
     mock_find_device.return_value = ble_device
@@ -59,54 +57,54 @@
     args = mock_namespace(extra=True, raw=True)
     mug = await get_mug(args)
     assert mug is not None
     captured = capsys.readouterr()
     assert captured.out == ""
 
 
-@patch('ember_mug.cli.commands.find_mug')
+@patch("ember_mug.cli.commands.find_mug")
 async def test_find_device(mock_find_mug: AsyncMock, capsys: CaptureFixture, ble_device: BLEDevice) -> None:
     mock_find_mug.return_value = ble_device
     args = mock_namespace(mac=ble_device.address)
     device = await find_device(args)
     assert device == ble_device
     mock_find_mug.assert_called_once_with(mac=ble_device.address, adapter=None)
     captured = capsys.readouterr()
     assert captured.out == f"Found mug: {ble_device}\n"
 
     # Raw prints nothing
     args = Namespace(mac=ble_device.address, adapter=None, raw=True)
     await find_device(args)
     captured = capsys.readouterr()
-    assert captured.out == f""
+    assert captured.out == ""
 
 
-@patch('ember_mug.cli.commands.find_mug')
+@patch("ember_mug.cli.commands.find_mug")
 async def test_find_device_no_device(mock_find_mug: AsyncMock, capsys: CaptureFixture) -> None:
     mock_find_mug.return_value = None
     args = mock_namespace(mac=TEST_MAC)
     with pytest.raises(SystemExit):
         await find_device(args)
     mock_find_mug.assert_called_once_with(mac=TEST_MAC, adapter=None)
     captured = capsys.readouterr()
     assert captured.out == "No mug was found.\n"
 
 
-@patch('ember_mug.cli.commands.find_mug')
+@patch("ember_mug.cli.commands.find_mug")
 async def test_find_device_bleak_error(mock_find_mug: AsyncMock, capsys: CaptureFixture) -> None:
-    mock_find_mug.side_effect = BleakError('Test Error')
+    mock_find_mug.side_effect = BleakError("Test Error")
     args = mock_namespace(mac=TEST_MAC)
     with pytest.raises(SystemExit):
         await find_device(args)
     mock_find_mug.assert_called_once_with(mac=TEST_MAC, adapter=None)
     captured = capsys.readouterr()
     assert captured.out == "An error occurred trying to find a mug: Test Error\n"
 
 
-@patch('ember_mug.cli.commands.discover_mugs')
+@patch("ember_mug.cli.commands.discover_mugs")
 async def test_discover(mock_discover_mugs: AsyncMock, capsys: CaptureFixture, ble_device: BLEDevice) -> None:
     mock_discover_mugs.return_value = [ble_device]
     args = mock_namespace(mac=TEST_MAC)
     mugs = await discover(args)
     assert mugs == [ble_device]
     mock_discover_mugs.assert_called_once_with(mac=TEST_MAC)
     captured = capsys.readouterr()
@@ -117,37 +115,37 @@
     mugs = await discover(args)
     assert mugs == [ble_device]
     mock_discover_mugs.assert_called_once_with(mac=TEST_MAC)
     captured = capsys.readouterr()
     assert captured.out == f"{TEST_MAC}\n"
 
 
-@patch('ember_mug.cli.commands.discover_mugs')
+@patch("ember_mug.cli.commands.discover_mugs")
 async def test_discover_no_device(mock_discover_mugs: AsyncMock, capsys: CaptureFixture) -> None:
     mock_discover_mugs.return_value = []
     args = mock_namespace(mac=TEST_MAC)
     with pytest.raises(SystemExit):
         await discover(args)
     mock_discover_mugs.assert_called_once_with(mac=TEST_MAC)
     captured = capsys.readouterr()
-    assert captured.out == "No mugs were found. Be sure it is in pairing mode. Or use \"find\" if already paired.\n"
+    assert captured.out == 'No mugs were found. Be sure it is in pairing mode. Or use "find" if already paired.\n'
 
 
-@patch('ember_mug.cli.commands.discover_mugs')
+@patch("ember_mug.cli.commands.discover_mugs")
 async def test_discover_bleak_error(mock_discover_mugs: AsyncMock, capsys: CaptureFixture) -> None:
-    mock_discover_mugs.side_effect = BleakError('Test Error')
+    mock_discover_mugs.side_effect = BleakError("Test Error")
     args = mock_namespace(mac=TEST_MAC)
     with pytest.raises(SystemExit):
         await discover(args)
     mock_discover_mugs.assert_called_once_with(mac=TEST_MAC)
     captured = capsys.readouterr()
     assert captured.out == "An error occurred trying to discover mugs: Test Error\n"
 
 
-@patch('ember_mug.cli.commands.print_info')
+@patch("ember_mug.cli.commands.print_info")
 async def test_fetch_info(
     mock_print_info: AsyncMock,
     mock_mug_with_connection: AsyncMock,
     capsys: CaptureFixture,
 ) -> None:
     # Test normal
     args = mock_namespace(mac=TEST_MAC)
@@ -159,61 +157,61 @@
     # Test with Raw
     args = mock_namespace(mac=TEST_MAC, raw=True)
     await fetch_info(args)
     captured = capsys.readouterr()
     assert captured.out == ""
 
 
-@patch('ember_mug.cli.commands.print_table')
+@patch("ember_mug.cli.commands.print_table")
 async def test_get_mug_value(
     mocked_print_table: Mock,
     mock_mug_with_connection: AsyncMock,
     capsys: CaptureFixture,
 ) -> None:
-    mock_mug_with_connection.data = MugData(Model('Test'))
-    mock_mug_with_connection.data.get_formatted_attr = Mock(return_value='test')  # type: ignore[assignment]
+    mock_mug_with_connection.data = MugData(Model("Test"))
+    mock_mug_with_connection.data.get_formatted_attr = Mock(return_value="test")  # type: ignore[assignment]
     mock_mug_with_connection.get_target_temp.return_value = 55.5
-    mock_mug_with_connection.get_name.return_value = 'test'
-    args = mock_namespace(attributes=['target_temp', 'name'])
+    mock_mug_with_connection.get_name.return_value = "test"
+    args = mock_namespace(attributes=["target_temp", "name"])
     await get_mug_value(args)
     mock_mug_with_connection.get_target_temp.assert_called_once()
-    mocked_print_table.assert_called_once_with([('Target Temp', "test"), ('Mug Name', "test")])
+    mocked_print_table.assert_called_once_with([("Target Temp", "test"), ("Mug Name", "test")])
 
     mock_mug_with_connection.get_led_colour.return_value = 55.5
-    args = mock_namespace(attributes=['led_colour', 'name'], raw=True)
+    args = mock_namespace(attributes=["led_colour", "name"], raw=True)
     await get_mug_value(args)
     captured = capsys.readouterr()
     assert captured.out == "55.5\ntest\n"
 
 
 def test_ember_cli():
     cli = EmberMugCli()
-    args = cli.parser.parse_args(['find'])
-    assert args.command == 'find'
+    args = cli.parser.parse_args(["find"])
+    assert args.command == "find"
 
-    args = cli.parser.parse_args(['discover'])
-    assert args.command == 'discover'
+    args = cli.parser.parse_args(["discover"])
+    assert args.command == "discover"
 
-    args = cli.parser.parse_args(['info', '-m', TEST_MAC, '--imperial'])
-    assert args.command == 'info'
+    args = cli.parser.parse_args(["info", "-m", TEST_MAC, "--imperial"])
+    assert args.command == "info"
     assert args.mac == TEST_MAC
     assert args.imperial is True
 
-    args = cli.parser.parse_args(['poll'])
-    assert args.command == 'poll'
+    args = cli.parser.parse_args(["poll"])
+    assert args.command == "poll"
 
-    args = cli.parser.parse_args(['get', 'led-colour'])
-    assert args.command == 'get'
-    assert args.attributes == ['led-colour']
+    args = cli.parser.parse_args(["get", "led-colour"])
+    assert args.command == "get"
+    assert args.attributes == ["led-colour"]
 
-    args = cli.parser.parse_args(['set', '--name', 'TEST'])
-    assert args.command == 'set'
-    assert args.name == 'TEST'
+    args = cli.parser.parse_args(["set", "--name", "TEST"])
+    assert args.command == "set"
+    assert args.name == "TEST"
 
 
-@patch('sys.argv', ['file.py', 'find', '-m', TEST_MAC])
+@patch("sys.argv", ["file.py", "find", "-m", TEST_MAC])
 async def test_cli_run():
     cli = EmberMugCli()
     mock_find = AsyncMock()
-    with patch.object(cli, '_commands', {'find': mock_find}):
+    with patch.object(cli, "_commands", {"find": mock_find}):
         await cli.run()
     mock_find.assert_called_once()
```

### Comparing `python_ember_mug-0.7.0b7/tests/cli/test_helpers.py` & `python_ember_mug-0.8.0/tests/cli/test_helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 from textwrap import dedent
 
 import pytest
 from pytest import CaptureFixture
 
 from ember_mug import EmberMug
 from ember_mug.cli.helpers import build_sub_rows, print_changes, print_info, print_table, validate_mac
-from ember_mug.consts import EMBER_MUG, LiquidState
-from ember_mug.data import Change, Model
+from ember_mug.consts import LiquidState
+from ember_mug.data import Change
 
 
 def test_validate_mac() -> None:
     with pytest.raises(ArgumentTypeError):
-        validate_mac('potato')
-    assert validate_mac('9C:DA:8C:19:27:DA') == '9c:da:8c:19:27:da'
+        validate_mac("potato")
+    assert validate_mac("9C:DA:8C:19:27:DA") == "9c:da:8c:19:27:da"
 
 
 def test_build_sub_rows() -> None:
-    sub_rows = build_sub_rows(('Test', 'test1, test2, test3', 'test4'))
-    assert sub_rows[0][0] == 'Test'
-    assert sub_rows[0][1] == 'test1'
-    assert sub_rows[0][2] == 'test4'
-    assert sub_rows[1][0] == ''
-    assert sub_rows[1][1] == 'test2'
-    assert sub_rows[1][2] == ''
-    assert sub_rows[2][1] == 'test3'
+    sub_rows = build_sub_rows(("Test", "test1, test2, test3", "test4"))
+    assert sub_rows[0][0] == "Test"
+    assert sub_rows[0][1] == "test1"
+    assert sub_rows[0][2] == "test4"
+    assert sub_rows[1][0] == ""
+    assert sub_rows[1][1] == "test2"
+    assert sub_rows[1][2] == ""
+    assert sub_rows[2][1] == "test3"
 
 
 def test_print_changes(capsys: CaptureFixture) -> None:
     changes = [
-        Change('name', 'Mug Name', 'Test Mug'),
-        Change('liquid_level', 1, 2),
-        Change('liquid_state', LiquidState.EMPTY, LiquidState.HEATING),
-        Change('target_temp', 45, 55),
+        Change("name", "Mug Name", "Test Mug"),
+        Change("liquid_level", 1, 2),
+        Change("liquid_state", LiquidState.EMPTY, LiquidState.HEATING),
+        Change("target_temp", 45, 55),
     ]
     print_changes(changes, True)
     captured = capsys.readouterr()
     assert captured.out == dedent(
         """\
         Name changed from "Mug Name" to "Test Mug"
         Liquid Level changed from "3.33%" to "6.67%"
@@ -47,15 +47,15 @@
         """,
     )
 
 
 def test_print_table(ember_mug: EmberMug, capsys: CaptureFixture) -> None:
     print_table([])
     captured = capsys.readouterr()
-    assert captured.out == ''
+    assert captured.out == ""
 
 
 def test_print_info(ember_mug: EmberMug, capsys: CaptureFixture) -> None:
     print_info(ember_mug)
     captured = capsys.readouterr()
     assert captured.out == dedent(
         """\
```

### Comparing `python_ember_mug-0.7.0b7/tests/conftest.py` & `python_ember_mug-0.8.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pytest_asyncio
 from bleak.backends.device import BLEDevice
 
 from ember_mug import EmberMug
 from ember_mug.consts import EMBER_MUG
 from ember_mug.data import Model, MugData
 
-TEST_MAC = '32:36:a5:be:88:cb'
+TEST_MAC = "32:36:a5:be:88:cb"
 TEST_MODEL_NAME = EMBER_MUG
 
 
 class AsyncContextManager:
     """Stub for mocking."""
 
     async def __aenter__(self):
@@ -26,22 +26,22 @@
         """Close and do nothing."""
         pass
 
 
 mock_connection = MagicMock(AsyncContextManager)
 
 
-@pytest.fixture(name='ble_device')
-def ble_device_fixture() -> Generator[BLEDevice, None, None]:
-    yield BLEDevice(address=TEST_MAC, name=TEST_MODEL_NAME, details={}, rssi=1)
+@pytest.fixture(name="ble_device")
+def ble_device_fixture() -> BLEDevice:
+    return BLEDevice(address=TEST_MAC, name=TEST_MODEL_NAME, details={}, rssi=1)
 
 
-@pytest.fixture
-def mug_data(ble_device: BLEDevice) -> Generator[MugData, None, None]:
-    yield MugData(Model(ble_device.name or TEST_MODEL_NAME))
+@pytest.fixture()
+def mug_data(ble_device: BLEDevice) -> MugData:
+    return MugData(Model(ble_device.name or TEST_MODEL_NAME))
 
 
 @pytest_asyncio.fixture
 async def ember_mug(ble_device: BLEDevice) -> AsyncGenerator[EmberMug | AsyncMock, None]:
     mug = EmberMug(ble_device)
     mug._client = AsyncMock()
     yield mug
```

### Comparing `python_ember_mug-0.7.0b7/tests/test_connection.py` & `python_ember_mug-0.8.0/tests/test_connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,28 +16,28 @@
     TemperatureUnit,
     VolumeLevel,
 )
 from ember_mug.data import Colour, Model
 from ember_mug.mug import EmberMug
 
 
-@patch('ember_mug.mug.IS_LINUX', True)
+@patch("ember_mug.mug.IS_LINUX", True)
 async def test_adapter_with_bluez(ble_device: BLEDevice):
-    mug = EmberMug(ble_device, adapter='hci0')
-    assert mug._client_kwargs['adapter'] == 'hci0'
+    mug = EmberMug(ble_device, adapter="hci0")
+    assert mug._client_kwargs["adapter"] == "hci0"
 
 
-@patch('ember_mug.mug.IS_LINUX', False)
+@patch("ember_mug.mug.IS_LINUX", False)
 async def test_adapter_without_bluez(ble_device: BLEDevice):
     with pytest.raises(ValueError):
-        EmberMug(ble_device, adapter='hci0')
+        EmberMug(ble_device, adapter="hci0")
 
 
-@patch('ember_mug.mug.EmberMug.subscribe')
-@patch('ember_mug.mug.establish_connection')
+@patch("ember_mug.mug.EmberMug.subscribe")
+@patch("ember_mug.mug.establish_connection")
 async def test_connect(
     mug_subscribe: AsyncMock,
     mock_establish_connection: AsyncMock,
     ember_mug: AsyncMock,
 ) -> None:
     # Already connected
     ember_mug._client = AsyncMock()
@@ -55,16 +55,16 @@
 
     mock_establish_connection.assert_called()
     mug_subscribe.assert_called()
     assert ember_mug._client is not None
     ember_mug.disconnect.assert_called()
 
 
-@patch('ember_mug.mug.logger')
-@patch('ember_mug.mug.establish_connection')
+@patch("ember_mug.mug.logger")
+@patch("ember_mug.mug.establish_connection")
 async def test_connect_error(
     mock_establish_connection: AsyncMock,
     mock_logger: Mock,
     ember_mug: AsyncMock,
 ) -> None:
     ember_mug._client = None  # type: ignore[assignment]
     mock_establish_connection.side_effect = BleakError
@@ -72,16 +72,16 @@
         await ember_mug._ensure_connection()
     msg, device, exception = mock_logger.error.mock_calls[0].args
     assert msg == "%s: Failed to connect to the mug: %s"
     assert device == ember_mug.device
     assert isinstance(exception, BleakError)
 
 
-@patch('ember_mug.mug.logger')
-@patch('ember_mug.mug.establish_connection')
+@patch("ember_mug.mug.logger")
+@patch("ember_mug.mug.establish_connection")
 async def test_pairing_exceptions_esphome(
     mock_establish_connection: AsyncMock,
     mock_logger: Mock,
     ember_mug: AsyncMock,
 ) -> None:
     ember_mug._client.is_connected = False
     mock_client = AsyncMock()
@@ -93,20 +93,20 @@
         update_initial=AsyncMock(),
         subscribe=AsyncMock(),
     ):
         await ember_mug._ensure_connection()
 
     mock_establish_connection.assert_called_once()
     mock_logger.warning.assert_called_with(
-        'Pairing not implemented. '
-        'If your mug is still in pairing mode (blinking blue) tap the button on the bottom to exit.',
+        "Pairing not implemented. "
+        "If your mug is still in pairing mode (blinking blue) tap the button on the bottom to exit.",
     )
 
 
-@patch('ember_mug.mug.establish_connection')
+@patch("ember_mug.mug.establish_connection")
 async def test_pairing_exceptions(
     mock_establish_connection: AsyncMock,
     ember_mug: AsyncMock,
 ) -> None:
     mock_client = AsyncMock()
     mock_client.pair.side_effect = BleakError
     mock_establish_connection.return_value = mock_client
@@ -130,48 +130,48 @@
     mock_client.is_connected = True
     ember_mug._client = mock_client
     await ember_mug.disconnect()
     assert ember_mug._client is None
     mock_client.disconnect.assert_called()
 
 
-@patch('ember_mug.mug.logger')
+@patch("ember_mug.mug.logger")
 def test_disconnect_callback(mock_logger: Mock, ember_mug: AsyncMock) -> None:
     ember_mug._expected_disconnect = True
     ember_mug._disconnect_callback(AsyncMock())
     mock_logger.debug.assert_called_with("Disconnect callback called")
     mock_logger.reset_mock()
 
     ember_mug._expected_disconnect = False
     ember_mug._disconnect_callback(AsyncMock())
     mock_logger.warning.assert_called_with("Unexpectedly disconnected")
 
 
-@patch('ember_mug.mug.logger')
+@patch("ember_mug.mug.logger")
 async def test_read(
     mock_logger: Mock,
     ember_mug: AsyncMock,
 ) -> None:
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'TEST'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"TEST"
         await ember_mug._read(MugCharacteristic.MUG_NAME)
         ember_mug._client.read_gatt_char.assert_called_with(
             MugCharacteristic.MUG_NAME.uuid,
         )
         mock_logger.debug.assert_called_with(
             "Read attribute '%s' with value '%s'",
             MugCharacteristic.MUG_NAME,
-            b'TEST',
+            b"TEST",
         )
 
 
-@patch('ember_mug.mug.logger')
+@patch("ember_mug.mug.logger")
 async def test_write(mock_logger: Mock, ember_mug: AsyncMock) -> None:
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        test_name = bytearray(b'TEST')
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        test_name = bytearray(b"TEST")
         await ember_mug._write(
             MugCharacteristic.MUG_NAME,
             test_name,
         )
         ember_mug._client.write_gatt_char.assert_called_with(
             MugCharacteristic.MUG_NAME.uuid,
             test_name,
@@ -198,318 +198,317 @@
         assert data == test_name
         assert char == MugCharacteristic.MUG_NAME
         assert isinstance(exception, BleakError)
 
 
 def test_set_device(ember_mug: AsyncMock) -> None:
     new_device = BLEDevice(
-        address='BA:36:a5:be:88:cb',
-        name='Ember Ceramic Mug',
+        address="BA:36:a5:be:88:cb",
+        name="Ember Ceramic Mug",
         details={},
         rssi=1,
     )
     assert ember_mug.device.address != new_device.address
     ember_mug.set_device(new_device)
     assert ember_mug.device.address == new_device.address
 
 
 async def test_get_mug_meta(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'Yw====-ABCDEFGHIJ'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"Yw====-ABCDEFGHIJ"
         meta = await ember_mug.get_meta()
-        assert meta.mug_id == 'WXc9PT09'
-        assert meta.serial_number == 'ABCDEFGHIJ'
+        assert meta.mug_id == "WXc9PT09"
+        assert meta.serial_number == "ABCDEFGHIJ"
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.MUG_ID.uuid)
 
 
 async def test_get_mug_battery(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'5\x01'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"5\x01"
         battery = await ember_mug.get_battery()
         assert battery.percent == 53.00
         assert battery.on_charging_base is True
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.BATTERY.uuid)
 
 
 async def test_get_mug_led_colour(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'\xf4\x00\xa1\xff'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"\xf4\x00\xa1\xff"
         colour = await ember_mug.get_led_colour()
-        assert colour.as_hex() == '#f400a1'
+        assert colour.as_hex() == "#f400a1"
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.LED.uuid)
 
 
 async def test_set_mug_led_colour(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
         await ember_mug.set_led_colour(Colour(244, 0, 161))
         ember_mug._ensure_connection.assert_called_once()
         ember_mug._client.write_gatt_char.assert_called_once_with(
             MugCharacteristic.LED.uuid,
-            bytearray(b'\xf4\x00\xa1\xff'),
+            bytearray(b"\xf4\x00\xa1\xff"),
         )
 
 
 async def test_set_volume_level_travel_mug(ember_mug: AsyncMock):
     ember_mug.is_travel_mug = True
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
         await ember_mug.set_volume_level(VolumeLevel.HIGH)
         ember_mug._ensure_connection.assert_called_once()
         ember_mug._client.write_gatt_char.assert_called_once_with(
             MugCharacteristic.VOLUME.uuid,
-            bytearray(b'\02'),
+            bytearray(b"\02"),
         )
         ember_mug._ensure_connection.reset_mock()
         ember_mug._client.write_gatt_char.reset_mock()
 
         await ember_mug.set_volume_level(0)
         ember_mug._ensure_connection.assert_called_once()
         ember_mug._client.write_gatt_char.assert_called_once_with(
             MugCharacteristic.VOLUME.uuid,
-            bytearray(b'\00'),
+            bytearray(b"\00"),
         )
 
 
 async def test_set_volume_level_mug(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
         with pytest.raises(NotImplementedError):
             await ember_mug.set_volume_level(VolumeLevel.HIGH)
         ember_mug._ensure_connection.assert_not_called()
         ember_mug._client.write_gatt_char.assert_not_called()
 
 
 async def test_get_mug_target_temp(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'\xcd\x15'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"\xcd\x15"
         assert (await ember_mug.get_target_temp()) == 55.81
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.TARGET_TEMPERATURE.uuid)
 
 
 async def test_set_mug_target_temp(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
         await ember_mug.set_target_temp(55.81)
         ember_mug._ensure_connection.assert_called_once()
         ember_mug._client.write_gatt_char.assert_called_once_with(
             MugCharacteristic.TARGET_TEMPERATURE.uuid,
-            bytearray(b'\xcd\x15'),
+            bytearray(b"\xcd\x15"),
         )
 
 
 async def test_get_mug_current_temp(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'\xcd\x15'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"\xcd\x15"
         assert (await ember_mug.get_current_temp()) == 55.81
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.CURRENT_TEMPERATURE.uuid)
 
 
 async def test_get_mug_liquid_level(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'\n'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"\n"
         assert (await ember_mug.get_liquid_level()) == 10
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.LIQUID_LEVEL.uuid)
 
 
 async def test_get_mug_liquid_state(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'\x06'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"\x06"
         assert (await ember_mug.get_liquid_state()) == 6
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.LIQUID_STATE.uuid)
 
 
 async def test_get_mug_name(ember_mug):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'Mug Name'
-        assert (await ember_mug.get_name()) == 'Mug Name'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"Mug Name"
+        assert (await ember_mug.get_name()) == "Mug Name"
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.MUG_NAME.uuid)
 
 
 async def test_set_mug_name(ember_mug):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        with pytest.raises(ValueError):
-            await ember_mug.set_name('Hé!')
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()), pytest.raises(ValueError):
+        await ember_mug.set_name("Hé!")
 
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        await ember_mug.set_name('Mug name')
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        await ember_mug.set_name("Mug name")
         ember_mug._ensure_connection.assert_called()
         ember_mug._client.write_gatt_char.assert_called_once_with(
             MugCharacteristic.MUG_NAME.uuid,
-            bytearray(b'Mug name'),
+            bytearray(b"Mug name"),
         )
 
 
 async def test_get_mug_udsk(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'abcd12345'
-        assert (await ember_mug.get_udsk()) == 'YWJjZDEyMzQ1'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"abcd12345"
+        assert (await ember_mug.get_udsk()) == "YWJjZDEyMzQ1"
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.UDSK.uuid)
 
 
 async def test_set_mug_udsk(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        await ember_mug.set_udsk('abcd12345')
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        await ember_mug.set_udsk("abcd12345")
         ember_mug._ensure_connection.assert_called_once()
         ember_mug._client.write_gatt_char.assert_called_once_with(
             MugCharacteristic.UDSK.uuid,
-            bytearray(b'YWJjZDEyMzQ1'),
+            bytearray(b"YWJjZDEyMzQ1"),
         )
 
 
 async def test_get_mug_dsk(ember_mug):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'abcd12345'
-        assert (await ember_mug.get_dsk()) == 'YWJjZDEyMzQ1'
-        ember_mug._client.read_gatt_char.return_value = b'something else'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"abcd12345"
+        assert (await ember_mug.get_dsk()) == "YWJjZDEyMzQ1"
+        ember_mug._client.read_gatt_char.return_value = b"something else"
         assert (await ember_mug.get_dsk()) == "c29tZXRoaW5nIGVsc2U="
         ember_mug._client.read_gatt_char.assert_called_with(MugCharacteristic.DSK.uuid)
 
 
 async def test_get_mug_temperature_unit(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'\x01'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"\x01"
         assert (await ember_mug.get_temperature_unit()) == TemperatureUnit.FAHRENHEIT
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.TEMPERATURE_UNIT.uuid)
         ember_mug._client.read_gatt_char.reset_mock()
-        ember_mug._client.read_gatt_char.return_value = b'\x00'
+        ember_mug._client.read_gatt_char.return_value = b"\x00"
         assert (await ember_mug.get_temperature_unit()) == TemperatureUnit.CELSIUS
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.TEMPERATURE_UNIT.uuid)
 
 
 async def test_set_mug_temperature_unit(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
         await ember_mug.set_temperature_unit(TemperatureUnit.CELSIUS)
         ember_mug._ensure_connection.assert_called_once()
         ember_mug._client.write_gatt_char.assert_called_once_with(
             MugCharacteristic.TEMPERATURE_UNIT.uuid,
-            bytearray(b'\x00'),
+            bytearray(b"\x00"),
         )
 
 
 async def test_mug_ensure_correct_unit(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
         ember_mug.data.temperature_unit = TemperatureUnit.CELSIUS
         ember_mug.data.use_metric = True
         ember_mug.set_temperature_unit = AsyncMock(return_value=None)
         await ember_mug.ensure_correct_unit()
         ember_mug.set_temperature_unit.assert_not_called()
         ember_mug.data.temperature_unit = TemperatureUnit.FAHRENHEIT
         await ember_mug.ensure_correct_unit()
         ember_mug.set_temperature_unit.assert_called_with(TemperatureUnit.CELSIUS)
 
 
 async def test_get_mug_battery_voltage(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'\x01'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"\x01"
         assert (await ember_mug.get_battery_voltage()) == 1
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.CONTROL_REGISTER_DATA.uuid)
 
 
 async def test_get_mug_date_time_zone(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'c\x0f\xf6\x00'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"c\x0f\xf6\x00"
         date_time = await ember_mug.get_date_time_zone()
         assert date_time.timestamp() == 1661990400.0
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.DATE_TIME_AND_ZONE.uuid)
 
 
 async def test_read_firmware(ember_mug: AsyncMock):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug._client.read_gatt_char.return_value = b'c\x01\x80\x00\x12\x00'
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug._client.read_gatt_char.return_value = b"c\x01\x80\x00\x12\x00"
         firmware = await ember_mug.get_firmware()
         assert firmware.version == 355
         assert firmware.hardware == 128
         assert firmware.bootloader == 18
         ember_mug._client.read_gatt_char.assert_called_once_with(MugCharacteristic.FIRMWARE.uuid)
 
 
 async def test_mug_update_initial(ember_mug):
     no_extra = INITIAL_ATTRS - EXTRA_ATTRS
 
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
         ember_mug._update_multiple = AsyncMock(return_value={})
         ember_mug.data.model = Model(EMBER_MUG, include_extra=False)
         assert (await ember_mug.update_initial()) == {}
         ember_mug._update_multiple.assert_called_once_with(no_extra)
 
     # Try with extra
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
         ember_mug._update_multiple.reset_mock()
         ember_mug.data.model = Model(EMBER_MUG, include_extra=True)
         assert (await ember_mug.update_initial()) == {}
         ember_mug._update_multiple.assert_called_once_with(INITIAL_ATTRS)
 
 
 async def test_mug_update_all(ember_mug):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
         ember_mug._update_multiple = AsyncMock(return_value={})
         assert (await ember_mug.update_all()) == {}
         ember_mug._update_multiple.assert_called_once_with(UPDATE_ATTRS - EXTRA_ATTRS)
 
     # Try with extras
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
         ember_mug._update_multiple.reset_mock()
         ember_mug._update_attrs = UPDATE_ATTRS
         assert (await ember_mug.update_all()) == {}
         ember_mug._update_multiple.assert_called_once_with(UPDATE_ATTRS)
 
 
 async def test_mug_update_multiple(ember_mug):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
-        ember_mug.get_name = AsyncMock(return_value='name')
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
+        ember_mug.get_name = AsyncMock(return_value="name")
         ember_mug.data.update_info = AsyncMock()
-        await ember_mug._update_multiple(('name',))
-        ember_mug.data.update_info.assert_called_once_with(name='name')
+        await ember_mug._update_multiple(("name",))
+        ember_mug.data.update_info.assert_called_once_with(name="name")
 
 
 async def test_mug_update_queued_attributes(ember_mug):
-    with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
+    with patch.object(ember_mug, "_ensure_connection", AsyncMock()):
         ember_mug._queued_updates = set()
         assert (await ember_mug.update_queued_attributes()) == []
-        ember_mug.get_name = AsyncMock(return_value='name')
+        ember_mug.get_name = AsyncMock(return_value="name")
         ember_mug.data.update_info = AsyncMock()
-        ember_mug._queued_updates = {'name'}
+        ember_mug._queued_updates = {"name"}
         await ember_mug.update_queued_attributes()
-        ember_mug.data.update_info.assert_called_once_with(name='name')
+        ember_mug.data.update_info.assert_called_once_with(name="name")
 
 
 def test_mug_notify_callback(ember_mug: EmberMug) -> None:
     gatt_char = AsyncMock()
-    ember_mug._notify_callback(gatt_char, bytearray(b'\x01'))
-    ember_mug._notify_callback(gatt_char, bytearray(b'\x02'))
+    ember_mug._notify_callback(gatt_char, bytearray(b"\x01"))
+    ember_mug._notify_callback(gatt_char, bytearray(b"\x02"))
     assert 2 in ember_mug._latest_events
-    ember_mug._notify_callback(gatt_char, bytearray(b'\x04'))
+    ember_mug._notify_callback(gatt_char, bytearray(b"\x04"))
     assert 4 in ember_mug._latest_events
-    ember_mug._notify_callback(gatt_char, bytearray(b'\x05'))
+    ember_mug._notify_callback(gatt_char, bytearray(b"\x05"))
     assert 5 in ember_mug._latest_events
-    ember_mug._notify_callback(gatt_char, bytearray(b'\x06'))
+    ember_mug._notify_callback(gatt_char, bytearray(b"\x06"))
     assert 6 in ember_mug._latest_events
-    ember_mug._notify_callback(gatt_char, bytearray(b'\x07'))
+    ember_mug._notify_callback(gatt_char, bytearray(b"\x07"))
     assert 7 in ember_mug._latest_events
-    ember_mug._notify_callback(gatt_char, bytearray(b'\x08'))
+    ember_mug._notify_callback(gatt_char, bytearray(b"\x08"))
     assert 8 in ember_mug._latest_events
     callback = Mock()
     second_callback = Mock()
     unregister = ember_mug.register_callback(callback)
     second_unregister = ember_mug.register_callback(second_callback)
     repeat_unregister = ember_mug.register_callback(callback)
     assert unregister is repeat_unregister
     assert unregister is not second_unregister
 
     assert callback in ember_mug._callbacks
-    ember_mug._notify_callback(gatt_char, bytearray(b'\x09'))
+    ember_mug._notify_callback(gatt_char, bytearray(b"\x09"))
     assert 9 in ember_mug._latest_events
     callback.assert_not_called()
     assert ember_mug._queued_updates == {
         "battery",
         "target_temp",
         "current_temp",
         "liquid_level",
         "liquid_state",
         "battery_voltage",
     }
     ember_mug._latest_events = {}
-    ember_mug._notify_callback(gatt_char, bytearray(b'\x02'))
+    ember_mug._notify_callback(gatt_char, bytearray(b"\x02"))
     callback.assert_called_once()
     callback.reset_mock()
-    ember_mug._notify_callback(gatt_char, bytearray(b'\x02'))
+    ember_mug._notify_callback(gatt_char, bytearray(b"\x02"))
     callback.assert_not_called()
     # Remove callback
     unregister()
     assert callback not in ember_mug._callbacks
```

### Comparing `python_ember_mug-0.7.0b7/tests/test_consts.py` & `python_ember_mug-0.8.0/tests/test_consts.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.7.0b7/tests/test_data.py` & `python_ember_mug-0.8.0/tests/test_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,75 @@
 """Tests for `ember_mug.data`."""
 from __future__ import annotations
 
-from ember_mug.consts import EMBER_CUP, EMBER_MUG, EMBER_TRAVEL_MUG
+from ember_mug.consts import EMBER_CUP, EMBER_MUG, EMBER_TRAVEL_MUG, EMBER_TRAVEL_MUG_2
 from ember_mug.data import BatteryInfo, Change, Colour, Model, MugFirmwareInfo, MugMeta
 
 
 def test_change() -> None:
-    change = Change('mug_name', 'EMBER', 'Test Mug')
+    change = Change("mug_name", "EMBER", "Test Mug")
     expected = 'Mug Name changed from "EMBER" to "Test Mug"'
     assert str(change) == expected
 
 
 def test_battery_info() -> None:
-    battery_info = BatteryInfo.from_bytes(b'5\x01')
+    battery_info = BatteryInfo.from_bytes(b"5\x01")
     assert battery_info.percent == 53.00
     assert battery_info.on_charging_base is True
-    assert str(battery_info) == '53.0%, on charging base'
+    assert str(battery_info) == "53.0%, on charging base"
 
 
 def test_colour() -> None:
-    colour = Colour.from_bytes(b'\xf4\x00\xa1\xff')
-    assert colour.as_bytearray() == b'\xf4\x00\xa1'
-    assert colour.as_hex() == '#f400a1'
-    assert str(colour) == '#f400a1'
+    colour = Colour(*bytearray(b"\xf4\x00\xa1\xff"))
+    assert colour.as_bytearray() == b"\xf4\x00\xa1\xff"
+    assert colour.brightness == 255
+    assert colour.as_hex() == "#f400a1"
+    assert str(colour) == "#f400a1"
+    colour = Colour(100, 100, 100, 100)
+    assert colour.brightness == 100
+    assert colour.as_bytearray() == b"dddd"
 
 
 def test_mug_firmware_info() -> None:
-    firmware = MugFirmwareInfo.from_bytes(b'c\x01\x80\x00\x12\x00')
+    firmware = MugFirmwareInfo.from_bytes(b"c\x01\x80\x00\x12\x00")
     assert firmware.version == 355
     assert firmware.hardware == 128
     assert firmware.bootloader == 18
-    assert str(firmware) == 'Version: 355, Hardware: 128, Bootloader: 18'
+    assert str(firmware) == "Version: 355, Hardware: 128, Bootloader: 18"
 
 
 def test_mug_meta() -> None:
-    meta = MugMeta.from_bytes(b'Yw====-ABCDEFGHIJ')
-    assert meta.mug_id == 'WXc9PT09'
-    assert meta.serial_number == 'ABCDEFGHIJ'
-    assert str(meta) == 'Mug ID: WXc9PT09, Serial Number: ABCDEFGHIJ'
+    meta = MugMeta.from_bytes(b"Yw====-ABCDEFGHIJ")
+    assert meta.mug_id == "WXc9PT09"
+    assert meta.serial_number == "ABCDEFGHIJ"
+    assert str(meta) == "Mug ID: WXc9PT09, Serial Number: ABCDEFGHIJ"
 
 
 def test_mug_model() -> None:
     mug = Model(EMBER_MUG)
     assert mug.is_travel_mug is False
     assert mug.is_travel_mug is False
-    assert 'udsk' not in mug.initial_attributes
-    assert 'name' in mug.update_attributes
-    assert 'name' in mug.attribute_labels
-    assert 'battery_voltage' not in mug.update_attributes
+    assert "udsk" not in mug.initial_attributes
+    assert "name" in mug.update_attributes
+    assert "name" in mug.attribute_labels
+    assert "battery_voltage" not in mug.update_attributes
     mug_with_extra = Model(EMBER_MUG, include_extra=True)
-    assert 'udsk' in mug_with_extra.initial_attributes
-    assert 'battery_voltage' not in mug.update_attributes
+    assert "udsk" in mug_with_extra.initial_attributes
+    assert "battery_voltage" not in mug.update_attributes
+
+    travel_mug = Model(EMBER_TRAVEL_MUG_2)
+    assert travel_mug.is_travel_mug is True
+    assert travel_mug.is_cup is False
 
     travel_mug = Model(EMBER_TRAVEL_MUG)
     assert travel_mug.is_travel_mug is True
     assert travel_mug.is_cup is False
-    assert 'name' in travel_mug.update_attributes
-    assert 'name' in travel_mug.attribute_labels
-    assert 'volume_level' in travel_mug.attribute_labels
+    assert "name" in travel_mug.update_attributes
+    assert "name" in travel_mug.attribute_labels
+    assert "volume_level" in travel_mug.attribute_labels
 
     cup = Model(EMBER_CUP)
     assert cup.is_cup is True
     assert cup.is_travel_mug is False
-    assert 'name' not in cup.update_attributes
-    assert 'name' not in cup.attribute_labels
-    assert 'volume_level' not in cup.update_attributes
+    assert "name" not in cup.update_attributes
+    assert "name" not in cup.attribute_labels
+    assert "volume_level" not in cup.update_attributes
```

### Comparing `python_ember_mug-0.7.0b7/tests/test_formatting.py` & `python_ember_mug-0.8.0/tests/test_formatting.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 def test_format_liquid_level() -> None:
     assert format_liquid_level(5) == "16.67%"
     assert format_liquid_level(6) == "20.00%"
 
 
 def test_format_temp() -> None:
-    assert format_temp(25.445) == '25.45°C'
-    assert format_temp(36.443, metric=False) == '36.44°F'
+    assert format_temp(25.445) == "25.45°C"
+    assert format_temp(36.443, metric=False) == "36.44°F"
```

### Comparing `python_ember_mug-0.7.0b7/tests/test_mug_data.py` & `python_ember_mug-0.8.0/tests/test_mug_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,59 +4,59 @@
 from typing import Any
 
 from ember_mug.consts import EMBER_MUG, LiquidState, TemperatureUnit
 from ember_mug.data import BatteryInfo, Change, Colour, Model, MugData, MugFirmwareInfo, MugMeta
 
 
 def test_mug_formatting(mug_data: MugData) -> None:
-    meta = MugMeta('A', 'ABCDEF')
+    meta = MugMeta("A", "ABCDEF")
     battery = BatteryInfo(35.46, False)
     firmware = MugFirmwareInfo(12, 35, 55)
     colour = Colour(244, 0, 161)
     mug_data.update_info(
-        name='Mug Name',
+        name="Mug Name",
         meta=meta,
         battery=battery,
         firmware=firmware,
         led_colour=colour,
         liquid_state=LiquidState.HEATING,
         liquid_level=5,
         current_temp=25,
         target_temp=55,
-        dsk='dsk',
-        udsk='udsk',
+        dsk="dsk",
+        udsk="udsk",
         date_time_zone=None,
         battery_voltage=0.1,
     )
     assert mug_data.meta_display == "Serial Number: ABCDEF"
     mug_data.model = Model(EMBER_MUG, include_extra=True)
     assert mug_data.meta_display == "Mug ID: A, Serial Number: ABCDEF"
     assert mug_data.led_colour_display == "#f400a1"
     assert mug_data.liquid_state_display == "Heating"
     assert mug_data.liquid_level_display == "16.67%"
     assert mug_data.current_temp_display == "25.00°C"
     assert mug_data.target_temp_display == "55.00°C"
     basic_info: dict[str, Any] = {
-        'Mug Name': 'Mug Name',
-        'Meta': "Serial Number: ABCDEF",
-        'Battery': battery,
-        'Firmware': firmware,
-        'LED Colour': "#f400a1",
-        'Liquid State': "Heating",
-        'Liquid Level': "16.67%",
-        'Current Temp': "25.00°C",
-        'Target Temp': "55.00°C",
-        'Use Metric': True,
+        "Mug Name": "Mug Name",
+        "Meta": "Serial Number: ABCDEF",
+        "Battery": battery,
+        "Firmware": firmware,
+        "LED Colour": "#f400a1",
+        "Liquid State": "Heating",
+        "Liquid Level": "16.67%",
+        "Current Temp": "25.00°C",
+        "Target Temp": "55.00°C",
+        "Use Metric": True,
     }
     assert mug_data.formatted == {
         **basic_info,
-        'Meta': "Mug ID: A, Serial Number: ABCDEF",
-        'DSK': "dsk",
-        'UDSK': "udsk",
-        'Date Time + Time Zone': None,
+        "Meta": "Mug ID: A, Serial Number: ABCDEF",
+        "DSK": "dsk",
+        "UDSK": "udsk",
+        "Date Time + Time Zone": None,
     }
     mug_data.model = Model(EMBER_MUG, include_extra=False)
     assert mug_data.formatted == basic_info
 
 
 def test_update_info(mug_data: MugData) -> None:
     mug_data.current_temp = 55
@@ -64,39 +64,39 @@
     mug_data.led_colour = Colour(255, 0, 0)
     changes = mug_data.update_info(
         current_temp=55,
         target_temp=68,
         led_colour=Colour(0, 255, 0),
     )
     assert changes == [
-        Change('target_temp', 55, 68),
-        Change('led_colour', Colour(255, 0, 0), Colour(0, 255, 0)),
+        Change("target_temp", 55, 68),
+        Change("led_colour", Colour(255, 0, 0), Colour(0, 255, 0)),
     ]
 
 
 def test_mug_dict(mug_data: MugData) -> None:
-    mug_data.update_info(meta=MugMeta('test_id', 'serial number'))
+    mug_data.update_info(meta=MugMeta("test_id", "serial number"))
     assert mug_data.as_dict() == {
-        'model': {'include_extra': False, 'name': 'Ember Ceramic Mug'},
-        'use_metric': True,
-        'battery': None,
-        'battery_voltage': None,
-        'current_temp': 0.0,
-        'current_temp_display': '0.00°C',
-        'date_time_zone': None,
-        'dsk': '',
-        'firmware': None,
-        'led_colour': Colour(red=255, green=255, blue=255),
-        'led_colour_display': '#ffffff',
-        'liquid_level': 0,
-        'liquid_level_display': '0.00%',
-        'liquid_state': LiquidState.UNKNOWN,
-        'liquid_state_display': 'Unknown',
-        'meta': {'mug_id': 'test_id', 'serial_number': 'serial number'},
-        'meta_display': 'Serial Number: serial number',
-        'name': '',
-        'target_temp': 0.0,
-        'target_temp_display': '0.00°C',
-        'temperature_unit': TemperatureUnit.CELSIUS,
-        'udsk': '',
-        'volume_level': None,
+        "model": {"include_extra": False, "name": "Ember Ceramic Mug"},
+        "use_metric": True,
+        "battery": None,
+        "battery_voltage": None,
+        "current_temp": 0.0,
+        "current_temp_display": "0.00°C",
+        "date_time_zone": None,
+        "dsk": "",
+        "firmware": None,
+        "led_colour": Colour(red=255, green=255, blue=255),
+        "led_colour_display": "#ffffff",
+        "liquid_level": 0,
+        "liquid_level_display": "0.00%",
+        "liquid_state": LiquidState.UNKNOWN,
+        "liquid_state_display": "Unknown",
+        "meta": {"mug_id": "test_id", "serial_number": "serial number"},
+        "meta_display": "Serial Number: serial number",
+        "name": "",
+        "target_temp": 0.0,
+        "target_temp_display": "0.00°C",
+        "temperature_unit": TemperatureUnit.CELSIUS,
+        "udsk": "",
+        "volume_level": None,
     }
```

### Comparing `python_ember_mug-0.7.0b7/tests/test_scanner.py` & `python_ember_mug-0.8.0/tests/test_scanner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 from unittest.mock import AsyncMock, patch
 
 import pytest
 from bleak.backends.device import BLEDevice
 
 from ember_mug.scanner import build_find_filter, build_scanner_kwargs, discover_mugs, find_mug
 
-MUG_1 = BLEDevice(address='32:36:a5:be:88:cb', name='Ember Ceramic Mug', details={}, rssi=1)
-MUG_2 = BLEDevice(address='9c:da:8c:19:27:da', name='Ember Ceramic Mug', details={}, rssi=1)
+MUG_1 = BLEDevice(address="32:36:a5:be:88:cb", name="Ember Ceramic Mug", details={}, rssi=1)
+MUG_2 = BLEDevice(address="9c:da:8c:19:27:da", name="Ember Ceramic Mug", details={}, rssi=1)
 EXAMPLE_MUGS = [MUG_1, MUG_2]
 
 
-@patch('ember_mug.scanner.IS_LINUX', True)
+@patch("ember_mug.scanner.IS_LINUX", True)
 def test_build_scanner_kwargs_linux() -> None:
     assert build_scanner_kwargs() == {}
-    assert build_scanner_kwargs(adapter='hci0') == {'adapter': 'hci0'}
+    assert build_scanner_kwargs(adapter="hci0") == {"adapter": "hci0"}
 
 
-@patch('ember_mug.scanner.IS_LINUX', False)
+@patch("ember_mug.scanner.IS_LINUX", False)
 def test_build_scanner_kwargs_other() -> None:
     with pytest.raises(ValueError):
-        assert build_scanner_kwargs(adapter='hci0')
+        assert build_scanner_kwargs(adapter="hci0")
 
 
-@patch('asyncio.sleep')
+@patch("asyncio.sleep")
 @patch("ember_mug.scanner.BleakScanner")
 async def test_discover_mugs(mock_scanner: AsyncMock, mock_sleep: AsyncMock) -> None:
     mock_scanner.return_value.__aenter__.return_value.discovered_devices = EXAMPLE_MUGS
     mugs = await discover_mugs()
     assert len(mugs) == 2
-    mugs = await discover_mugs(mac='32:36:a5:be:88:cb')
+    mugs = await discover_mugs(mac="32:36:a5:be:88:cb")
     assert len(mugs) == 1
-    assert mugs[0].address == '32:36:a5:be:88:cb'
+    assert mugs[0].address == "32:36:a5:be:88:cb"
     assert mock_sleep.called_with(delay=5)
 
 
 @patch(
     "bleak.BleakScanner.find_device_by_filter",
     return_value=MUG_1,
 )
 async def test_find_mug(mock_find_device_by_filter: AsyncMock) -> None:
     # Without filter
     mug = await find_mug()
     assert mug is not None
     assert mug.name == "Ember Ceramic Mug"
-    assert mug.address == '32:36:a5:be:88:cb'
+    assert mug.address == "32:36:a5:be:88:cb"
     # With Filter
-    mug = await find_mug(mac='32:36:a5:be:88:cb')
+    mug = await find_mug(mac="32:36:a5:be:88:cb")
     assert mug is not None
     assert mug.name == "Ember Ceramic Mug"
-    assert mug.address == '32:36:a5:be:88:cb'
+    assert mug.address == "32:36:a5:be:88:cb"
     mock_find_device_by_filter.assert_called()
 
 
 def test_build_find_filter() -> None:
-    mac_filter = build_find_filter(mac='32:36:a5:be:88:cb')
+    mac_filter = build_find_filter(mac="32:36:a5:be:88:cb")
     assert mac_filter(MUG_1, None) is True
     assert mac_filter(MUG_2, None) is False
```

### Comparing `python_ember_mug-0.7.0b7/PKG-INFO` & `python_ember_mug-0.8.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,60 @@
-Metadata-Version: 2.1
-Name: python-ember-mug
-Version: 0.7.0b7
-Summary: Python Library for Ember Mugs.
-Home-page: https://github.com/sopelj/python-ember-mug
-License: MIT
-Author: Jesse Sopel
-Author-email: jesse.sopel@gmail.com
-Requires-Python: >=3.9,<3.12
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: build
-Provides-Extra: dev
-Provides-Extra: doc
-Provides-Extra: test
-Requires-Dist: bleak (>=0.19.5)
-Requires-Dist: bleak-retry-connector (>=2.13.0)
-Project-URL: Bug Tracker, https://github.com/sopelj/python-ember-mug/issues
-Project-URL: Changelog, https://github.com/sopelj/python-ember-mug/blob/main/CHANGELOG.md
-Description-Content-Type: text/markdown
-
 # Python Ember Mug
 
 [![pypi](https://img.shields.io/pypi/v/python-ember-mug.svg)](https://pypi.org/project/python-ember-mug/)
 [![python](https://img.shields.io/pypi/pyversions/python-ember-mug.svg)](https://pypi.org/project/python-ember-mug/)
-[![Build Status](https://github.com/sopelj/python-ember-mug/actions/workflows/dev.yml/badge.svg)](https://github.com/sopelj/python-ember-mug/actions/workflows/dev.yml)
+[![Build Status](https://github.com/sopelj/python-ember-mug/actions/workflows/tests.yml/badge.svg)](https://github.com/sopelj/python-ember-mug/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/sopelj/python-ember-mug/branch/main/graphs/badge.svg)](https://codecov.io/github/sopelj/python-ember-mug)
-![Project Maintenance](https://img.shields.io/maintenance/yes/2023.svg?style=for-the-badge)
+![Project Maintenance](https://img.shields.io/maintenance/yes/2023.svg)
+[![Maintainer](https://img.shields.io/badge/maintainer-%40sopelj-blue.svg)](https://github.com/sopelj)
+[![License](https://img.shields.io/github/license/sopelj/python-ember-mug.svg)](LICENSE)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen)](https://github.com/pre-commit/pre-commit)
 
-Python Library for interacting with Ember Mugs over Bluetooth
+Python Library for interacting with Ember Mugs, Cups and Travel Mugs via Bluetooth
 
 * Documentation: <https://sopelj.github.io/python-ember-mug>
 * GitHub: <https://github.com/sopelj/python-ember-mug>
 * PyPI: <https://pypi.org/project/python-ember-mug/>
-* Free software: MIT
 
 ## Summary
 
 This is an *unofficial* library to attempt to interact with Ember Mugs via Bluetooth.
 This was created for use with my [Home Assistant integration](https://github.com/sopelj/hass-ember-mug-component),
 but could be useful separately and has a simple CLI interface too.
 
-**Note**: Confirmed working with the standard Ember Mug (1 and 2), Ember Cup (2) and Travel Mug (1). If you have another device, and it works or doesn't, please let me know.
+| Device       | Tested  |
+|--------------|---------|
+| Mug          | ✓       |
+| Mug 2        | ✓       |
+| Cup          | ✓       |
+| Travel Mug   | ✓       |
+| Travel Mug 2 | ✓       |
 
 ## Features
 
 * Finding devices
 * Connecting to devices
-* Reading Information (Colour, temp, liquid level, etc.)
-* Writing (Desired temp, colour, temperature unit)*
-* Polling for changes
+* Reading/Writing most values
+* Poll for changes
+
+Attributes by device:
+
+| Attribute           | Mug | Cup | Travel Mug | Description                                   |
+|---------------------|-----|-----|------------|-----------------------------------------------|
+| Name                | R/W | N/A | R          | Name to give device                           |
+| LED Colour          | R/W | R/W | N/A        | Colour of front LED                           |
+| Current Temperature | R   | R   | R          | Current temperature of the liquid in the mug  |
+| Target Temperature  | R/W | R/W | R/W        | Desired temperature for the liquid            |
+| Temperature Unit    | R/W | R/W | R/W        | Internal temperature unit for the app (C/F)   |
+| Liquid Level        | R   | R   | R          | Approximate level of the liquid in the device |
+| Volume level        | N/A | N/A | R/W        | Volume of the button press beep               |
+| Battery Percent     | R   | R   | R          | Current battery level                         |
+| On Charger          | R   | R   | R          | Device is on it's charger                     |
 
-*** Writing only works if the devices has been set up in the app previously
+*** Writing may only work if the devices has been set up in the app previously
 
 ## Usage
 
 ### Python
 
 ```python
 from ember_mug.scanner import find_mug, discover_mugs
@@ -98,45 +88,60 @@
 ember-mug poll  # fetches info and keeps listening for notifications
 ember-mug get name target-temp  # Prints name and target temp of mug
 ember-mug set --name "My mug" --target-temp 56.8  # Sets the name and target temp to specified values
 ```
 
 Basic options:
 
-| Command     | Use                                                                            |
-|-------------|--------------------------------------------------------------------------------|
-| `discover`  | Find/List all detected unpaired mugs in pairing mode                           |
-| `find`      | Find *one* already paired mugs                                                 |
-| `info`      | Connect to *one* mug and print its current state                               |
-| `poll`      | Connect to *one* mug and print its current state and keep watching for changes |
-| `get`       | Get the value(s) of one or more attribute(s) by name                           |
-| `set`       | Set one or more values on the mug                                              |
-
+| Command     | Use                                                                               |
+|-------------|-----------------------------------------------------------------------------------|
+| `discover`  | Find/List all detected unpaired devices in pairing mode                           |
+| `find`      | Find *one* already paired devices                                                 |
+| `info`      | Connect to *one* device and print its current state                               |
+| `poll`      | Connect to *one* device and print its current state and keep watching for changes |
+| `get`       | Get the value(s) of one or more attribute(s) by name                              |
+| `set`       | Set one or more values on the device                                              |
 
 ![CLI Example](./docs/images/cli-example.png)
 
 ## Caveats
 
-- Since this api is not public, a lot of guesswork and reverse engineering is involved, so it's not perfect.
-- If the mug has not been set up in the app since it was reset, writing is not allowed. I don't know what they set in the app, but it changes something, and it doesn't work without it.
-- Once that mug has been set up in the app, you should ideally forget the device or at least turn off bluetooth whilst using it here, or you will probably get disconnected often
-- I haven't figured out some attributes like udsk, dsk, location and timezone.
+* Since this api is not public, a lot of guesswork and reverse engineering is involved, so it's not perfect.
+* If the device has not been set up in the app since it was reset, writing is not allowed. I don't know what they set in the app, but it changes something, and it doesn't work without it.
+* Once that device has been set up in the app, you should ideally forget the device or at least turn off bluetooth whilst using it here, or you will probably get disconnected often
+* I haven't figured out some attributes like udsk, dsk, location and timezone, but they are not very useful anyway.
 
 ## Troubleshooting
 
 ### 'Operation failed with ATT error: 0x0e' or another connection error
+
 This seems to be caused by the bluetooth adaptor being in some sort of passive mode. I have not yet figured out how to wake it programmatically so sadly, you need to manually open `bluetoothctl` to do so.
-Please ensure the mug is in pairing mode (ie the light is flashing blue) and run the `bluetoothctl` command. You don,t need to type anything. run it and wait until the mug connects.
+Please ensure the device is in pairing mode (ie the light is flashing blue or says "PAIR") and run the `bluetoothctl` command. You don't need to type anything. run it and wait until the mug connects.
+
 
-## Todo
-- Test with other devices. Please let me know if you have tried it with others.
+## Development
+
+Install:
+- [hatch](https://hatch.pypa.io/latest/install/)
+- [pre-commit](https://pre-commit.com/)
+
+```bash
+pip install hatch
+# Use CLI interface
+hatch run ember-mug --help
+# Run Tests
+hatch run test:cov
+# View docs
+hatch docs:serve
+# Lint code
+pre-commit run --all-files
+```
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [waynerv/cookiecutter-pypackage](https://github.com/waynerv/cookiecutter-pypackage) project template.
 
 ## Notice of Non-Affiliation and Disclaimer
 
 This project is not affiliated, associated, authorized, endorsed by, or in any way officially connected with Ember.
 
 The name Ember as well as related names, marks, emblems and images are registered trademarks of their respective owners.
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

