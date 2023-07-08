# Comparing `tmp/ReverseTwitterScraper-0.7.tar.gz` & `tmp/ReverseTwitterScraper-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseTwitterScraper-0.7.tar", last modified: Wed May 24 21:55:56 2023, max compression
+gzip compressed data, was "ReverseTwitterScraper-0.8.tar", last modified: Sat Jul  8 11:48:20 2023, max compression
```

## Comparing `ReverseTwitterScraper-0.7.tar` & `ReverseTwitterScraper-0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 21:55:56.674830 ReverseTwitterScraper-0.7/
--rw-rw-rw-   0        0        0     1090 2023-03-08 21:13:40.000000 ReverseTwitterScraper-0.7/LICENSE
--rw-rw-rw-   0        0        0     7972 2023-05-24 21:55:56.673829 ReverseTwitterScraper-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     7157 2023-05-24 21:49:25.000000 ReverseTwitterScraper-0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 21:55:56.650824 ReverseTwitterScraper-0.7/ReverseTwitterScraper/
--rw-rw-rw-   0        0        0    20277 2023-05-24 21:49:50.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper/Scraper.py
--rw-rw-rw-   0        0        0       37 2023-03-09 02:04:31.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 21:55:56.672829 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/
--rw-rw-rw-   0        0        0     7972 2023-05-24 21:55:56.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-05-24 21:55:56.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 21:55:56.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-24 21:55:56.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-24 21:55:56.000000 ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 21:55:56.674830 ReverseTwitterScraper-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1161 2023-05-24 21:55:29.000000 ReverseTwitterScraper-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 11:48:20.252277 ReverseTwitterScraper-0.8/
+-rw-rw-rw-   0        0        0     1090 2023-03-08 21:13:40.000000 ReverseTwitterScraper-0.8/LICENSE
+-rw-rw-rw-   0        0        0     8887 2023-07-08 11:48:20.252277 ReverseTwitterScraper-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8072 2023-07-08 11:45:44.000000 ReverseTwitterScraper-0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 11:48:20.231273 ReverseTwitterScraper-0.8/ReverseTwitterScraper/
+-rw-rw-rw-   0        0        0    20603 2023-07-08 11:47:03.000000 ReverseTwitterScraper-0.8/ReverseTwitterScraper/Scraper.py
+-rw-rw-rw-   0        0        0       37 2023-03-09 02:04:31.000000 ReverseTwitterScraper-0.8/ReverseTwitterScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 11:48:20.251277 ReverseTwitterScraper-0.8/ReverseTwitterScraper.egg-info/
+-rw-rw-rw-   0        0        0     8887 2023-07-08 11:48:20.000000 ReverseTwitterScraper-0.8/ReverseTwitterScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-07-08 11:48:20.000000 ReverseTwitterScraper-0.8/ReverseTwitterScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 11:48:20.000000 ReverseTwitterScraper-0.8/ReverseTwitterScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-08 11:48:20.000000 ReverseTwitterScraper-0.8/ReverseTwitterScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-08 11:48:20.000000 ReverseTwitterScraper-0.8/ReverseTwitterScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 11:48:20.253278 ReverseTwitterScraper-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-07-08 11:46:16.000000 ReverseTwitterScraper-0.8/setup.py
```

### Comparing `ReverseTwitterScraper-0.7/LICENSE` & `ReverseTwitterScraper-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseTwitterScraper-0.7/PKG-INFO` & `ReverseTwitterScraper-0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,18 @@
-Metadata-Version: 2.1
-Name: ReverseTwitterScraper
-Version: 0.7
-Summary: A Python package for scraping Twitter data without API. With proxy and account-cookie support
-Home-page: https://github.com/1220moritz/reverse-twitter-scraper
-Author: 1220moritz
-Project-URL: Documentation, https://github.com/1220moritz/reverse-twitter-scraper/blob/main/README.md
-Project-URL: Github, https://github.com/1220moritz/reverse-twitter-scraper
-Project-URL: PyPi, https://pypi.org/project/ReverseTwitterScraper/
-Project-URL: Contact, https://discordapp.com/users/713118695165263923
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ReverseTwitterScraper
+## Description
 ReverseTwitterScraper is a Python package that provides an easy-to-use tool for scraping tweets of a single or multiple Twitter accounts. This package uses Selenium and httpx to scrape tweets and other account data.
 
