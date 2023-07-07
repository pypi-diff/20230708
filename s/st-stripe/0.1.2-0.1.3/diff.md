# Comparing `tmp/st_stripe-0.1.2.tar.gz` & `tmp/st_stripe-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_stripe-0.1.2.tar", last modified: Fri Jul  7 22:51:49 2023, max compression
+gzip compressed data, was "st_stripe-0.1.3.tar", last modified: Fri Jul  7 23:07:15 2023, max compression
```

## Comparing `st_stripe-0.1.2.tar` & `st_stripe-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 22:51:49.295974 st_stripe-0.1.2/
--rw-r--r--   0 trichards   (501) staff       (20)     5425 2023-07-07 22:51:49.295765 st_stripe-0.1.2/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)     5205 2023-07-07 02:13:03.000000 st_stripe-0.1.2/README.md
--rw-r--r--   0 trichards   (501) staff       (20)      355 2023-07-07 22:49:47.000000 st_stripe-0.1.2/pyproject.toml
--rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-07 22:51:49.296042 st_stripe-0.1.2/setup.cfg
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 22:51:49.291686 st_stripe-0.1.2/src/
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 22:51:49.293634 st_stripe-0.1.2/src/st_stripe/
--rw-r--r--   0 trichards   (501) staff       (20)       50 2023-07-07 22:36:24.000000 st_stripe-0.1.2/src/st_stripe/__init__.py
--rw-r--r--   0 trichards   (501) staff       (20)     1257 2023-07-07 22:45:43.000000 st_stripe-0.1.2/src/st_stripe/aggregate_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     2915 2023-07-07 01:57:46.000000 st_stripe-0.1.2/src/st_stripe/google_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     1077 2023-07-07 01:58:32.000000 st_stripe-0.1.2/src/st_stripe/stripe_auth.py
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 22:51:49.295425 st_stripe-0.1.2/src/st_stripe.egg-info/
--rw-r--r--   0 trichards   (501) staff       (20)     5425 2023-07-07 22:51:49.000000 st_stripe-0.1.2/src/st_stripe.egg-info/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)      324 2023-07-07 22:51:49.000000 st_stripe-0.1.2/src/st_stripe.egg-info/SOURCES.txt
--rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-07 22:51:49.000000 st_stripe-0.1.2/src/st_stripe.egg-info/dependency_links.txt
--rw-r--r--   0 trichards   (501) staff       (20)       25 2023-07-07 22:51:49.000000 st_stripe-0.1.2/src/st_stripe.egg-info/requires.txt
--rw-r--r--   0 trichards   (501) staff       (20)       10 2023-07-07 22:51:49.000000 st_stripe-0.1.2/src/st_stripe.egg-info/top_level.txt
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:07:15.610650 st_stripe-0.1.3/
+-rw-r--r--   0 trichards   (501) staff       (20)     5425 2023-07-07 23:07:15.610417 st_stripe-0.1.3/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)     5205 2023-07-07 02:13:03.000000 st_stripe-0.1.3/README.md
+-rw-r--r--   0 trichards   (501) staff       (20)      355 2023-07-07 23:07:05.000000 st_stripe-0.1.3/pyproject.toml
+-rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-07 23:07:15.610718 st_stripe-0.1.3/setup.cfg
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:07:15.605555 st_stripe-0.1.3/src/
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:07:15.608117 st_stripe-0.1.3/src/st_stripe/
+-rw-r--r--   0 trichards   (501) staff       (20)       50 2023-07-07 22:36:24.000000 st_stripe-0.1.3/src/st_stripe/__init__.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1399 2023-07-07 23:00:46.000000 st_stripe-0.1.3/src/st_stripe/aggregate_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     2915 2023-07-07 01:57:46.000000 st_stripe-0.1.3/src/st_stripe/google_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1077 2023-07-07 01:58:32.000000 st_stripe-0.1.3/src/st_stripe/stripe_auth.py
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:07:15.609949 st_stripe-0.1.3/src/st_stripe.egg-info/
+-rw-r--r--   0 trichards   (501) staff       (20)     5425 2023-07-07 23:07:15.000000 st_stripe-0.1.3/src/st_stripe.egg-info/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)      324 2023-07-07 23:07:15.000000 st_stripe-0.1.3/src/st_stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-07 23:07:15.000000 st_stripe-0.1.3/src/st_stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       25 2023-07-07 23:07:15.000000 st_stripe-0.1.3/src/st_stripe.egg-info/requires.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       10 2023-07-07 23:07:15.000000 st_stripe-0.1.3/src/st_stripe.egg-info/top_level.txt
```

### Comparing `st_stripe-0.1.2/PKG-INFO` & `st_stripe-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_stripe
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for creating subscription Streamlit apps
 Author-email: Tyler <your.email@example.com>
 License: MIT
 Description-Content-Type: text/markdown
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
```

### Comparing `st_stripe-0.1.2/README.md` & `st_stripe-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `st_stripe-0.1.2/src/st_stripe/aggregate_auth.py` & `st_stripe-0.1.3/src/st_stripe/aggregate_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,23 @@
         st.experimental_rerun()
 
 def add_auth():
     user_email = get_logged_in_user_email()
 
     if not user_email:
         show_login_button()
+        st.session_state.email = ""
+        st.sidebar.markdown("")
 
     customer_emails = get_customer_emails()
     if user_email not in customer_emails:
-        redirect_button(text="Subscribe now!", customer_email=user_email)
+        redirect_button(text="Subscribe now!", customer_email="")
+        st.sidebar.markdown("")
         st.session_state.user_subscribed = False
+
     elif user_email in customer_emails:
         st.session_state.user_subscribed = True
 
-    if st.sidebar.button("Logout", type="primary"):
-        del st.session_state.email
-        st.experimental_rerun()
+    if st.session_state.email != "":
+        if st.sidebar.button("Logout", type="primary"):
+            del st.session_state.email
+            st.experimental_rerun()
```

### Comparing `st_stripe-0.1.2/src/st_stripe/google_auth.py` & `st_stripe-0.1.3/src/st_stripe/google_auth.py`

 * *Files identical despite different names*

### Comparing `st_stripe-0.1.2/src/st_stripe/stripe_auth.py` & `st_stripe-0.1.3/src/st_stripe/stripe_auth.py`

 * *Files identical despite different names*

### Comparing `st_stripe-0.1.2/src/st_stripe.egg-info/PKG-INFO` & `st_stripe-0.1.3/src/st_stripe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-stripe
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for creating subscription Streamlit apps
 Author-email: Tyler <your.email@example.com>
 License: MIT
 Description-Content-Type: text/markdown
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
```

