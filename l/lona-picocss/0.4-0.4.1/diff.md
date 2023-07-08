# Comparing `tmp/lona-picocss-0.4.tar.gz` & `tmp/lona-picocss-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lona-picocss-0.4.tar", last modified: Thu Jul  6 14:38:23 2023, max compression
+gzip compressed data, was "lona-picocss-0.4.1.tar", last modified: Sat Jul  8 19:42:57 2023, max compression
```

## Comparing `lona-picocss-0.4.tar` & `lona-picocss-0.4.1.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1071 2023-05-31 16:56:42.000000 lona-picocss-0.4/LICENSE.txt
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2690 2023-07-06 14:38:23.032607 lona-picocss-0.4/PKG-INFO
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      652 2023-07-06 14:34:02.000000 lona-picocss-0.4/README.md
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1766 2023-07-06 14:36:15.000000 lona-picocss-0.4/lona_picocss/__init__.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      147 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/apps.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     7498 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/color_schemes.py
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss/html/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      333 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/__init__.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1588 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/base.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1817 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/buttons.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      929 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/cards.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      498 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/generic.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2866 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/icons.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      472 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/inputs.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      885 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/links.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1837 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/modal.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      701 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/progress.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1706 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/scroller.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1848 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/html/tabs.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1881 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/middlewares.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3613 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/navigation.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2563 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/routes.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     6028 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/settings.py
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss/static/
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.024607 lona-picocss-0.4/lona_picocss/static/lona-picocss/
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.024607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1081 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/LICENSE
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    60317 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather-sprite.svg
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)   158900 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    66446 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js.map
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    75963 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    80886 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js.map
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    53786 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/icons.json
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.024607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1066 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/LICENSE.md
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.024607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    78670 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)   193178 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css.map
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    69329 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)   193408 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css.map
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    83517 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)   201166 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.css.map
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    78207 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)   192522 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css.map
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    68998 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)   192745 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css.map
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    73571 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)   201142 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css.map
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    44881 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)   112715 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css.map
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    40179 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)   113084 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css.map
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      165 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/postcss.config.js
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.024607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    27484 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    58820 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css.map
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    25324 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    59593 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css.map
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      135 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/_functions.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1811 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/_variables.scss
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2147 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_accordion.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1190 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_card.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4993 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_dropdown.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3247 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_modal.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2802 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_nav.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2114 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_progress.scss
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     5158 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_button.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1670 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_code.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1061 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_embedded.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     6670 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-alt-input-types.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3029 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-checkbox-radio.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     9239 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      701 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_miscs.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1133 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_table.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4935 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_typography.scss
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      940 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_container.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1583 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_document.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      536 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_grid.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      276 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_scroller.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      115 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_section.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1845 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_sectioning.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      248 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.classless.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      370 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.fluid.classless.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1567 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1307 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.slim.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      139 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/postcss.config.js
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2029 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_colors.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     9649 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_dark.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     9438 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_light.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     5408 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_styles.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      657 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default.scss
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1096 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_accessibility.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1038 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_loading.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1034 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_reduce-motion.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     5558 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_tooltip.scss
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      456 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/feather-widgets.js
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)    19278 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/logo.svg
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1658 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/lona-picocss.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3172 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/static/lona-picocss/picocss-widgets.js
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss/templates/
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/templates/picocss/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)       40 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/403.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)       36 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/404.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      349 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/500.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4600 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/base.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1734 2023-06-09 19:36:12.000000 lona-picocss-0.4/lona_picocss/templates/picocss/color-scheme.css
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      139 2023-06-10 13:44:23.000000 lona-picocss-0.4/lona_picocss/templates/picocss/disconnect-message.html
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.028607 lona-picocss-0.4/lona_picocss/templates/picocss/django/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      207 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/django/403.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      207 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/django/404.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      379 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/django/500.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1973 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/django/base.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      108 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/templates/picocss/footer.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1373 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/picocss/header.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)       43 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/templates/picocss/waiting-for-server-message.html
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/lona_picocss/templates/registration/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      261 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/logged_out.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1739 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/login.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      547 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_change_done.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1715 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_change_form.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      599 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_reset_complete.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2176 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_reset_confirm.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1011 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_reset_done.html
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1146 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templates/registration/password_reset_form.html
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/lona_picocss/templatetags/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templatetags/__init__.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      539 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/templatetags/lona_picocss_filter.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      459 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/utils.py
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/lona_picocss/views/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)       75 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/views/__init__.py
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/lona_picocss/views/components/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)        0 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/__init__.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1157 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/buttons.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1126 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/cards.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1285 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/forms.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4268 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/icons.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2598 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/modal.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      383 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/progress.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      952 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/scroller.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      371 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/tabs.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3589 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/components/typography.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      546 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/views/django_error_views.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1670 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/views/error_views.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      469 2023-05-31 16:56:42.000000 lona-picocss-0.4/lona_picocss/views/it_works.py
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     8056 2023-07-06 14:34:02.000000 lona-picocss-0.4/lona_picocss/views/settings.py
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.020606 lona-picocss-0.4/lona_picocss.egg-info/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2690 2023-07-06 14:38:23.000000 lona-picocss-0.4/lona_picocss.egg-info/PKG-INFO
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     7280 2023-07-06 14:38:23.000000 lona-picocss-0.4/lona_picocss.egg-info/SOURCES.txt
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)        1 2023-07-06 14:38:23.000000 lona-picocss-0.4/lona_picocss.egg-info/dependency_links.txt
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)      199 2023-07-06 14:38:23.000000 lona-picocss-0.4/lona_picocss.egg-info/requires.txt
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)       13 2023-07-06 14:38:23.000000 lona-picocss-0.4/lona_picocss.egg-info/top_level.txt
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1492 2023-07-06 14:36:06.000000 lona-picocss-0.4/pyproject.toml
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)       38 2023-07-06 14:38:23.032607 lona-picocss-0.4/setup.cfg
-drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-06 14:38:23.032607 lona-picocss-0.4/tests/
--rw-r--r--   0 fscherf   (1000) fscherf   (1000)     8042 2023-07-06 14:34:02.000000 lona-picocss-0.4/tests/test_screenshots.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.903854 lona-picocss-0.4.1/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1071 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/LICENSE.txt
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2692 2023-07-08 19:42:57.903854 lona-picocss-0.4.1/PKG-INFO
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      652 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/README.md
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.891854 lona-picocss-0.4.1/lona_picocss/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1769 2023-07-08 19:41:23.000000 lona-picocss-0.4.1/lona_picocss/__init__.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      147 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/apps.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     7498 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/color_schemes.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.891854 lona-picocss-0.4.1/lona_picocss/html/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      333 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/html/__init__.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1588 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/html/base.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1817 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/html/buttons.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      929 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/html/cards.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      498 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/html/generic.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2866 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/html/icons.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      472 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/html/inputs.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      885 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/html/links.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1837 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/html/modal.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      701 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/html/progress.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1706 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/html/scroller.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1848 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/html/tabs.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1881 2023-07-08 19:38:00.000000 lona-picocss-0.4.1/lona_picocss/middlewares.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3613 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/navigation.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2563 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/routes.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     6028 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/settings.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.887853 lona-picocss-0.4.1/lona_picocss/static/
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.891854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.887853 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.891854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1081 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/LICENSE
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    60317 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather-sprite.svg
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   158900 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    66446 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    75963 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    80886 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    53786 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/icons.json
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.891854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1066 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/LICENSE.md
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.895854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    78670 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   193178 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    69329 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   193408 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    83517 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   201166 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    78207 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   192522 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    68998 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   192745 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    73571 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   201142 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    44881 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   112715 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    40179 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)   113084 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      165 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/postcss.config.js
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.895854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    27484 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    58820 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css.map
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    25324 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    59593 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css.map
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.895854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      135 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/_functions.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1811 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/_variables.scss
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.895854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2147 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_accordion.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1190 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_card.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4993 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_dropdown.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3247 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_modal.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2802 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_nav.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2114 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_progress.scss
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.899854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     5158 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_button.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1670 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_code.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1061 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_embedded.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     6670 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-alt-input-types.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3029 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-checkbox-radio.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     9239 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      701 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_miscs.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1133 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_table.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4935 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_typography.scss
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.899854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      940 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_container.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1583 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_document.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      536 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_grid.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      276 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_scroller.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      115 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_section.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1845 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_sectioning.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      248 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.classless.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      370 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.fluid.classless.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1567 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1307 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.slim.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      139 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/postcss.config.js
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.899854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.899854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2029 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_colors.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     9649 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_dark.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     9438 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_light.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     5408 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_styles.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      657 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default.scss
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.899854 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1096 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_accessibility.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1038 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_loading.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1034 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_reduce-motion.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     5558 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_tooltip.scss
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      456 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/feather-widgets.js
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)    19278 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/logo.svg
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1658 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/lona-picocss.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3172 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/static/lona-picocss/picocss-widgets.js
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.887853 lona-picocss-0.4.1/lona_picocss/templates/
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.899854 lona-picocss-0.4.1/lona_picocss/templates/picocss/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       40 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/403.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       36 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/404.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      349 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/500.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4600 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/base.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1734 2023-06-09 19:36:12.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/color-scheme.css
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      139 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/disconnect-message.html
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.899854 lona-picocss-0.4.1/lona_picocss/templates/picocss/django/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      207 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/django/403.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      207 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/django/404.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      379 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/django/500.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1973 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/django/base.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      108 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/footer.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1373 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/header.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       43 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/picocss/waiting-for-server-message.html
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.899854 lona-picocss-0.4.1/lona_picocss/templates/registration/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      261 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/registration/logged_out.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1739 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/registration/login.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      547 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/registration/password_change_done.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1715 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/registration/password_change_form.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      599 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/registration/password_reset_complete.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2176 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1011 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/registration/password_reset_done.html
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1146 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templates/registration/password_reset_form.html
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.899854 lona-picocss-0.4.1/lona_picocss/templatetags/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templatetags/__init__.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      539 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/templatetags/lona_picocss_filter.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      459 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/utils.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.899854 lona-picocss-0.4.1/lona_picocss/views/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       75 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/views/__init__.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.903854 lona-picocss-0.4.1/lona_picocss/views/components/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)        0 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/views/components/__init__.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1157 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/views/components/buttons.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1126 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/views/components/cards.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1285 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/views/components/forms.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     4268 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/views/components/icons.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2598 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/views/components/modal.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      383 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/views/components/progress.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      952 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/views/components/scroller.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      371 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/views/components/tabs.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     3589 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/views/components/typography.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      632 2023-07-08 19:37:51.000000 lona-picocss-0.4.1/lona_picocss/views/django_error_views.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1670 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/views/error_views.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      469 2023-05-31 16:56:42.000000 lona-picocss-0.4.1/lona_picocss/views/it_works.py
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     8056 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/lona_picocss/views/settings.py
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.891854 lona-picocss-0.4.1/lona_picocss.egg-info/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     2692 2023-07-08 19:42:57.000000 lona-picocss-0.4.1/lona_picocss.egg-info/PKG-INFO
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     7280 2023-07-08 19:42:57.000000 lona-picocss-0.4.1/lona_picocss.egg-info/SOURCES.txt
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)        1 2023-07-08 19:42:57.000000 lona-picocss-0.4.1/lona_picocss.egg-info/dependency_links.txt
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)      199 2023-07-08 19:42:57.000000 lona-picocss-0.4.1/lona_picocss.egg-info/requires.txt
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       13 2023-07-08 19:42:57.000000 lona-picocss-0.4.1/lona_picocss.egg-info/top_level.txt
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     1494 2023-07-08 19:41:17.000000 lona-picocss-0.4.1/pyproject.toml
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)       38 2023-07-08 19:42:57.903854 lona-picocss-0.4.1/setup.cfg
+drwxr-xr-x   0 fscherf   (1000) fscherf   (1000)        0 2023-07-08 19:42:57.903854 lona-picocss-0.4.1/tests/
+-rw-r--r--   0 fscherf   (1000) fscherf   (1000)     8042 2023-07-08 19:33:43.000000 lona-picocss-0.4.1/tests/test_screenshots.py
```

### Comparing `lona-picocss-0.4/LICENSE.txt` & `lona-picocss-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/PKG-INFO` & `lona-picocss-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lona-picocss
-Version: 0.4
+Version: 0.4.1
 Summary: Pico.css bindings for Lona
 Author-email: Florian Scherf <mail@florianscherf.de>
 License: MIT License
         
         Copyright (c) 2023 Florian Scherf
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lona-picocss-0.4/README.md` & `lona-picocss-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/__init__.py` & `lona-picocss-0.4.1/lona_picocss/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from lona_picocss.views.error_views import (
     Error403View,
     Error404View,
     Error500View,
 )
 
 