+## IMPORTANT NOTICE in 0.8
+**Twitter has introduced a change in its system, which now mandates the use of account cookies for viewing tweets.**
+
+Please note that the use of cookies is associated with a **high risk of account suspension or ban** by Twitter.  
+Using account cookies essentially means that you are automating actions on behalf of a specific user account, which is against Twitter's Terms of Service. Always make sure to use this tool responsibly, adhering to Twitter's rules, and avoid excessive or suspicious activity that could lead to account limitations. Always make sure that you are informed about and compliant with the Twitter Terms of Service, as well as all relevant privacy laws and regulations.   
+**The creators of the ReverseTwitterScraper are not responsible for any misuse of the tool or violations of these terms.**
+
 ## Links
 GitHub: https://github.com/1220moritz/reverse-twitter-scraper  
 PyPI: https://pypi.org/project/ReverseTwitterScraper/
 
 ## Installation
 To install the package, simply run the following command:
 ```
@@ -36,16 +27,15 @@
 3. Call any method of the TwitterScraper class.  
 
 Here's an example code:
 ```
 from ReverseTwitterScraper import TwitterScraper
 
 chromedriver_path = "C:/Program Files (x86)/chromedriver.exe"
-cookies = "" #no account cookies
-cookies = {'Cookie': 'your Cookie', 'X-Csrf-Token': 'your csrf token'} #with account cookie
+cookies = {'Cookie': 'your Cookie', 'X-Csrf-Token': 'your csrf token'} # required account cookie
 proxy_list = []
 
 
 twitter_handle = ["elonmusk"]  # single account
 twitter_handles = ["elonmusk", "POTUS", "latestinspace"]  # multiple accounts
 scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
 tweets = scraper.getTweetsText()
@@ -55,31 +45,31 @@
 
 In the above code, we first import the TwitterScraper class from the package. Then, we create an object of the TwitterScraper class with the required parameters.
 Finally, we call the getTweetsText() method to get the tweets of the specified Twitter account.
 
 ## Parameters
 The TwitterScraper class takes the following parameters:
 
-- twitterHandle: The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to ['elonmusk'].
+- twitterHandle (Required): The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to ['elonmusk'].
 
-- chromedriverPath: The path of the Chrome driver executable file. This file is required to use the Selenium module.
+- chromedriverPath (Required): The path of the Chrome driver executable file. This file is required to use the Selenium module.
 
-- cookies: (Optional) The cookies of a logged-in Twitter account. If you have a Twitter account and want to scrape tweets that are not publicly available, you can pass the cookies of your logged-in account.
+- cookies (Required): The cookies of a logged-in Twitter account. If you have a Twitter account and want to scrape tweets that are not publicly available, you can pass the cookies of your logged-in account.
 
 - proxyList: (Optional) A list of proxies to use for scraping. The list should contain proxy addresses in the format ip:port:user:pw.
 
 
-## How to get account cookies:
+## How to get account cookies + x-csrf-token:
 Following a private "target" account is necessary to access its data. Then, account cookies can be used to scrape the account.
 1. Open the Chrome browser and go to the Twitter website.
 2. If you're not already logged in, log in to your Twitter account.
 3. Right-click anywhere on the page and select "Inspect" from the context menu. Alternatively, you can press "Ctrl+Shift+I" (Windows) or "Cmd+Option+I" (Mac) on your keyboard.
 4. This will open the Developer Tools pane. Click on the "Network" tab at the top and then filter with fetch/XHR.
 5. On the left-hand sidebar, click on any request.
