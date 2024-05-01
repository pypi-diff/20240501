# Comparing `tmp/openai_api_with_easy_tools_and_web_browsing-1.0.5.tar.gz` & `tmp/openai_api_with_easy_tools_and_web_browsing-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_with_easy_tools_and_web_browsing-1.0.5.tar", last modified: Mon Apr 29 21:34:54 2024, max compression
+gzip compressed data, was "openai_api_with_easy_tools_and_web_browsing-1.0.6.tar", last modified: Wed May  1 09:12:02 2024, max compression
```

## Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.5.tar` & `openai_api_with_easy_tools_and_web_browsing-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 21:34:54.263247 openai_api_with_easy_tools_and_web_browsing-1.0.5/
--rw-rw-rw-   0        0        0     1087 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     4627 2024-04-29 21:34:54.263247 openai_api_with_easy_tools_and_web_browsing-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3837 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/README.md
--rw-rw-rw-   0        0        0      879 2024-04-29 21:31:52.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 21:34:54.264249 openai_api_with_easy_tools_and_web_browsing-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 21:34:54.252159 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 21:34:54.262244 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/
--rw-rw-rw-   0        0        0     4627 2024-04-29 21:34:54.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-04-29 21:34:54.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 21:34:54.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-04-29 21:34:54.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       44 2024-04-29 21:34:54.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11022 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:34:54.261244 openai_api_with_easy_tools_and_web_browsing-1.0.5/tests/
--rw-rw-rw-   0        0        0     2851 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/tests/test.py
--rw-rw-rw-   0        0        0     2990 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/tests/test_fr.py
+drwxrwxrwx   0        0        0        0 2024-05-01 09:12:02.827296 openai_api_with_easy_tools_and_web_browsing-1.0.6/
+-rw-rw-rw-   0        0        0     1087 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4973 2024-05-01 09:12:02.826251 openai_api_with_easy_tools_and_web_browsing-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4183 2024-05-01 09:04:23.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/README.md
+-rw-rw-rw-   0        0        0      879 2024-05-01 09:08:40.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 09:12:02.828301 openai_api_with_easy_tools_and_web_browsing-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 09:12:02.792275 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 09:12:02.824920 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/
+-rw-rw-rw-   0        0        0     4973 2024-05-01 09:12:02.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-05-01 09:12:02.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 09:12:02.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-01 09:12:02.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2024-05-01 09:12:02.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11332 2024-05-01 08:42:51.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.py
+drwxrwxrwx   0        0        0        0 2024-05-01 09:12:02.823914 openai_api_with_easy_tools_and_web_browsing-1.0.6/tests/
+-rw-rw-rw-   0        0        0     2871 2024-05-01 08:40:45.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/tests/test.py
+-rw-rw-rw-   0        0        0     3009 2024-05-01 09:05:30.000000 openai_api_with_easy_tools_and_web_browsing-1.0.6/tests/test_fr.py
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.5/LICENSE` & `openai_api_with_easy_tools_and_web_browsing-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.5/PKG-INFO` & `openai_api_with_easy_tools_and_web_browsing-1.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_with_easy_tools_and_web_browsing
-Version: 1.0.5
+Version: 1.0.6
 Summary: An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools
 Author-email: ThomLecha <hamster12@hotmail.fr>
 Project-URL: Homepage, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing
 Project-URL: Issues, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,19 +21,21 @@
 
 If you ask the program:
 *Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result*
 
 The response, using a web search and a custom tool to add two numbers, should be something like:
 *The total population of Paris and New York in 2015 was about 31,082,144 inhabitants. If 10,000,000 is added to this number, it becomes 41,082,144.*
 
-See code below to reproduce this example.
+**See code below to reproduce this example.**
 
-First, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
+First, get an API key from OpenAI [here](https://openai.com/blog/openai-api) and get a Bing Custom Search API key, which you can get [here](https://azuremarketplace.microsoft.com/fr/marketplace/apps/Microsoft.BingCustomSearch?tab=Overview) ([free for limited use](https://www.microsoft.com/en-us/bing/apis/pricing))
 
-Then, you can use the following code to get started:
+Then, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
+
+And then, you can use the following code to get started:
 
 ```
 import openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
 
 # Enter our API keys
 subscriptionKey = ""
 openAIAPIKey = ""
