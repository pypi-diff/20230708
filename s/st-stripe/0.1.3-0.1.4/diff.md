# Comparing `tmp/st_stripe-0.1.3.tar.gz` & `tmp/st_stripe-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_stripe-0.1.3.tar", last modified: Fri Jul  7 23:07:15 2023, max compression
+gzip compressed data, was "st_stripe-0.1.4.tar", last modified: Fri Jul  7 23:27:57 2023, max compression
```

## Comparing `st_stripe-0.1.3.tar` & `st_stripe-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:07:15.610650 st_stripe-0.1.3/
--rw-r--r--   0 trichards   (501) staff       (20)     5425 2023-07-07 23:07:15.610417 st_stripe-0.1.3/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)     5205 2023-07-07 02:13:03.000000 st_stripe-0.1.3/README.md
--rw-r--r--   0 trichards   (501) staff       (20)      355 2023-07-07 23:07:05.000000 st_stripe-0.1.3/pyproject.toml
--rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-07 23:07:15.610718 st_stripe-0.1.3/setup.cfg
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:07:15.605555 st_stripe-0.1.3/src/
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:07:15.608117 st_stripe-0.1.3/src/st_stripe/
--rw-r--r--   0 trichards   (501) staff       (20)       50 2023-07-07 22:36:24.000000 st_stripe-0.1.3/src/st_stripe/__init__.py
--rw-r--r--   0 trichards   (501) staff       (20)     1399 2023-07-07 23:00:46.000000 st_stripe-0.1.3/src/st_stripe/aggregate_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     2915 2023-07-07 01:57:46.000000 st_stripe-0.1.3/src/st_stripe/google_auth.py
--rw-r--r--   0 trichards   (501) staff       (20)     1077 2023-07-07 01:58:32.000000 st_stripe-0.1.3/src/st_stripe/stripe_auth.py
-drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:07:15.609949 st_stripe-0.1.3/src/st_stripe.egg-info/
--rw-r--r--   0 trichards   (501) staff       (20)     5425 2023-07-07 23:07:15.000000 st_stripe-0.1.3/src/st_stripe.egg-info/PKG-INFO
--rw-r--r--   0 trichards   (501) staff       (20)      324 2023-07-07 23:07:15.000000 st_stripe-0.1.3/src/st_stripe.egg-info/SOURCES.txt
--rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-07 23:07:15.000000 st_stripe-0.1.3/src/st_stripe.egg-info/dependency_links.txt
--rw-r--r--   0 trichards   (501) staff       (20)       25 2023-07-07 23:07:15.000000 st_stripe-0.1.3/src/st_stripe.egg-info/requires.txt
--rw-r--r--   0 trichards   (501) staff       (20)       10 2023-07-07 23:07:15.000000 st_stripe-0.1.3/src/st_stripe.egg-info/top_level.txt
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:27:57.506013 st_stripe-0.1.4/
+-rw-r--r--   0 trichards   (501) staff       (20)     4931 2023-07-07 23:27:57.505819 st_stripe-0.1.4/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)     4710 2023-07-07 23:26:12.000000 st_stripe-0.1.4/README.md
+-rw-r--r--   0 trichards   (501) staff       (20)      357 2023-07-07 23:27:49.000000 st_stripe-0.1.4/pyproject.toml
+-rw-r--r--   0 trichards   (501) staff       (20)       38 2023-07-07 23:27:57.506067 st_stripe-0.1.4/setup.cfg
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:27:57.501539 st_stripe-0.1.4/src/
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:27:57.503683 st_stripe-0.1.4/src/st_stripe/
+-rw-r--r--   0 trichards   (501) staff       (20)       50 2023-07-07 22:36:24.000000 st_stripe-0.1.4/src/st_stripe/__init__.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1399 2023-07-07 23:00:46.000000 st_stripe-0.1.4/src/st_stripe/aggregate_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     2915 2023-07-07 01:57:46.000000 st_stripe-0.1.4/src/st_stripe/google_auth.py
+-rw-r--r--   0 trichards   (501) staff       (20)     1077 2023-07-07 01:58:32.000000 st_stripe-0.1.4/src/st_stripe/stripe_auth.py
+drwxr-xr-x   0 trichards   (501) staff       (20)        0 2023-07-07 23:27:57.505467 st_stripe-0.1.4/src/st_stripe.egg-info/
+-rw-r--r--   0 trichards   (501) staff       (20)     4931 2023-07-07 23:27:57.000000 st_stripe-0.1.4/src/st_stripe.egg-info/PKG-INFO
+-rw-r--r--   0 trichards   (501) staff       (20)      324 2023-07-07 23:27:57.000000 st_stripe-0.1.4/src/st_stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 trichards   (501) staff       (20)        1 2023-07-07 23:27:57.000000 st_stripe-0.1.4/src/st_stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       25 2023-07-07 23:27:57.000000 st_stripe-0.1.4/src/st_stripe.egg-info/requires.txt
+-rw-r--r--   0 trichards   (501) staff       (20)       10 2023-07-07 23:27:57.000000 st_stripe-0.1.4/src/st_stripe.egg-info/top_level.txt
```

### Comparing `st_stripe-0.1.3/PKG-INFO` & `st_stripe-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,52 @@
-Metadata-Version: 2.1
-Name: st_stripe
-Version: 0.1.3
-Summary: A Python package for creating subscription Streamlit apps
-Author-email: Tyler <your.email@example.com>
-License: MIT
-Description-Content-Type: text/markdown
-
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
 
 # 🥟 st-stripe
 