-6. You should now see a list of metadata associated with this specific request. Look for the "Request Headers" section and then find the "cookies" entry. Copy the entire value of the cookies.
+6. You should now see a list of metadata associated with this specific request. Look for the "Request Headers" section and then find the "cookies" and x-csrf-token entries. Copy the entire value of the cookies and x-csrf-token.
 7. In your Python code, create a new instance of the TwitterScraper class and paste the cookie value as the value of the "cookies" parameter.
 8. That's it! You can now use the TwitterScraper class to scrape data from your Twitter account.  
 
 By following these steps, you should be able to retrieve the necessary cookies from your Twitter account and use them in your Python code to scrape data.
 
 ## Methodes:
 
@@ -147,8 +137,8 @@
 
 ### filterDescription(singleUserPlain)
         returns the description of an account
         :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
 ### getUserSpecificData(singleUserPlain)
         returns all (unfiltered) data about an account
-        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
```

### Comparing `ReverseTwitterScraper-0.7/README.md` & `ReverseTwitterScraper-0.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,35 @@
+Metadata-Version: 2.1
+Name: ReverseTwitterScraper
+Version: 0.8
+Summary: A Python package for scraping Twitter data without API. With proxy and account-cookie support
+Home-page: https://github.com/1220moritz/reverse-twitter-scraper
+Author: 1220moritz
+Project-URL: Documentation, https://github.com/1220moritz/reverse-twitter-scraper/blob/main/README.md
+Project-URL: Github, https://github.com/1220moritz/reverse-twitter-scraper
+Project-URL: PyPi, https://pypi.org/project/ReverseTwitterScraper/
+Project-URL: Contact, https://discordapp.com/users/713118695165263923
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ReverseTwitterScraper
+## Description
 ReverseTwitterScraper is a Python package that provides an easy-to-use tool for scraping tweets of a single or multiple Twitter accounts. This package uses Selenium and httpx to scrape tweets and other account data.
 
+## IMPORTANT NOTICE in 0.8
+**Twitter has introduced a change in its system, which now mandates the use of account cookies for viewing tweets.**
+
+Please note that the use of cookies is associated with a **high risk of account suspension or ban** by Twitter.  
+Using account cookies essentially means that you are automating actions on behalf of a specific user account, which is against Twitter's Terms of Service. Always make sure to use this tool responsibly, adhering to Twitter's rules, and avoid excessive or suspicious activity that could lead to account limitations. Always make sure that you are informed about and compliant with the Twitter Terms of Service, as well as all relevant privacy laws and regulations.   
+**The creators of the ReverseTwitterScraper are not responsible for any misuse of the tool or violations of these terms.**
+
 ## Links
 GitHub: https://github.com/1220moritz/reverse-twitter-scraper  
 PyPI: https://pypi.org/project/ReverseTwitterScraper/
 
 ## Installation
 To install the package, simply run the following command:
 ```
@@ -19,16 +44,15 @@
 3. Call any method of the TwitterScraper class.  
 
 Here's an example code:
 ```
 from ReverseTwitterScraper import TwitterScraper
 
 chromedriver_path = "C:/Program Files (x86)/chromedriver.exe"
-cookies = "" #no account cookies
-cookies = {'Cookie': 'your Cookie', 'X-Csrf-Token': 'your csrf token'} #with account cookie
+cookies = {'Cookie': 'your Cookie', 'X-Csrf-Token': 'your csrf token'} # required account cookie
 proxy_list = []
 
 
 twitter_handle = ["elonmusk"]  # single account
 twitter_handles = ["elonmusk", "POTUS", "latestinspace"]  # multiple accounts
 scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
 tweets = scraper.getTweetsText()
@@ -38,31 +62,31 @@
 
 In the above code, we first import the TwitterScraper class from the package. Then, we create an object of the TwitterScraper class with the required parameters.
 Finally, we call the getTweetsText() method to get the tweets of the specified Twitter account.
 
 ## Parameters
 The TwitterScraper class takes the following parameters:
 
-- twitterHandle: The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to ['elonmusk'].
+- twitterHandle (Required): The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to ['elonmusk'].
 
-- chromedriverPath: The path of the Chrome driver executable file. This file is required to use the Selenium module.
+- chromedriverPath (Required): The path of the Chrome driver executable file. This file is required to use the Selenium module.
 
