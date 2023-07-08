# Comparing `tmp/flet_lite-1.0.tar.gz` & `tmp/flet_lite-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_lite-1.0.tar", last modified: Fri Jul  7 18:31:51 2023, max compression
+gzip compressed data, was "flet_lite-1.4.tar", last modified: Fri Jul  7 20:21:31 2023, max compression
```

## Comparing `flet_lite-1.0.tar` & `flet_lite-1.4.tar`

### file list

```diff
@@ -1,127 +1,190 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 18:31:51.793468 flet_lite-1.0/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1071 2023-07-07 16:56:58.000000 flet_lite-1.0/LICENSE
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      145 2023-07-07 18:31:45.000000 flet_lite-1.0/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2976 2023-07-07 18:31:51.793334 flet_lite-1.0/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2582 2023-07-07 16:56:58.000000 flet_lite-1.0/README.md
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 18:31:51.773386 flet_lite-1.0/flet/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8196 2023-07-07 17:00:35.000000 flet_lite-1.0/flet/.DS_Store
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      270 2023-07-07 16:56:58.000000 flet_lite-1.0/flet/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1114 2023-07-07 16:56:58.000000 flet_lite-1.0/flet/flet.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6335 2023-07-07 16:56:58.000000 flet_lite-1.0/flet/page.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1056 2023-07-07 16:56:58.000000 flet_lite-1.0/flet/publish.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 18:31:51.775988 flet_lite-1.0/flet/web/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6148 2023-07-07 17:00:35.000000 flet_lite-1.0/flet/web/.DS_Store
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 17:08:00.000000 flet_lite-1.0/flet/web/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)  4313577 2023-07-07 16:56:58.000000 flet_lite-1.0/flet/web/development.zip
--rw-r--r--   0 yousifaladwani   (501) staff       (20)  4292224 2023-07-07 16:56:58.000000 flet_lite-1.0/flet/web/dist.zip
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 18:31:51.792523 flet_lite-1.0/flet_core/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6457 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6774 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/alert_dialog.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      407 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/alignment.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     7226 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/animated_switcher.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2806 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/animation.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5403 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/app_bar.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     7301 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/audio.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5446 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/banner.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      326 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/blur.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1079 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/border.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      958 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/border_radius.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2826 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/bottom_sheet.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2202 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/buttons.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3044 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/callable_control.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5695 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/card.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     7156 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/checkbox.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6795 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/circle_avatar.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3085 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/client_storage.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1002 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/clipboard.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    10708 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/colors.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6924 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/column.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1132 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/connection.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     7099 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/constrained_control.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    14684 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/container.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    14133 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/control.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      260 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/control_event.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    20707 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/datatable.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2263 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/divider.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6270 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/drag_target.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6063 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/draggable.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     9177 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/dropdown.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8804 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/elevated_button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1978 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/embed_json_encoder.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      166 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/event.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1839 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/event_handler.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     9777 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/file_picker.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2694 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/filled_button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2828 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/filled_tonal_button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2542 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/flet_app.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     7111 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/floating_action_button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    13981 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/form_field_control.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    28044 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/gesture_detector.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1531 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/gradients.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6804 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/grid_view.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2134 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/haptic_feedback.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3430 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/icon.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8438 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/icon_button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)   362652 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/icons.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6585 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/image.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      367 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/inline_span.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8360 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/list_tile.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6401 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/list_view.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8644 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/local_connection.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      223 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/locks.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      583 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/margin.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6129 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/markdown.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5180 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/matplotlib_chart.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8322 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/navigation_bar.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    11986 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/navigation_rail.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     7489 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/outlined_button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      587 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/padding.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    53719 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/page.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2674 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/painting.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4410 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/plotly_chart.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6811 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/popup_menu_button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4293 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/progress_bar.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4491 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/progress_ring.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4088 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/protocol.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3419 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/querystring.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5765 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/radio.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2389 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/radio_group.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      291 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/ref.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6344 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/responsive_row.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6908 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/row.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4486 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/scrollable_control.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1637 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/semantics.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      576 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/session_storage.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5318 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/shader_mask.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      572 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/shadow.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2919 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/shake_detector.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     7382 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/slider.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3971 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/snack_bar.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4889 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/stack.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8104 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/switch.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    10820 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/tabs.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      632 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/template_route.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    10568 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/text.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     7462 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/text_button.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     3092 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/text_span.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1260 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/text_style.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)    15444 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/textfield.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     6172 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/theme.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     8362 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/tooltip.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      544 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/transform.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2753 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/transparent_pointer.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5186 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/types.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      684 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/user_control.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      409 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/utils.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2337 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/vertical_divider.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     5852 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/view.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     4049 2023-07-07 16:56:58.000000 flet_lite-1.0/flet_core/window_drag_area.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 18:31:51.793139 flet_lite-1.0/flet_lite.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2976 2023-07-07 18:31:51.000000 flet_lite-1.0/flet_lite.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2807 2023-07-07 18:31:51.000000 flet_lite-1.0/flet_lite.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-07-07 18:31:51.000000 flet_lite-1.0/flet_lite.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       28 2023-07-07 18:31:51.000000 flet_lite-1.0/flet_lite.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       15 2023-07-07 18:31:51.000000 flet_lite-1.0/flet_lite.egg-info/top_level.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      103 2023-07-07 16:56:58.000000 flet_lite-1.0/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-07-07 18:31:51.793509 flet_lite-1.0/setup.cfg
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      834 2023-07-07 18:30:18.000000 flet_lite-1.0/setup.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 20:21:31.964056 flet_lite-1.4/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1071 2023-07-07 18:44:58.000000 flet_lite-1.4/LICENSE
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      285 2023-07-07 19:43:23.000000 flet_lite-1.4/MANIFEST.in
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2976 2023-07-07 20:21:31.963898 flet_lite-1.4/PKG-INFO
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2582 2023-07-07 18:44:58.000000 flet_lite-1.4/README.md
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 20:21:31.909500 flet_lite-1.4/flet/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8196 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/.DS_Store
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      270 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 20:21:31.910994 flet_lite-1.4/flet/api/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/api/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      788 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/api/manage_client_pushes.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      443 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/api/push_add_request.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      309 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/api/push_clean_request.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      307 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/api/push_go_route_request.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1208 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/api/push_page_update_request.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      348 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/api/push_remove_request.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      507 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/api/push_update_request.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 20:21:31.911301 flet_lite-1.4/flet/cli_tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/cli_tools/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3173 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/cli_tools/publish.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1114 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/flet.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6335 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/page.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1056 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/publish.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 20:21:31.912931 flet_lite-1.4/flet/tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/tools/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1426 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/tools/append_assets_to_dist.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      347 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/tools/edit_control_props.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1361 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/tools/run_event_function.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2402 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/tools/setup_web.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      521 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/tools/update_control_on_event.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1084 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/tools/update_page_info.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 20:21:31.914956 flet_lite-1.4/flet/utils/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/utils/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      860 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/utils/all_props_posible.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2158 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/utils/api_host.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2857 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/utils/appbar_coder.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1892 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/utils/control_coder.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1507 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/utils/get_all_subcontrols.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      616 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/utils/get_control_data.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      176 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/utils/get_free_port.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      722 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/utils/page_posible_props.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2334 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/utils/view_coder.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      663 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/utils/web_host.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 20:21:31.918823 flet_lite-1.4/flet/web/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6148 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/web/.DS_Store
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/web/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)  4313577 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/web/development.zip
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)  4292224 2023-07-07 18:44:58.000000 flet_lite-1.4/flet/web/dist.zip
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 20:21:31.954301 flet_lite-1.4/flet_core/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6457 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6774 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/alert_dialog.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      407 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/alignment.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     7226 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/animated_switcher.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2806 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/animation.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5403 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/app_bar.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     7301 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/audio.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5446 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/banner.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      326 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/blur.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1079 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/border.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      958 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/border_radius.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2826 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/bottom_sheet.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2202 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/buttons.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3044 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/callable_control.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 20:21:31.958391 flet_lite-1.4/flet_core/canvas/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      514 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2903 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/arc.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4629 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/canvas.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1639 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/circle.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1361 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/color.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      837 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/fill.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1862 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/line.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1907 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/oval.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3486 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/path.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1772 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/points.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2361 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/rect.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1963 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/shadow.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      347 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/shape.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4172 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/canvas/text.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5695 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/card.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 20:21:31.962603 flet_lite-1.4/flet_core/charts/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     9855 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/bar_chart.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2061 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/bar_chart_group.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6837 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/bar_chart_rod.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1949 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/bar_chart_rod_stack_item.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2924 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/chart_axis.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1293 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/chart_axis_label.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      338 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/chart_grid_lines.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      286 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/chart_point_line.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1006 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/chart_point_shape.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    11228 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/line_chart.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8258 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/line_chart_data.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5496 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/line_chart_data_point.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5888 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/pie_chart.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3824 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/charts/pie_chart_section.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     7156 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/checkbox.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6795 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/circle_avatar.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3085 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/client_storage.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1002 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/clipboard.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    10708 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/colors.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6924 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/column.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1132 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/connection.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     7099 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/constrained_control.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    14684 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/container.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    14133 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/control.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      260 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/control_event.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    20707 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/datatable.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2263 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/divider.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6270 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/drag_target.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6063 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/draggable.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     9177 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/dropdown.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8804 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/elevated_button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1978 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/embed_json_encoder.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      166 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/event.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1839 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/event_handler.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     9777 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/file_picker.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2694 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/filled_button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2828 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/filled_tonal_button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2542 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/flet_app.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     7111 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/floating_action_button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    13981 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/form_field_control.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    28044 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/gesture_detector.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1531 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/gradients.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6804 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/grid_view.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2134 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/haptic_feedback.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3430 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/icon.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8438 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/icon_button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)   362652 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/icons.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6585 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/image.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      367 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/inline_span.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8360 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/list_tile.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6401 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/list_view.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8644 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/local_connection.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      223 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/locks.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      583 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/margin.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6129 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/markdown.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5180 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/matplotlib_chart.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8322 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/navigation_bar.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    11986 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/navigation_rail.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     7489 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/outlined_button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      587 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/padding.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    53719 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/page.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2674 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/painting.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4410 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/plotly_chart.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6811 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/popup_menu_button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4293 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/progress_bar.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4491 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/progress_ring.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4088 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/protocol.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3419 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/querystring.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5765 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/radio.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2389 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/radio_group.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      291 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/ref.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6344 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/responsive_row.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6908 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/row.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4486 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/scrollable_control.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1637 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/semantics.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      576 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/session_storage.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5318 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/shader_mask.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      572 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/shadow.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2919 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/shake_detector.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     7382 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/slider.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3971 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/snack_bar.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4889 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/stack.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8104 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/switch.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    10820 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/tabs.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      632 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/template_route.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    10568 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/text.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     7462 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/text_button.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     3092 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/text_span.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1260 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/text_style.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)    15444 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/textfield.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     6172 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/theme.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     8362 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/tooltip.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      544 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/transform.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2753 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/transparent_pointer.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5186 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/types.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      684 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/user_control.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      409 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/utils.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2337 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/vertical_divider.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     5852 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/view.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4049 2023-07-07 18:44:58.000000 flet_lite-1.4/flet_core/window_drag_area.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-07-07 20:21:31.963657 flet_lite-1.4/flet_lite.egg-info/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2976 2023-07-07 20:21:31.000000 flet_lite-1.4/flet_lite.egg-info/PKG-INFO
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     4528 2023-07-07 20:21:31.000000 flet_lite-1.4/flet_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-07-07 20:21:31.000000 flet_lite-1.4/flet_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       35 2023-07-07 20:21:31.000000 flet_lite-1.4/flet_lite.egg-info/requires.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       15 2023-07-07 20:21:31.000000 flet_lite-1.4/flet_lite.egg-info/top_level.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      103 2023-07-07 18:44:58.000000 flet_lite-1.4/pyproject.toml
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-07-07 20:21:31.964108 flet_lite-1.4/setup.cfg
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      833 2023-07-07 20:21:23.000000 flet_lite-1.4/setup.py
```

### Comparing `flet_lite-1.0/LICENSE` & `flet_lite-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/PKG-INFO` & `flet_lite-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_lite
-Version: 1.0
+Version: 1.4
 Summary: A tiny version of flet to work on mobile developments
 Home-page: https://github.com/SKbarbon/flet_lite
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_lite-1.0/README.md` & `flet_lite-1.4/README.md`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet/.DS_Store` & `flet_lite-1.4/flet/.DS_Store`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet/flet.py` & `flet_lite-1.4/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet/page.py` & `flet_lite-1.4/flet/page.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet/publish.py` & `flet_lite-1.4/flet/publish.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet/web/.DS_Store` & `flet_lite-1.4/flet/web/.DS_Store`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet/web/development.zip` & `flet_lite-1.4/flet/web/development.zip`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet/web/dist.zip` & `flet_lite-1.4/flet/web/dist.zip`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/__init__.py` & `flet_lite-1.4/flet_core/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/alert_dialog.py` & `flet_lite-1.4/flet_core/alert_dialog.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/animated_switcher.py` & `flet_lite-1.4/flet_core/animated_switcher.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/animation.py` & `flet_lite-1.4/flet_core/animation.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/app_bar.py` & `flet_lite-1.4/flet_core/app_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/audio.py` & `flet_lite-1.4/flet_core/audio.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/banner.py` & `flet_lite-1.4/flet_core/banner.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/border.py` & `flet_lite-1.4/flet_core/border.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/border_radius.py` & `flet_lite-1.4/flet_core/border_radius.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/bottom_sheet.py` & `flet_lite-1.4/flet_core/bottom_sheet.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/buttons.py` & `flet_lite-1.4/flet_core/buttons.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/callable_control.py` & `flet_lite-1.4/flet_core/callable_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/card.py` & `flet_lite-1.4/flet_core/card.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/checkbox.py` & `flet_lite-1.4/flet_core/checkbox.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/circle_avatar.py` & `flet_lite-1.4/flet_core/circle_avatar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/client_storage.py` & `flet_lite-1.4/flet_core/client_storage.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/clipboard.py` & `flet_lite-1.4/flet_core/clipboard.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/colors.py` & `flet_lite-1.4/flet_core/colors.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/column.py` & `flet_lite-1.4/flet_core/column.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/connection.py` & `flet_lite-1.4/flet_core/connection.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/constrained_control.py` & `flet_lite-1.4/flet_core/constrained_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/container.py` & `flet_lite-1.4/flet_core/container.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/control.py` & `flet_lite-1.4/flet_core/control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/datatable.py` & `flet_lite-1.4/flet_core/datatable.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/divider.py` & `flet_lite-1.4/flet_core/divider.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/drag_target.py` & `flet_lite-1.4/flet_core/drag_target.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/draggable.py` & `flet_lite-1.4/flet_core/draggable.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/dropdown.py` & `flet_lite-1.4/flet_core/dropdown.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/elevated_button.py` & `flet_lite-1.4/flet_core/elevated_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/embed_json_encoder.py` & `flet_lite-1.4/flet_core/embed_json_encoder.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/event_handler.py` & `flet_lite-1.4/flet_core/event_handler.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/file_picker.py` & `flet_lite-1.4/flet_core/file_picker.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/filled_button.py` & `flet_lite-1.4/flet_core/filled_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/filled_tonal_button.py` & `flet_lite-1.4/flet_core/filled_tonal_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/flet_app.py` & `flet_lite-1.4/flet_core/flet_app.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/floating_action_button.py` & `flet_lite-1.4/flet_core/floating_action_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/form_field_control.py` & `flet_lite-1.4/flet_core/form_field_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/gesture_detector.py` & `flet_lite-1.4/flet_core/gesture_detector.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/gradients.py` & `flet_lite-1.4/flet_core/gradients.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/grid_view.py` & `flet_lite-1.4/flet_core/grid_view.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/haptic_feedback.py` & `flet_lite-1.4/flet_core/haptic_feedback.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/icon.py` & `flet_lite-1.4/flet_core/icon.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/icon_button.py` & `flet_lite-1.4/flet_core/icon_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/icons.py` & `flet_lite-1.4/flet_core/icons.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/image.py` & `flet_lite-1.4/flet_core/image.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/list_tile.py` & `flet_lite-1.4/flet_core/list_tile.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/list_view.py` & `flet_lite-1.4/flet_core/list_view.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/local_connection.py` & `flet_lite-1.4/flet_core/local_connection.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/margin.py` & `flet_lite-1.4/flet_core/margin.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/markdown.py` & `flet_lite-1.4/flet_core/markdown.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/matplotlib_chart.py` & `flet_lite-1.4/flet_core/matplotlib_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/navigation_bar.py` & `flet_lite-1.4/flet_core/navigation_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/navigation_rail.py` & `flet_lite-1.4/flet_core/navigation_rail.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/outlined_button.py` & `flet_lite-1.4/flet_core/outlined_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/padding.py` & `flet_lite-1.4/flet_core/padding.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/page.py` & `flet_lite-1.4/flet_core/page.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/painting.py` & `flet_lite-1.4/flet_core/painting.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/plotly_chart.py` & `flet_lite-1.4/flet_core/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/popup_menu_button.py` & `flet_lite-1.4/flet_core/popup_menu_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/progress_bar.py` & `flet_lite-1.4/flet_core/progress_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/progress_ring.py` & `flet_lite-1.4/flet_core/progress_ring.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/protocol.py` & `flet_lite-1.4/flet_core/protocol.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/querystring.py` & `flet_lite-1.4/flet_core/querystring.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/radio.py` & `flet_lite-1.4/flet_core/radio.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/radio_group.py` & `flet_lite-1.4/flet_core/radio_group.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/responsive_row.py` & `flet_lite-1.4/flet_core/responsive_row.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/row.py` & `flet_lite-1.4/flet_core/row.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/scrollable_control.py` & `flet_lite-1.4/flet_core/scrollable_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/semantics.py` & `flet_lite-1.4/flet_core/semantics.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/session_storage.py` & `flet_lite-1.4/flet_core/session_storage.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/shader_mask.py` & `flet_lite-1.4/flet_core/shader_mask.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/shadow.py` & `flet_lite-1.4/flet_core/shadow.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/shake_detector.py` & `flet_lite-1.4/flet_core/shake_detector.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/slider.py` & `flet_lite-1.4/flet_core/slider.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/snack_bar.py` & `flet_lite-1.4/flet_core/snack_bar.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/stack.py` & `flet_lite-1.4/flet_core/stack.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/switch.py` & `flet_lite-1.4/flet_core/switch.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/tabs.py` & `flet_lite-1.4/flet_core/tabs.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/template_route.py` & `flet_lite-1.4/flet_core/template_route.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/text.py` & `flet_lite-1.4/flet_core/text.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/text_button.py` & `flet_lite-1.4/flet_core/text_button.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/text_span.py` & `flet_lite-1.4/flet_core/text_span.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/text_style.py` & `flet_lite-1.4/flet_core/text_style.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/textfield.py` & `flet_lite-1.4/flet_core/textfield.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/theme.py` & `flet_lite-1.4/flet_core/theme.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/tooltip.py` & `flet_lite-1.4/flet_core/tooltip.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/transform.py` & `flet_lite-1.4/flet_core/transform.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/transparent_pointer.py` & `flet_lite-1.4/flet_core/transparent_pointer.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/types.py` & `flet_lite-1.4/flet_core/types.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/user_control.py` & `flet_lite-1.4/flet_core/user_control.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/vertical_divider.py` & `flet_lite-1.4/flet_core/vertical_divider.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/view.py` & `flet_lite-1.4/flet_core/view.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_core/window_drag_area.py` & `flet_lite-1.4/flet_core/window_drag_area.py`

 * *Files identical despite different names*