@@ -75,20 +77,20 @@
     }
 }
 
 # Create an instance of the 'OpenaiApiWithEasyToolsAndWebBrowsing' class
 openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Return a response to a prompt in 'ponctual' mode ###
-print("\n\n\nPONCTUAL MODE\n")
+print("PONCTUAL MODE\n")
 prompt = "Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result"
 # Use the 'getLLMAnswerWithWebBrowsingAndTools' function to get a response from a user message
-answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
 # The response, using a web search and a custom tool to add two numbers, should be something like:
 # "The total population of Paris and New York in 2015 was about 31,082,144 inhabitants.
 # If 10,000,000 is added to this number, it becomes 41,082,144."
 print(answer)
 
 ### Discussion in 'continuous' mode ###
 print("\n\n\nCONTINUOUS MODE\n")
-openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
 ```
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.5/README.md` & `openai_api_with_easy_tools_and_web_browsing-1.0.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 
 If you ask the program:
 *Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result*
 
 The response, using a web search and a custom tool to add two numbers, should be something like:
 *The total population of Paris and New York in 2015 was about 31,082,144 inhabitants. If 10,000,000 is added to this number, it becomes 41,082,144.*
 
-See code below to reproduce this example.
+**See code below to reproduce this example.**
 
-First, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
+First, get an API key from OpenAI [here](https://openai.com/blog/openai-api) and get a Bing Custom Search API key, which you can get [here](https://azuremarketplace.microsoft.com/fr/marketplace/apps/Microsoft.BingCustomSearch?tab=Overview) ([free for limited use](https://www.microsoft.com/en-us/bing/apis/pricing))
 
-Then, you can use the following code to get started:
+Then, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
+
+And then, you can use the following code to get started:
 
 ```
 import openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
 
 # Enter our API keys
 subscriptionKey = ""
 openAIAPIKey = ""
@@ -59,20 +61,20 @@
     }
 }
 
 # Create an instance of the 'OpenaiApiWithEasyToolsAndWebBrowsing' class
 openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Return a response to a prompt in 'ponctual' mode ###
-print("\n\n\nPONCTUAL MODE\n")
+print("PONCTUAL MODE\n")
 prompt = "Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result"
 # Use the 'getLLMAnswerWithWebBrowsingAndTools' function to get a response from a user message
-answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
 # The response, using a web search and a custom tool to add two numbers, should be something like:
 # "The total population of Paris and New York in 2015 was about 31,082,144 inhabitants.
 # If 10,000,000 is added to this number, it becomes 41,082,144."
 print(answer)
 
 ### Discussion in 'continuous' mode ###
 print("\n\n\nCONTINUOUS MODE\n")
-openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
 ```
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.5/pyproject.toml` & `openai_api_with_easy_tools_and_web_browsing-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openai_api_with_easy_tools_and_web_browsing"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="ThomLecha", email="hamster12@hotmail.fr" },
 ]
 description = "An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools"
 
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO` & `openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_with_easy_tools_and_web_browsing
-Version: 1.0.5
+Version: 1.0.6
 Summary: An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools
 Author-email: ThomLecha <hamster12@hotmail.fr>
 Project-URL: Homepage, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing
 Project-URL: Issues, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,19 +21,21 @@
 
 If you ask the program:
 *Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result*
 
 The response, using a web search and a custom tool to add two numbers, should be something like:
 *The total population of Paris and New York in 2015 was about 31,082,144 inhabitants. If 10,000,000 is added to this number, it becomes 41,082,144.*
 
-See code below to reproduce this example.
+**See code below to reproduce this example.**
 
-First, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
+First, get an API key from OpenAI [here](https://openai.com/blog/openai-api) and get a Bing Custom Search API key, which you can get [here](https://azuremarketplace.microsoft.com/fr/marketplace/apps/Microsoft.BingCustomSearch?tab=Overview) ([free for limited use](https://www.microsoft.com/en-us/bing/apis/pricing))
 
-Then, you can use the following code to get started:
+Then, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
+
+And then, you can use the following code to get started:
 
 ```
 import openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
 
 # Enter our API keys
 subscriptionKey = ""
 openAIAPIKey = ""
@@ -75,20 +77,20 @@
     }
 }
 
 # Create an instance of the 'OpenaiApiWithEasyToolsAndWebBrowsing' class
 openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Return a response to a prompt in 'ponctual' mode ###