-- cookies: (Optional) The cookies of a logged-in Twitter account. If you have a Twitter account and want to scrape tweets that are not publicly available, you can pass the cookies of your logged-in account.
+- cookies (Required): The cookies of a logged-in Twitter account. If you have a Twitter account and want to scrape tweets that are not publicly available, you can pass the cookies of your logged-in account.
 
 - proxyList: (Optional) A list of proxies to use for scraping. The list should contain proxy addresses in the format ip:port:user:pw.
 
 
-## How to get account cookies:
+## How to get account cookies + x-csrf-token:
 Following a private "target" account is necessary to access its data. Then, account cookies can be used to scrape the account.
 1. Open the Chrome browser and go to the Twitter website.
 2. If you're not already logged in, log in to your Twitter account.
 3. Right-click anywhere on the page and select "Inspect" from the context menu. Alternatively, you can press "Ctrl+Shift+I" (Windows) or "Cmd+Option+I" (Mac) on your keyboard.
 4. This will open the Developer Tools pane. Click on the "Network" tab at the top and then filter with fetch/XHR.
 5. On the left-hand sidebar, click on any request.
-6. You should now see a list of metadata associated with this specific request. Look for the "Request Headers" section and then find the "cookies" entry. Copy the entire value of the cookies.
+6. You should now see a list of metadata associated with this specific request. Look for the "Request Headers" section and then find the "cookies" and x-csrf-token entries. Copy the entire value of the cookies and x-csrf-token.
 7. In your Python code, create a new instance of the TwitterScraper class and paste the cookie value as the value of the "cookies" parameter.
 8. That's it! You can now use the TwitterScraper class to scrape data from your Twitter account.  
 
 By following these steps, you should be able to retrieve the necessary cookies from your Twitter account and use them in your Python code to scrape data.
 
 ## Methodes:
 
@@ -130,8 +154,8 @@
 
 ### filterDescription(singleUserPlain)
         returns the description of an account
         :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
 
 ### getUserSpecificData(singleUserPlain)
         returns all (unfiltered) data about an account
-        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
+        :param singleUserPlain: plain (unfiltered) info of a Twitter account. Use getUserPlain() to get the info
```

### Comparing `ReverseTwitterScraper-0.7/ReverseTwitterScraper/Scraper.py` & `ReverseTwitterScraper-0.8/ReverseTwitterScraper/Scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             return self.proxies[self.__proxyCounter]
         elif type(self.proxies) is list and self.__proxyCounter >= len(self.proxies) - 1: # restart with first proxy in list
             self.__proxyCounter = 0
             return self.proxies[self.__proxyCounter]
         else:
             return None
         