### Comparing `flet_lite-1.0/flet_lite.egg-info/PKG-INFO` & `flet_lite-1.4/flet_lite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-lite
-Version: 1.0
+Version: 1.4
 Summary: A tiny version of flet to work on mobile developments
 Home-page: https://github.com/SKbarbon/flet_lite
 Author: SKbarbon
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `flet_lite-1.0/flet_lite.egg-info/SOURCES.txt` & `flet_lite-1.4/flet_lite.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,42 @@
 pyproject.toml
 setup.py
 flet/.DS_Store
 flet/__init__.py
 flet/flet.py
 flet/page.py
 flet/publish.py
+flet/api/__init__.py
+flet/api/manage_client_pushes.py
+flet/api/push_add_request.py
+flet/api/push_clean_request.py
+flet/api/push_go_route_request.py
+flet/api/push_page_update_request.py
+flet/api/push_remove_request.py
+flet/api/push_update_request.py
+flet/cli_tools/__init__.py
+flet/cli_tools/publish.py
+flet/tools/__init__.py
+flet/tools/append_assets_to_dist.py
+flet/tools/edit_control_props.py
+flet/tools/run_event_function.py
+flet/tools/setup_web.py
+flet/tools/update_control_on_event.py
+flet/tools/update_page_info.py
+flet/utils/__init__.py
+flet/utils/all_props_posible.py
+flet/utils/api_host.py
+flet/utils/appbar_coder.py
+flet/utils/control_coder.py
+flet/utils/get_all_subcontrols.py
+flet/utils/get_control_data.py
+flet/utils/get_free_port.py
+flet/utils/page_posible_props.py
+flet/utils/view_coder.py
+flet/utils/web_host.py
 flet/web/.DS_Store
 flet/web/__init__.py
 flet/web/development.zip
 flet/web/dist.zip
 flet_core/__init__.py
 flet_core/alert_dialog.py
 flet_core/alignment.py
@@ -109,12 +137,41 @@
 flet_core/transparent_pointer.py
 flet_core/types.py
 flet_core/user_control.py
 flet_core/utils.py
 flet_core/vertical_divider.py
 flet_core/view.py
 flet_core/window_drag_area.py
+flet_core/canvas/__init__.py
+flet_core/canvas/arc.py
+flet_core/canvas/canvas.py
+flet_core/canvas/circle.py
+flet_core/canvas/color.py
+flet_core/canvas/fill.py
+flet_core/canvas/line.py
+flet_core/canvas/oval.py
+flet_core/canvas/path.py
+flet_core/canvas/points.py
+flet_core/canvas/rect.py
+flet_core/canvas/shadow.py
+flet_core/canvas/shape.py
+flet_core/canvas/text.py
+flet_core/charts/__init__.py
+flet_core/charts/bar_chart.py
+flet_core/charts/bar_chart_group.py
+flet_core/charts/bar_chart_rod.py
+flet_core/charts/bar_chart_rod_stack_item.py
+flet_core/charts/chart_axis.py
+flet_core/charts/chart_axis_label.py
+flet_core/charts/chart_grid_lines.py
+flet_core/charts/chart_point_line.py
+flet_core/charts/chart_point_shape.py
+flet_core/charts/line_chart.py
+flet_core/charts/line_chart_data.py
+flet_core/charts/line_chart_data_point.py
+flet_core/charts/pie_chart.py
+flet_core/charts/pie_chart_section.py
 flet_lite.egg-info/PKG-INFO
 flet_lite.egg-info/SOURCES.txt
 flet_lite.egg-info/dependency_links.txt
 flet_lite.egg-info/requires.txt
 flet_lite.egg-info/top_level.txt
```

### Comparing `flet_lite-1.0/setup.py` & `flet_lite-1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import os
 
 with open("README.md", encoding="utf-8") as f:
     long_descibe = str(f.read())
 
 setup(
     name='flet_lite',
-    version='1.0',
+    version='1.4',
     author='SKbarbon',
     description='A tiny version of flet to work on mobile developments',
     long_description=long_descibe,
     long_description_content_type='text/markdown',
     url='https://github.com/SKbarbon/flet_lite',
-    install_requires=["flask_cors", "flask", "jsonpickle"],
-    packages=find_packages(include=["flet", "flet_core", "flet.web"], exclude=["web_development_app"]),
+    install_requires=["flask_cors", "flask", "jsonpickle", "repath"],
+    packages=find_packages(include=["flet", "flet_core", "flet.web", "flet/*", "flet.api"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows"
     ],
     include_package_data=True,
     include_dirs=["flet", "flet_core", "flet.web"]
```