-<strong>A template for how to create subscription Streamlit apps </strong>
-
-## Thanks for demoing!!
-
-I'm temporarily putting this here for all the folks who nicely agreed to try this out. A lot of the reason behind me creating this is that data scientists currently lack a good avenue to making small businesses online, and with the LLM app craze going on right now I wanted to also make it easier for folks to share LLM apps without having to pay on their own for API calls. Either way, I greatly appreciate you trying this out. I'm trying to figure out:
-1. Should this be a example repo? Should I wrap this in a python package?
-2. Does this even really work? Where are the bugs?
-3. Do the abstractions i've created make sense here? What can be done to improve usability?
-
-Let me know!
+<strong>A python package for creating subscription Streamlit apps </strong>
 
 ## Overview
 
-This repo shows you how to add both Google authentication and a Stripe subscription to your Streamlit apps. I hope you use this to create tons of value, and capture some of it with the magic of Streamlit!
-
-- google_auth.py: this holds all of the Google Oauth parts of this code
-- stripe_auth.py: this holds all the Stripe button creation and customer listing aspects of the code
-- streamlit_app.py: this brings it all together, and has the code after users have subscribed
+This package gives you two basic functions (require_auth and add_auth) that add subscription functionality to your Streamlit apps. require_auth will add both a Google login button and a Stripe subscription button to your sidebar, and will stop your entire app with st.stop() if the user is not logged in and subscribed. If they are subscribed, st.session_state.user_subscribed will be true, and if they are logged in, st.session_state.email will have their email. If the user is not logged in or subscribed, they will be prompted to do so in the sidebar.
+Add_auth does the same, except it does not stop the app but instead just surfaces the st.session_state information detailed above, which means the developer can control exactly what they would like to show to the subscribed vs unsubscribed user!
 
-There is also one file you will have to create yourself:
+ I hope you use this to create tons of value, and capture some of it with the magic of Streamlit!
 