-    def __init__(self, twitterHandle: list, chromedriverPath: str, cookies="", proxyList=""):
+    def __init__(self, twitterHandle: list, chromedriverPath: str, cookies: dict, proxyList=""):
         """
         makes everything ready to scrape twitter.
 
         :param list twitterHandle: e.g. https://twitter.com/elonmusk -> handle = [elonmusk] or multiple handles ["elonmusk", "POTUS", "BitcoinMagazine"]
         :param str chromedriverPath: e.g. C:/Program Files (x86)/chromedriver.exe
         :param str cookies: your twitter account cookies
         :param arr proxyList: your array of proxies. ip:port:user:pw
@@ -81,28 +81,30 @@
 
         # get all the important data to send a request
         retries = 0
         while retries < 5:
             try:
                 self.getTwitterGuestData(cookies=cookies)
                 break
+            except KeyboardInterrupt:
+                exit("KeyboardInterrupt")
             except:
-                #print(traceback.format_exc())
+                print(traceback.format_exc())
                 retries += 1
                 self.__proxyCounter += 1
             
         retries = 0
         while retries < 5:
             try:
                 resp =  httpx.get(url=self.__reqUrl, headers=self.__headers, cookies=self.__cookies)
                 if resp.status_code == 200:
                     print("got valid meta-information")
                 break
             except:
-                #print(traceback.format_exc())
+                print(traceback.format_exc())
                 print("failed openingResp. Trying again with new proxy")
                 retries += 1
                 self.__proxyCounter += 1
                 self.getTwitterGuestData(cookies=self.__accCookies)
 
     async def __getID(self, client: httpx.Client, handle):
         headers = {'content-type': 'application/x-www-form-urlencoded; charset=UTF-8'}
@@ -126,22 +128,25 @@
             await client.aclose()
             return info
  
     def getTwitterGuestData(self, cookies):
         print("gathering meta-information")
         self.__resetData() #clear old data
             
-        # get driver
+        # create driver
         options = Options()
         options.add_argument("--headless")
         driver = webdriver.Chrome(self.__chromedriverPath, options=options) #headless
-        #driver = webdriver.Chrome(self.__chromedriverPath) #window
-    
-    
-        driver.get(f"https://twitter.com/{self.__twitterHandle[0]}") 
+        # driver = webdriver.Chrome(self.__chromedriverPath) #window
+
+        # add cookies to selenium
+        driver.get(f"https://twitter.com/{self.__twitterHandle[0]}") # get correct url to set cookies
+        for key, value in self.cookieDict(cookies['Cookie']).items():
+            driver.add_cookie({"name": key, "value": value})
+        driver.get(f"https://twitter.com/{self.__twitterHandle[0]}") # again same url to get needed headers
         
         
         headersDict = {}
         for headerReq in driver.requests:
             url = headerReq.url
             if "UserTweets" in url and "cursor" not in url:
                 self.__reqUrl = url
@@ -150,16 +155,15 @@
         
         driver.close()
         
         self.__headers = {
             'authorization': headersDict['authorization'],
             'cookie': headersDict['cookie'],
             'user-agent': headersDict['user-agent'],
-            'x-csrf-token': headersDict['x-csrf-token'],
-            'x-guest-token': headersDict['x-guest-token']
+            'x-csrf-token': headersDict['x-csrf-token']
         }
         
         # check for cookies
         if type(cookies) is dict and 'Cookie' in cookies and 'X-Csrf-Token' in cookies:
             self.__cookies = self.cookieDict(cookies['Cookie'])
             self.__headers['cookie'] = cookies['Cookie']
             self.__headers['x-csrf-token'] = cookies['X-Csrf-Token']
```

### Comparing `ReverseTwitterScraper-0.7/ReverseTwitterScraper.egg-info/PKG-INFO` & `ReverseTwitterScraper-0.8/ReverseTwitterScraper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseTwitterScraper
-Version: 0.7
+Version: 0.8
 Summary: A Python package for scraping Twitter data without API. With proxy and account-cookie support
 Home-page: https://github.com/1220moritz/reverse-twitter-scraper
 Author: 1220moritz
 Project-URL: Documentation, https://github.com/1220moritz/reverse-twitter-scraper/blob/main/README.md
 Project-URL: Github, https://github.com/1220moritz/reverse-twitter-scraper
 Project-URL: PyPi, https://pypi.org/project/ReverseTwitterScraper/
 Project-URL: Contact, https://discordapp.com/users/713118695165263923
@@ -12,16 +12,24 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ReverseTwitterScraper
+## Description
 ReverseTwitterScraper is a Python package that provides an easy-to-use tool for scraping tweets of a single or multiple Twitter accounts. This package uses Selenium and httpx to scrape tweets and other account data.
 
+## IMPORTANT NOTICE in 0.8
+**Twitter has introduced a change in its system, which now mandates the use of account cookies for viewing tweets.**
+
+Please note that the use of cookies is associated with a **high risk of account suspension or ban** by Twitter.  
+Using account cookies essentially means that you are automating actions on behalf of a specific user account, which is against Twitter's Terms of Service. Always make sure to use this tool responsibly, adhering to Twitter's rules, and avoid excessive or suspicious activity that could lead to account limitations. Always make sure that you are informed about and compliant with the Twitter Terms of Service, as well as all relevant privacy laws and regulations.   
+**The creators of the ReverseTwitterScraper are not responsible for any misuse of the tool or violations of these terms.**
+
 ## Links
 GitHub: https://github.com/1220moritz/reverse-twitter-scraper  
 PyPI: https://pypi.org/project/ReverseTwitterScraper/
 
 ## Installation
 To install the package, simply run the following command:
 ```
@@ -36,16 +44,15 @@
 3. Call any method of the TwitterScraper class.  
 
 Here's an example code:
 ```
 from ReverseTwitterScraper import TwitterScraper
 
 chromedriver_path = "C:/Program Files (x86)/chromedriver.exe"
-cookies = "" #no account cookies
-cookies = {'Cookie': 'your Cookie', 'X-Csrf-Token': 'your csrf token'} #with account cookie
+cookies = {'Cookie': 'your Cookie', 'X-Csrf-Token': 'your csrf token'} # required account cookie
 proxy_list = []
 
 
 twitter_handle = ["elonmusk"]  # single account
 twitter_handles = ["elonmusk", "POTUS", "latestinspace"]  # multiple accounts
 scraper = TwitterScraper(twitter_handle, chromedriver_path, cookies, proxy_list)
 tweets = scraper.getTweetsText()
@@ -55,31 +62,31 @@
 
 In the above code, we first import the TwitterScraper class from the package. Then, we create an object of the TwitterScraper class with the required parameters.
 Finally, we call the getTweetsText() method to get the tweets of the specified Twitter account.
 
 ## Parameters
 The TwitterScraper class takes the following parameters:
 
-- twitterHandle: The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to ['elonmusk'].
+- twitterHandle (Required): The Twitter handle of the account(s) to be scraped. For example, if the account URL is https://twitter.com/elonmusk, then the twitterHandle parameter should be set to ['elonmusk'].
 
-- chromedriverPath: The path of the Chrome driver executable file. This file is required to use the Selenium module.
+- chromedriverPath (Required): The path of the Chrome driver executable file. This file is required to use the Selenium module.
 
-- cookies: (Optional) The cookies of a logged-in Twitter account. If you have a Twitter account and want to scrape tweets that are not publicly available, you can pass the cookies of your logged-in account.
+- cookies (Required): The cookies of a logged-in Twitter account. If you have a Twitter account and want to scrape tweets that are not publicly available, you can pass the cookies of your logged-in account.
 
 - proxyList: (Optional) A list of proxies to use for scraping. The list should contain proxy addresses in the format ip:port:user:pw.
 
 
-## How to get account cookies:
+## How to get account cookies + x-csrf-token:
 Following a private "target" account is necessary to access its data. Then, account cookies can be used to scrape the account.
 1. Open the Chrome browser and go to the Twitter website.
 2. If you're not already logged in, log in to your Twitter account.
 3. Right-click anywhere on the page and select "Inspect" from the context menu. Alternatively, you can press "Ctrl+Shift+I" (Windows) or "Cmd+Option+I" (Mac) on your keyboard.
 4. This will open the Developer Tools pane. Click on the "Network" tab at the top and then filter with fetch/XHR.
 5. On the left-hand sidebar, click on any request.
-6. You should now see a list of metadata associated with this specific request. Look for the "Request Headers" section and then find the "cookies" entry. Copy the entire value of the cookies.
+6. You should now see a list of metadata associated with this specific request. Look for the "Request Headers" section and then find the "cookies" and x-csrf-token entries. Copy the entire value of the cookies and x-csrf-token.
 7. In your Python code, create a new instance of the TwitterScraper class and paste the cookie value as the value of the "cookies" parameter.
 8. That's it! You can now use the TwitterScraper class to scrape data from your Twitter account.  
 
 By following these steps, you should be able to retrieve the necessary cookies from your Twitter account and use them in your Python code to scrape data.
 
 ## Methodes:
```

### Comparing `ReverseTwitterScraper-0.7/setup.py` & `ReverseTwitterScraper-0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ReverseTwitterScraper",
-    version="0.7",
+    version="0.8",
     author="1220moritz",
     description="A Python package for scraping Twitter data without API. With proxy and account-cookie support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/1220moritz/reverse-twitter-scraper",
       install_requires=[
           'selenium-wire',
```

