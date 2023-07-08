# Comparing `tmp/riotee_probe-1.0.0.tar.gz` & `tmp/riotee_probe-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riotee_probe-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "riotee_probe-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `riotee_probe-1.0.0.tar` & `riotee_probe-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1116 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      515 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      325 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/__init__.py
--rw-r--r--   0        0        0     2980 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/cli.py
--rw-r--r--   0        0        0     1668 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/intelhex.py
--rw-r--r--   0        0        0     2591 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/probe.py
--rw-r--r--   0        0        0      893 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/protocol.py
--rw-r--r--   0        0        0      965 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/session.py
--rw-r--r--   0        0        0     4223 2023-06-30 16:04:42.980481 riotee_probe-1.0.0/riotee_probe/target.py
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 riotee_probe-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1116 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      515 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      376 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/__init__.py
+-rw-r--r--   0        0        0     3056 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/cli.py
+-rw-r--r--   0        0        0     1668 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/intelhex.py
+-rw-r--r--   0        0        0     2591 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/probe.py
+-rw-r--r--   0        0        0      893 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/protocol.py
+-rw-r--r--   0        0        0      965 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/session.py
+-rw-r--r--   0        0        0     4223 2023-07-08 15:08:22.419236 riotee_probe-1.0.1/riotee_probe/target.py
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 riotee_probe-1.0.1/PKG-INFO
```

### Comparing `riotee_probe-1.0.0/LICENSE.txt` & `riotee_probe-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.0/pyproject.toml` & `riotee_probe-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.0/riotee_probe/cli.py` & `riotee_probe-1.0.1/riotee_probe/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 @click.group
 def cli():
     pass
 
 
-@cli.command(short_help="Control power supply bypass")
+@cli.command(short_help="Control power supply bypass (Board only)")
 @click.option("--on/--off", required=True)
 @click.pass_context
 def bypass(ctx, on):
     with get_connected_probe() as probe:
         probe.bypass(on)
 
 
@@ -71,51 +71,56 @@
 @cli.command
 @device_option
 def resume(device):
     with get_target(device) as target:
         target.resume()
 
 
-@cli.command(short_help="Configure GPIO pin direction")
+@cli.group(short_help="Control GPIOs (Probe only)")
+def gpio():
+    pass
+
+
+@gpio.command(short_help="Configure GPIO pin direction")
 @click.option("--pin-no", "-p", type=int, required=True, help="Pin number")
 @click.option(
     "--direction",
     "-d",
     type=click.Choice(["in", "out"], case_sensitive=False),
     required=True,
     help="Pin direction",
 )
-def gpio_dir(pin_no, direction):
+def dir(pin_no, direction):
     with get_connected_probe() as probe:
         if direction == "in":
             probe.gpio_dir(pin_no, GpioDir.GPIO_DIR_IN)
         else:
             probe.gpio_dir(pin_no, GpioDir.GPIO_DIR_OUT)
 
 
-@cli.command(short_help="Set GPIO pin")
+@gpio.command(short_help="Set GPIO pin")
 @click.option("--pin-no", "-p", type=int, required=True, help="Pin number")
 @click.option(
     "--state",
     "-s",
     type=click.Choice(["high", "1", "low", "0"], case_sensitive=False),
     required=True,
     help="Pin state",
 )
-def gpio_set(pin_no, state):
+def set(pin_no, state):
     with get_connected_probe() as probe:
         if state in ["high", "1"]:
             probe.gpio_set(pin_no, True)
         else:
             probe.gpio_set(pin_no, False)
 
 
-@cli.command(short_help="Read GPIO pin")
+@gpio.command(short_help="Read GPIO pin")
 @click.option("--pin-no", "-p", type=int, required=True, help="Pin number")
-def gpio_get(pin_no):
+def get(pin_no):
     with get_connected_probe() as probe:
         state = probe.gpio_get(pin_no)
         click.echo(state)
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `riotee_probe-1.0.0/riotee_probe/intelhex.py` & `riotee_probe-1.0.1/riotee_probe/intelhex.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.0/riotee_probe/probe.py` & `riotee_probe-1.0.1/riotee_probe/probe.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.0/riotee_probe/protocol.py` & `riotee_probe-1.0.1/riotee_probe/protocol.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.0/riotee_probe/session.py` & `riotee_probe-1.0.1/riotee_probe/session.py`

 * *Files identical despite different names*

### Comparing `riotee_probe-1.0.0/riotee_probe/target.py` & `riotee_probe-1.0.1/riotee_probe/target.py`

 * *Files identical despite different names*