-VERSION = (0, 4)
+VERSION = (0, 4, 1)
 VERSION_STRING = '.'.join(str(i) for i in VERSION)
 
 logger = logging.getLogger('lona-picocss')
 
 
 def install_picocss(app, debug=False):
     app.settings.PICOCSS_LONA_PROJECT_TYPE = 'app'
```

### Comparing `lona-picocss-0.4/lona_picocss/color_schemes.py` & `lona-picocss-0.4.1/lona_picocss/color_schemes.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/html/base.py` & `lona-picocss-0.4.1/lona_picocss/html/base.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/html/buttons.py` & `lona-picocss-0.4.1/lona_picocss/html/buttons.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/html/cards.py` & `lona-picocss-0.4.1/lona_picocss/html/cards.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/html/icons.py` & `lona-picocss-0.4.1/lona_picocss/html/icons.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/html/links.py` & `lona-picocss-0.4.1/lona_picocss/html/links.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/html/modal.py` & `lona-picocss-0.4.1/lona_picocss/html/modal.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/html/progress.py` & `lona-picocss-0.4.1/lona_picocss/html/progress.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/html/scroller.py` & `lona-picocss-0.4.1/lona_picocss/html/scroller.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/html/tabs.py` & `lona-picocss-0.4.1/lona_picocss/html/tabs.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/middlewares.py` & `lona-picocss-0.4.1/lona_picocss/middlewares.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/navigation.py` & `lona-picocss-0.4.1/lona_picocss/navigation.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/routes.py` & `lona-picocss-0.4.1/lona_picocss/routes.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/settings.py` & `lona-picocss-0.4.1/lona_picocss/settings.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/LICENSE` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/LICENSE`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather-sprite.svg` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather-sprite.svg`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.js.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/feather.min.js.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/feather-icons/icons.json` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/feather-icons/icons.json`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/LICENSE.md` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.classless.min.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.css` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.css.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.fluid.classless.min.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.min.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/pico.slim.min.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css.map` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/css/themes/default.min.css.map`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/_variables.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_accordion.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_accordion.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_card.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_card.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_dropdown.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_modal.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_modal.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_nav.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_nav.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/components/_progress.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/components/_progress.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_button.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_button.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_code.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_code.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_embedded.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_embedded.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-alt-input-types.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-alt-input-types.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-checkbox-radio.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form-checkbox-radio.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_form.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_miscs.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_miscs.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_table.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_table.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/content/_typography.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/content/_typography.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_container.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_container.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_document.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_document.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_grid.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_grid.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_sectioning.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/layout/_sectioning.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/pico.slim.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/pico.slim.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_colors.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_colors.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_dark.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_dark.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_light.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_light.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_styles.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default/_styles.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/themes/default.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_accessibility.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_accessibility.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_loading.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_loading.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_reduce-motion.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_reduce-motion.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_tooltip.scss` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/dist/pico/scss/utilities/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/logo.svg` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/logo.svg`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/lona-picocss.css` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/lona-picocss.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/static/lona-picocss/picocss-widgets.js` & `lona-picocss-0.4.1/lona_picocss/static/lona-picocss/picocss-widgets.js`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templates/picocss/base.html` & `lona-picocss-0.4.1/lona_picocss/templates/picocss/base.html`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templates/picocss/color-scheme.css` & `lona-picocss-0.4.1/lona_picocss/templates/picocss/color-scheme.css`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templates/picocss/django/base.html` & `lona-picocss-0.4.1/lona_picocss/templates/picocss/django/base.html`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templates/picocss/header.html` & `lona-picocss-0.4.1/lona_picocss/templates/picocss/header.html`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templates/registration/login.html` & `lona-picocss-0.4.1/lona_picocss/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templates/registration/password_change_done.html` & `lona-picocss-0.4.1/lona_picocss/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templates/registration/password_change_form.html` & `lona-picocss-0.4.1/lona_picocss/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templates/registration/password_reset_complete.html` & `lona-picocss-0.4.1/lona_picocss/templates/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templates/registration/password_reset_confirm.html` & `lona-picocss-0.4.1/lona_picocss/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templates/registration/password_reset_done.html` & `lona-picocss-0.4.1/lona_picocss/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templates/registration/password_reset_form.html` & `lona-picocss-0.4.1/lona_picocss/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/templatetags/lona_picocss_filter.py` & `lona-picocss-0.4.1/lona_picocss/templatetags/lona_picocss_filter.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/views/components/buttons.py` & `lona-picocss-0.4.1/lona_picocss/views/components/buttons.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/views/components/cards.py` & `lona-picocss-0.4.1/lona_picocss/views/components/cards.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/views/components/forms.py` & `lona-picocss-0.4.1/lona_picocss/views/components/forms.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/views/components/icons.py` & `lona-picocss-0.4.1/lona_picocss/views/components/icons.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/views/components/modal.py` & `lona-picocss-0.4.1/lona_picocss/views/components/modal.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/views/components/scroller.py` & `lona-picocss-0.4.1/lona_picocss/views/components/scroller.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/views/components/typography.py` & `lona-picocss-0.4.1/lona_picocss/views/components/typography.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/views/error_views.py` & `lona-picocss-0.4.1/lona_picocss/views/error_views.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss/views/settings.py` & `lona-picocss-0.4.1/lona_picocss/views/settings.py`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/lona_picocss.egg-info/PKG-INFO` & `lona-picocss-0.4.1/lona_picocss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lona-picocss
-Version: 0.4
+Version: 0.4.1
 Summary: Pico.css bindings for Lona
 Author-email: Florian Scherf <mail@florianscherf.de>
 License: MIT License
         
         Copyright (c) 2023 Florian Scherf
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lona-picocss-0.4/lona_picocss.egg-info/SOURCES.txt` & `lona-picocss-0.4.1/lona_picocss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lona-picocss-0.4/pyproject.toml` & `lona-picocss-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
-version = "0.4"
+version = "0.4.1"
 name = "lona-picocss"
 description = "Pico.css bindings for Lona"
 
 authors = [
   { name="Florian Scherf", email="mail@florianscherf.de" },
 ]
```

### Comparing `lona-picocss-0.4/tests/test_screenshots.py` & `lona-picocss-0.4.1/tests/test_screenshots.py`

 * *Files identical despite different names*