-print("\n\n\nPONCTUAL MODE\n")
+print("PONCTUAL MODE\n")
 prompt = "Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result"
 # Use the 'getLLMAnswerWithWebBrowsingAndTools' function to get a response from a user message
-answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
 # The response, using a web search and a custom tool to add two numbers, should be something like:
 # "The total population of Paris and New York in 2015 was about 31,082,144 inhabitants.
 # If 10,000,000 is added to this number, it becomes 41,082,144."
 print(answer)
 
 ### Discussion in 'continuous' mode ###
 print("\n\n\nCONTINUOUS MODE\n")
-openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
 ```
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.6/src/openai_api_with_easy_tools_and_web_browsing.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,119 +2,135 @@
 import openai
 import requests
 import json
 
 BING_CUSTOM_SEARCH_API_URL = "https://api.bing.microsoft.com/v7.0/custom/search?"
 
 class BingSearchEngine():
-    """Class to encapsulate Bing search functions and search result analysis."""
+    """We define a class to encapsulate Bing search functions and search result analysis."""
 
     def __init__(self, openAIAPIKey, subscriptionKey, model="gpt-3.5-turbo"):
-        """Initializes the OpenAI client and Bing subscription with the provided API keys."""
+        """Initialize the OpenAI client and the Bing subscription key using the provided API keys."""
         self.openaiClient = openai.OpenAI(api_key=openAIAPIKey)
         self.subscriptionKey = subscriptionKey
         self.model = model
 
     def getLLMAnswer(self, userMessage, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo") :
-        """This function interacts with a LLM to get a response from a user message."""
+        """This function interacts with an LLM to get a response from a user message."""
         chatCompletion = self.openaiClient.chat.completions.create(model=model, messages=[{"role": "system", "content": systemMessage}, {"role": "user", "content": userMessage}])
         return(chatCompletion.choices[0].message.content)
 
-    def runBingSearch(self, searchQuery, verbose=False):
+    def runBingSearch(self,searchQuery, verbosity=0):
         """This function performs a Bing search and returns the results as text."""
 
-        print("Running Bing search for query: " + searchQuery)
+        if verbosity >= 1:
+            print("Running Bing search for query: " + searchQuery)
 
-        # Create HTTP request
+        # Create the HTTP request
         bingQuery = BING_CUSTOM_SEARCH_API_URL + "q='" + searchQuery + "'&customconfig=0"
 
-        # Execute HTTP request
+        # Perform the HTTP request
         response = requests.get(bingQuery, headers={'Ocp-Apim-Subscription-Key': self.subscriptionKey})
 
         # Retrieve the results
         responseData = json.loads(response.text)
         results = responseData.get("webPages", {}).get("value", [])
 
-        # Format results properly
+        # Format the results properly
         searchResultsString = ""
-        for result in results:
-            searchResultsString += "Title: " + result["name"] + "\n"
-            searchResultsString += "URL: " + result["url"] + "\n"
-            searchResultsString += "Snippet: " + result["snippet"] + "\n\n"
+        for result in results :
+            searchResultsString += "Title : " + result["name"] + "\n"
+            searchResultsString += "URL : " + result["url"] + "\n"
+            searchResultsString += "Snippet : " + result["snippet"] + "\n\n"
 
-        # Remove the last newline
+        # Remove the last line break
         searchResultsString = searchResultsString[:-2]
 
-        if verbose:
-            print("bingQuery:")
+        if verbosity >= 2:
+            print("bingQuery :")
             print(bingQuery)
-            print("searchResultsString:")
+            print("searchResultsString :")
             print(searchResultsString)
 
         return(searchResultsString)
 
-    def getSearchQueries(self, userRequest, verbose=False):
-        """This function generates Bing search queries to fulfill the user's request (processed by a LLM)."""
 
-        print("Generating search queries for Bing to satisfy the user's request...")
-        # Enhance the prompt with examples to guide the generation of queries better
+
+    def getSearchQueries(self, userRequest, verbosity=0):
+        """This function generates Bing search queries to meet the user's request
+        (via processing by an LLM)"""
+
+        if verbosity >= 1:
+            print("Generating search queries for Bing to satisfy the user's request...")
+
+        # Enrich the prompt with examples to better guide the generation of queries
         prompt = "Based on the user's request, generate one or several (but non-redundant) short search queries for Bing. " \
                  "If the request covers multiple topics, provide separate queries for each topic, using semicolons to separate them." \
-                 "\nFor example, if the user asks about the population of Paris, Beijing, and Baghdad, give only the response: " \
+                 "\nFor example, if the user asks about the population of Paris, Beijing, and Baghdad, give only the response : " \
                  "'population Paris;current population Beijing;Baghdad population estimate'." \
-                 "\nSimilarly, if asked about both the height of the Eiffel Tower and historical events in 1923 in England, give only the response: " \
+                 "\nSimilarly, if asked about both the height of the Eiffel Tower and historical events in 1923 in England, give only the response : " \
                  "'Eiffel Tower height;historical events in 1923 England'." \
                  "Here is the user request: " + userRequest
 
         # Interact with the LLM to generate search queries
         searchQueries = self.getLLMAnswer(prompt, model=self.model)
 
-        # Split the response using the semicolon as a separator and trim unnecessary spaces
+        # Split the response using semicolon as a separator and eliminate unnecessary spaces
         searchQueriesList = [query.strip() for query in searchQueries.split(';')]
 
-        if verbose:
-            print("searchQueriesList:")
+        if verbosity >= 1:
+            print("searchQueriesList :")
             print(searchQueriesList)
 
         return(searchQueriesList)
 
-    def processSearchResults(self, userRequest, searchResultsString, verbose=False):
-        """This function analyzes Bing search results to respond to the user's request (processed by a LLM)."""
 
-        print("Processing Bing search results...")
-        # Interact with the LLM to analyze Bing search results
+
+    def processSearchResults(self, userRequest, searchResultsString, verbosity=0):
+        """This function analyzes the Bing search results to respond to the user's request
+        (via processing by an LLM)"""
+
+        if verbosity >= 1:
+            print("Processing Bing search results...")
+
+        # Interact with Anthropic's Haiku LLM to analyze Bing search results
         prompt = "Analyze these Bing search results below to give a short answer to this user request '" + userRequest + "'\n\n'" + searchResultsString + "'"
         analysis = self.getLLMAnswer(prompt, model=self.model)
 
-        if verbose:
-            print("analysis:")
+        if verbosity >= 2:
+            print("analysis :")
             print(analysis)
 
         # Return the analysis
         return(analysis)
 
-    def bingSearch(self, userRequest, verbose=False):
-        """This function performs a Bing search based on the user's request and analyzes the results (processed by a LLM)."""
+
+
+    def bingSearch(self, userRequest, verbosity=0):
+        """This function performs a Bing search based on the user's request and analyzes the results
+        (via processing by an LLM)"""
 
         # Generate one or more Bing search queries
-        searchQueriesList = self.getSearchQueries(userRequest, verbose=verbose)
+        searchQueriesList = self.getSearchQueries(userRequest, verbosity=verbosity)
 
-        # Execute Bing searches
-        searchResultsString = [self.runBingSearch(query, verbose) for query in searchQueriesList]
+        # Execute the Bing search(es)
+        searchResultsString = [self.runBingSearch(e, verbosity) for e in searchQueriesList]
 
-        # Concatenate search results with formatting to separate different queries
+        # Concatenate the search results with some formatting to separate the different queries
         cleanSearchResultsString = ""
         for i in range(len(searchResultsString)):
-            cleanSearchResultsString += "SEARCH QUERY " + str(i+1) + ": '" + searchQueriesList[i] + "'\n'''\n" + searchResultsString[i] + "'''\n\n"
+            cleanSearchResultsString += "SEARCH QUERY " + str(i+1) + " : '" + searchQueriesList[i] + "'\n'''\n" + searchResultsString[i] + "'''\n\n"
 
-        # Analyze search results
-        analysis = self.processSearchResults(userRequest, cleanSearchResultsString, verbose=verbose)
+        # Analyze the search result(s)
+        analysis = self.processSearchResults(userRequest, cleanSearchResultsString, verbosity=verbosity)
 
         # Return the analysis with an introductory text
-        return "HERE IS THE ANALYSIS OF THE BING SEARCH RESULT BASED ON THE USER'S REQUEST:\n" + analysis
+        analysis = "HERE IS THE ANALYSIS OF THE BING SEARCH RESULT BASED ON THE USER'S REQUEST : \n" + analysis
+
+        return(analysis)
 
 BING_SEARCH_DESCRIPTION = {
 "type": "function",
 "function": {
     "name": "bingSearch",
     "description": "Perform a Bing search based on the user's request and analyze the results",
     "parameters": {
@@ -127,98 +143,101 @@
             },
         "required": ["userRequest"]
         }
     }
 }
 
 class OpenaiApiWithEasyToolsAndWebBrowsing():
-    """This class allows interaction with the OpenAI API to obtain answers from user messages."""
+    """This class allows interacting with the OpenAI API to get responses from user messages."""
 
     def __init__(self, openAIAPIKey):
-        """Initializes the OpenAI client with the provided API key."""
+        """Initialize the OpenAI client with the provided API key."""
         self.openaiClient = openai.OpenAI(api_key=openAIAPIKey)
 
     def getMessageListFromThread(self, threadId):
-        """This function displays the messages of a thread/conversation. The output list is completed from right to left, the last message being the first in the list."""
+        """This function displays the messages of a thread/discussion thread.
+        The output list is populated from right to left, the last message is the first in the list."""
         messageList = self.openaiClient.beta.threads.messages.list(thread_id=threadId)
         messageListThread = [message.content[0].text.value for message in messageList if message.role == "assistant"]
         return(messageListThread)
 
     def waitForRunCompletion(self, threadId, runId):
-        """This function waits for the completion of a thread/conversation execution and returns the result."""
+        """This function waits for the completion of a thread/conversation run and returns the result"""
         while True:
-            # Check the execution status 10 times per second
+            # Check the status of the run 10 times per second
             time.sleep(0.1)
             run = self.openaiClient.beta.threads.runs.retrieve(thread_id=threadId, run_id=runId)
             if run.status in ["completed", "failed", "requires_action"]:
                 return(run)
-            # Below lines are unnecessary
-            elif run.status == "in_progress":
+            # Lines below are not necessary
+            elif run.status == "in_progress" :
                 continue
 
     def getToolReturnList(self, toolsToCall, toolList=[]):
-        """This function returns a list of tool outputs from a list of tools to be called."""
+        """This function returns a list of tool returns from a list of tools to call"""
 
         toolReturnList = []
 
-        # Call the requested tools one by one by the assistant
+        # Call the tools requested by the assistant one by one
         for tool in toolsToCall:
             toolReturn = None
             toolCallId = tool.id
             functionName = tool.function.name
             functionArgs = tool.function.arguments
 
-            # Search for the corresponding tool in the list of available tools
+            # Find the corresponding tool in the list of available tools
             for t in toolList:
                 if functionName == t.__name__:
                     toolReturn = t(**json.loads(functionArgs))
 
-            # Add the tool output to the list
+            # Add the tool return to the list
             toolReturnList.append({"tool_call_id": toolCallId, "output": toolReturn})
 
         return(toolReturnList)
 
-    def getLLMAnswerWithWebBrowsingAndTools(self, userMessage, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[], toolDescriptionList=[]) :
-        """This function interacts with a LLM to get a response from a user message. It includes 'ponctual' mode for a single return or 'continuous' mode for a continuous conversation with user input (set userMessage=None for the latter)."""
+    def getLLMAnswerWithWebBrowsingAndTools(self, userMessage, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[], toolDescriptionList=[], verbosity=0):
+        """This function interacts with an LLM to get a response from a user message.
+        There is 'ponctual' mode for a single response or 'continuous' mode for continuous conversation with user input (then set userMessage=None)."""
 
         # Initialize the assistant with the list of tools
         assistant = self.openaiClient.beta.assistants.create(instructions=systemMessage, model=model, tools=toolDescriptionList)
 
-        # Create a conversation thread
+        # Create a discussion thread
         thread = self.openaiClient.beta.threads.create()
 
         # Continuous conversation loop
         while True:
             if mode == "continuous":
-                print("Type 'exit' to exit the program. \nYour request: ")
+                print("\nYour request (Type 'exit' to exit the program) : ")
                 userMessage = input()
                 if userMessage.lower() == "exit":
                     break
 
-            # Create a message and an execution
+            # Create a message and a run
             self.openaiClient.beta.threads.messages.create(thread_id=thread.id, role="user", content=userMessage)
             run = self.openaiClient.beta.threads.runs.create(thread_id=thread.id, assistant_id=assistant.id)
-            # Wait for the execution to complete
+            # Wait for the end of the run
             run = self.waitForRunCompletion(thread.id, run.id)
 
-            # If (and while) the conversation execution returns a tool to call, it is called
+            # If (and as long as) the discussion run returns a tool to be called, call it
             while run.status == "requires_action":
                 # Retrieve the tools to be called
                 toolsToCall = run.required_action.submit_tool_outputs.tool_calls
-                print("Tools to call:")
-                [print("   " + str(t)) for t in toolsToCall]
+                if verbosity >= 1:
+                    print("Tools to call :")
+                    [print("   " + str(t)) for t in toolsToCall]
                 toolReturnList = self.getToolReturnList(toolsToCall, toolList=toolList)
                 run = self.openaiClient.beta.threads.runs.submit_tool_outputs(thread_id=thread.id, run_id=run.id, tool_outputs=toolReturnList)
-                # Wait for the execution to complete
+                # Wait for the end of the run
                 run = self.waitForRunCompletion(thread.id, run.id)
 
-            # If the conversation execution returns a failure, it is displayed
+            # If the discussion run returns a failure, display it
             if run.status == "failed":
                 print(run.error)
 
-            # If in 'ponctual' mode, display messages and exit the loop
+            # If in punctual mode, display the messages and exit the loop
             if mode == "ponctual":
                 return(self.getMessageListFromThread(thread.id)[0])
 
-            # Display messages and restart the loop to continue the conversation
-            print("Assistant response:\n" + self.getMessageListFromThread(thread.id)[0])
-            time.sleep(0.1)
+            # Display the messages and restart the loop to continue the conversation
+            print("\nAssistant response:\n" + self.getMessageListFromThread(thread.id)[0])
+            time.sleep(0.1)
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.5/tests/test.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.6/tests/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,19 +41,19 @@
     }
 }
 
 # Create an instance of the 'OpenaiApiWithEasyToolsAndWebBrowsing' class
 openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Return a response to a prompt in 'ponctual' mode ###
-print("\n\n\nPONCTUAL MODE\n")
+print("PONCTUAL MODE\n")
 prompt = "Can you search the internet for the population of Paris and New York in the year 2015, then add the two values together and tell me the result, and then add 10,000,000 to that result"
 # Use the 'getLLMAnswerWithWebBrowsingAndTools' function to get a response from a user message
-answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
 # The response, using a web search and a custom tool to add two numbers, should be something like:
 # "The total population of Paris and New York in 2015 was about 31,082,144 inhabitants.
 # If 10,000,000 is added to this number, it becomes 41,082,144."
 print(answer)
 
 ### Discussion in 'continuous' mode ###
 print("\n\n\nCONTINUOUS MODE\n")
-openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.5/tests/test_fr.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.6/tests/test_fr.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,19 @@
     }
 }
 
 # On crée une instance de la classe 'OpenaiApiWithEasyToolsAndWebBrowsing'
 openaiEpiWithEasyToolsAndWebBrowsing = webBrowsingApiGPT.OpenaiApiWithEasyToolsAndWebBrowsing(openAIAPIKey)
 
 ### Renvoie d'une réponse à un prompt en mode 'ponctual' ###
-print("\n\n\nMODE PONCTUEL\n")
+print("MODE PONCTUEL\n")
 prompt = "Tu peux chercher sur internet la population de Paris et de New York en l'année 2015, puis additionner les 2 valeurs et me dire le résultat, et enfin ensuite ajouter 10 000 000 à ce résultat"
 # On utilise la fonction 'getLLMAnswerWithWebBrowsingAndTools' pour obtenir une réponse à partir d'un message utilisateur
-answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+answer = openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(prompt, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="ponctual", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
 # La réponse, en utilisant l'outil de web browsing et l'additionneur doit être quelque chose du genre :
 # "La population totale de Paris et de New York en 2015 était d'environ 31 082 144 habitants.
 # Si l'on ajoute 10 000 000 à ce nombre, on obtient 41 082 144."
 print(answer)
 
-### Discussion en mode 'continuous' ###
+### Discussion en mode 'continuous' ###s
 print("\n\n\nMODE CONTINUE\n")
-openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription])
+openaiEpiWithEasyToolsAndWebBrowsing.getLLMAnswerWithWebBrowsingAndTools(None, systemMessage="You are a helpful assistant", model="gpt-3.5-turbo", mode="continuous", toolList=[bingSearch, adder], toolDescriptionList=[bingSearchDescription, adderDescription], verbosity=1)
```

