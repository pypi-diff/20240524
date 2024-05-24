# Comparing `tmp/chatgptautomation-0.6.3.tar.gz` & `tmp/chatgptautomation-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgptautomation-0.6.3.tar", last modified: Mon May  6 13:45:13 2024, max compression
+gzip compressed data, was "chatgptautomation-0.7.0.tar", last modified: Fri May 24 13:53:46 2024, max compression
```

## Comparing `chatgptautomation-0.6.3.tar` & `chatgptautomation-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:45:13.976327 chatgptautomation-0.6.3/
-drwxrwxrwx   0        0        0        0 2024-05-06 13:45:13.975326 chatgptautomation-0.6.3/ChatGPTAutomation.egg-info/
--rw-rw-rw-   0        0        0     9679 2024-05-06 13:45:13.000000 chatgptautomation-0.6.3/ChatGPTAutomation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      399 2024-05-06 13:45:13.000000 chatgptautomation-0.6.3/ChatGPTAutomation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:45:13.000000 chatgptautomation-0.6.3/ChatGPTAutomation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      827 2024-05-06 13:45:13.000000 chatgptautomation-0.6.3/ChatGPTAutomation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-06 13:45:13.000000 chatgptautomation-0.6.3/ChatGPTAutomation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1111 2024-05-06 13:20:39.000000 chatgptautomation-0.6.3/LICENCE.md
--rw-rw-rw-   0        0        0     9679 2024-05-06 13:45:13.975326 chatgptautomation-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     6925 2024-05-06 13:20:39.000000 chatgptautomation-0.6.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 13:45:13.973326 chatgptautomation-0.6.3/chatgpt_automation/
--rw-rw-rw-   0        0        0        0 2024-05-06 13:20:39.000000 chatgptautomation-0.6.3/chatgpt_automation/__init__.py
--rw-rw-rw-   0        0        0    39576 2024-05-06 13:21:21.000000 chatgptautomation-0.6.3/chatgpt_automation/chatgpt_automation.py
--rw-rw-rw-   0        0        0     5956 2024-05-06 13:20:39.000000 chatgptautomation-0.6.3/chatgpt_automation/chromedriver_manager.py
--rw-rw-rw-   0        0        0       42 2024-05-06 13:45:13.976327 chatgptautomation-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1504 2024-05-06 13:23:18.000000 chatgptautomation-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 13:45:13.974327 chatgptautomation-0.6.3/tests/
--rw-rw-rw-   0        0        0        0 2024-05-06 13:20:39.000000 chatgptautomation-0.6.3/tests/__init__.py
--rw-rw-rw-   0        0        0     2762 2024-05-06 13:20:39.000000 chatgptautomation-0.6.3/tests/test_chatgpt_automation.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:53:46.797479 chatgptautomation-0.7.0/
+-rw-rw-rw-   0        0        0      144 2024-05-24 10:47:42.000000 chatgptautomation-0.7.0/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-24 13:53:46.795478 chatgptautomation-0.7.0/ChatGPTAutomation.egg-info/
+-rw-rw-rw-   0        0        0     9679 2024-05-24 13:53:46.000000 chatgptautomation-0.7.0/ChatGPTAutomation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2024-05-24 13:53:46.000000 chatgptautomation-0.7.0/ChatGPTAutomation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 13:53:46.000000 chatgptautomation-0.7.0/ChatGPTAutomation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      827 2024-05-24 13:53:46.000000 chatgptautomation-0.7.0/ChatGPTAutomation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-24 13:53:46.000000 chatgptautomation-0.7.0/ChatGPTAutomation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1111 2024-05-24 10:47:42.000000 chatgptautomation-0.7.0/LICENCE.md
+-rw-rw-rw-   0        0        0     9679 2024-05-24 13:53:46.796478 chatgptautomation-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6925 2024-05-24 10:47:42.000000 chatgptautomation-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 13:53:46.793512 chatgptautomation-0.7.0/chatgpt_automation/
+-rw-rw-rw-   0        0        0        0 2024-05-24 10:47:42.000000 chatgptautomation-0.7.0/chatgpt_automation/__init__.py
+-rw-rw-rw-   0        0        0    40086 2024-05-24 13:46:53.000000 chatgptautomation-0.7.0/chatgpt_automation/chatgpt_automation.py
+-rw-rw-rw-   0        0        0     5956 2024-05-24 10:47:42.000000 chatgptautomation-0.7.0/chatgpt_automation/chromedriver_manager.py
+-rw-rw-rw-   0        0        0      875 2024-05-24 10:47:42.000000 chatgptautomation-0.7.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 13:53:46.797479 chatgptautomation-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1504 2024-05-24 13:48:59.000000 chatgptautomation-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:53:46.794478 chatgptautomation-0.7.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-24 10:47:42.000000 chatgptautomation-0.7.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2762 2024-05-24 13:48:12.000000 chatgptautomation-0.7.0/tests/test_chatgpt_automation.py
```

### Comparing `chatgptautomation-0.6.3/ChatGPTAutomation.egg-info/PKG-INFO` & `chatgptautomation-0.7.0/ChatGPTAutomation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTAutomation
-Version: 0.6.3
+Version: 0.7.0
 Summary: A Python package for automating interactions with ChatGPT using Selenium. Chatgpt automation without api. Chatgptautomation
 Home-page: https://github.com/iamseyedalipro/ChatGPTAutomation
 Author: Seyed Ali Hosseini
 Author-email: iamseyedalipro@gmail.com
 Keywords: chatgpt automation selenium openai chatbot test automation webdriver gpt-3 automation gpt-4 automation file upload automation chat history retrieval login automation developers QA testers automation engineers pytest robot framework python library automation library best chatgpt automation tool selenium chatgpt integration
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `chatgptautomation-0.6.3/ChatGPTAutomation.egg-info/requires.txt` & `chatgptautomation-0.7.0/ChatGPTAutomation.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `chatgptautomation-0.6.3/LICENCE.md` & `chatgptautomation-0.7.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `chatgptautomation-0.6.3/PKG-INFO` & `chatgptautomation-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPTAutomation
-Version: 0.6.3
+Version: 0.7.0
 Summary: A Python package for automating interactions with ChatGPT using Selenium. Chatgpt automation without api. Chatgptautomation
 Home-page: https://github.com/iamseyedalipro/ChatGPTAutomation
 Author: Seyed Ali Hosseini
 Author-email: iamseyedalipro@gmail.com
 Keywords: chatgpt automation selenium openai chatbot test automation webdriver gpt-3 automation gpt-4 automation file upload automation chat history retrieval login automation developers QA testers automation engineers pytest robot framework python library automation library best chatgpt automation tool selenium chatgpt integration
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `chatgptautomation-0.6.3/README.md` & `chatgptautomation-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `chatgptautomation-0.6.3/chatgpt_automation/chatgpt_automation.py` & `chatgptautomation-0.7.0/chatgpt_automation/chatgpt_automation.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,41 +20,42 @@
                     format='%(asctime)s:%(levelname)s:%(message)s')
 
 
 class ChatGPTLocators:
     MSG_BOX_INPUT = (By.CSS_SELECTOR, 'textarea#prompt-textarea')
     MSG_BOX_INPUT2 = (By.TAG_NAME, 'textarea')
 
-    SEND_MSG_BTN = (By.CSS_SELECTOR, 'button[data-testid="send-button"]')
+    SEND_MSG_BTN = (By.XPATH, "//*[contains(@data-testid, 'send-button')]")
 
     GPT4_FILE_INPUT = (By.CSS_SELECTOR, 'input.hidden')
 
     CHAT_GPT_CONVERSION = (By.CSS_SELECTOR, 'div.text-base')
     REGENERATE_BTN = (By.CSS_SELECTOR, 'button[as="button"]')
 
     FIRST_DELETE_BTN = (By.CSS_SELECTOR, 'button[data-state="closed"]')
-    SECOND_DELETE_BTN = (By.CSS_SELECTOR, 'div[role="menuitem"].text-red-500')
+    SECOND_DELETE_BTN = (By.CSS_SELECTOR, 'div[role="menuitem"].text-token-text-error')
     THIRD_DELETE_BTN = (By.CSS_SELECTOR, 'button.btn.btn-danger[as="button"]')
 
-    RECYCLE_BTN = (By.CSS_SELECTOR, 'button.p-1.hover\:text-token-text-primary:nth-child(2)')
+    RECYCLE_BTN = (By.CSS_SELECTOR, 'button.p-1.hover\\:text-token-text-primary:nth-child(2)')
     DELETE_CONFIRM_BTN = (By.CSS_SELECTOR, 'button.btn.relative.btn-danger')
 
     NEW_CHAT_BTN = (By.CSS_SELECTOR, 'button.text-token-text-primary')
 
     LOGIN_BTN = (By.XPATH, '//button[//div[text()="Log in"]]')
     CONTINUE_BTN = (By.XPATH, '//button[text()="Continue"]')
     USERNAME_INPUT = (By.ID, "username")
     PASSWORD_INPUT = (By.ID, "password")
 
     CHATGPT_SWITCH_HOVER_BTN = (By.CSS_SELECTOR, 'div[aria-haspopup="menu"]')
-    CHAT_GPT_SWITCH_TO_4 = (By.XPATH, '//div[contains(text(), "GPT-4")]')
+    CHAT_GPT_SWITCH_TO_4 = (By.XPATH, '//div[text()="GPT-4"]')
     CHAT_GPT_SWITCH_TO_3 = (By.XPATH, '//div[contains(text(), "GPT-3.5")]')
+    CHAT_GPT_SWITCH_TO_4O = (By.XPATH, '//div[text()="GPT-4o"]')
     UPGRADE_TO_PLUS_BTN = (By.XPATH, '//div[contains(text(), "Upgrade to Plus")]')
     
-    COPY_LAST_RESPONSE_BTN = (By.CSS_SELECTOR, '.final-completion > div:nth-child(2) > div:nth-child(2) > div:nth-child(2) > div:nth-child(1) > button:nth-child(1)')
+    COPY_LAST_RESPONSE_BTN = (By.CSS_SELECTOR, '.rounded-lg.text-token-text-secondary.hover\\:bg-token-main-surface-secondary')
 
     LOGIN_WITH_GMAIL_BTN = (By.CSS_SELECTOR, 'form[data-provider="google"] button[data-provider="google"]')
     GMAIL_BTN = (By.XPATH, '//div[@data-email="{}"]')
 
     GMAIL_INPUT = (By.CSS_SELECTOR, 'input[type="email"][id="identifierId"]')
     GMAIL_NEXT_BTN = (By.ID, 'identifierNext')
     GMAIL_PASSWORD_INPUT = (By.CSS_SELECTOR, 'input[type="password"][name="password"]')
@@ -78,24 +79,25 @@
         GMAIL_SELECT_DELAY = 25
         AFTER_LOGIN_CLICK_DELAY = 5
         ADD_GMAIL_CLICK_DELAY = 3
         GMAIL_NEXT_CLICK_DELAY = 5
         GMAIL_PASSWORD_NEXT_CLICK_DELAY = 11
 
 
-    def __init__(self, chrome_path=None, chrome_driver_path=None, username: str = None, password: str=None):
+    def __init__(self, chrome_path=None, chrome_driver_path=None, username: str = None, password: str=None, user_data_dir= "remote-profile"):
         """
         This constructor automates the following steps:
         1. Open a Chrome browser with remote debugging enabled at a specified URL.
         2. Prompt the user to complete the log-in/registration/human verification, if required.
         3. Connect a Selenium WebDriver to the browser instance after human verification is completed.
 
         :param chrome_path: file path to chrome.exe (ex. C:\\Users\\User\\...\\chromedriver.exe)
         :param chrome_driver_path: file path to chrome.exe (ex. C:\\Users\\User\\...\\chromedriver.exe)
         """
+        self.user_data_dir = user_data_dir
         self.lock = threading.Lock()
         user_data_dir = r'--user-data-dir=C:\path\to\custom\user\data\directory'
         if chrome_path is None:
             chrome_path = self.get_chrome_path()
             if chrome_path is None:
                 raise FileNotFoundError("Unable to automatically find the Chrome path. "
                                 "Please provide the path to the Chrome executable.")
@@ -228,15 +230,15 @@
         Raises:
             RuntimeError: If there is an error in launching the Chrome browser.
         """
 
         def open_chrome():
             try:
                 # Construct the command to launch Chrome with specified debugging port and URL
-                chrome_cmd = f"{self.chrome_path} --remote-debugging-port={port} --user-data-dir=remote-profile {url}"
+                chrome_cmd = f"{self.chrome_path} --remote-debugging-port={port} --user-data-dir={self.user_data_dir} {url}"
                 # Execute the command in the system shell
                 os.system(chrome_cmd)
             except Exception as e:
                 # Log and raise an exception if there's an error in launching Chrome
                 logging.error(f"Failed to launch Chrome: {e}")
                 raise RuntimeError(f"Failed to launch Chrome with remote debugging: {e}")
 
@@ -395,15 +397,15 @@
 
             delimiter = "----------------------------------------"
             chatgpt_conversation = self.return_chatgpt_conversation()
             del chatgpt_conversation[::2]
 
             with open(os.path.join(directory_name, file_name), "a") as file:
                 for i in range(0, len(chatgpt_conversation)):
-                    file.write(f"{chatgpt_conversation[i].text}\n\n{delimiter}\n\n")
+                    file.write(f"{chatgpt_conversation[i]}\n\n{delimiter}\n\n")
 
         except FileNotFoundError as e:
             logging.error(f"File not found: {e}")
             raise
         except PermissionError as e:
             logging.error(f"Permission denied: {e}")
             raise
@@ -440,15 +442,15 @@
             logging.error(f'Unexpected error in return_last_response: {str(e)}')
             return f"An unexpected error occurred: {str(e)}"
     
     def return_last_response_md(self):
         try:
             copy_btns = self.driver.find_elements(*ChatGPTLocators.COPY_LAST_RESPONSE_BTN)
             if copy_btns:
-                copy_btns[0].click()
+                copy_btns[-3].click()
                 time.sleep(self.DelayTimes.RETURN_LAST_RESPONSE_DELAY)
                 return pyperclip.paste()
             else:
                 logging.warning("No copy button found.")
                 return "No copy button found."
 
         except Exception as e:
@@ -657,43 +659,49 @@
                 # If 'send' button is not found, continue the loop
                 pass
 
             # Log and wait before checking again
             logging.info("Responding...")
             time.sleep(self.DelayTimes.CHECK_RESPONSE_STATUS_DELAY)
 
-    def switch_model(self, model_name: float):
+    def switch_model(self, model_name: str):
         """
         Switches between different ChatGPT models in the application's user interface.
 
         :param model_name: A float representing the desired ChatGPT model version.
                         Supported values are 3.5 and 4.
         :return: None
         :raises: Exception if an unsupported model_name is provided.
         """
         menu_element = self.driver.find_element(*ChatGPTLocators.CHATGPT_SWITCH_HOVER_BTN)
 
         # Hover over the menu to activate it
         menu_element.click()
 
         # Wait for the submenu to be visible (adjust timeout as needed)
-        if model_name == 4:
+        if model_name == "4":
             submenu_locator = ChatGPTLocators.CHAT_GPT_SWITCH_TO_4
             try:
                 # Check for the UPGRADE_TO_PLUS_BTN
                 self.driver.find_element(*ChatGPTLocators.UPGRADE_TO_PLUS_BTN)
                 raise Exception("You must upgrade your ChatGPT account to plus")
             except NoSuchElementException:
                 pass
-        elif model_name == 3:
+        elif model_name == "3.5":
             submenu_locator = ChatGPTLocators.CHAT_GPT_SWITCH_TO_3
+        elif model_name == "4o":
+            submenu_locator = ChatGPTLocators.CHAT_GPT_SWITCH_TO_4O
+            try:
+                # Check for the UPGRADE_TO_PLUS_BTN
+                self.driver.find_element(*ChatGPTLocators.UPGRADE_TO_PLUS_BTN)
+                raise Exception("You must upgrade your ChatGPT account to plus")
+            except NoSuchElementException:
+                pass
         else:
             raise Exception("To switch between models, you need to set the 'model_name' to 3.5 or 4")
-
-
         
         submenu_element = WebDriverWait(self.driver, 10).until(EC.visibility_of_element_located(submenu_locator))
 
         # Click on the submenu item
         submenu_element.click()
     
     @staticmethod
```

### Comparing `chatgptautomation-0.6.3/chatgpt_automation/chromedriver_manager.py` & `chatgptautomation-0.7.0/chatgpt_automation/chromedriver_manager.py`

 * *Files identical despite different names*

### Comparing `chatgptautomation-0.6.3/setup.py` & `chatgptautomation-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read requirements from the requirements.txt file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='ChatGPTAutomation',
-    version='0.6.3',
+    version='0.7.0',
     author='Seyed Ali Hosseini',
     author_email='iamseyedalipro@gmail.com',
     description='A Python package for automating interactions with ChatGPT using Selenium. Chatgpt automation without api. Chatgptautomation',
     long_description=open('README.md', encoding="utf8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/iamseyedalipro/ChatGPTAutomation',
     packages=find_packages(),
```

### Comparing `chatgptautomation-0.6.3/tests/test_chatgpt_automation.py` & `chatgptautomation-0.7.0/tests/test_chatgpt_automation.py`

 * *Files identical despite different names*