-- .streamlit/secrets.toml: this holds all of your secret credentials to access Google and Stripe. Note that you will need to create the .streamlit/ folder first, and then secrets.toml
+This package expects that you have a .streamlit/secrets.toml file which you will have to create. Inside it, you will need to add your Stripe and Google API information that runs the authentication and subscription parts of the package.
 
 ### Stripe
 
 In order to set up your Stripe (the best and easiest payment infrastructure in the world), go to [Stripe.com](https://stripe.com) and make an account. Once you make an account, you need to make a [payment subscription link](https://dashboard.stripe.com/test/payment-links/create) (which is in test mode by default) and add the link to your app (currently held in streamlit_app.py). If the user to your app logs in and has not already signed up and paid via Stripe, they will be asked to subscribe before they can see the rest of the app.
 
 The subscription link should be added to secrets.toml like this.
 
 ```toml
 stripe_link = 'https://buy.stripe.com/test_...'`
 ```
 
 You also need to create an [API key](https://dashboard.stripe.com/test/apikeys), which just like subscription links have test options as well. Store your API key in your secrets file as stripe_api_key and you're off to the races.
 
-The subscription link should be added to secrets.toml like this
+The api key link should be added to secrets.toml like this
 
 ```toml
 stripe_api_key = 'sk_test_...'`
 ```
 
-By default we link out to creating test subscription links and test api keys (you probably already noticed the 'test' in the Stripe dashboard, the subscription link, and in our example api key). When you launch your app and want folks to pay real money, you will need to create production links and api keys from your [Stripe dashboard](https://dashboard.stripe.com) and use those instead. While you are testing out the Stripe part of your code, you can use [Stripe's test cards](https://stripe.com/docs/testing) instead of inputting your own credit card info!
+By default this repo links to creating test subscription links and test api keys (you probably already noticed the 'test' in the Stripe dashboard, the subscription link, and in our example api key). When you launch your app and want folks to pay real money, you will need to create production links and api keys from your [Stripe dashboard](https://dashboard.stripe.com) and use those instead. While you are testing out the Stripe part of your code, you can use [Stripe's test cards](https://stripe.com/docs/testing) instead of inputting your own credit card info! To run st-stripe in test mode, add the following to your secrets file.
+
+```toml
+testing_mode = true
+```
+
+Then, the package will look for the following secrets. Otherwise, it will look for the production api and link secrets. I highly encourage you to start out in test mode!
+
+```toml
+stripe_api_key_test = 'sk_test_...'`
+stripe_link_test = 'https://buy.stripe.com/test_...'`
+```
 
 ### Google
 
 In order to set up your Google Oauth, you need to register your web app with Google's OAuth system! Basically, you need to tell
 
 So head over to [this url](https://console.cloud.google.com/apis/credentials/oauthclient) and create a web application (and a project, if this is your first go around with Google Cloud). Give a unique name, and add 'http://localhost:8501/' as an "Authorized redirect URI" (when you deploy your app, you'll also need to add the final url of your app to this list). Now press create, and store your client id, and client secret in the secrets.toml file as client_id and client_secret.
 
@@ -63,26 +54,17 @@
 
 ```toml
 client_id = '1234.....googleusercontent.com'
 client_secret = 'GOC...'
 redirect_url = 'http://localhost.com:8501'
 ```
 
-The last step for your Google Oauth provisioning is to head over to the [consent screen](https://console.cloud.google.com/apis/credentials/consent) and edit what users will see when logging in. Fill out all the info they ask for, and make sure to add the email scope (called '.../auth/userinfo.email' by Google with the user description 'See your primary Google Account email address'). That should be it!
-
-### Testing Mode
-
-You can also test this package out by going into 'testing mode', which will look for different credentials in your secrets.toml file. To activate test mode, go ahead and the following to the top of your secrets file.
+The last step for your Google Oauth provisioning is to head over to the [consent screen](https://console.cloud.google.com/apis/credentials/consent) and edit what users will see when logging in. Fill out all the info they ask for, and make sure to add the email scope (called '.../auth/userinfo.email' by Google with the user description 'See your primary Google Account email address'). That should be it! If you are in testing mode, st-stripe will look for the following secrets.
 
 ```toml
-testing_mode = true
+client_id = '1234.....googleusercontent.com'
+client_secret = 'GOC...'
+redirect_url_test = 'http://localhost.com:8501'
 ```
 
-After this, add test urls, api keys, and links to your secrets like so.
 
-```toml
-redirect_url_test = "your_google_test_client_id"
-stripe_api_key_test = "your_stripe_test_api_key"
-stripe_link_test = "your_stripe_test_link"
-```
 
-With testing mode enabled, you can safely test your Streamlit app's authentication and subscription functionality without affecting real user data or transactions. When you're ready to deploy your app, simply set testing_mode to false in your secrets.toml file to use the production credentials.
```

### Comparing `st_stripe-0.1.3/README.md` & `st_stripe-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,60 @@
+Metadata-Version: 2.1
+Name: st_stripe
+Version: 0.1.4
+Summary: A Python package for creating subscription Streamlit apps
+Author-email: Tyler <tylerjrichards@gmail.com>
+License: MIT
+Description-Content-Type: text/markdown
+
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
 
 # 🥟 st-stripe
 
-<strong>A template for how to create subscription Streamlit apps </strong>
-
-## Thanks for demoing!!
-
-I'm temporarily putting this here for all the folks who nicely agreed to try this out. A lot of the reason behind me creating this is that data scientists currently lack a good avenue to making small businesses online, and with the LLM app craze going on right now I wanted to also make it easier for folks to share LLM apps without having to pay on their own for API calls. Either way, I greatly appreciate you trying this out. I'm trying to figure out:
-1. Should this be a example repo? Should I wrap this in a python package?
-2. Does this even really work? Where are the bugs?
-3. Do the abstractions i've created make sense here? What can be done to improve usability?
-
-Let me know!
+<strong>A python package for creating subscription Streamlit apps </strong>
 
 ## Overview
 
-This repo shows you how to add both Google authentication and a Stripe subscription to your Streamlit apps. I hope you use this to create tons of value, and capture some of it with the magic of Streamlit!
-
-- google_auth.py: this holds all of the Google Oauth parts of this code
-- stripe_auth.py: this holds all the Stripe button creation and customer listing aspects of the code
-- streamlit_app.py: this brings it all together, and has the code after users have subscribed
+This package gives you two basic functions (require_auth and add_auth) that add subscription functionality to your Streamlit apps. require_auth will add both a Google login button and a Stripe subscription button to your sidebar, and will stop your entire app with st.stop() if the user is not logged in and subscribed. If they are subscribed, st.session_state.user_subscribed will be true, and if they are logged in, st.session_state.email will have their email. If the user is not logged in or subscribed, they will be prompted to do so in the sidebar.
+Add_auth does the same, except it does not stop the app but instead just surfaces the st.session_state information detailed above, which means the developer can control exactly what they would like to show to the subscribed vs unsubscribed user!
 
-There is also one file you will have to create yourself:
+ I hope you use this to create tons of value, and capture some of it with the magic of Streamlit!
 
-- .streamlit/secrets.toml: this holds all of your secret credentials to access Google and Stripe. Note that you will need to create the .streamlit/ folder first, and then secrets.toml
+This package expects that you have a .streamlit/secrets.toml file which you will have to create. Inside it, you will need to add your Stripe and Google API information that runs the authentication and subscription parts of the package.
 
 ### Stripe
 
 In order to set up your Stripe (the best and easiest payment infrastructure in the world), go to [Stripe.com](https://stripe.com) and make an account. Once you make an account, you need to make a [payment subscription link](https://dashboard.stripe.com/test/payment-links/create) (which is in test mode by default) and add the link to your app (currently held in streamlit_app.py). If the user to your app logs in and has not already signed up and paid via Stripe, they will be asked to subscribe before they can see the rest of the app.
 
 The subscription link should be added to secrets.toml like this.
 
 ```toml
 stripe_link = 'https://buy.stripe.com/test_...'`
 ```
 
 You also need to create an [API key](https://dashboard.stripe.com/test/apikeys), which just like subscription links have test options as well. Store your API key in your secrets file as stripe_api_key and you're off to the races.
 
-The subscription link should be added to secrets.toml like this
+The api key link should be added to secrets.toml like this
 
 ```toml
 stripe_api_key = 'sk_test_...'`
 ```
 
-By default we link out to creating test subscription links and test api keys (you probably already noticed the 'test' in the Stripe dashboard, the subscription link, and in our example api key). When you launch your app and want folks to pay real money, you will need to create production links and api keys from your [Stripe dashboard](https://dashboard.stripe.com) and use those instead. While you are testing out the Stripe part of your code, you can use [Stripe's test cards](https://stripe.com/docs/testing) instead of inputting your own credit card info!
+By default this repo links to creating test subscription links and test api keys (you probably already noticed the 'test' in the Stripe dashboard, the subscription link, and in our example api key). When you launch your app and want folks to pay real money, you will need to create production links and api keys from your [Stripe dashboard](https://dashboard.stripe.com) and use those instead. While you are testing out the Stripe part of your code, you can use [Stripe's test cards](https://stripe.com/docs/testing) instead of inputting your own credit card info! To run st-stripe in test mode, add the following to your secrets file.
+
+```toml
+testing_mode = true
+```
+
+Then, the package will look for the following secrets. Otherwise, it will look for the production api and link secrets. I highly encourage you to start out in test mode!
+
+```toml
+stripe_api_key_test = 'sk_test_...'`
+stripe_link_test = 'https://buy.stripe.com/test_...'`
+```
 
 ### Google
 
 In order to set up your Google Oauth, you need to register your web app with Google's OAuth system! Basically, you need to tell
 
 So head over to [this url](https://console.cloud.google.com/apis/credentials/oauthclient) and create a web application (and a project, if this is your first go around with Google Cloud). Give a unique name, and add 'http://localhost:8501/' as an "Authorized redirect URI" (when you deploy your app, you'll also need to add the final url of your app to this list). Now press create, and store your client id, and client secret in the secrets.toml file as client_id and client_secret.
 
@@ -55,26 +62,17 @@
 
 ```toml
 client_id = '1234.....googleusercontent.com'
 client_secret = 'GOC...'
 redirect_url = 'http://localhost.com:8501'
 ```
 
-The last step for your Google Oauth provisioning is to head over to the [consent screen](https://console.cloud.google.com/apis/credentials/consent) and edit what users will see when logging in. Fill out all the info they ask for, and make sure to add the email scope (called '.../auth/userinfo.email' by Google with the user description 'See your primary Google Account email address'). That should be it!
-
-### Testing Mode
-
-You can also test this package out by going into 'testing mode', which will look for different credentials in your secrets.toml file. To activate test mode, go ahead and the following to the top of your secrets file.
+The last step for your Google Oauth provisioning is to head over to the [consent screen](https://console.cloud.google.com/apis/credentials/consent) and edit what users will see when logging in. Fill out all the info they ask for, and make sure to add the email scope (called '.../auth/userinfo.email' by Google with the user description 'See your primary Google Account email address'). That should be it! If you are in testing mode, st-stripe will look for the following secrets.
 
 ```toml
-testing_mode = true
+client_id = '1234.....googleusercontent.com'
+client_secret = 'GOC...'
+redirect_url_test = 'http://localhost.com:8501'
 ```
 
-After this, add test urls, api keys, and links to your secrets like so.
 
-```toml
-redirect_url_test = "your_google_test_client_id"
-stripe_api_key_test = "your_stripe_test_api_key"
-stripe_link_test = "your_stripe_test_link"
-```
 
-With testing mode enabled, you can safely test your Streamlit app's authentication and subscription functionality without affecting real user data or transactions. When you're ready to deploy your app, simply set testing_mode to false in your secrets.toml file to use the production credentials.
```

### Comparing `st_stripe-0.1.3/src/st_stripe/aggregate_auth.py` & `st_stripe-0.1.4/src/st_stripe/aggregate_auth.py`

 * *Files identical despite different names*

### Comparing `st_stripe-0.1.3/src/st_stripe/google_auth.py` & `st_stripe-0.1.4/src/st_stripe/google_auth.py`

 * *Files identical despite different names*

### Comparing `st_stripe-0.1.3/src/st_stripe/stripe_auth.py` & `st_stripe-0.1.4/src/st_stripe/stripe_auth.py`

 * *Files identical despite different names*

### Comparing `st_stripe-0.1.3/src/st_stripe.egg-info/PKG-INFO` & `st_stripe-0.1.4/src/st_stripe.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 Metadata-Version: 2.1
 Name: st-stripe
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for creating subscription Streamlit apps
-Author-email: Tyler <your.email@example.com>
+Author-email: Tyler <tylerjrichards@gmail.com>
 License: MIT
 Description-Content-Type: text/markdown
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://subscription.streamlit.app)
 
 # 🥟 st-stripe
 
-<strong>A template for how to create subscription Streamlit apps </strong>
-
-## Thanks for demoing!!
-
-I'm temporarily putting this here for all the folks who nicely agreed to try this out. A lot of the reason behind me creating this is that data scientists currently lack a good avenue to making small businesses online, and with the LLM app craze going on right now I wanted to also make it easier for folks to share LLM apps without having to pay on their own for API calls. Either way, I greatly appreciate you trying this out. I'm trying to figure out:
-1. Should this be a example repo? Should I wrap this in a python package?
-2. Does this even really work? Where are the bugs?
-3. Do the abstractions i've created make sense here? What can be done to improve usability?
-
-Let me know!
+<strong>A python package for creating subscription Streamlit apps </strong>
 
 ## Overview
 
-This repo shows you how to add both Google authentication and a Stripe subscription to your Streamlit apps. I hope you use this to create tons of value, and capture some of it with the magic of Streamlit!
+This package gives you two basic functions (require_auth and add_auth) that add subscription functionality to your Streamlit apps. require_auth will add both a Google login button and a Stripe subscription button to your sidebar, and will stop your entire app with st.stop() if the user is not logged in and subscribed. If they are subscribed, st.session_state.user_subscribed will be true, and if they are logged in, st.session_state.email will have their email. If the user is not logged in or subscribed, they will be prompted to do so in the sidebar.
+Add_auth does the same, except it does not stop the app but instead just surfaces the st.session_state information detailed above, which means the developer can control exactly what they would like to show to the subscribed vs unsubscribed user!
 
-- google_auth.py: this holds all of the Google Oauth parts of this code
-- stripe_auth.py: this holds all the Stripe button creation and customer listing aspects of the code
-- streamlit_app.py: this brings it all together, and has the code after users have subscribed
+ I hope you use this to create tons of value, and capture some of it with the magic of Streamlit!
 
-There is also one file you will have to create yourself:
-
-- .streamlit/secrets.toml: this holds all of your secret credentials to access Google and Stripe. Note that you will need to create the .streamlit/ folder first, and then secrets.toml
+This package expects that you have a .streamlit/secrets.toml file which you will have to create. Inside it, you will need to add your Stripe and Google API information that runs the authentication and subscription parts of the package.
 
 ### Stripe
 
 In order to set up your Stripe (the best and easiest payment infrastructure in the world), go to [Stripe.com](https://stripe.com) and make an account. Once you make an account, you need to make a [payment subscription link](https://dashboard.stripe.com/test/payment-links/create) (which is in test mode by default) and add the link to your app (currently held in streamlit_app.py). If the user to your app logs in and has not already signed up and paid via Stripe, they will be asked to subscribe before they can see the rest of the app.
 
 The subscription link should be added to secrets.toml like this.
 
 ```toml
 stripe_link = 'https://buy.stripe.com/test_...'`
 ```
 
 You also need to create an [API key](https://dashboard.stripe.com/test/apikeys), which just like subscription links have test options as well. Store your API key in your secrets file as stripe_api_key and you're off to the races.
 
-The subscription link should be added to secrets.toml like this
+The api key link should be added to secrets.toml like this
 
 ```toml
 stripe_api_key = 'sk_test_...'`
 ```
 
-By default we link out to creating test subscription links and test api keys (you probably already noticed the 'test' in the Stripe dashboard, the subscription link, and in our example api key). When you launch your app and want folks to pay real money, you will need to create production links and api keys from your [Stripe dashboard](https://dashboard.stripe.com) and use those instead. While you are testing out the Stripe part of your code, you can use [Stripe's test cards](https://stripe.com/docs/testing) instead of inputting your own credit card info!
+By default this repo links to creating test subscription links and test api keys (you probably already noticed the 'test' in the Stripe dashboard, the subscription link, and in our example api key). When you launch your app and want folks to pay real money, you will need to create production links and api keys from your [Stripe dashboard](https://dashboard.stripe.com) and use those instead. While you are testing out the Stripe part of your code, you can use [Stripe's test cards](https://stripe.com/docs/testing) instead of inputting your own credit card info! To run st-stripe in test mode, add the following to your secrets file.
+
+```toml
+testing_mode = true
+```
+
+Then, the package will look for the following secrets. Otherwise, it will look for the production api and link secrets. I highly encourage you to start out in test mode!
+
+```toml
+stripe_api_key_test = 'sk_test_...'`
+stripe_link_test = 'https://buy.stripe.com/test_...'`
+```
 
 ### Google
 
 In order to set up your Google Oauth, you need to register your web app with Google's OAuth system! Basically, you need to tell
 
 So head over to [this url](https://console.cloud.google.com/apis/credentials/oauthclient) and create a web application (and a project, if this is your first go around with Google Cloud). Give a unique name, and add 'http://localhost:8501/' as an "Authorized redirect URI" (when you deploy your app, you'll also need to add the final url of your app to this list). Now press create, and store your client id, and client secret in the secrets.toml file as client_id and client_secret.
 
@@ -63,26 +62,17 @@
 
 ```toml
 client_id = '1234.....googleusercontent.com'
 client_secret = 'GOC...'
 redirect_url = 'http://localhost.com:8501'
 ```
 
-The last step for your Google Oauth provisioning is to head over to the [consent screen](https://console.cloud.google.com/apis/credentials/consent) and edit what users will see when logging in. Fill out all the info they ask for, and make sure to add the email scope (called '.../auth/userinfo.email' by Google with the user description 'See your primary Google Account email address'). That should be it!
-
-### Testing Mode
-
-You can also test this package out by going into 'testing mode', which will look for different credentials in your secrets.toml file. To activate test mode, go ahead and the following to the top of your secrets file.
+The last step for your Google Oauth provisioning is to head over to the [consent screen](https://console.cloud.google.com/apis/credentials/consent) and edit what users will see when logging in. Fill out all the info they ask for, and make sure to add the email scope (called '.../auth/userinfo.email' by Google with the user description 'See your primary Google Account email address'). That should be it! If you are in testing mode, st-stripe will look for the following secrets.
 
 ```toml
-testing_mode = true
+client_id = '1234.....googleusercontent.com'
+client_secret = 'GOC...'
+redirect_url_test = 'http://localhost.com:8501'
 ```
 
-After this, add test urls, api keys, and links to your secrets like so.
 
-```toml
-redirect_url_test = "your_google_test_client_id"
-stripe_api_key_test = "your_stripe_test_api_key"
-stripe_link_test = "your_stripe_test_link"
-```
 
-With testing mode enabled, you can safely test your Streamlit app's authentication and subscription functionality without affecting real user data or transactions. When you're ready to deploy your app, simply set testing_mode to false in your secrets.toml file to use the production credentials.
```

