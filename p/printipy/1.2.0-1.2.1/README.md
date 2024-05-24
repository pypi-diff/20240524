# Comparing `tmp/printipy-1.2.0.tar.gz` & `tmp/printipy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printipy-1.2.0.tar", last modified: Wed Jan 24 21:28:19 2024, max compression
+gzip compressed data, was "printipy-1.2.1.tar", last modified: Fri May 24 19:20:43 2024, max compression
```

## Comparing `printipy-1.2.0.tar` & `printipy-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:28:19.208987 printipy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-24 21:28:12.000000 printipy-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-01-24 21:28:19.208987 printipy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-01-24 21:28:12.000000 printipy-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:28:19.208987 printipy-1.2.0/printipy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-24 21:28:12.000000 printipy-1.2.0/printipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71424 2024-01-24 21:28:12.000000 printipy-1.2.0/printipy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37429 2024-01-24 21:28:12.000000 printipy-1.2.0/printipy/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-01-24 21:28:12.000000 printipy-1.2.0/printipy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 21:28:19.208987 printipy-1.2.0/printipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-01-24 21:28:19.000000 printipy-1.2.0/printipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-24 21:28:19.000000 printipy-1.2.0/printipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 21:28:19.000000 printipy-1.2.0/printipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-24 21:28:19.000000 printipy-1.2.0/printipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-24 21:28:19.000000 printipy-1.2.0/printipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 21:28:19.208987 printipy-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-24 21:28:12.000000 printipy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:20:43.562303 printipy-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 19:20:40.000000 printipy-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-24 19:20:43.562303 printipy-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-24 19:20:40.000000 printipy-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:20:43.558303 printipy-1.2.1/printipy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:20:40.000000 printipy-1.2.1/printipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63864 2024-05-24 19:20:40.000000 printipy-1.2.1/printipy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34789 2024-05-24 19:20:40.000000 printipy-1.2.1/printipy/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-24 19:20:40.000000 printipy-1.2.1/printipy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:20:43.562303 printipy-1.2.1/printipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-24 19:20:43.000000 printipy-1.2.1/printipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-24 19:20:43.000000 printipy-1.2.1/printipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:20:43.000000 printipy-1.2.1/printipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 19:20:43.000000 printipy-1.2.1/printipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 19:20:43.000000 printipy-1.2.1/printipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:20:43.562303 printipy-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-24 19:20:40.000000 printipy-1.2.1/setup.py
```

### Comparing `printipy-1.2.0/LICENSE` & `printipy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `printipy-1.2.0/PKG-INFO` & `printipy-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: printipy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Printify API for Python
 Home-page: https://github.com/lawrencemq/printipy
 Author: Lawrence Weikum
 Keywords: printify,print on demand,api
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: dataclasses-json
 
 # PrintiPy
 The Printify API for Python
 
 Printify's REST API gives your scripts or applications power to manage Printify shops. Create and update products, submit orders, build custom integrations, and so much more!
 
-Tested with Python 3.9 - 3.11.
+Tested with Python 3.9 - 3.12.
 
 ## Install
 
 ```shell
 pipenv install printipy
 ```
```

### Comparing `printipy-1.2.0/README.md` & `printipy-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PrintiPy
 The Printify API for Python
 
 Printify's REST API gives your scripts or applications power to manage Printify shops. Create and update products, submit orders, build custom integrations, and so much more!
 
-Tested with Python 3.9 - 3.11.
+Tested with Python 3.9 - 3.12.
 
 ## Install
 
 ```shell
 pipenv install printipy
 ```
```

### Comparing `printipy-1.2.0/printipy/api.py` & `printipy-1.2.1/printipy/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,1524 +4,1613 @@
 from copy import deepcopy
 from json import JSONDecodeError
 from typing import List, Optional, Dict, Union, Any
 
 import requests
 from requests import Response
 
-from printipy.data_objects import Shop, Blueprint, PrintProvider, PrintProviderVariants, \
-    ShippingInfo, ShippingCost, CreateShippingEstimate, Product, Publish, PublishingSucceeded, Order, \
-    CreateOrderByExistingProduct, CreateOrderByAdvancedImageProcessing, \
-    CreateOrderByPrintDetails, CreateOrderBySku, Artwork, Webhook, CreateWebhook, UpdateWebhook, \
-    CreateProduct, UpdateProduct
-from printipy.exceptions import PrintiPyException, PrintiPyParseException, InvalidScopeException, \
-    InvalidRequestException, PrintifyException
+from printipy.data_objects import (
+	Shop,
+	Blueprint,
+	PrintProvider,
+	PrintProviderVariants,
+	ShippingInfo,
+	ShippingCost,
+	CreateShippingEstimate,
+	Product,
+	Publish,
+	PublishingSucceeded,
+	Order,
+	CreateOrderByExistingProduct,
+	CreateOrderByAdvancedImageProcessing,
+	CreateOrderByPrintDetails,
+	CreateOrderBySku,
+	Artwork,
+	Webhook,
+	CreateWebhook,
+	UpdateWebhook,
+	CreateProduct,
+	UpdateProduct,
+)
+from printipy.exceptions import (
+	PrintiPyException,
+	PrintiPyParseException,
+	InvalidScopeException,
+	InvalidRequestException,
+	PrintifyException,
+)
 
 
 class _ApiHandlingMixin:
-    api_url = 'https://api.printify.com'
+	api_url = 'https://api.printify.com'
 
-    def __init__(self, api_token: str):
-        self.api_token = api_token
+	def __init__(self, api_token: str):
+		self.api_token = api_token
 
-    @staticmethod
-    def __check_status(resp: Response, url: str):
-        if resp.status_code == 400:
-            try:
-                info = json.loads(resp.text)
-                message = f'{info["message"]} {info["errors"]["reason"]}'
-            except JSONDecodeError:
-                message = f'Bad Request: {url}'
-            raise PrintifyException(message)
-        elif resp.status_code == 403:
-            raise InvalidScopeException('This API key is not permitted to access this information.')
-        elif resp.status_code == 500:
-            raise InvalidRequestException(f'Bad request to {url}')
-        data = resp.json()
-        if 'error' in data:
-            raise PrintifyException(data['error'])
-        return data
-
-    def _get(self, url):
-        headers = {'Authorization': f'Bearer {self.api_token}'}
-        resp = requests.get(url, headers=headers)
-        data = self.__check_status(resp, url)
-        return data
-
-    def _post(self, url: str, data: Optional[Dict[str, Any]] = None):
-        headers = {'Authorization': f'Bearer {self.api_token}', 'content-type': 'application/json'}
-        resp = requests.post(url, headers=headers, json=data)
-        data = self.__check_status(resp, url)
-        return data
-
-    def _put(self, url, data):
-        headers = {'Authorization': f'Bearer {self.api_token}', 'content-type': 'application/json'}
-        resp = requests.put(url, headers=headers, json=data)
-        data = self.__check_status(resp, url)
-        return data
-
-    def _delete(self, url):
-        headers = {'Authorization': f'Bearer {self.api_token}'}
-        resp = requests.delete(url, headers=headers)
-        data = self.__check_status(resp, url)
-        return data
-
-    @staticmethod
-    def _parse(clazz, data: Union[List, Dict]):
-        if type(data) == list:
-            all_elements = []
-            for item in data:
-                all_elements.append(clazz.from_dict(item))
-            return all_elements
-        elif type(data) == dict:
-            return clazz.from_dict(data)
-        else:
-            raise PrintiPyParseException('Unable to parse response: was not a list or object')
-
-    @staticmethod
-    def _get_next_page_url(initial_url: str, info: Dict) -> Optional[str]:
-        next_page = info.get('next_page_url', None)
-        if not next_page:
-            return None
-        return f'{initial_url}{next_page}'
+	@staticmethod
+	def __check_status(resp: Response, url: str):
+		if resp.status_code == 400:
+			try:
+				info = json.loads(resp.text)
+				message = f'{info["message"]} {info["errors"]["reason"]}'
+			except JSONDecodeError:
+				message = f'Bad Request: {url}'
+			raise PrintifyException(message)
+		elif resp.status_code == 403:
+			raise InvalidScopeException('This API key is not permitted to access this information.')
+		elif resp.status_code == 500:
+			raise InvalidRequestException(f'Bad request to {url}')
+		data = resp.json()
+		if 'error' in data:
+			raise PrintifyException(data['error'])
+		return data
+
+	def _get(self, url):
+		headers = {'Authorization': f'Bearer {self.api_token}'}
+		resp = requests.get(url, headers=headers)
+		data = self.__check_status(resp, url)
+		return data
+
+	def _post(self, url: str, data: Optional[Dict[str, Any]] = None):
+		headers = {
+			'Authorization': f'Bearer {self.api_token}',
+			'content-type': 'application/json',
+		}
+		resp = requests.post(url, headers=headers, json=data)
+		data = self.__check_status(resp, url)
+		return data
+
+	def _put(self, url, data):
+		headers = {
+			'Authorization': f'Bearer {self.api_token}',
+			'content-type': 'application/json',
+		}
+		resp = requests.put(url, headers=headers, json=data)
+		data = self.__check_status(resp, url)
+		return data
+
+	def _delete(self, url):
+		headers = {'Authorization': f'Bearer {self.api_token}'}
+		resp = requests.delete(url, headers=headers)
+		data = self.__check_status(resp, url)
+		return data
+
+	@staticmethod
+	def _parse(clazz, data: Union[List, Dict]):
+		if isinstance(data, list):
+			all_elements = []
+			for item in data:
+				all_elements.append(clazz.from_dict(item))
+			return all_elements
+		elif isinstance(data, dict):
+			return clazz.from_dict(data)
+		else:
+			raise PrintiPyParseException('Unable to parse response: was not a list or object')
+
+	@staticmethod
+	def _get_next_page_url(initial_url: str, info: Dict) -> Optional[str]:
+		next_page = info.get('next_page_url', None)
+		if not next_page:
+			return None
+		return f'{initial_url}{next_page}'
 
 
 class PrintiPyShop(_ApiHandlingMixin):
-    """
-    Used to access the [Printify Shops](https://developers.printify.com/#shops) APIs
+	"""
+	Used to access the [Printify Shops](https://developers.printify.com/#shops) APIs
 
-    Examples:
-        >>> from printipy.api import PrintiPy
-        >>> api = PrintiPy(api_token='...')
-        >>> shops = api.shops.get_shops()
-    """
-
-    def get_shops(self) -> List[Shop]:
-        """
-        Pulls a list of shops for a Printify account. Returns empty list if no shops exist for account.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> shops = api.shops.get_shops()
-
-        Returns:
-            List of `printipy.data_objects.Shop` objects
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        shops_url = f'{self.api_url}/v1/shops.json'
-        shop_information = self._get(shops_url)
-        return self._parse(Shop, shop_information)
-
-    def delete_shop(self, shop: Shop) -> None:
-        """
-        Deletes a shop from a Printify account
-
-        Examples:
-            By pass in data pulled from `printipy.api.PrintiPyShop.get_shops`
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> shops = api.shops.get_shops()
-            >>> api.shops.delete_shop(shops[0])
-
-            By passing in specific shop information
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import Shop
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> api.shops.delete_shop(shop)
-
-        Args:
-            shop (Shop): A Shop to delete. Pull all shops using :func:`get_shops <printipy.api.PrintiPyShop.get_shops>`
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        delete_url = f'{self.api_url}/v1/shops/{shop.id}/connection.json'
-        self._delete(delete_url)
+	Examples:
+	    >>> from printipy.api import PrintiPy
+	    >>> api = PrintiPy(api_token='...')
+	    >>> shops = api.shops.get_shops()
+	"""
+
+	def get_shops(self) -> List[Shop]:
+		"""
+		Pulls a list of shops for a Printify account. Returns empty list if no shops exist for account.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> shops = api.shops.get_shops()
+
+		Returns:
+		    List of `printipy.data_objects.Shop` objects
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		shops_url = f'{self.api_url}/v1/shops.json'
+		shop_information = self._get(shops_url)
+		return self._parse(Shop, shop_information)
+
+	def delete_shop(self, shop: Shop) -> None:
+		"""
+		Deletes a shop from a Printify account
+
+		Examples:
+		    By pass in data pulled from `printipy.api.PrintiPyShop.get_shops`
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> shops = api.shops.get_shops()
+		    >>> api.shops.delete_shop(shops[0])
+
+		    By passing in specific shop information
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import Shop
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> api.shops.delete_shop(shop)
+
+		Args:
+		    shop (Shop): A Shop to delete. Pull all shops using :func:`get_shops <printipy.api.PrintiPyShop.get_shops>`
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		delete_url = f'{self.api_url}/v1/shops/{shop.id}/connection.json'
+		self._delete(delete_url)
 
 
 class PrintiPyCatalog(_ApiHandlingMixin):
-    """
-    Used to access the [Printify Catalog](https://developers.printify.com/#catalog) APIs
+	"""
+	Used to access the [Printify Catalog](https://developers.printify.com/#catalog) APIs
 
-    Examples:
-        >>> from printipy.api import PrintiPy
-        >>> api = PrintiPy(api_token='...')
-        >>> print_providers = api.catalog.get_print_providers()
-    """
-    def get_blueprints(self) -> List[Blueprint]:
-        """
-        Pulls a list of all blueprints available from Printify.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> blueprints = api.catalog.get_blueprints()
-
-        Returns:
-            List of `printipy.data_objects.Blueprint` objects
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-        """
-        blueprint_url = f'{self.api_url}/v1/catalog/blueprints.json'
-        blueprint_information = self._get(blueprint_url)
-        return self._parse(Blueprint, blueprint_information)
-
-    def get_blueprint(self, blueprint_id: Union[str, int]) -> Blueprint:
-        """
-        Pulls a specific blueprint from Printify.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> blueprint = api.catalog.get_blueprint('...')
-
-        Returns:
-            Blueprint `printipy.data_objects.Blueprint` object
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the Blueprint ID does not exist in Printify
-        """
-        # GET / v1 / catalog / blueprints / {blueprint_id}.json
-        blueprint_url = f'{self.api_url}/v1/catalog/blueprints/{blueprint_id}.json'
-        blueprint_information = self._get(blueprint_url)
-        return self._parse(Blueprint, blueprint_information)
-
-    def get_print_providers_for_blueprint(self, blueprint_id: Union[str, int]) -> List[PrintProvider]:
-        """
-        Pulls a list of print providers for a given blueprint from Printify.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> blueprint = api.catalog.get_blueprint('...')
-            >>> print_providers = api.catalog.get_print_providers_for_blueprint(blueprint.id)
-
-        Returns:
-            List of `printipy.data_objects.PrintProvider` objects
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the Blueprint ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # GET / v1 / catalog / blueprints / {blueprint_id} / print_providers.json
-        print_providers_url = f'{self.api_url}/v1/catalog/blueprints/{blueprint_id}/print_providers.json'
-        print_provider_information = self._get(print_providers_url)
-        return self._parse(PrintProvider, print_provider_information)
-
-    def get_variants(self, blueprint_id: Union[str, int], print_provider_id: Union[str, int]) -> PrintProviderVariants:
-        """
-        Pulls a list of variants for a given blueprint and print provider from Printify.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> blueprint = api.catalog.get_blueprint('...')
-            >>> print_providers = api.catalog.get_print_providers_for_blueprint(blueprint.id)
-            >>> variants = api.catalog.get_variants(blueprint.id, print_providers[0].id)
-
-        Returns:
-            Variant `printipy.data_objects.PrintProviderVariants` object
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the Blueprint ID or Print Provider ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # GET / v1 / catalog / blueprints / {blueprint_id} / print_providers / {print_provider_id} / variants.json
-        variants_url = f'{self.api_url}/v1/catalog/blueprints/{blueprint_id}/' \
-                       f'print_providers/{print_provider_id}/variants.json'
-        variant_information = self._get(variants_url)
-        return self._parse(PrintProviderVariants, variant_information)
-
-    def get_shipping_info(self, blueprint_id: Union[str, int], print_provider_id: Union[str, int]) -> ShippingInfo:
-        """
-        Pulls a shipping information a given blueprint and print provider from Printify.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> blueprint = api.catalog.get_blueprint('...')
-            >>> print_providers = api.catalog.get_print_providers_for_blueprint(blueprint.id)
-            >>> shipping_info = api.catalog.get_shipping_info(blueprint.id, print_providers[0].id)
-
-        Returns:
-            Shipping information `printipy.data_objects.ShippingInfo` object
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the Blueprint ID or Print Provider ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # GET / v1 / catalog / blueprints / {blueprint_id} / print_providers / {print_provider_id} / shipping.json
-        shipping_url = f'{self.api_url}/v1/catalog/blueprints/{blueprint_id}/' \
-                       f'print_providers/{print_provider_id}/shipping.json'
-        shipping_information = self._get(shipping_url)
-        return self._parse(ShippingInfo, shipping_information)
-
-    def get_print_providers(self) -> List[PrintProvider]:
-        """
-        Pulls a list of all print providers from Printify.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> print_providers = api.catalog.get_print_providers()
-
-        Returns:
-            List of `printipy.data_objects.PrintProvider` objects
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # GET / v1 / catalog / print_providers.json
-        print_providers_url = f'{self.api_url}/v1/catalog/print_providers.json'
-        print_provider_information = self._get(print_providers_url)
-        return self._parse(PrintProvider, print_provider_information)
-
-    def get_print_provider(self, print_provider_id: Union[str, int]) -> PrintProvider:
-        """
-        Pulls a specific print provider from Printify.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> print_provider = api.catalog.get_print_provider('...')
-
-        Returns:
-            Print Provider `printipy.data_objects.PrintProvider` object
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the Print Provider ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # GET / v1 / catalog / print_providers / {print_provider_id}.json
-        print_provider_url = f'{self.api_url}/v1/catalog/print_providers/{print_provider_id}.json'
-        print_provider_information = self._get(print_provider_url)
-        return self._parse(PrintProvider, print_provider_information)
+	Examples:
+	    >>> from printipy.api import PrintiPy
+	    >>> api = PrintiPy(api_token='...')
+	    >>> print_providers = api.catalog.get_print_providers()
+	"""
+
+	def get_blueprints(self) -> List[Blueprint]:
+		"""
+		Pulls a list of all blueprints available from Printify.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> blueprints = api.catalog.get_blueprints()
+
+		Returns:
+		    List of `printipy.data_objects.Blueprint` objects
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		"""
+		blueprint_url = f'{self.api_url}/v1/catalog/blueprints.json'
+		blueprint_information = self._get(blueprint_url)
+		return self._parse(Blueprint, blueprint_information)
+
+	def get_blueprint(self, blueprint_id: Union[str, int]) -> Blueprint:
+		"""
+		Pulls a specific blueprint from Printify.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> blueprint = api.catalog.get_blueprint('...')
+
+		Returns:
+		    Blueprint `printipy.data_objects.Blueprint` object
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the Blueprint ID does not exist in Printify
+		"""
+		# GET / v1 / catalog / blueprints / {blueprint_id}.json
+		blueprint_url = f'{self.api_url}/v1/catalog/blueprints/{blueprint_id}.json'
+		blueprint_information = self._get(blueprint_url)
+		return self._parse(Blueprint, blueprint_information)
+
+	def get_print_providers_for_blueprint(
+		self, blueprint_id: Union[str, int]
+	) -> List[PrintProvider]:
+		"""
+		Pulls a list of print providers for a given blueprint from Printify.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> blueprint = api.catalog.get_blueprint('...')
+		    >>> print_providers = api.catalog.get_print_providers_for_blueprint(blueprint.id)
+
+		Returns:
+		    List of `printipy.data_objects.PrintProvider` objects
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the Blueprint ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# GET / v1 / catalog / blueprints / {blueprint_id} / print_providers.json
+		print_providers_url = (
+			f'{self.api_url}/v1/catalog/blueprints/{blueprint_id}/print_providers.json'
+		)
+		print_provider_information = self._get(print_providers_url)
+		return self._parse(PrintProvider, print_provider_information)
+
+	def get_variants(
+		self, blueprint_id: Union[str, int], print_provider_id: Union[str, int]
+	) -> PrintProviderVariants:
+		"""
+		Pulls a list of variants for a given blueprint and print provider from Printify.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> blueprint = api.catalog.get_blueprint('...')
+		    >>> print_providers = api.catalog.get_print_providers_for_blueprint(blueprint.id)
+		    >>> variants = api.catalog.get_variants(blueprint.id, print_providers[0].id)
+
+		Returns:
+		    Variant `printipy.data_objects.PrintProviderVariants` object
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the Blueprint ID or Print Provider ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# GET / v1 / catalog / blueprints / {blueprint_id} / print_providers / {print_provider_id} / variants.json
+		variants_url = (
+			f'{self.api_url}/v1/catalog/blueprints/{blueprint_id}/'
+			f'print_providers/{print_provider_id}/variants.json'
+		)
+		variant_information = self._get(variants_url)
+		return self._parse(PrintProviderVariants, variant_information)
+
+	def get_shipping_info(
+		self, blueprint_id: Union[str, int], print_provider_id: Union[str, int]
+	) -> ShippingInfo:
+		"""
+		Pulls a shipping information a given blueprint and print provider from Printify.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> blueprint = api.catalog.get_blueprint('...')
+		    >>> print_providers = api.catalog.get_print_providers_for_blueprint(blueprint.id)
+		    >>> shipping_info = api.catalog.get_shipping_info(blueprint.id, print_providers[0].id)
+
+		Returns:
+		    Shipping information `printipy.data_objects.ShippingInfo` object
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the Blueprint ID or Print Provider ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# GET / v1 / catalog / blueprints / {blueprint_id} / print_providers / {print_provider_id} / shipping.json
+		shipping_url = (
+			f'{self.api_url}/v1/catalog/blueprints/{blueprint_id}/'
+			f'print_providers/{print_provider_id}/shipping.json'
+		)
+		shipping_information = self._get(shipping_url)
+		return self._parse(ShippingInfo, shipping_information)
+
+	def get_print_providers(self) -> List[PrintProvider]:
+		"""
+		Pulls a list of all print providers from Printify.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> print_providers = api.catalog.get_print_providers()
+
+		Returns:
+		    List of `printipy.data_objects.PrintProvider` objects
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# GET / v1 / catalog / print_providers.json
+		print_providers_url = f'{self.api_url}/v1/catalog/print_providers.json'
+		print_provider_information = self._get(print_providers_url)
+		return self._parse(PrintProvider, print_provider_information)
+
+	def get_print_provider(self, print_provider_id: Union[str, int]) -> PrintProvider:
+		"""
+		Pulls a specific print provider from Printify.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> print_provider = api.catalog.get_print_provider('...')
+
+		Returns:
+		    Print Provider `printipy.data_objects.PrintProvider` object
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the Print Provider ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# GET / v1 / catalog / print_providers / {print_provider_id}.json
+		print_provider_url = f'{self.api_url}/v1/catalog/print_providers/{print_provider_id}.json'
+		print_provider_information = self._get(print_provider_url)
+		return self._parse(PrintProvider, print_provider_information)
 
 
 class _ShopIdMixin:
-    def __init__(self, shop_id: Optional[Union[str, int]]):
-        self.__shop_id = shop_id
+	def __init__(self, shop_id: Optional[Union[str, int]]):
+		self.__shop_id = shop_id
 
-    def _get_shop_id(self, shop_id: Optional[Union[str, int]]):
-        shop_id_to_use = shop_id or self.__shop_id
-        if not shop_id_to_use:
-            raise PrintiPyException(
-                "No shop_id was specified. Add it to the method call or the instantiation of the API.")
-        return shop_id_to_use
-
-    def _require_shop_id(func):
-        def inner(ref, *args, **kwargs):
-            given_shop_id = kwargs.pop('shop_id', None)
-            shop_id = ref._get_shop_id(given_shop_id)
-            return func(ref, *args, **kwargs, shop_id=shop_id)
+	def _get_shop_id(self, shop_id: Optional[Union[str, int]]):
+		shop_id_to_use = shop_id or self.__shop_id
+		if not shop_id_to_use:
+			raise PrintiPyException(
+				'No shop_id was specified. Add it to the method call or the instantiation of the API.'
+			)
+		return shop_id_to_use
+
+	def _require_shop_id(func):
+		def inner(ref, *args, **kwargs):
+			given_shop_id = kwargs.pop('shop_id', None)
+			shop_id = ref._get_shop_id(given_shop_id)
+			return func(ref, *args, **kwargs, shop_id=shop_id)
 
-        return inner
+		return inner
 
 
 class PrintiPyProducts(_ApiHandlingMixin, _ShopIdMixin):
-    """
-    Used to access the [Printify Products](https://developers.printify.com/#products) APIs
+	"""
+	Used to access the [Printify Products](https://developers.printify.com/#products) APIs
 
-    Examples:
-        >>> from printipy.api import PrintiPy
-        >>> api = PrintiPy(api_token='...', shop_id='...')
-        >>> shop_products = api.products.get_products()
-    """
-    def __init__(self, api_token: str, shop_id: Optional[Union[str, int]]):
-        _ApiHandlingMixin.__init__(self, api_token=api_token)
-        _ShopIdMixin.__init__(self, shop_id=shop_id)
-
-    @_ShopIdMixin._require_shop_id
-    def get_products(self, shop_id: Union[str, int], max_pages: int = 1) -> List[Product]:
-        """
-        Pulls products for specific shop in Printify.
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> products = api.products.get_products(shop_id='...')
-
-            Or, with specifying the shop_id at PrintiPy-creation time
-
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> products = api.products.get_products()
-
-        Args:
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull products.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-            max_pages: Printify's API is paginated for requests. This will set the maximum number of pages to ingest.
-        Returns:
-            List of products `printipy.data_objects.Product` object
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the Shop ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # GET / v1 / shops / {shop_id} / products.json
-        initial_url = f'{self.api_url}/v1/shops/{shop_id}/products.json'
-        products_url = deepcopy(initial_url)
-        all_products = []
-        for _ in range(max_pages):
-            if products_url is None:
-                break
-            products_information = self._get(products_url)
-            all_products.extend(self._parse(Product, products_information['data']))
-            products_url = self._get_next_page_url(initial_url, products_information)
-        return all_products
-
-    @_ShopIdMixin._require_shop_id
-    def get_product(self, product_id: str, shop_id: Union[str, int]) -> Product:
-        """
-        Pull a specific product for specific shop in Printify.
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> product = api.products.get_product(product_id='...', shop_id='...')
-
-            Or, with specifying the shop_id at PrintiPy-creation time
-
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> product = api.products.get_product(product_id='...')
-
-        Args:
-            product_id: The ID of the specific product to pull
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull products.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-        Returns:
-            Product `printipy.data_objects.Product` object
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If either the Shop ID or Product ID do not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # GET / v1 / shops / {shop_id} / products / {product_id}.json
-        product_url = f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}.json'
-        product_information = self._get(product_url)
-        return self._parse(Product, product_information)
-
-    @_ShopIdMixin._require_shop_id
-    def create_product(self, create_product: CreateProduct, shop_id: Union[str, int]) -> Product:
-        """
-        Create a product for a given shop in Printify
-
-        Examples:
-            With specifying the shop_id at the function level and using CreateProduct.from_dict
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import CreateProduct
-            >>> api = PrintiPy(api_token='...')
-            >>> product_info = {
-            >>>     "title": '...',
-            >>>     "description": '...',
-            >>>     "blueprint_id": ...,
-            >>>     "print_provider_id": ...,
-            >>>     "variants": [...],
-            >>>     "print_areas": [...],
-            >>> }
-            >>> product = api.products.create_product(
-            >>>                create_product=CreateProduct.from_dict(product_info), shop_id='...')
-
-            Or, with specifying the shop_id at PrintiPy-creation time and using a CreateProduct object
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import CreateProduct
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> product_info = CreateProduct(
-            >>>     title='...',
-            >>>     description='...',
-            >>>     blueprint_id=...,
-            >>>     print_provider_id=...,
-            >>>     variants=[...],
-            >>>     print_areas=[...],
-            >>> )
-            >>> product = api.products.create_product(create_product=product_info)
-
-        Args:
-            create_product: Product metadata to pass to Printify
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-
-        Returns:
-            Product `printipy.data_objects.Product` object
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        shop_id_to_use = self._get_shop_id(shop_id)
-        # POST / v1 / shops / {shop_id} / products.json
-        create_product_url = f'{self.api_url}/v1/shops/{shop_id_to_use}/products.json'
-        product_information = self._post(create_product_url, data=create_product.to_dict())
-        return self._parse(Product, product_information)
-
-    @_ShopIdMixin._require_shop_id
-    def update_product(self, product_id: str, update_product: UpdateProduct, shop_id: Union[str, int]) -> Product:
-        """
-        Updates a specific product for a given shop in Printify
-
-        Examples:
-            With specifying the shop_id at the function level and using UpdateProduct.from_dict
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import UpdateProduct
-            >>> api = PrintiPy(api_token='...')
-            >>> product_info = {
-            >>>     "title": '...',
-            >>>     "description": '...',
-            >>>     "blueprint_id": ...,
-            >>>     "print_provider_id": ...,
-            >>>     "variants": [...],
-            >>>     "print_areas": [...],
-            >>> }
-            >>> product = api.products.update_product(product_id='...',
-            >>>             update_product=UpdateProduct.from_dict(product_info), shop_id='...')
-
-            Or, with specifying the shop_id at PrintiPy-creation time and using a UpdateProduct object
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import UpdateProduct
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> product_info = UpdateProduct(
-            >>>     title='...',
-            >>>     description='...',
-            >>>     blueprint_id=...,
-            >>>     print_provider_id=...,
-            >>>     variants=[...],
-            >>>     print_areas=[...],
-            >>> )
-            >>> product = api.products.update_product(product_id='...', update_product=product_info)
-
-        Args:
-            product_id: ID of the product to update
-            update_product: Product metadata to pass to Printify
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-
-        Returns:
-            Product `printipy.data_objects.Product` object
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # PUT / v1 / shops / {shop_id} / products / {product_id}.json
-        update_product_url = f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}.json'
-        product_information = self._put(update_product_url, data=update_product.to_dict())
-        return self._parse(Product, product_information)
-
-    @_ShopIdMixin._require_shop_id
-    def delete_product(self, product_id: str, shop_id: Union[str, int]) -> True:
-        """
-        Examples:
-            By passing in data pulled from `printipy.api.PrintiPyShop.get_products`
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> products = api.products.get_products()
-            >>> api.products.delete_product(product_id=products[0].id)
-
-            By passing in specific shop information
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import Shop
-            >>> api = PrintiPy(api_token='...')
-            >>> products = api.products.get_products()
-            >>> api.products.delete_product(product_id=products[0].id, shop_id='...')
-
-        Args:
-            product_id: ID of the product to publish
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # DELETE / v1 / shops / {shop_id} / products / {product_id}.json
-        delete_product_url = f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}.json'
-        self._delete(delete_product_url)
-        return True
-
-    @_ShopIdMixin._require_shop_id
-    def publish_product(self, product_id: str, publish: Publish, shop_id: Union[str, int]) -> True:
-        """
-        Publishes changes for a specific product for a given store in Printify
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import UpdateProduct
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> product = api.products.create_product(...)
-            >>> api.products.publish_product(product.id, Publish())
-
-        Args:
-            product_id: ID of the product to publish
-            publish: Publish settings for the product
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-
-        Returns:
-            True when a product has been marked for publishing
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # POST / v1 / shops / {shop_id} / products / {product_id} / publish.json
-        publish_product_url = f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}/publish.json'
-        self._post(publish_product_url, data=publish.to_dict())
-        return True
-
-    @_ShopIdMixin._require_shop_id
-    def set_product_published_success(self, product_id: str, publishing_succeeded: PublishingSucceeded,
-                                      shop_id: Union[str, int]) -> True:
-        """
-        Marks a product as published for a given store in Printify. Useful when managing a custom site,
-        not a linked store supportd by Printify.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import UpdateProduct
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> product = api.products.create_product(...)
-            >>> api.products.publish_product(product.id, Publish())
-            >>> api.products.set_product_published_success(product.id, PublishingSucceeded(...))
-
-        Args:
-            product_id: ID of the product
-            publishing_succeeded: Publishing details for the external store
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-
-        Returns:
-            True when a product has been marked as published
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # POST / v1 / shops / {shop_id} / products / {product_id} / publishing_succeeded.json
-        publishing_succeeded_url = f'{self.api_url}/v1/shops/{shop_id}/products/' \
-                                   f'{product_id}/publishing_succeeded.json'
-        self._post(publishing_succeeded_url, data=publishing_succeeded.to_dict())
-        return True
-
-    @_ShopIdMixin._require_shop_id
-    def set_product_published_failed(self, product_id: str, reason: str, shop_id: Union[str, int]) -> True:
-        """
-        Marks a product as not published for a given store in Printify. Useful when managing a custom site,
-        not a linked store supportd by Printify.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import UpdateProduct
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> product = api.products.create_product(...)
-            >>> api.products.publish_product(product.id, Publish())
-            >>> api.products.set_product_published_failed(product.id, reason='...')
-
-        Args:
-            product_id: ID of the product
-            reason: Explination of a publishing failure - useful for tacking
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-
-        Returns:
-            True when a product has been marked as not published
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # POST / v1 / shops / {shop_id} / products / {product_id} / publishing_failed.json
-        publishing_failed_url = f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}/publishing_failed.json'
-        self._post(publishing_failed_url, data={"reason": reason})
-        return True
-
-    @_ShopIdMixin._require_shop_id
-    def unpublish_product(self, product_id: str, shop_id: Union[str, int]) -> True:
-        """
-        Removes a published product from the storefront a given store in Printify
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import UpdateProduct
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> product_id = '...'
-            >>> api.products.unpublish_product(product_id)
-
-        Args:
-            product_id: ID of the product to unpublish
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-
-        Returns:
-            True when a product has been marked as unpublished
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # POST / v1 / shops / {shop_id} / products / {product_id} / unpublish.json
-        unpublish_product_url = f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}/unpublish.json'
-        self._post(unpublish_product_url)
-        return True
+	Examples:
+	    >>> from printipy.api import PrintiPy
+	    >>> api = PrintiPy(api_token='...', shop_id='...')
+	    >>> shop_products = api.products.get_products()
+	"""
+
+	def __init__(self, api_token: str, shop_id: Optional[Union[str, int]]):
+		_ApiHandlingMixin.__init__(self, api_token=api_token)
+		_ShopIdMixin.__init__(self, shop_id=shop_id)
+
+	@_ShopIdMixin._require_shop_id
+	def get_products(self, shop_id: Union[str, int], max_pages: int = 1) -> List[Product]:
+		"""
+		Pulls products for specific shop in Printify.
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> products = api.products.get_products(shop_id='...')
+
+		    Or, with specifying the shop_id at PrintiPy-creation time
+
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> products = api.products.get_products()
+
+		Args:
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull products.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+		    max_pages: Printify's API is paginated for requests. This will set the maximum number of pages to ingest.
+		Returns:
+		    List of products `printipy.data_objects.Product` object
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the Shop ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# GET / v1 / shops / {shop_id} / products.json
+		initial_url = f'{self.api_url}/v1/shops/{shop_id}/products.json'
+		products_url = deepcopy(initial_url)
+		all_products = []
+		for _ in range(max_pages):
+			if products_url is None:
+				break
+			products_information = self._get(products_url)
+			all_products.extend(self._parse(Product, products_information['data']))
+			products_url = self._get_next_page_url(initial_url, products_information)
+		return all_products
+
+	@_ShopIdMixin._require_shop_id
+	def get_product(self, product_id: str, shop_id: Union[str, int]) -> Product:
+		"""
+		Pull a specific product for specific shop in Printify.
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> product = api.products.get_product(product_id='...', shop_id='...')
+
+		    Or, with specifying the shop_id at PrintiPy-creation time
+
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> product = api.products.get_product(product_id='...')
+
+		Args:
+		    product_id: The ID of the specific product to pull
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull products.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+		Returns:
+		    Product `printipy.data_objects.Product` object
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If either the Shop ID or Product ID do not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# GET / v1 / shops / {shop_id} / products / {product_id}.json
+		product_url = f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}.json'
+		product_information = self._get(product_url)
+		return self._parse(Product, product_information)
+
+	@_ShopIdMixin._require_shop_id
+	def create_product(self, create_product: CreateProduct, shop_id: Union[str, int]) -> Product:
+		"""
+		Create a product for a given shop in Printify
+
+		Examples:
+		    With specifying the shop_id at the function level and using CreateProduct.from_dict
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import CreateProduct
+		    >>> api = PrintiPy(api_token='...')
+		    >>> product_info = {
+		    >>>     "title": '...',
+		    >>>     "description": '...',
+		    >>>     "blueprint_id": ...,
+		    >>>     "print_provider_id": ...,
+		    >>>     "variants": [...],
+		    >>>     "print_areas": [...],
+		    >>> }
+		    >>> product = api.products.create_product(
+		    >>>                create_product=CreateProduct.from_dict(product_info), shop_id='...')
+
+		    Or, with specifying the shop_id at PrintiPy-creation time and using a CreateProduct object
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import CreateProduct
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> product_info = CreateProduct(
+		    >>>     title='...',
+		    >>>     description='...',
+		    >>>     blueprint_id=...,
+		    >>>     print_provider_id=...,
+		    >>>     variants=[...],
+		    >>>     print_areas=[...],
+		    >>> )
+		    >>> product = api.products.create_product(create_product=product_info)
+
+		Args:
+		    create_product: Product metadata to pass to Printify
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+
+		Returns:
+		    Product `printipy.data_objects.Product` object
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		shop_id_to_use = self._get_shop_id(shop_id)
+		# POST / v1 / shops / {shop_id} / products.json
+		create_product_url = f'{self.api_url}/v1/shops/{shop_id_to_use}/products.json'
+		product_information = self._post(create_product_url, data=create_product.to_dict())
+		return self._parse(Product, product_information)
+
+	@_ShopIdMixin._require_shop_id
+	def update_product(
+		self, product_id: str, update_product: UpdateProduct, shop_id: Union[str, int]
+	) -> Product:
+		"""
+		Updates a specific product for a given shop in Printify
+
+		Examples:
+		    With specifying the shop_id at the function level and using UpdateProduct.from_dict
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import UpdateProduct
+		    >>> api = PrintiPy(api_token='...')
+		    >>> product_info = {
+		    >>>     "title": '...',
+		    >>>     "description": '...',
+		    >>>     "blueprint_id": ...,
+		    >>>     "print_provider_id": ...,
+		    >>>     "variants": [...],
+		    >>>     "print_areas": [...],
+		    >>> }
+		    >>> product = api.products.update_product(product_id='...',
+		    >>>             update_product=UpdateProduct.from_dict(product_info), shop_id='...')
+
+		    Or, with specifying the shop_id at PrintiPy-creation time and using a UpdateProduct object
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import UpdateProduct
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> product_info = UpdateProduct(
+		    >>>     title='...',
+		    >>>     description='...',
+		    >>>     blueprint_id=...,
+		    >>>     print_provider_id=...,
+		    >>>     variants=[...],
+		    >>>     print_areas=[...],
+		    >>> )
+		    >>> product = api.products.update_product(product_id='...', update_product=product_info)
+
+		Args:
+		    product_id: ID of the product to update
+		    update_product: Product metadata to pass to Printify
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+
+		Returns:
+		    Product `printipy.data_objects.Product` object
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# PUT / v1 / shops / {shop_id} / products / {product_id}.json
+		update_product_url = f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}.json'
+		product_information = self._put(update_product_url, data=update_product.to_dict())
+		return self._parse(Product, product_information)
+
+	@_ShopIdMixin._require_shop_id
+	def delete_product(self, product_id: str, shop_id: Union[str, int]) -> True:
+		"""
+		Examples:
+		    By passing in data pulled from `printipy.api.PrintiPyShop.get_products`
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> products = api.products.get_products()
+		    >>> api.products.delete_product(product_id=products[0].id)
+
+		    By passing in specific shop information
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import Shop
+		    >>> api = PrintiPy(api_token='...')
+		    >>> products = api.products.get_products()
+		    >>> api.products.delete_product(product_id=products[0].id, shop_id='...')
+
+		Args:
+		    product_id: ID of the product to publish
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# DELETE / v1 / shops / {shop_id} / products / {product_id}.json
+		delete_product_url = f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}.json'
+		self._delete(delete_product_url)
+		return True
+
+	@_ShopIdMixin._require_shop_id
+	def publish_product(self, product_id: str, publish: Publish, shop_id: Union[str, int]) -> True:
+		"""
+		Publishes changes for a specific product for a given store in Printify
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import UpdateProduct
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> product = api.products.create_product(...)
+		    >>> api.products.publish_product(product.id, Publish())
+
+		Args:
+		    product_id: ID of the product to publish
+		    publish: Publish settings for the product
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+
+		Returns:
+		    True when a product has been marked for publishing
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# POST / v1 / shops / {shop_id} / products / {product_id} / publish.json
+		publish_product_url = (
+			f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}/publish.json'
+		)
+		self._post(publish_product_url, data=publish.to_dict())
+		return True
+
+	@_ShopIdMixin._require_shop_id
+	def set_product_published_success(
+		self,
+		product_id: str,
+		publishing_succeeded: PublishingSucceeded,
+		shop_id: Union[str, int],
+	) -> True:
+		"""
+		Marks a product as published for a given store in Printify. Useful when managing a custom site,
+		not a linked store supportd by Printify.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import UpdateProduct
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> product = api.products.create_product(...)
+		    >>> api.products.publish_product(product.id, Publish())
+		    >>> api.products.set_product_published_success(product.id, PublishingSucceeded(...))
+
+		Args:
+		    product_id: ID of the product
+		    publishing_succeeded: Publishing details for the external store
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+
+		Returns:
+		    True when a product has been marked as published
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# POST / v1 / shops / {shop_id} / products / {product_id} / publishing_succeeded.json
+		publishing_succeeded_url = (
+			f'{self.api_url}/v1/shops/{shop_id}/products/' f'{product_id}/publishing_succeeded.json'
+		)
+		self._post(publishing_succeeded_url, data=publishing_succeeded.to_dict())
+		return True
+
+	@_ShopIdMixin._require_shop_id
+	def set_product_published_failed(
+		self, product_id: str, reason: str, shop_id: Union[str, int]
+	) -> True:
+		"""
+		Marks a product as not published for a given store in Printify. Useful when managing a custom site,
+		not a linked store supportd by Printify.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import UpdateProduct
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> product = api.products.create_product(...)
+		    >>> api.products.publish_product(product.id, Publish())
+		    >>> api.products.set_product_published_failed(product.id, reason='...')
+
+		Args:
+		    product_id: ID of the product
+		    reason: Explination of a publishing failure - useful for tacking
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+
+		Returns:
+		    True when a product has been marked as not published
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# POST / v1 / shops / {shop_id} / products / {product_id} / publishing_failed.json
+		publishing_failed_url = (
+			f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}/publishing_failed.json'
+		)
+		self._post(publishing_failed_url, data={'reason': reason})
+		return True
+
+	@_ShopIdMixin._require_shop_id
+	def unpublish_product(self, product_id: str, shop_id: Union[str, int]) -> True:
+		"""
+		Removes a published product from the storefront a given store in Printify
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import UpdateProduct
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> product_id = '...'
+		    >>> api.products.unpublish_product(product_id)
+
+		Args:
+		    product_id: ID of the product to unpublish
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+
+		Returns:
+		    True when a product has been marked as unpublished
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# POST / v1 / shops / {shop_id} / products / {product_id} / unpublish.json
+		unpublish_product_url = (
+			f'{self.api_url}/v1/shops/{shop_id}/products/{product_id}/unpublish.json'
+		)
+		self._post(unpublish_product_url)
+		return True
 
 
 class PrintiPyOrders(_ApiHandlingMixin, _ShopIdMixin):
-    """
-    Used to access the [Printify Orders](https://developers.printify.com/#orders) APIs
+	"""
+	Used to access the [Printify Orders](https://developers.printify.com/#orders) APIs
 
-    Examples:
-        >>> from printipy.api import PrintiPy
-        >>> api = PrintiPy(api_token='...', shop_id='...')
-        >>> shop_orders = api.orders.get_orders()
-    """
-    def __init__(self, api_token: str, shop_id: Optional[Union[str, int]]):
-        _ApiHandlingMixin.__init__(self, api_token=api_token)
-        _ShopIdMixin.__init__(self, shop_id=shop_id)
-
-    @_ShopIdMixin._require_shop_id
-    def get_orders(self, max_pages: int = 1, shop_id: Optional[Union[str, int]] = None) -> List[Order]:
-        """
-        Pulls orders for specific shop in Printify.
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> orders = api.orders.get_orders(shop_id='...')
-
-            Or, with specifying the shop_id at PrintiPy-creation time
-
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> orders = api.orders.get_orders()
-
-        Args:
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-            max_pages: Printify's API is paginated for requests. This will set the maximum number of pages to ingest.
-        Returns:
-            List of orders `printipy.data_objects.Order` object
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the Shop ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        shop_id_to_use = self._get_shop_id(shop_id)
-        # GET / v1 / shops / {shop_id} / orders.json
-        initial_url = f'{self.api_url}/v1/shops/{shop_id_to_use}/orders.json'
-        orders_url = deepcopy(initial_url)
-        all_orders = []
-        for _ in range(max_pages):
-            if orders_url is None:
-                break
-            orders_information = self._get(orders_url)
-            all_orders.extend(self._parse(Order, orders_information['data']))
-            orders_url = self._get_next_page_url(initial_url, orders_information)
-        return all_orders
-
-    @_ShopIdMixin._require_shop_id
-    def get_order(self, order_id: str, shop_id: Optional[Union[str, int]] = None) -> Order:
-        """
-        Pulls a specific order for specific shop in Printify.
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> order = api.orders.get_order(order_id='...', shop_id='...')
-
-            Or, with specifying the shop_id at PrintiPy-creation time
-
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> order = api.orders.get_order(order_id='...')
-
-        Args:
-            order_id: ID of the order to pull for a specific shop in Printify.
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-        Returns:
-            Orders `printipy.data_objects.Order` object
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If either the Shop ID or Order ID do not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        shop_id_to_use = self._get_shop_id(shop_id)
-        # GET / v1 / shops / {shop_id} / orders / {order_id}.json
-        order_url = f'{self.api_url}/v1/shops/{shop_id_to_use}/orders/{order_id}.json'
-        order_information = self._get(order_url)
-        return self._parse(Order, order_information)
-
-    def __create_order(self, create_order: Union[CreateOrderByPrintDetails, CreateOrderBySku,
-                       CreateOrderByExistingProduct, CreateOrderByAdvancedImageProcessing],
-                       shop_id: Union[str, int]) -> str:
-        # POST / v1 / shops / {shop_id} / orders.json
-        create_order_url = f'{self.api_url}/v1/shops/{shop_id}/orders.json'
-        order_information = self._post(create_order_url, data=create_order.to_dict())
-        return order_information['id']
-
-    @_ShopIdMixin._require_shop_id
-    def create_order_for_existing_product(self, create_order: CreateOrderByExistingProduct,
-                                          shop_id: Union[str, int]) -> str:
-        """
-        Create an order for an existing project for specific shop in Printify.
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> new_order_props = CreateOrderByExistingProduct.from_dict({
-            >>>   "external_id": "2750e210-39bb-11e9-a503-452618153e4a",
-            >>>   "label": "00012",
-            >>>   "line_items": [
-            >>>     {
-            >>>       "product_id": "5bfd0b66a342bcc9b5563216",
-            >>>       "variant_id": 17887,
-            >>>       "quantity": 1
-            >>>     }
-            >>>   ],
-            >>>   "shipping_method": 1,
-            >>>   "send_shipping_notification": False,
-            >>>   "address_to": {
-            >>>     "first_name": "John",
-            >>>     "last_name": "Smith",
-            >>>     "email": "example@msn.com",
-            >>>     "phone": "0574 69 21 90",
-            >>>     "country": "BE",
-            >>>     "region": "",
-            >>>     "address1": "ExampleBaan 121",
-            >>>     "address2": "45",
-            >>>     "city": "Retie",
-            >>>     "zip": "2470"
-            >>> })
-            >>> order_number = api.orders.create_order_for_existing_product(new_order_props)
-
-
-        Args:
-            create_order: Order information
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-        Returns:
-            Order reference number
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If either the Shop ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        return self.__create_order(create_order, shop_id=shop_id)
-
-    @_ShopIdMixin._require_shop_id
-    def create_order_with_simple_image_positioning(self, create_order: CreateOrderByExistingProduct,
-                                                   shop_id: Union[str, int]) -> str:
-        """
-        Create an order for a new product using simple image positioning.
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> new_order_props = CreateOrderByExistingProduct.from_dict({
-            >>>    "external_id": "2750e210-39bb-11e9-a503-452618153e5a",
-            >>>    "label": "00012",
-            >>>    "line_items": [
-            >>>      {
-            >>>        "print_provider_id": 5,
-            >>>        "blueprint_id": 9,
-            >>>        "variant_id": 17887,
-            >>>        "print_areas": {
-            >>>          "front": "https://images.example.com/image.png"
-            >>>        },
-            >>>        "quantity": 1
-            >>>      }
-            >>>    ],
-            >>>    "shipping_method": 1,
-            >>>    "send_shipping_notification": False,
-            >>>    "address_to": {
-            >>>      "first_name": "John",
-            >>>      "last_name": "Smith",
-            >>>      "email": "example@msn.com",
-            >>>      "phone": "0574 69 21 90",
-            >>>      "country": "BE",
-            >>>      "region": "",
-            >>>      "address1": "ExampleBaan 121",
-            >>>      "address2": "45",
-            >>>      "city": "Retie",
-            >>>      "zip": "2470"
-            >>>    }
-            >>> })
-            >>> order_number = api.orders.create_order_with_simple_image_positioning(new_order_props)
-
-
-        Args:
-            create_order: Order information
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-        Returns:
-            Order reference number
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If either the Shop ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        return self.__create_order(create_order, shop_id=shop_id)
-
-    @_ShopIdMixin._require_shop_id
-    def create_order_with_advanced_image_positioning(self, create_order: CreateOrderByAdvancedImageProcessing,
-                                                     shop_id: Union[str, int]) -> str:
-        """
-        Create an order for a new product using advanced image positioning.
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> new_order_props = CreateOrderByAdvancedImageProcessing.from_dict({
-            >>>    "external_id": "2750e210-39bb-11e9-a503-452618153e5a",
-            >>>    "label": "00012",
-            >>>    "line_items": [
-            >>>      {
-            >>>        "print_provider_id": 5,
-            >>>        "blueprint_id": 9,
-            >>>        "variant_id": 17887,
-            >>>        "print_areas": {
-            >>>          "front": [
-            >>>            {
-            >>>                "src": "https://images.example.com/image.png",
-            >>>                "scale": 0.15,
-            >>>                "x": 0.80,
-            >>>                "y": 0.34,
-            >>>                "angle": 0.34
-            >>>            },
-            >>>            {
-            >>>                "src": "https://images.example.com/image.png",
-            >>>                "scale": 1,
-            >>>                "x": 0.5,
-            >>>                "y": 0.5,
-            >>>                "angle": 1
-            >>>            }
-            >>>          ]
-            >>>        },
-            >>>        "quantity": 1
-            >>>      }
-            >>>    ],
-            >>>    "shipping_method": 1,
-            >>>    "send_shipping_notification": False,
-            >>>    "address_to": {
-            >>>      "first_name": "John",
-            >>>      "last_name": "Smith",
-            >>>      "email": "example@msn.com",
-            >>>      "phone": "0574 69 21 90",
-            >>>      "country": "BE",
-            >>>      "region": "",
-            >>>      "address1": "ExampleBaan 121",
-            >>>      "address2": "45",
-            >>>      "city": "Retie",
-            >>>      "zip": "2470"
-            >>>    }
-            >>> })
-            >>> order_number = api.orders.create_order_with_advanced_image_positioning(new_order_props)
-
-        Args:
-            create_order: Order information
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-        Returns:
-            Order reference number
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If either the Shop ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        return self.__create_order(create_order, shop_id=shop_id)
-
-    @_ShopIdMixin._require_shop_id
-    def create_order_with_print_details(self, create_order: CreateOrderByPrintDetails, shop_id: Union[str, int]) -> str:
-        """
-        Create an order for a new product using print deatils.
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> new_order_props = CreateOrderByPrintDetails.from_dict({
-            >>>        "external_id": "2750e210-39bb-11e9-a503-452618153e5a",
-            >>>        "label": "00012",
-            >>>        "line_items": [
-            >>>          {
-            >>>            "print_provider_id": 5,
-            >>>            "blueprint_id": 9,
-            >>>            "variant_id": 17887,
-            >>>            "print_areas": {
-            >>>              "front": "https://images.example.com/image.png"
-            >>>            },
-            >>>            "print_details": {
-            >>>                "print_on_side": "mirror"
-            >>>            },
-            >>>            "quantity": 1
-            >>>          }
-            >>>        ],
-            >>>        "shipping_method": 1,
-            >>>        "send_shipping_notification": False,
-            >>>        "address_to": {
-            >>>          "first_name": "John",
-            >>>          "last_name": "Smith",
-            >>>          "email": "example@msn.com",
-            >>>          "phone": "0574 69 21 90",
-            >>>          "country": "BE",
-            >>>          "region": "",
-            >>>          "address1": "ExampleBaan 121",
-            >>>          "address2": "45",
-            >>>          "city": "Retie",
-            >>>          "zip": "2470"
-            >>>    }
-            >>> })
-            >>> order_number = api.orders.create_order_with_print_details(new_order_props)
-
-        Args:
-            create_order: Order information
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-        Returns:
-            Order reference number
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If either the Shop ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        return self.__create_order(create_order, shop_id=shop_id)
-
-    @_ShopIdMixin._require_shop_id
-    def create_order_with_sku(self, create_order: CreateOrderBySku, shop_id: Union[str, int]) -> str:
-        """
-        Create an order for a product based on its SKU.
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> new_order_props = CreateOrderBySku.from_dict({
-            >>>    "external_id": "2750e210-39bb-11e9-a503-452618153e6a",
-            >>>    "label": "00012",
-            >>>    "line_items": [
-            >>>      {
-            >>>        "sku": "MY-SKU",
-            >>>        "quantity": 1
-            >>>      }
-            >>>    ],
-            >>>    "shipping_method": 1,
-            >>>    "send_shipping_notification": False,
-            >>>    "address_to": {
-            >>>      "first_name": "John",
-            >>>      "last_name": "Smith",
-            >>>      "email": "example@msn.com",
-            >>>      "phone": "0574 69 21 90",
-            >>>      "country": "BE",
-            >>>      "region": "",
-            >>>      "address1": "ExampleBaan 121",
-            >>>      "address2": "45",
-            >>>      "city": "Retie",
-            >>>      "zip": "2470"
-            >>>    }
-            >>> })
-            >>> order_number = api.orders.create_order_with_sku(new_order_props)
-
-        Args:
-            create_order: Order information
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-        Returns:
-            Order reference number
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If either the Shop ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        return self.__create_order(create_order, shop_id=shop_id)
-
-    @_ShopIdMixin._require_shop_id
-    def send_order_to_production(self, order_id: str, shop_id: Union[str, int]) -> Order:
-        """
-        Sends an open order to production in Printify.
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> order_number = api.orders.create_order_with_sku(...)
-            >>> order = api.orders.send_order_to_production(order_number)
-
-        Args:
-            order_id: Order ID
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-        Returns:
-            Order `printipy.data_objects.Order` information
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If either the Shop ID or Order Number does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # POST / v1 / shops / {shop_id} / orders / {order_id} / send_to_production.json
-        send_order_to_production_url = f'{self.api_url}/v1/shops/{shop_id}/orders/{order_id}/send_to_production.json'
-        order_information = self._post(send_order_to_production_url)
-        return self._parse(Order, order_information)
-
-    @_ShopIdMixin._require_shop_id
-    def calc_shipping_for_order(self, create_shipping_cost_estimate: CreateShippingEstimate,
-                                shop_id: Union[str, int]) -> ShippingCost:
-        """
-        Calculate shipping cost for an order for a given shop in Printify
-
-        Examples:
-            With specifying the shop_id at the function level and using CreateShippingEstimate.from_dict
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import CreateShippingEstimate
-            >>> api = PrintiPy(api_token='...')
-            >>> estimate_info = {
-            >>>     "line_items": [...],
-            >>>     "address_to": {...},
-            >>> }
-            >>> shipping_cost = api.orders.calc_shipping_for_order(
-            >>>                   create_shipping_cost_estimate=CreateShippingEstimate.from_dict(estimate_info),
-            >>>                   shop_id='...')
-
-            Or, with specifying the shop_id at PrintiPy-creation time and using a CreateShippingEstimate object
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import CreateShippingEstimate
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> estimate_info = CreateShippingEstimate(
-            >>>     line_items=[...],
-            >>>     address_to=...,
-            >>> )
-            >>> shipping_cost = api.orders.calc_shipping_for_order(create_shipping_cost_estimate=estimate_info)
-
-        Args:
-            create_shipping_cost_estimate: Order adn shipping information to pass to Printify
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-
-        Returns:
-            Shipping cost `printipy.data_objects.ShippingCost` object
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # POST / v1 / shops / {shop_id} / orders / shipping.json
-        shipping_estimate_url = f'{self.api_url}/v1/shops/{shop_id}/orders/shipping.json'
-        shipping_information = self._post(shipping_estimate_url, data=create_shipping_cost_estimate.to_dict())
-        return self._parse(ShippingCost, shipping_information)
-
-    @_ShopIdMixin._require_shop_id
-    def cancel_order(self, order_id: str, shop_id: Union[str, int]) -> Order:
-        """
-        Canceles a specific order for a given shop in Printify
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> order = api.orders.cancel_order(order_id='...', shop_id='...')
-
-            Or, with specifying the shop_id at PrintiPy-creation time
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> order = api.orders.cancel_order(order_id='...')
-
-        Args:
-            order_id: ID of the order to cancel
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-
-        Returns:
-            Order `printipy.data_objects.Order` object
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed
-             input or why the order cannot be canceled
-        """
-        # POST / v1 / shops / {shop_id} / orders / {order_id} / cancel.json
-        cancel_order_url = f'{self.api_url}/v1/shops/{shop_id}/orders/{order_id}/cancel.json'
-        order_information = self._post(cancel_order_url)
-        return self._parse(Order, order_information)
+	Examples:
+	    >>> from printipy.api import PrintiPy
+	    >>> api = PrintiPy(api_token='...', shop_id='...')
+	    >>> shop_orders = api.orders.get_orders()
+	"""
+
+	def __init__(self, api_token: str, shop_id: Optional[Union[str, int]]):
+		_ApiHandlingMixin.__init__(self, api_token=api_token)
+		_ShopIdMixin.__init__(self, shop_id=shop_id)
+
+	@_ShopIdMixin._require_shop_id
+	def get_orders(
+		self, max_pages: int = 1, shop_id: Optional[Union[str, int]] = None
+	) -> List[Order]:
+		"""
+		Pulls orders for specific shop in Printify.
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> orders = api.orders.get_orders(shop_id='...')
+
+		    Or, with specifying the shop_id at PrintiPy-creation time
+
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> orders = api.orders.get_orders()
+
+		Args:
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+		    max_pages: Printify's API is paginated for requests. This will set the maximum number of pages to ingest.
+		Returns:
+		    List of orders `printipy.data_objects.Order` object
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the Shop ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		shop_id_to_use = self._get_shop_id(shop_id)
+		# GET / v1 / shops / {shop_id} / orders.json
+		initial_url = f'{self.api_url}/v1/shops/{shop_id_to_use}/orders.json'
+		orders_url = deepcopy(initial_url)
+		all_orders = []
+		for _ in range(max_pages):
+			if orders_url is None:
+				break
+			orders_information = self._get(orders_url)
+			all_orders.extend(self._parse(Order, orders_information['data']))
+			orders_url = self._get_next_page_url(initial_url, orders_information)
+		return all_orders
+
+	@_ShopIdMixin._require_shop_id
+	def get_order(self, order_id: str, shop_id: Optional[Union[str, int]] = None) -> Order:
+		"""
+		Pulls a specific order for specific shop in Printify.
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> order = api.orders.get_order(order_id='...', shop_id='...')
+
+		    Or, with specifying the shop_id at PrintiPy-creation time
+
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> order = api.orders.get_order(order_id='...')
+
+		Args:
+		    order_id: ID of the order to pull for a specific shop in Printify.
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+		Returns:
+		    Orders `printipy.data_objects.Order` object
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If either the Shop ID or Order ID do not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		shop_id_to_use = self._get_shop_id(shop_id)
+		# GET / v1 / shops / {shop_id} / orders / {order_id}.json
+		order_url = f'{self.api_url}/v1/shops/{shop_id_to_use}/orders/{order_id}.json'
+		order_information = self._get(order_url)
+		return self._parse(Order, order_information)
+
+	def __create_order(
+		self,
+		create_order: Union[
+			CreateOrderByPrintDetails,
+			CreateOrderBySku,
+			CreateOrderByExistingProduct,
+			CreateOrderByAdvancedImageProcessing,
+		],
+		shop_id: Union[str, int],
+	) -> str:
+		# POST / v1 / shops / {shop_id} / orders.json
+		create_order_url = f'{self.api_url}/v1/shops/{shop_id}/orders.json'
+		order_information = self._post(create_order_url, data=create_order.to_dict())
+		return order_information['id']
+
+	@_ShopIdMixin._require_shop_id
+	def create_order_for_existing_product(
+		self, create_order: CreateOrderByExistingProduct, shop_id: Union[str, int]
+	) -> str:
+		"""
+		Create an order for an existing project for specific shop in Printify.
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> new_order_props = CreateOrderByExistingProduct.from_dict({
+		    >>>   "external_id": "2750e210-39bb-11e9-a503-452618153e4a",
+		    >>>   "label": "00012",
+		    >>>   "line_items": [
+		    >>>     {
+		    >>>       "product_id": "5bfd0b66a342bcc9b5563216",
+		    >>>       "variant_id": 17887,
+		    >>>       "quantity": 1
+		    >>>     }
+		    >>>   ],
+		    >>>   "shipping_method": 1,
+		    >>>   "send_shipping_notification": False,
+		    >>>   "address_to": {
+		    >>>     "first_name": "John",
+		    >>>     "last_name": "Smith",
+		    >>>     "email": "example@msn.com",
+		    >>>     "phone": "0574 69 21 90",
+		    >>>     "country": "BE",
+		    >>>     "region": "",
+		    >>>     "address1": "ExampleBaan 121",
+		    >>>     "address2": "45",
+		    >>>     "city": "Retie",
+		    >>>     "zip": "2470"
+		    >>> })
+		    >>> order_number = api.orders.create_order_for_existing_product(new_order_props)
+
+
+		Args:
+		    create_order: Order information
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+		Returns:
+		    Order reference number
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If either the Shop ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		return self.__create_order(create_order, shop_id=shop_id)
+
+	@_ShopIdMixin._require_shop_id
+	def create_order_with_simple_image_positioning(
+		self, create_order: CreateOrderByExistingProduct, shop_id: Union[str, int]
+	) -> str:
+		"""
+		Create an order for a new product using simple image positioning.
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> new_order_props = CreateOrderByExistingProduct.from_dict({
+		    >>>    "external_id": "2750e210-39bb-11e9-a503-452618153e5a",
+		    >>>    "label": "00012",
+		    >>>    "line_items": [
+		    >>>      {
+		    >>>        "print_provider_id": 5,
+		    >>>        "blueprint_id": 9,
+		    >>>        "variant_id": 17887,
+		    >>>        "print_areas": {
+		    >>>          "front": "https://images.example.com/image.png"
+		    >>>        },
+		    >>>        "quantity": 1
+		    >>>      }
+		    >>>    ],
+		    >>>    "shipping_method": 1,
+		    >>>    "send_shipping_notification": False,
+		    >>>    "address_to": {
+		    >>>      "first_name": "John",
+		    >>>      "last_name": "Smith",
+		    >>>      "email": "example@msn.com",
+		    >>>      "phone": "0574 69 21 90",
+		    >>>      "country": "BE",
+		    >>>      "region": "",
+		    >>>      "address1": "ExampleBaan 121",
+		    >>>      "address2": "45",
+		    >>>      "city": "Retie",
+		    >>>      "zip": "2470"
+		    >>>    }
+		    >>> })
+		    >>> order_number = api.orders.create_order_with_simple_image_positioning(new_order_props)
+
+
+		Args:
+		    create_order: Order information
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+		Returns:
+		    Order reference number
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If either the Shop ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		return self.__create_order(create_order, shop_id=shop_id)
+
+	@_ShopIdMixin._require_shop_id
+	def create_order_with_advanced_image_positioning(
+		self,
+		create_order: CreateOrderByAdvancedImageProcessing,
+		shop_id: Union[str, int],
+	) -> str:
+		"""
+		Create an order for a new product using advanced image positioning.
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> new_order_props = CreateOrderByAdvancedImageProcessing.from_dict({
+		    >>>    "external_id": "2750e210-39bb-11e9-a503-452618153e5a",
+		    >>>    "label": "00012",
+		    >>>    "line_items": [
+		    >>>      {
+		    >>>        "print_provider_id": 5,
+		    >>>        "blueprint_id": 9,
+		    >>>        "variant_id": 17887,
+		    >>>        "print_areas": {
+		    >>>          "front": [
+		    >>>            {
+		    >>>                "src": "https://images.example.com/image.png",
+		    >>>                "scale": 0.15,
+		    >>>                "x": 0.80,
+		    >>>                "y": 0.34,
+		    >>>                "angle": 0.34
+		    >>>            },
+		    >>>            {
+		    >>>                "src": "https://images.example.com/image.png",
+		    >>>                "scale": 1,
+		    >>>                "x": 0.5,
+		    >>>                "y": 0.5,
+		    >>>                "angle": 1
+		    >>>            }
+		    >>>          ]
+		    >>>        },
+		    >>>        "quantity": 1
+		    >>>      }
+		    >>>    ],
+		    >>>    "shipping_method": 1,
+		    >>>    "send_shipping_notification": False,
+		    >>>    "address_to": {
+		    >>>      "first_name": "John",
+		    >>>      "last_name": "Smith",
+		    >>>      "email": "example@msn.com",
+		    >>>      "phone": "0574 69 21 90",
+		    >>>      "country": "BE",
+		    >>>      "region": "",
+		    >>>      "address1": "ExampleBaan 121",
+		    >>>      "address2": "45",
+		    >>>      "city": "Retie",
+		    >>>      "zip": "2470"
+		    >>>    }
+		    >>> })
+		    >>> order_number = api.orders.create_order_with_advanced_image_positioning(new_order_props)
+
+		Args:
+		    create_order: Order information
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+		Returns:
+		    Order reference number
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If either the Shop ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		return self.__create_order(create_order, shop_id=shop_id)
+
+	@_ShopIdMixin._require_shop_id
+	def create_order_with_print_details(
+		self, create_order: CreateOrderByPrintDetails, shop_id: Union[str, int]
+	) -> str:
+		"""
+		Create an order for a new product using print deatils.
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> new_order_props = CreateOrderByPrintDetails.from_dict({
+		    >>>        "external_id": "2750e210-39bb-11e9-a503-452618153e5a",
+		    >>>        "label": "00012",
+		    >>>        "line_items": [
+		    >>>          {
+		    >>>            "print_provider_id": 5,
+		    >>>            "blueprint_id": 9,
+		    >>>            "variant_id": 17887,
+		    >>>            "print_areas": {
+		    >>>              "front": "https://images.example.com/image.png"
+		    >>>            },
+		    >>>            "print_details": {
+		    >>>                "print_on_side": "mirror"
+		    >>>            },
+		    >>>            "quantity": 1
+		    >>>          }
+		    >>>        ],
+		    >>>        "shipping_method": 1,
+		    >>>        "send_shipping_notification": False,
+		    >>>        "address_to": {
+		    >>>          "first_name": "John",
+		    >>>          "last_name": "Smith",
+		    >>>          "email": "example@msn.com",
+		    >>>          "phone": "0574 69 21 90",
+		    >>>          "country": "BE",
+		    >>>          "region": "",
+		    >>>          "address1": "ExampleBaan 121",
+		    >>>          "address2": "45",
+		    >>>          "city": "Retie",
+		    >>>          "zip": "2470"
+		    >>>    }
+		    >>> })
+		    >>> order_number = api.orders.create_order_with_print_details(new_order_props)
+
+		Args:
+		    create_order: Order information
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+		Returns:
+		    Order reference number
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If either the Shop ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		return self.__create_order(create_order, shop_id=shop_id)
+
+	@_ShopIdMixin._require_shop_id
+	def create_order_with_sku(
+		self, create_order: CreateOrderBySku, shop_id: Union[str, int]
+	) -> str:
+		"""
+		Create an order for a product based on its SKU.
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> new_order_props = CreateOrderBySku.from_dict({
+		    >>>    "external_id": "2750e210-39bb-11e9-a503-452618153e6a",
+		    >>>    "label": "00012",
+		    >>>    "line_items": [
+		    >>>      {
+		    >>>        "sku": "MY-SKU",
+		    >>>        "quantity": 1
+		    >>>      }
+		    >>>    ],
+		    >>>    "shipping_method": 1,
+		    >>>    "send_shipping_notification": False,
+		    >>>    "address_to": {
+		    >>>      "first_name": "John",
+		    >>>      "last_name": "Smith",
+		    >>>      "email": "example@msn.com",
+		    >>>      "phone": "0574 69 21 90",
+		    >>>      "country": "BE",
+		    >>>      "region": "",
+		    >>>      "address1": "ExampleBaan 121",
+		    >>>      "address2": "45",
+		    >>>      "city": "Retie",
+		    >>>      "zip": "2470"
+		    >>>    }
+		    >>> })
+		    >>> order_number = api.orders.create_order_with_sku(new_order_props)
+
+		Args:
+		    create_order: Order information
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+		Returns:
+		    Order reference number
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If either the Shop ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		return self.__create_order(create_order, shop_id=shop_id)
+
+	@_ShopIdMixin._require_shop_id
+	def send_order_to_production(self, order_id: str, shop_id: Union[str, int]) -> Order:
+		"""
+		Sends an open order to production in Printify.
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> order_number = api.orders.create_order_with_sku(...)
+		    >>> order = api.orders.send_order_to_production(order_number)
+
+		Args:
+		    order_id: Order ID
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to create orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+		Returns:
+		    Order `printipy.data_objects.Order` information
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If either the Shop ID or Order Number does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# POST / v1 / shops / {shop_id} / orders / {order_id} / send_to_production.json
+		send_order_to_production_url = (
+			f'{self.api_url}/v1/shops/{shop_id}/orders/{order_id}/send_to_production.json'
+		)
+		order_information = self._post(send_order_to_production_url)
+		return self._parse(Order, order_information)
+
+	@_ShopIdMixin._require_shop_id
+	def calc_shipping_for_order(
+		self,
+		create_shipping_cost_estimate: CreateShippingEstimate,
+		shop_id: Union[str, int],
+	) -> ShippingCost:
+		"""
+		Calculate shipping cost for an order for a given shop in Printify
+
+		Examples:
+		    With specifying the shop_id at the function level and using CreateShippingEstimate.from_dict
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import CreateShippingEstimate
+		    >>> api = PrintiPy(api_token='...')
+		    >>> estimate_info = {
+		    >>>     "line_items": [...],
+		    >>>     "address_to": {...},
+		    >>> }
+		    >>> shipping_cost = api.orders.calc_shipping_for_order(
+		    >>>                   create_shipping_cost_estimate=CreateShippingEstimate.from_dict(estimate_info),
+		    >>>                   shop_id='...')
+
+		    Or, with specifying the shop_id at PrintiPy-creation time and using a CreateShippingEstimate object
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import CreateShippingEstimate
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> estimate_info = CreateShippingEstimate(
+		    >>>     line_items=[...],
+		    >>>     address_to=...,
+		    >>> )
+		    >>> shipping_cost = api.orders.calc_shipping_for_order(create_shipping_cost_estimate=estimate_info)
+
+		Args:
+		    create_shipping_cost_estimate: Order adn shipping information to pass to Printify
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+
+		Returns:
+		    Shipping cost `printipy.data_objects.ShippingCost` object
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# POST / v1 / shops / {shop_id} / orders / shipping.json
+		shipping_estimate_url = f'{self.api_url}/v1/shops/{shop_id}/orders/shipping.json'
+		shipping_information = self._post(
+			shipping_estimate_url, data=create_shipping_cost_estimate.to_dict()
+		)
+		return self._parse(ShippingCost, shipping_information)
+
+	@_ShopIdMixin._require_shop_id
+	def cancel_order(self, order_id: str, shop_id: Union[str, int]) -> Order:
+		"""
+		Canceles a specific order for a given shop in Printify
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> order = api.orders.cancel_order(order_id='...', shop_id='...')
+
+		    Or, with specifying the shop_id at PrintiPy-creation time
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> order = api.orders.cancel_order(order_id='...')
+
+		Args:
+		    order_id: ID of the order to cancel
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+
+		Returns:
+		    Order `printipy.data_objects.Order` object
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed
+		     input or why the order cannot be canceled
+		"""
+		# POST / v1 / shops / {shop_id} / orders / {order_id} / cancel.json
+		cancel_order_url = f'{self.api_url}/v1/shops/{shop_id}/orders/{order_id}/cancel.json'
+		order_information = self._post(cancel_order_url)
+		return self._parse(Order, order_information)
 
 
 class PrintiPyArtwork(_ApiHandlingMixin):
-    """
-    Used to access the [Printify Uploads](https://developers.printify.com/#uploads) APIs
+	"""
+	Used to access the [Printify Uploads](https://developers.printify.com/#uploads) APIs
 
-    Examples:
-        >>> from printipy.api import PrintiPy
-        >>> api = PrintiPy(api_token='...')
-        >>> artwork = api.artwork.upload_artwork(filename='...')
-    """
-    def get_artwork_uploads(self, max_pages: int = 1) -> List[Artwork]:
-        """
-        Pulls artwork/image information for an account in Printify.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> artworks = api.artwork.get_artwork_uploads()
-
-        Args:
-            max_pages: Printify's API is paginated for requests. This will set the maximum number of pages to ingest.
-        Returns:
-            List of artwork `printipy.data_objects.Artwork` object
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the Artwork ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # GET / v1 / uploads.json
-        initial_url = f'{self.api_url}/v1/uploads.json'
-        artwork_url = deepcopy(initial_url)
-        all_artworks = []
-        for _ in range(max_pages):
-            if artwork_url is None:
-                break
-            artwork_information = self._get(artwork_url)
-            all_artworks.extend(self._parse(Artwork, artwork_information['data']))
-            artwork_url = self._get_next_page_url(initial_url, artwork_information)
-        return all_artworks
-
-    def get_artwork(self, image_id: str) -> Artwork:
-        """
-        Pulls information for a speciic artwork/image for an account in Printify.
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> artwork = api.artwork.get_artwork(image_id='...')
-
-        Args:
-            image_id: The ID of the specific artwork for an account in Printify.
-        Returns:
-            Artwork `printipy.data_objects.Artwork` object
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-        """
-        # GET / v1 / uploads / {image_id}.json
-        artwork_url = f'{self.api_url}/v1/uploads/{image_id}.json'
-        artwork_information = self._get(artwork_url)
-        return self._parse(Artwork, artwork_information)
-
-    def upload_artwork(self, filename: Optional[str] = None, url: Optional[str] = None) -> Artwork:
-        """
-        Uploads a new image/artwork to an account in Printify
-
-        Examples:
-            Using a local file
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import Shop
-            >>> api = PrintiPy(api_token='...')
-            >>> filename = '...'
-            >>> artwork = api.artwork.upload_artwork(filename=filename)
-
-            Using a URL
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import Shop
-            >>> api = PrintiPy(api_token='...')
-            >>> url = '...'
-            >>> artwork = api.artwork.upload_artwork(url=url)
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the artwork isn't transmissible to Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-            PrintiPyException: If neither or both filename and url are presented. Only one must be given.
-        """
-        if filename and url:
-            raise PrintiPyException("Must provide a local filename or url for upload, not both.")
-
-        # POST / v1 / uploads / images.json
-        upload_artwork_url = f'{self.api_url}/v1/uploads/images.json'
-        if url:
-            artwork_data = {
-                "file_name": url.split('/')[-1],
-                "url": url,
-            }
-        elif filename:
-            with open(filename, 'rb') as f:
-                b64data = base64.b64encode(f.read())
-            artwork_data = {
-                "file_name": os.path.basename(filename),
-                "contents": b64data.decode('utf-8'),
-            }
-        else:
-            raise PrintiPyException("Must provide at least a local filename or url for upload.")
-
-        artwork_information = self._post(upload_artwork_url, data=artwork_data)
-        return self._parse(Artwork, artwork_information)
-
-    def archive_artwork(self, image_id: str) -> True:
-        """
-        Archives a specific artwork/image for an account in Printify
-
-        Examples:
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import Shop
-            >>> api = PrintiPy(api_token='...')
-            >>> artworks = api.artwork.get_artwork_uploads()
-            >>> api.artwork.archive_artwork(artworks[0].id)
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the Artwork ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # post / v1 / uploads / {image_id} / archive.json
-        archive_artwork_url = f'{self.api_url}/v1/uploads/{image_id}/archive.json'
-        self._post(archive_artwork_url)
-        return True
+	Examples:
+	    >>> from printipy.api import PrintiPy
+	    >>> api = PrintiPy(api_token='...')
+	    >>> artwork = api.artwork.upload_artwork(filename='...')
+	"""
+
+	def get_artwork_uploads(self, max_pages: int = 1) -> List[Artwork]:
+		"""
+		Pulls artwork/image information for an account in Printify.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> artworks = api.artwork.get_artwork_uploads()
+
+		Args:
+		    max_pages: Printify's API is paginated for requests. This will set the maximum number of pages to ingest.
+		Returns:
+		    List of artwork `printipy.data_objects.Artwork` object
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the Artwork ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# GET / v1 / uploads.json
+		initial_url = f'{self.api_url}/v1/uploads.json'
+		artwork_url = deepcopy(initial_url)
+		all_artworks = []
+		for _ in range(max_pages):
+			if artwork_url is None:
+				break
+			artwork_information = self._get(artwork_url)
+			all_artworks.extend(self._parse(Artwork, artwork_information['data']))
+			artwork_url = self._get_next_page_url(initial_url, artwork_information)
+		return all_artworks
+
+	def get_artwork(self, image_id: str) -> Artwork:
+		"""
+		Pulls information for a speciic artwork/image for an account in Printify.
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> artwork = api.artwork.get_artwork(image_id='...')
+
+		Args:
+		    image_id: The ID of the specific artwork for an account in Printify.
+		Returns:
+		    Artwork `printipy.data_objects.Artwork` object
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		"""
+		# GET / v1 / uploads / {image_id}.json
+		artwork_url = f'{self.api_url}/v1/uploads/{image_id}.json'
+		artwork_information = self._get(artwork_url)
+		return self._parse(Artwork, artwork_information)
+
+	def upload_artwork(self, filename: Optional[str] = None, url: Optional[str] = None) -> Artwork:
+		"""
+		Uploads a new image/artwork to an account in Printify
+
+		Examples:
+		    Using a local file
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import Shop
+		    >>> api = PrintiPy(api_token='...')
+		    >>> filename = '...'
+		    >>> artwork = api.artwork.upload_artwork(filename=filename)
+
+		    Using a URL
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import Shop
+		    >>> api = PrintiPy(api_token='...')
+		    >>> url = '...'
+		    >>> artwork = api.artwork.upload_artwork(url=url)
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the artwork isn't transmissible to Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		    PrintiPyException: If neither or both filename and url are presented. Only one must be given.
+		"""
+		if filename and url:
+			raise PrintiPyException('Must provide a local filename or url for upload, not both.')
+
+		# POST / v1 / uploads / images.json
+		upload_artwork_url = f'{self.api_url}/v1/uploads/images.json'
+		if url:
+			artwork_data = {
+				'file_name': url.split('/')[-1],
+				'url': url,
+			}
+		elif filename:
+			with open(filename, 'rb') as f:
+				b64data = base64.b64encode(f.read())
+			artwork_data = {
+				'file_name': os.path.basename(filename),
+				'contents': b64data.decode('utf-8'),
+			}
+		else:
+			raise PrintiPyException('Must provide at least a local filename or url for upload.')
+
+		artwork_information = self._post(upload_artwork_url, data=artwork_data)
+		return self._parse(Artwork, artwork_information)
+
+	def archive_artwork(self, image_id: str) -> True:
+		"""
+		Archives a specific artwork/image for an account in Printify
+
+		Examples:
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import Shop
+		    >>> api = PrintiPy(api_token='...')
+		    >>> artworks = api.artwork.get_artwork_uploads()
+		    >>> api.artwork.archive_artwork(artworks[0].id)
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the Artwork ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# post / v1 / uploads / {image_id} / archive.json
+		archive_artwork_url = f'{self.api_url}/v1/uploads/{image_id}/archive.json'
+		self._post(archive_artwork_url)
+		return True
 
 
 class PrintiPyWebhooks(_ApiHandlingMixin, _ShopIdMixin):
-    """
-    Used to access the [Printify Webhooks](https://developers.printify.com/#webhooks) APIs
+	"""
+	Used to access the [Printify Webhooks](https://developers.printify.com/#webhooks) APIs
 
-    Examples:
-        >>> from printipy.api import PrintiPy
-        >>> api = PrintiPy(api_token='...', shop_id='...')
-        >>> webhooks = api.webhooks.get_webhooks()
-    """
-    def __init__(self, api_token: str, shop_id: Optional[Union[str, int]]):
-        _ApiHandlingMixin.__init__(self, api_token=api_token)
-        _ShopIdMixin.__init__(self, shop_id=shop_id)
-
-    @_ShopIdMixin._require_shop_id
-    def get_webhooks(self, shop_id: Union[str, int]) -> List[Webhook]:
-        """
-        Pulls webhooks for specific shop in Printify.
-
-        Examples:
-            With specifying the shop_id at the function level
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...')
-            >>> webhooks = api.webhooks.get_webhooks(shop_id='...')
-
-            Or, with specifying the shop_id at PrintiPy-creation time
-
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> webhooks = api.webhooks.get_webhooks()
-
-        Args:
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-        Returns:
-            List of webhooks `printipy.data_objects.Webhook` object
-
-        Raises:
-            ParseException: If unable to parse Printify's response
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the Shop ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # / v1 / shops / {shop_id} / webhooks.json
-        webhooks_url = f'{self.api_url}/v1/shops/{shop_id}/webhooks.json'
-        webhooks_information = self._get(webhooks_url)
-        return self._parse(Webhook, webhooks_information)
-
-    @_ShopIdMixin._require_shop_id
-    def create_webhook(self, create_webhook: CreateWebhook, shop_id: Union[str, int]) -> Webhook:
-        """
-        Create a webhook for a given shop in Printify
-
-        Examples:
-            With specifying the shop_id at the function level and using CreateWebhook.from_dict
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import CreateWebhook
-            >>> api = PrintiPy(api_token='...')
-            >>> webhook_info = {
-            >>>    "topic": "order:created",
-            >>>    "url": "https://example.com/webhooks/order/created"
-            >>> }
-            >>> webhook = api.webhooks.create_webhook(
-            >>>               create_webhook=CreateWebhook.from_dict(webhook_info), shop_id='...')
-
-            Or, with specifying the shop_id at PrintiPy-creation time and using a CreateWebhook object
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import CreateWebhook
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> webhook_info = CreateWebhook(
-            >>>     topic="order:created",
-            >>>     url="https://example.com/webhooks/order/created"
-            >>> )
-            >>> webhook = api.webhooks.create_webhook(create_webhook=webhook_info)
-
-        Args:
-            create_webhook: Webhook metadata to pass to Printify
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-
-        Returns:
-            Webhooks `printipy.data_objects.Webhook` object
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # POST /v1/shops/{shop_id}/webhooks.json
-        create_webhook_url = f'{self.api_url}/v1/shops/{shop_id}/webhooks.json'
-        webhook_information = self._post(create_webhook_url, data=create_webhook.to_dict())
-        return self._parse(Webhook, webhook_information)
-
-    @_ShopIdMixin._require_shop_id
-    def update_webhook(self, webhook_id: str, update_webhook: UpdateWebhook, shop_id: Union[str, int]) -> Webhook:
-        """
-        Updates a specific webhook for a given shop in Printify
-
-        Examples:
-            With specifying the shop_id at the function level and using UpdateWebhook.from_dict
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import UpdateWebhook
-            >>> api = PrintiPy(api_token='...')
-            >>> webhook_info = {
-            >>>     "topic": "order:created",
-            >>>     "url": "https://example.com/webhooks/order/created"
-            >>> }
-            >>> webhook = api.webhooks.update_webhook(
-            >>>     webhook_id='...',
-            >>>     update_webhook=UpdateWebhook.from_dict(webhook_info), shop_id='...'
-            >>> )
-
-            Or, with specifying the shop_id at PrintiPy-creation time and using a CreateWebhook object
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import UpdateWebhook
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> webhook_info = UpdateWebhook(
-            >>>     topic="order:created",
-            >>>     url="https://example.com/webhooks/order/created"
-            >>> )
-            >>> webhook = api.webhooks.update_webhook(update_webhook=webhook_info)
-
-        Args:
-            webhook_id: ID of the webhook to update in Printify
-            update_webhook: Webhook metadata to pass to Printify
-            shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
-            This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
-
-        Returns:
-            Webhooks `printipy.data_objects.Webhook` object
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # PUT /v1/shops/{shop_id}/webhooks/{webhook_id}.json
-        create_webhook_url = f'{self.api_url}/v1/shops/{shop_id}/webhooks/{webhook_id}.json'
-        webhook_information = self._put(create_webhook_url, data=update_webhook.to_dict())
-        return self._parse(Webhook, webhook_information)
-
-    @_ShopIdMixin._require_shop_id
-    def delete_webhook(self, webhook_id: str, shop_id: Union[str, int]) -> True:
-        """
-        Deletes a specific webhook for a specific shop in Printify
-
-        Examples:
-            By passing in data pulled from `printipy.api.PrintiPyWebhook.get_shops`
-            >>> from printipy.api import PrintiPy
-            >>> api = PrintiPy(api_token='...', shop_id='...')
-            >>> webhooks = api.webhooks.get_webhooks()
-            >>> api.webhooks.delete_webhook(webhook_id=webhooks[0].id)
-
-            By passing in specific shop information
-            >>> from printipy.api import PrintiPy
-            >>> from printipy.data_objects import Shop
-            >>> api = PrintiPy(api_token='...')
-            >>> webhooks = api.webhooks.get_webhooks()
-            >>> api.webhooks.delete_webhook(webhook_id=webhooks[0].id, shop_id='...')
-
-        Raises:
-            InvalidScopeException: If the API keys isn't permitted to perform this operation
-            InvalidRequestException: If the Webhook ID does not exist in Printify
-            PrintifyException: If Printify returned an error - usually contains information regarding malformed input
-        """
-        # DELETE /v1/shops/{shop_id}/webhooks/{webhook_id}.json
-        delete_webhook_url = f'{self.api_url}/v1/shops/{shop_id}/webhooks/{webhook_id}.json'
-        self._delete(delete_webhook_url)
-        return True
+	Examples:
+	    >>> from printipy.api import PrintiPy
+	    >>> api = PrintiPy(api_token='...', shop_id='...')
+	    >>> webhooks = api.webhooks.get_webhooks()
+	"""
+
+	def __init__(self, api_token: str, shop_id: Optional[Union[str, int]]):
+		_ApiHandlingMixin.__init__(self, api_token=api_token)
+		_ShopIdMixin.__init__(self, shop_id=shop_id)
+
+	@_ShopIdMixin._require_shop_id
+	def get_webhooks(self, shop_id: Union[str, int]) -> List[Webhook]:
+		"""
+		Pulls webhooks for specific shop in Printify.
+
+		Examples:
+		    With specifying the shop_id at the function level
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...')
+		    >>> webhooks = api.webhooks.get_webhooks(shop_id='...')
+
+		    Or, with specifying the shop_id at PrintiPy-creation time
+
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> webhooks = api.webhooks.get_webhooks()
+
+		Args:
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+		Returns:
+		    List of webhooks `printipy.data_objects.Webhook` object
+
+		Raises:
+		    ParseException: If unable to parse Printify's response
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the Shop ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# / v1 / shops / {shop_id} / webhooks.json
+		webhooks_url = f'{self.api_url}/v1/shops/{shop_id}/webhooks.json'
+		webhooks_information = self._get(webhooks_url)
+		return self._parse(Webhook, webhooks_information)
+
+	@_ShopIdMixin._require_shop_id
+	def create_webhook(self, create_webhook: CreateWebhook, shop_id: Union[str, int]) -> Webhook:
+		"""
+		Create a webhook for a given shop in Printify
+
+		Examples:
+		    With specifying the shop_id at the function level and using CreateWebhook.from_dict
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import CreateWebhook
+		    >>> api = PrintiPy(api_token='...')
+		    >>> webhook_info = {
+		    >>>    "topic": "order:created",
+		    >>>    "url": "https://example.com/webhooks/order/created"
+		    >>> }
+		    >>> webhook = api.webhooks.create_webhook(
+		    >>>               create_webhook=CreateWebhook.from_dict(webhook_info), shop_id='...')
+
+		    Or, with specifying the shop_id at PrintiPy-creation time and using a CreateWebhook object
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import CreateWebhook
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> webhook_info = CreateWebhook(
+		    >>>     topic="order:created",
+		    >>>     url="https://example.com/webhooks/order/created"
+		    >>> )
+		    >>> webhook = api.webhooks.create_webhook(create_webhook=webhook_info)
+
+		Args:
+		    create_webhook: Webhook metadata to pass to Printify
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+
+		Returns:
+		    Webhooks `printipy.data_objects.Webhook` object
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# POST /v1/shops/{shop_id}/webhooks.json
+		create_webhook_url = f'{self.api_url}/v1/shops/{shop_id}/webhooks.json'
+		webhook_information = self._post(create_webhook_url, data=create_webhook.to_dict())
+		return self._parse(Webhook, webhook_information)
+
+	@_ShopIdMixin._require_shop_id
+	def update_webhook(
+		self, webhook_id: str, update_webhook: UpdateWebhook, shop_id: Union[str, int]
+	) -> Webhook:
+		"""
+		Updates a specific webhook for a given shop in Printify
+
+		Examples:
+		    With specifying the shop_id at the function level and using UpdateWebhook.from_dict
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import UpdateWebhook
+		    >>> api = PrintiPy(api_token='...')
+		    >>> webhook_info = {
+		    >>>     "topic": "order:created",
+		    >>>     "url": "https://example.com/webhooks/order/created"
+		    >>> }
+		    >>> webhook = api.webhooks.update_webhook(
+		    >>>     webhook_id='...',
+		    >>>     update_webhook=UpdateWebhook.from_dict(webhook_info), shop_id='...'
+		    >>> )
+
+		    Or, with specifying the shop_id at PrintiPy-creation time and using a CreateWebhook object
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import UpdateWebhook
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> webhook_info = UpdateWebhook(
+		    >>>     topic="order:created",
+		    >>>     url="https://example.com/webhooks/order/created"
+		    >>> )
+		    >>> webhook = api.webhooks.update_webhook(update_webhook=webhook_info)
+
+		Args:
+		    webhook_id: ID of the webhook to update in Printify
+		    update_webhook: Webhook metadata to pass to Printify
+		    shop_id (Optional[Union[str, int]]): Specific shop ID in Printify from which to pull orders.
+		    This may be set at every call to speicy different shops, or this may be set when initiating PrintiPy.
+
+		Returns:
+		    Webhooks `printipy.data_objects.Webhook` object
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# PUT /v1/shops/{shop_id}/webhooks/{webhook_id}.json
+		create_webhook_url = f'{self.api_url}/v1/shops/{shop_id}/webhooks/{webhook_id}.json'
+		webhook_information = self._put(create_webhook_url, data=update_webhook.to_dict())
+		return self._parse(Webhook, webhook_information)
+
+	@_ShopIdMixin._require_shop_id
+	def delete_webhook(self, webhook_id: str, shop_id: Union[str, int]) -> True:
+		"""
+		Deletes a specific webhook for a specific shop in Printify
+
+		Examples:
+		    By passing in data pulled from `printipy.api.PrintiPyWebhook.get_shops`
+		    >>> from printipy.api import PrintiPy
+		    >>> api = PrintiPy(api_token='...', shop_id='...')
+		    >>> webhooks = api.webhooks.get_webhooks()
+		    >>> api.webhooks.delete_webhook(webhook_id=webhooks[0].id)
+
+		    By passing in specific shop information
+		    >>> from printipy.api import PrintiPy
+		    >>> from printipy.data_objects import Shop
+		    >>> api = PrintiPy(api_token='...')
+		    >>> webhooks = api.webhooks.get_webhooks()
+		    >>> api.webhooks.delete_webhook(webhook_id=webhooks[0].id, shop_id='...')
+
+		Raises:
+		    InvalidScopeException: If the API keys isn't permitted to perform this operation
+		    InvalidRequestException: If the Webhook ID does not exist in Printify
+		    PrintifyException: If Printify returned an error - usually contains information regarding malformed input
+		"""
+		# DELETE /v1/shops/{shop_id}/webhooks/{webhook_id}.json
+		delete_webhook_url = f'{self.api_url}/v1/shops/{shop_id}/webhooks/{webhook_id}.json'
+		self._delete(delete_webhook_url)
+		return True
 
 
 class PrintiPy:
-    """
-    Used to access all [Printify APIs](https://developers.printify.com/)
+	"""
+	Used to access all [Printify APIs](https://developers.printify.com/)
 
-    Examples:
-        To use the same Shop ID for each call
-        >>> from printipy.api import PrintiPy
-        >>> api = PrintiPy(api_token='...', shop_id='...')
-        >>> artwork = api.artwork.upload_artwork(filename='...')
-
-        To use a differnt Shop ID for each call
-        >>> from printipy.api import PrintiPy
-        >>> api = PrintiPy(api_token='...')
-        >>> shop123_products = api.products.get_products(shop_id='shop123')
-        >>> shop456_products = api.products.get_products(shop_id='shop456')
-    """
-
-    def __init__(self, api_token: str, shop_id: Optional[Union[str, int]] = None):
-        """
-        Entrypoint needed to access all [Printify APIs](https://developers.printify.com/)
-
-        Args:
-            api_token (str): Every instance of PrintiPy requires an API Token. Follow
-            [these steps](https://help.printify.com/hc/en-us/articles/4483626447249-How-can-I-generate-an-API-token-)
-            to generate a token
-            shop_id (Optional[str]): The ID of a specific Printify shop. If none is given, some APIs will still
-            work (as they do not require a Shop) while others will require a Shop ID to be passed upon a function call
-        """
-        self.shops = PrintiPyShop(api_token=api_token)
-        self.catalog = PrintiPyCatalog(api_token=api_token)
-        self.products = PrintiPyProducts(api_token=api_token, shop_id=shop_id)
-        self.orders = PrintiPyOrders(api_token=api_token, shop_id=shop_id)
-        self.artwork = PrintiPyArtwork(api_token=api_token)
-        self.webhooks = PrintiPyWebhooks(api_token=api_token, shop_id=shop_id)
+	Examples:
+	    To use the same Shop ID for each call
+	    >>> from printipy.api import PrintiPy
+	    >>> api = PrintiPy(api_token='...', shop_id='...')
+	    >>> artwork = api.artwork.upload_artwork(filename='...')
+
+	    To use a differnt Shop ID for each call
+	    >>> from printipy.api import PrintiPy
+	    >>> api = PrintiPy(api_token='...')
+	    >>> shop123_products = api.products.get_products(shop_id='shop123')
+	    >>> shop456_products = api.products.get_products(shop_id='shop456')
+	"""
+
+	def __init__(self, api_token: str, shop_id: Optional[Union[str, int]] = None):
+		"""
+		Entrypoint needed to access all [Printify APIs](https://developers.printify.com/)
+
+		Args:
+		    api_token (str): Every instance of PrintiPy requires an API Token. Follow
+		    [these steps](https://help.printify.com/hc/en-us/articles/4483626447249-How-can-I-generate-an-API-token-)
+		    to generate a token
+		    shop_id (Optional[str]): The ID of a specific Printify shop. If none is given, some APIs will still
+		    work (as they do not require a Shop) while others will require a Shop ID to be passed upon a function call
+		"""
+		self.shops = PrintiPyShop(api_token=api_token)
+		self.catalog = PrintiPyCatalog(api_token=api_token)
+		self.products = PrintiPyProducts(api_token=api_token, shop_id=shop_id)
+		self.orders = PrintiPyOrders(api_token=api_token, shop_id=shop_id)
+		self.artwork = PrintiPyArtwork(api_token=api_token)
+		self.webhooks = PrintiPyWebhooks(api_token=api_token, shop_id=shop_id)
```

### Comparing `printipy-1.2.0/printipy/data_objects.py` & `printipy-1.2.1/printipy/data_objects.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1215 +1,1249 @@
 from dataclasses import dataclass, field
 from typing import List, Optional, Union, Dict, Any
 
 from dataclasses_json import dataclass_json, config
 
 
 def _exclude_if_none(value):
-    return value is None
+	return value is None
 
 
 @dataclass_json
 @dataclass
 class Shop:
-    """
-    Shop object to store and validate shop data between Python and Printify
+	"""
+	Shop object to store and validate shop data between Python and Printify
 
-    Args:
-        id: Shop ID
-        title: Shop Name
-        sales_channel: Sales Channel, e.g., Etsy, Walmart, etc.
-    """
-    id: str
-    title: str
-    sales_channel: str
+	Args:
+	    id: Shop ID
+	    title: Shop Name
+	    sales_channel: Sales Channel, e.g., Etsy, Walmart, etc.
+	"""
+
+	id: str
+	title: str
+	sales_channel: str
 
 
 @dataclass_json
 @dataclass
 class Blueprint:
-    """
-    Blueprint object to store and validate shop data between Python and Printify
+	"""
+	Blueprint object to store and validate shop data between Python and Printify
 
-    Args:
-        id: Blueprint ID
-        title: Name of Blueprint
-        description: Description of the Blueprint given by the provider
-        brand: Brand given by the provider
-        model: Model given by the provider
-        images: List of image URLs given by the provider
-    """
-    id: int
-    title: str
-    description: str
-    brand: str
-    model: str
-    images: List[str]
+	Args:
+	    id: Blueprint ID
+	    title: Name of Blueprint
+	    description: Description of the Blueprint given by the provider
+	    brand: Brand given by the provider
+	    model: Model given by the provider
+	    images: List of image URLs given by the provider
+	"""
+
+	id: int
+	title: str
+	description: str
+	brand: str
+	model: str
+	images: List[str]
 
 
 @dataclass_json
 @dataclass
 class Location:
-    """
-    Location object to store and validate shop data between Python and Printify
+	"""
+	Location object to store and validate shop data between Python and Printify
 
-    Args:
-        address1: First address line
-        city: City
-        country: Country
-        region: Region
-        zip: Zipcode
-        address2: Second address line. Defaults to None.
-    """
-    address1: str
-    city: str
-    country: str
-    region: str
-    zip: str
-    address2: Optional[str] = field(default=None)
+	Args:
+	    address1: First address line
+	    city: City
+	    country: Country
+	    region: Region
+	    zip: Zipcode
+	    address2: Second address line. Defaults to None.
+	"""
+
+	address1: str
+	city: str
+	country: str
+	region: str
+	zip: str
+	address2: Optional[str] = field(default=None)
 
 
 @dataclass_json
 @dataclass
 class Address:
-    """
-    Address object to store and validate shop data between Python and Printify.
-    This is similar to `Location` but includes more information and used for specific APIs
-
-    Args:
-        first_name: First name of recipient
-        last_name: Last name of recipient
-        address1: First line of the address
-        city: City
-        country: Country
-        region: Region
-        zip: Zipcode
-        address2: Second line of the address. Defaults to None.
-        email: Email of the recipient. Defaults to None.
-        phone: Phone of the recipient. Defaults to None.
-        company: Company name of the recipient. Defaults to None.
-    """
-    first_name: str
-    last_name: str
-    address1: str
-    city: str
-    country: str
-    region: str
-    zip: str
-    address2: Optional[str] = field(default=None)
-    email: Optional[str] = field(default=None)
-    phone: Optional[str] = field(default=None)
-    company: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
+	"""
+	Address object to store and validate shop data between Python and Printify.
+	This is similar to `Location` but includes more information and used for specific APIs
+
+	Args:
+	    first_name: First name of recipient
+	    last_name: Last name of recipient
+	    address1: First line of the address
+	    city: City
+	    country: Country
+	    region: Region
+	    zip: Zipcode
+	    address2: Second line of the address. Defaults to None.
+	    email: Email of the recipient. Defaults to None.
+	    phone: Phone of the recipient. Defaults to None.
+	    company: Company name of the recipient. Defaults to None.
+	"""
+
+	first_name: str
+	last_name: str
+	address1: str
+	city: str
+	country: str
+	region: str
+	zip: str
+	address2: Optional[str] = field(default=None)
+	email: Optional[str] = field(default=None)
+	phone: Optional[str] = field(default=None)
+	company: Optional[str] = field(default=None, metadata=config(exclude=_exclude_if_none))
 
 
 @dataclass_json
 @dataclass
 class PrintProvider:
-    """
-    Print Provider object to store and validate shop data between Python and Printify.
+	"""
+	Print Provider object to store and validate shop data between Python and Printify.
 
-    Args:
-        id: Provider's ID
-        title: Name of the provider.
-        location: Location of the provider. Defaults to None.
-    """
-    id: int
-    title: str
-    location: Optional[Location] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
+	Args:
+	    id: Provider's ID
+	    title: Name of the provider.
+	    location: Location of the provider. Defaults to None.
+	"""
+
+	id: int
+	title: str
+	location: Optional[Location] = field(default=None, metadata=config(exclude=_exclude_if_none))
 
 
 @dataclass_json
 @dataclass
 class VariantOption:
-    """
-    Object representing various options for Variants. Stores and validate data between Python and Printify.
-    Different products and their variants will use different combinations of values.
-
-    Args:
-        color: Color of item. Defaults to None.
-        size: Size of item. Defaults to None.
-        paper: Paper of item. Defaults to None.
-        quantity: Quantity of item. Defaults to None.
-    """
-    color: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    size: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    paper: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    quantity: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
+	"""
+	Object representing various options for Variants. Stores and validate data between Python and Printify.
+	Different products and their variants will use different combinations of values.
+
+	Args:
+	    color: Color of item. Defaults to None.
+	    size: Size of item. Defaults to None.
+	    paper: Paper of item. Defaults to None.
+	    quantity: Quantity of item. Defaults to None.
+	"""
+
+	color: Optional[str] = field(default=None, metadata=config(exclude=_exclude_if_none))
+	size: Optional[str] = field(default=None, metadata=config(exclude=_exclude_if_none))
+	paper: Optional[str] = field(default=None, metadata=config(exclude=_exclude_if_none))
+	quantity: Optional[str] = field(default=None, metadata=config(exclude=_exclude_if_none))
 
 
 @dataclass_json
 @dataclass
 class VariantPlaceholder:
-    """
-    Object representing the Placeholder for a product variant. Stores and validate data between Python and Printify.
+	"""
+	Object representing the Placeholder for a product variant. Stores and validate data between Python and Printify.
 
-    Args:
-        position: Position of artwork
-        height: Height of artwork
-        width: Width of artwork
-    """
-    position: str
-    height: int
-    width: int
+	Args:
+	    position: Position of artwork
+	    height: Height of artwork
+	    width: Width of artwork
+	"""
+
+	position: str
+	height: int
+	width: int
 
 
 @dataclass_json
 @dataclass
 class Variant:
-    """
-    Object representing a Variant for a product. Stores and validate data between Python and Printify.
+	"""
+	Object representing a Variant for a product. Stores and validate data between Python and Printify.
 
-    Args:
-        id: Variant ID
-        title: Name of the variant
-        options: Options given to the variant
-        placeholders: List of placeholders for the artwork
-    """
-    id: int
-    title: str
-    options: VariantOption
-    placeholders: List[VariantPlaceholder]
+	Args:
+	    id: Variant ID
+	    title: Name of the variant
+	    options: Options given to the variant
+	    placeholders: List of placeholders for the artwork
+	"""
+
+	id: int
+	title: str
+	options: VariantOption
+	placeholders: List[VariantPlaceholder]
 
 
 @dataclass_json
 @dataclass
 class PrintProviderVariants:
-    """
-    Object representing a Variant from a print provider. Stores and validate data between Python and Printify.
+	"""
+	Object representing a Variant from a print provider. Stores and validate data between Python and Printify.
 
-    Args:
-        id:  Provider ID
-        title: Name of provider
-        variants: List of variants provider offers
-    """
-    id: int
-    title: str
-    variants: List[Variant]
-
-    def get_variant_ids(self) -> List[int]:
-        """
-        Returns a list of all IDs from the associated variants
-        """
-        return [x.id for x in self.variants]
+	Args:
+	    id:  Provider ID
+	    title: Name of provider
+	    variants: List of variants provider offers
+	"""
+
+	id: int
+	title: str
+	variants: List[Variant]
+
+	def get_variant_ids(self) -> List[int]:
+		"""
+		Returns a list of all IDs from the associated variants
+		"""
+		return [x.id for x in self.variants]
 
 
 @dataclass_json
 @dataclass
 class ShippingInfoHandlingTime:
-    """
-    Object representing the handling time for a given shipping option from a print provider.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        value: The amount of time
-        unit: The unit of time
-    """
-    value: int
-    unit: str
+	"""
+	Object representing the handling time for a given shipping option from a print provider.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    value: The amount of time
+	    unit: The unit of time
+	"""
+
+	value: int
+	unit: str
 
 
 @dataclass_json
 @dataclass
 class ShippingInfoProfileCost:
-    """
-    Object representing the shipping cost for an item from a print provider.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        cost: shipping cost in whole values. E.g., $12.98 would be 1298
-        currency: currency of the shipping cost, e.g., USD
-    """
-    cost: int
-    currency: str
+	"""
+	Object representing the shipping cost for an item from a print provider.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    cost: shipping cost in whole values. E.g., $12.98 would be 1298
+	    currency: currency of the shipping cost, e.g., USD
+	"""
+
+	cost: int
+	currency: str
 
 
 @dataclass_json
 @dataclass
 class ShippingInfoProfile:
-    """
-    Object representing the shipping profile a group of items to a given set of countries from a print provider.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        variant_ids: A list of variants of a given product
-        first_item: cost to ship the first item
-        additional_items: cost to ship any additional items to the first item
-        countries: a list of country codes this shipping profile applies to
-    """
-    variant_ids: List[int]
-    first_item: ShippingInfoProfileCost
-    additional_items: ShippingInfoProfileCost
-    countries: List[str]
+	"""
+	Object representing the shipping profile a group of items to a given set of countries from a print provider.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    variant_ids: A list of variants of a given product
+	    first_item: cost to ship the first item
+	    additional_items: cost to ship any additional items to the first item
+	    countries: a list of country codes this shipping profile applies to
+	"""
+
+	variant_ids: List[int]
+	first_item: ShippingInfoProfileCost
+	additional_items: ShippingInfoProfileCost
+	countries: List[str]
 
 
 @dataclass_json
 @dataclass
 class ShippingInfo:
-    """
-    Object representing all shipping information for a group of items from a print provider.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        handling_time: Handling time information before an item is shipped
-        profiles: List of shipping information. Includes various prices to different countries.
-    """
-    handling_time: ShippingInfoHandlingTime
-    profiles: List[ShippingInfoProfile]
+	"""
+	Object representing all shipping information for a group of items from a print provider.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    handling_time: Handling time information before an item is shipped
+	    profiles: List of shipping information. Includes various prices to different countries.
+	"""
+
+	handling_time: ShippingInfoHandlingTime
+	profiles: List[ShippingInfoProfile]
 
 
 @dataclass_json
 @dataclass
 class ShippingCost:
-    """
-    Object representing all shipping costs from a print provider.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        standard: cost of shipping given standard shipping
-        express: cost of shipping given express shipping
-    """
-    standard: int
-    express: Optional[int] = None
+	"""
+	Object representing all shipping costs from a print provider.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    standard: cost of shipping given standard shipping
+	    express: cost of shipping given express shipping
+	"""
+
+	standard: int
+	express: Optional[int] = None
 
 
 @dataclass_json
 @dataclass
 class ShippingEstimateLineItemByProduct:
-    """
-    Object representing a shipping estimate for an item based on its product and variant information.
-    Stores and validate data between Python and Printify.
-
-    Used for `CreateShippingEstimate`
-
-    Args:
-        product_id: ID of a product already created in a shop
-        variant_id: Variant ID of that product
-        quantity: Number of items to send
-    """
-    product_id: str
-    variant_id: int
-    quantity: int
+	"""
+	Object representing a shipping estimate for an item based on its product and variant information.
+	Stores and validate data between Python and Printify.
+
+	Used for `CreateShippingEstimate`
+
+	Args:
+	    product_id: ID of a product already created in a shop
+	    variant_id: Variant ID of that product
+	    quantity: Number of items to send
+	"""
+
+	product_id: str
+	variant_id: int
+	quantity: int
 
 
 @dataclass_json
 @dataclass
 class ShippingEstimateLineItemByVariant:
-    """
-    Object representing a shipping estimate for a new item based on its variant information.
-    Stores and validate data between Python and Printify.
-
-    Used for `CreateShippingEstimate`
-
-    Args:
-        print_provider_id: ID of the Print Provider
-        blueprint_id: ID of the Blueprint of the product from the provider
-        variant_id: ID of the variant from the blueprint given from the producer
-        quantity: Positive integer of items
-    """
-    print_provider_id: int
-    blueprint_id: int
-    variant_id: int
-    quantity: int
+	"""
+	Object representing a shipping estimate for a new item based on its variant information.
+	Stores and validate data between Python and Printify.
+
+	Used for `CreateShippingEstimate`
+
+	Args:
+	    print_provider_id: ID of the Print Provider
+	    blueprint_id: ID of the Blueprint of the product from the provider
+	    variant_id: ID of the variant from the blueprint given from the producer
+	    quantity: Positive integer of items
+	"""
+
+	print_provider_id: int
+	blueprint_id: int
+	variant_id: int
+	quantity: int
 
 
 @dataclass_json
 @dataclass
 class ShippingEstimateLineItemBySku:
-    """
-    Object representing a shipping estimate for an item based on SKU number and quantity.
-    Stores and validate data between Python and Printify.
-
-    Used for `CreateShippingEstimate`
-
-    Args:
-        sku: SKU number of item
-        quantity: Number of items to send
-    """
-    sku: str
-    quantity: int
+	"""
+	Object representing a shipping estimate for an item based on SKU number and quantity.
+	Stores and validate data between Python and Printify.
+
+	Used for `CreateShippingEstimate`
+
+	Args:
+	    sku: SKU number of item
+	    quantity: Number of items to send
+	"""
+
+	sku: str
+	quantity: int
 
 
 @dataclass_json
 @dataclass
 class CreateShippingEstimate:
-    """
-    Object representing a shipping estimate for a list of items to a given address from a print provider.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        line_items: List of items. This can be a list of products, a list of items by their SKU, or a list of new
-        products given their variant details.
-        address_to: Address of the recipient
-    """
-    line_items: List[
-        Union[ShippingEstimateLineItemByProduct, ShippingEstimateLineItemByVariant, ShippingEstimateLineItemBySku]]
-    address_to: Address
+	"""
+	Object representing a shipping estimate for a list of items to a given address from a print provider.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    line_items: List of items. This can be a list of products, a list of items by their SKU, or a list of new
+	    products given their variant details.
+	    address_to: Address of the recipient
+	"""
+
+	line_items: List[
+		Union[
+			ShippingEstimateLineItemByProduct,
+			ShippingEstimateLineItemByVariant,
+			ShippingEstimateLineItemBySku,
+		]
+	]
+	address_to: Address
 
 
 @dataclass_json
 @dataclass
 class ProductOptionValue:
-    """
-    Object representing product option information for a published product.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        id: ID of the option
-        title: Display name for the option
-    """
-    id: str
-    title: str
+	"""
+	Object representing product option information for a published product.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    id: ID of the option
+	    title: Display name for the option
+	"""
+
+	id: str
+	title: str
 
 
 @dataclass_json
 @dataclass
 class ProductOption:
-    """
-    Object representing product option information for a published product.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        name: Option display name
-        type: Type of option
-        values: List of values to include as options
-    """
-    name: str
-    type: str
-    values: List[ProductOptionValue]
+	"""
+	Object representing product option information for a published product.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    name: Option display name
+	    type: Type of option
+	    values: List of values to include as options
+	"""
+
+	name: str
+	type: str
+	values: List[ProductOptionValue]
 
 
 @dataclass_json
 @dataclass
 class ProductVariant:
-    """
-    Object representing variant information for a published product.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        id: Variant ID
-        price: Price of the specific variant
-        is_enabled: Flag if the variant is included in the product
-        sku: SKU for the variant
-        cost: Cost to produce the variant
-        title: Display title of the variant
-        grams: Weight of the variant
-        is_default: Flag if the variant is the default in the storefront
-        is_available: Flag if the variant is available - false may mean out of stock
-        options: Additional options for the variant
-        quantity: The number of variants left
-    """
-    id: int
-    price: int
-    is_enabled: bool
-    sku: Optional[str] = None
-    cost: Optional[int] = None
-    title: Optional[str] = None
-    grams: Optional[int] = None
-    is_default: Optional[bool] = None
-    is_available: Optional[bool] = None
-    options: Optional[List[int]] = None
-    quantity: Optional[int] = None
+	"""
+	Object representing variant information for a published product.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    id: Variant ID
+	    price: Price of the specific variant
+	    is_enabled: Flag if the variant is included in the product
+	    sku: SKU for the variant
+	    cost: Cost to produce the variant
+	    title: Display title of the variant
+	    grams: Weight of the variant
+	    is_default: Flag if the variant is the default in the storefront
+	    is_available: Flag if the variant is available - false may mean out of stock
+	    options: Additional options for the variant
+	    quantity: The number of variants left
+	"""
+
+	id: int
+	price: int
+	is_enabled: bool
+	sku: Optional[str] = None
+	cost: Optional[int] = None
+	title: Optional[str] = None
+	grams: Optional[int] = None
+	is_default: Optional[bool] = None
+	is_available: Optional[bool] = None
+	options: Optional[List[int]] = None
+	quantity: Optional[int] = None
 
 
 @dataclass_json
 @dataclass
 class ProductImage:
-    """
-    Object representing image information for a published product.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        src: File source in Printify
-        variant_ids: List of possible variants for the product
-        position: Position of the image agaist the blueprint for the given variants
-        is_default: Flag if the image is the first image in the storefront
-        is_selected_for_publishing: Flag if the image should be published
-    """
-    src: str
-    variant_ids: List[int]
-    position: str
-    is_default: bool
-    is_selected_for_publishing: Optional[bool] = None
+	"""
+	Object representing image information for a published product.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    src: File source in Printify
+	    variant_ids: List of possible variants for the product
+	    position: Position of the image agaist the blueprint for the given variants
+	    is_default: Flag if the image is the first image in the storefront
+	    is_selected_for_publishing: Flag if the image should be published
+	"""
+
+	src: str
+	variant_ids: List[int]
+	position: str
+	is_default: bool
+	is_selected_for_publishing: Optional[bool] = None
 
 
 @dataclass_json
 @dataclass
 class PrintAreaInfo:
-    """
-    Options to create or update a print area for an image. Stores and validate data between Python and Printify.
+	"""
+	Options to create or update a print area for an image. Stores and validate data between Python and Printify.
 
-    Args:
-        x: Coordinate across the X axis for an image to start
-        y: Coordinate across the Y axis for an image to start
-        scale: The scaling factor for an image to be resized
-        angle: The angle at which an image will be rotated
-    """
-    x: float
-    y: float
-    scale: float
-    angle: int
+	Args:
+	    x: Coordinate across the X axis for an image to start
+	    y: Coordinate across the Y axis for an image to start
+	    scale: The scaling factor for an image to be resized
+	    angle: The angle at which an image will be rotated
+	"""
+
+	x: float
+	y: float
+	scale: float
+	angle: int
 
 
 @dataclass_json
 @dataclass
 class PlaceholderImage(PrintAreaInfo):
-    """
-    Object representing placeholder information for a published product.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        id: Placeholder ID
-        name: Name of the placeholder
-        type: Type of the placeholder
-        height: Height of the image
-        width: Width of the image
-        x (float): Coordinate across the X axis for an image to start
-        y (float): Coordinate across the Y axis for an image to start
-        scale (float): The scaling factor for an image to be resized
-        angle (int): The angle at which an image will be rotated
-    """
-    id: str
-    name: Optional[str] = None
-    type: Optional[str] = None
-    height: Optional[int] = None
-    width: Optional[int] = None
+	"""
+	Object representing placeholder information for a published product.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    id: Placeholder ID
+	    name: Name of the placeholder
+	    type: Type of the placeholder
+	    height: Height of the image
+	    width: Width of the image
+	    x (float): Coordinate across the X axis for an image to start
+	    y (float): Coordinate across the Y axis for an image to start
+	    scale (float): The scaling factor for an image to be resized
+	    angle (int): The angle at which an image will be rotated
+	"""
+
+	id: str
+	name: Optional[str] = None
+	type: Optional[str] = None
+	height: Optional[int] = None
+	width: Optional[int] = None
 
 
 @dataclass_json
 @dataclass
 class ProductPlaceholder:
-    """
-    Object representing placeholder information for a published product.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        position: Position of the image across the blueprint on its variant
-        images: List of image information - dimensions and alterations - across the blueprint on its variant
-    """
-    position: str
-    images: List[PlaceholderImage]
+	"""
+	Object representing placeholder information for a published product.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    position: Position of the image across the blueprint on its variant
+	    images: List of image information - dimensions and alterations - across the blueprint on its variant
+	"""
+
+	position: str
+	images: List[PlaceholderImage]
 
 
 @dataclass_json
 @dataclass
 class ProductPrintArea:
-    """
-    Object representing a print area for a published product.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        variant_ids: List of variants for the product
-        placeholders: List of placeholders against the variants for the product
-        background: Color for the background - useful if a placeholder is transparent
-    """
-    variant_ids: List[int]
-    placeholders: List[ProductPlaceholder]
-    background: Optional[str] = None
+	"""
+	Object representing a print area for a published product.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    variant_ids: List of variants for the product
+	    placeholders: List of placeholders against the variants for the product
+	    background: Color for the background - useful if a placeholder is transparent
+	"""
+
+	variant_ids: List[int]
+	placeholders: List[ProductPlaceholder]
+	background: Optional[str] = None
 
 
 @dataclass_json
 @dataclass
 class ProductExternal:
-    """
-    Object representing storefront information for a published product.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        id: ID in the storefront
-        handle: link associated with the product in the storefront
-        shipping_template_id: shipping profile associated with the product in the storefront
-        channel: type of storefront
-    """
-    id: str
-    handle: str
-    shipping_template_id: Optional[str] = None
-    channel: Optional[str] = None
+	"""
+	Object representing storefront information for a published product.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    id: ID in the storefront
+	    handle: link associated with the product in the storefront
+	    shipping_template_id: shipping profile associated with the product in the storefront
+	    channel: type of storefront
+	"""
+
+	id: str
+	handle: str
+	shipping_template_id: Optional[str] = None
+	channel: Optional[str] = None
 
 
 @dataclass_json
 @dataclass
 class Product:
-    """
-    Object representing a product in Printify.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        id: Product ID
-        title: Display name of the product
-        description: Lengthy description of the item
-        tags: List of tags associated with the product
-        options: List of product options - types and names
-        variants: List of product variants - features and measurements
-        images: List of URLs for displaying the product variants
-        created_at: ISO timestamp of when the product was created
-        updated_at: ISO timestamp of when the product was updated
-        visible: flag if the product is visible in shop (false typically means archived)
-        is_locked: flag if the features of the product are locked from changes
-        blueprint_id: Blueprint ID from the print provider
-        user_id: Printify account ID
-        shop_id: Storefront ID for the specific store in the Printify account
-        print_provider_id: Print Provider ID
-        print_areas: List of prrint areas for the product across its variants
-        twodaydelivery_enabled: flag if two-day delivery is allowed as an option
-        external: storefront information for published products
-    """
-    id: str
-    title: str
-    description: str
-    tags: List[str]
-    options: List[ProductOption]
-    variants: List[ProductVariant]
-    images: List[ProductImage]
-    created_at: str
-    updated_at: str
-    visible: bool
-    is_locked: bool
-    blueprint_id: int
-    user_id: int
-    shop_id: int
-    print_provider_id: int
-    print_areas: List[ProductPrintArea]
-    # sales_channel_properties: List
-    # print_details: List
-    twodaydelivery_enabled: Optional[bool] = None
-    external: Optional[ProductExternal] = None
+	"""
+	Object representing a product in Printify.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    id: Product ID
+	    title: Display name of the product
+	    description: Lengthy description of the item
+	    tags: List of tags associated with the product
+	    options: List of product options - types and names
+	    variants: List of product variants - features and measurements
+	    images: List of URLs for displaying the product variants
+	    created_at: ISO timestamp of when the product was created
+	    updated_at: ISO timestamp of when the product was updated
+	    visible: flag if the product is visible in shop (false typically means archived)
+	    is_locked: flag if the features of the product are locked from changes
+	    blueprint_id: Blueprint ID from the print provider
+	    user_id: Printify account ID
+	    shop_id: Storefront ID for the specific store in the Printify account
+	    print_provider_id: Print Provider ID
+	    print_areas: List of prrint areas for the product across its variants
+	    twodaydelivery_enabled: flag if two-day delivery is allowed as an option
+	    external: storefront information for published products
+	"""
+
+	id: str
+	title: str
+	description: str
+	tags: List[str]
+	options: List[ProductOption]
+	variants: List[ProductVariant]
+	images: List[ProductImage]
+	created_at: str
+	updated_at: str
+	visible: bool
+	is_locked: bool
+	blueprint_id: int
+	user_id: int
+	shop_id: int
+	print_provider_id: int
+	print_areas: List[ProductPrintArea]
+	# sales_channel_properties: List
+	# print_details: List
+	twodaydelivery_enabled: Optional[bool] = None
+	external: Optional[ProductExternal] = None
 
 
 @dataclass_json
 @dataclass
 class Publish:
-    """
-    Object that tells Printify what to publish to a shop for a given product.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        title: True if the title in the storefront should be updated to that in Printify
-        description: True if the description in the storefront should be updated to that in Printify
-        images: True if the images in the storefront should be updated to that in Printify
-        variants: True if the variants in the storefront should be updated to that in Printify
-        tags: True if the tags in the storefront should be updated to that in Printify
-        keyFeatures: True if the keyFeatures in the storefront should be updated to that in Printify
-        shipping_template: True if the shipping_template in the storefront should be updated to that in Printify
-    """
-    title: bool = True
-    description: bool = True
-    images: bool = True
-    variants: bool = True
-    tags: bool = True
-    keyFeatures: bool = True
-    shipping_template: bool = True
+	"""
+	Object that tells Printify what to publish to a shop for a given product.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    title: True if the title in the storefront should be updated to that in Printify
+	    description: True if the description in the storefront should be updated to that in Printify
+	    images: True if the images in the storefront should be updated to that in Printify
+	    variants: True if the variants in the storefront should be updated to that in Printify
+	    tags: True if the tags in the storefront should be updated to that in Printify
+	    keyFeatures: True if the keyFeatures in the storefront should be updated to that in Printify
+	    shipping_template: True if the shipping_template in the storefront should be updated to that in Printify
+	"""
+
+	title: bool = True
+	description: bool = True
+	images: bool = True
+	variants: bool = True
+	tags: bool = True
+	keyFeatures: bool = True
+	shipping_template: bool = True
 
 
 @dataclass_json
 @dataclass
 class PublishingSucceededExternal:
-    """
-    Options to set storefront information for a product that has been successfully published.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        id: the storefront id
-        handle: the type of storefront
-    """
-    id: str
-    handle: str
+	"""
+	Options to set storefront information for a product that has been successfully published.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    id: the storefront id
+	    handle: the type of storefront
+	"""
+
+	id: str
+	handle: str
 
 
 @dataclass_json
 @dataclass
 class PublishingSucceeded:
-    """
-    Options to set a product publishing to a storefront as succeeded.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        external: Storefront information
-    """
-    external: PublishingSucceededExternal
+	"""
+	Options to set a product publishing to a storefront as succeeded.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    external: Storefront information
+	"""
+
+	external: PublishingSucceededExternal
 
 
 @dataclass_json
 @dataclass
 class LineItem:
-    """
-    Information for an order containing specific product, the variant used, and the quantity ordered.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        product_id: ID of the product
-        quantity: Number of items the customer bought
-        variant_id: Specific variant of the product from the print provider
-        print_provider_id: ID of theprint provider
-        cost: Cost of all the items
-        shipping_cost: Shipping cost for the items
-        status: Status of the items
-        metadata: Any associated metadata for the items
-        sent_to_production_at: ISO timestamp of when the products were sent to production
-        fulfilled_at: ISO timestamp of when the products were fulfilled for the order
-    """
-    product_id: str
-    quantity: int
-    variant_id: int
-    print_provider_id: int
-    cost: int
-    shipping_cost: int
-    status: str
-    metadata: Dict
-    sent_to_production_at: Optional[str] = None
-    fulfilled_at: Optional[str] = None
+	"""
+	Information for an order containing specific product, the variant used, and the quantity ordered.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    product_id: ID of the product
+	    quantity: Number of items the customer bought
+	    variant_id: Specific variant of the product from the print provider
+	    print_provider_id: ID of theprint provider
+	    cost: Cost of all the items
+	    shipping_cost: Shipping cost for the items
+	    status: Status of the items
+	    metadata: Any associated metadata for the items
+	    sent_to_production_at: ISO timestamp of when the products were sent to production
+	    fulfilled_at: ISO timestamp of when the products were fulfilled for the order
+	"""
+
+	product_id: str
+	quantity: int
+	variant_id: int
+	print_provider_id: int
+	cost: int
+	shipping_cost: int
+	status: str
+	metadata: Dict
+	sent_to_production_at: Optional[str] = None
+	fulfilled_at: Optional[str] = None
 
 
 @dataclass_json
 @dataclass
 class Shipment:
-    """
-    Object representing a shipment for an order
-    Stores and validate data between Python and Printify.
-
-    Args:
-        carrier: Carrier name
-        number: Tracking number
-        url: URL for tracking
-        delivered_at: ISO timestamp of when the item was delivered
-    """
-    carrier: str
-    number: str
-    url: str
-    delivered_at: str
+	"""
+	Object representing a shipment for an order
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    carrier: Carrier name
+	    number: Tracking number
+	    url: URL for tracking
+	    delivered_at: ISO timestamp of when the item was delivered
+	"""
+
+	carrier: str
+	number: str
+	url: str
+	delivered_at: str
 
 
 @dataclass_json
 @dataclass
 class Order:
-    """
-    Object representing a previously created order.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        id: Order ID
-        address_to: Address of the recipient
-        line_items: List of items in the order - their products and quantities
-        metadata: Any extra metadata regarding the order
-        total_price: Total price the customer paid
-        total_shipping: Total price the shipping cost
-        total_tax: Total tax of the order
-        status: Current status of the order
-        shipping_method: Shipping ID linked to the storefront
-        created_at: ISO timestamp of when the order was created
-        sent_to_production_at: ISO timestamp of when the order was sent to production
-        shipments: List of shipments of the items in the order
-        fulfilled_at: ISO timestamp of when the order was fulfilled
-        fulfilment_type: How the order was fulfilled
-    """
-    id: str
-    address_to: Address
-    line_items: List[LineItem]
-    metadata: Dict
-    total_price: int
-    total_shipping: int
-    total_tax: int
-    status: str
-    shipping_method: int
-    created_at: str
-    sent_to_production_at: Optional[str] = None
-    shipments: Optional[List[Shipment]] = None
-    fulfilled_at: Optional[str] = None
-    fulfilment_type: Optional[str] = None
+	"""
+	Object representing a previously created order.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    id: Order ID
+	    address_to: Address of the recipient
+	    line_items: List of items in the order - their products and quantities
+	    metadata: Any extra metadata regarding the order
+	    total_price: Total price the customer paid
+	    total_shipping: Total price the shipping cost
+	    total_tax: Total tax of the order
+	    status: Current status of the order
+	    shipping_method: Shipping ID linked to the storefront
+	    created_at: ISO timestamp of when the order was created
+	    sent_to_production_at: ISO timestamp of when the order was sent to production
+	    shipments: List of shipments of the items in the order
+	    fulfilled_at: ISO timestamp of when the order was fulfilled
+	    fulfilment_type: How the order was fulfilled
+	"""
+
+	id: str
+	address_to: Address
+	line_items: List[LineItem]
+	metadata: Dict
+	total_price: int
+	total_shipping: int
+	total_tax: int
+	status: str
+	shipping_method: int
+	created_at: str
+	sent_to_production_at: Optional[str] = None
+	shipments: Optional[List[Shipment]] = None
+	fulfilled_at: Optional[str] = None
+	fulfilment_type: Optional[str] = None
 
 
 @dataclass_json
 @dataclass
 class __CreateOrderLineItemBase:
-    variant_id: int
-    quantity: int
+	variant_id: int
+	quantity: int
 
 
 @dataclass_json
 @dataclass
 class CreateOrderLineItem(__CreateOrderLineItemBase):
-    """
-    Options to create an line item for an order order by using product information.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        product_id: ID of the product to include in an order
-        variant_id (int): the variant of the product to use in an order
-        quantity (int): the number of copies to include int he line item for a specific product
-    """
-    product_id: str
+	"""
+	Options to create an line item for an order order by using product information.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    product_id: ID of the product to include in an order
+	    variant_id (int): the variant of the product to use in an order
+	    quantity (int): the number of copies to include int he line item for a specific product
+	"""
+
+	product_id: str
 
 
 @dataclass_json
 @dataclass
 class __CreateOrder:
-    pass
+	pass
 
 
 @dataclass_json
 @dataclass
 class CreateOrderByExistingProduct(__CreateOrder):
-    """
-    Options to create an order for existing products. Stores and validate data between Python and Printify.
+	"""
+	Options to create an order for existing products. Stores and validate data between Python and Printify.
 
-    Args:
-        external_id: ID of the external storefront
-        label: label for the order - typically an order number
-        line_items: list of items to include in order, specified by product information
-        shipping_method: ID of the shipping policy in the storefront
-        send_shipping_notification: flag to send or silence shipping notifications
-        address_to: address for the recipient
-    """
-    external_id: str
-    label: str
-    line_items: List[CreateOrderLineItem]
-    shipping_method: int
-    send_shipping_notification: bool
-    address_to: Address
+	Args:
+	    external_id: ID of the external storefront
+	    label: label for the order - typically an order number
+	    line_items: list of items to include in order, specified by product information
+	    shipping_method: ID of the shipping policy in the storefront
+	    send_shipping_notification: flag to send or silence shipping notifications
+	    address_to: address for the recipient
+	"""
+
+	external_id: str
+	label: str
+	line_items: List[CreateOrderLineItem]
+	shipping_method: int
+	send_shipping_notification: bool
+	address_to: Address
 
 
 @dataclass_json
 @dataclass
 class CreateOrderLineItemSimpleProcessing(__CreateOrderLineItemBase):
-    """
-    Options to create an line item for an order by using product information and using simple print area information
-    and transformations. Stores and validate data between Python and Printify.
-
-    Author's note - It may be best to create a product with a specific variant first and then use
-    `CreateOrderByExistingProduct` to create orders.
-
-    Args:
-        variant_id (int): the variant of the product to use in an order
-        quantity (int): the number of copies to include int he line item for a specific product
-        print_provider_id: ID of the print provider
-        blueprint_id: ID of the blueprint for the product
-        print_areas: information on print areas for a variant. Warning!
-        This is unchecked and it is likely to raise a `PrintifyException` or `PrintiPyException`
-        when used to created orders.
-    """
-    print_provider_id: int
-    blueprint_id: int
-    print_areas: Dict[str, Any]
+	"""
+	Options to create an line item for an order by using product information and using simple print area information
+	and transformations. Stores and validate data between Python and Printify.
+
+	Author's note - It may be best to create a product with a specific variant first and then use
+	`CreateOrderByExistingProduct` to create orders.
+
+	Args:
+	    variant_id (int): the variant of the product to use in an order
+	    quantity (int): the number of copies to include int he line item for a specific product
+	    print_provider_id: ID of the print provider
+	    blueprint_id: ID of the blueprint for the product
+	    print_areas: information on print areas for a variant. Warning!
+	    This is unchecked and it is likely to raise a `PrintifyException` or `PrintiPyException`
+	    when used to created orders.
+	"""
+
+	print_provider_id: int
+	blueprint_id: int
+	print_areas: Dict[str, Any]
 
 
 @dataclass_json
 @dataclass
 class CreateOrderBySimpleImageProcessing(CreateOrderByExistingProduct):
-    """
-    Options to create an order for existing products with simple image manipulations against a blueprint, variant,
-    and print area. Stores and validate data between Python and Printify.
-
-    Args:
-        external_id: ID of the external storefront
-        label: label for the order - typically an order number
-        line_items: list of items to include in order, specified by blueprints, variants, and print areas
-        shipping_method: ID of the shipping policy in the storefront
-        send_shipping_notification: flag to send or silence shipping notifications
-        address_to: address for the recipient
-    """
-    external_id: str
-    label: str
-    line_items: List[CreateOrderLineItemSimpleProcessing]
-    shipping_method: int
-    send_shipping_notification: bool
-    address_to: Address
+	"""
+	Options to create an order for existing products with simple image manipulations against a blueprint, variant,
+	and print area. Stores and validate data between Python and Printify.
+
+	Args:
+	    external_id: ID of the external storefront
+	    label: label for the order - typically an order number
+	    line_items: list of items to include in order, specified by blueprints, variants, and print areas
+	    shipping_method: ID of the shipping policy in the storefront
+	    send_shipping_notification: flag to send or silence shipping notifications
+	    address_to: address for the recipient
+	"""
+
+	external_id: str
+	label: str
+	line_items: List[CreateOrderLineItemSimpleProcessing]
+	shipping_method: int
+	send_shipping_notification: bool
+	address_to: Address
 
 
 @dataclass_json
 @dataclass
 class CreateOrderLineItemAdvancedProcessingPrintAreaInfo(PrintAreaInfo):
-    """
-    Options to create or update a print area for an image. Stores and validate data between Python and Printify.
+	"""
+	Options to create or update a print area for an image. Stores and validate data between Python and Printify.
+
+	Args:
+	    x (float): Coordinate across the X axis for an image to start
+	    y (float): Coordinate across the Y axis for an image to start
+	    scale (float): The scaling factor for an image to be resized
+	    angle (int): The angle at which an image will be rotated
+	    src: the filename of the image to use
+	"""
 
-    Args:
-        x (float): Coordinate across the X axis for an image to start
-        y (float): Coordinate across the Y axis for an image to start
-        scale (float): The scaling factor for an image to be resized
-        angle (int): The angle at which an image will be rotated
-        src: the filename of the image to use
-    """
-    src: str
+	src: str
 
 
 @dataclass_json
 @dataclass
 class CreateOrderLineItemAdvancedProcessing(__CreateOrderLineItemBase):
-    """
-    Options to create an line item for an order order by using advanced image processing.
-    Stores and validate data between Python and Printify.
-
-    Author's note - It may be best to create a product with a specific variant first and then use
-    `CreateOrderByExistingProduct` to create orders.
-
-    Args:
-        variant_id: ID of the variant
-        quantity: number of items to include
-        blueprint_id: ID of the blueprint from the print provider
-        print_provider_id: ID of the print provider
-        print_areas: information for new print areas
-    """
-
-    blueprint_id: int
-    print_provider_id: int
-    print_areas: Dict[str, List[PrintAreaInfo]]
+	"""
+	Options to create an line item for an order order by using advanced image processing.
+	Stores and validate data between Python and Printify.
+
+	Author's note - It may be best to create a product with a specific variant first and then use
+	`CreateOrderByExistingProduct` to create orders.
+
+	Args:
+	    variant_id: ID of the variant
+	    quantity: number of items to include
+	    blueprint_id: ID of the blueprint from the print provider
+	    print_provider_id: ID of the print provider
+	    print_areas: information for new print areas
+	"""
+
+	blueprint_id: int
+	print_provider_id: int
+	print_areas: Dict[str, List[PrintAreaInfo]]
 
 
 @dataclass_json
 @dataclass
 class CreateOrderByAdvancedImageProcessing(__CreateOrder):
-    """
-    Options to create an order by advanced image processing. This method allows for setting a new blueprint,
-    print provider, and print areas for each line item.
-
-    Author's note - It may be best to create a product with a specific variant first and then use
-    `CreateOrderByExistingProduct` to create orders.
-
-    Stores and validate data between Python and Printify.
-
-    Args:
-        external_id: ID of the external storefront
-        label: label for the order - typically an order number
-        line_items: list of items to include in order, specified by blueprints, print providers, and print areas
-        shipping_method: ID of the shipping policy in the storefront
-        send_shipping_notification: flag to send or silence shipping notifications
-        address_to: address for the recipient
-    """
-    external_id: str
-    label: str
-    line_items: List[CreateOrderLineItemAdvancedProcessing]
-    shipping_method: int
-    send_shipping_notification: bool
-    address_to: Address
+	"""
+	Options to create an order by advanced image processing. This method allows for setting a new blueprint,
+	print provider, and print areas for each line item.
+
+	Author's note - It may be best to create a product with a specific variant first and then use
+	`CreateOrderByExistingProduct` to create orders.
+
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    external_id: ID of the external storefront
+	    label: label for the order - typically an order number
+	    line_items: list of items to include in order, specified by blueprints, print providers, and print areas
+	    shipping_method: ID of the shipping policy in the storefront
+	    send_shipping_notification: flag to send or silence shipping notifications
+	    address_to: address for the recipient
+	"""
+
+	external_id: str
+	label: str
+	line_items: List[CreateOrderLineItemAdvancedProcessing]
+	shipping_method: int
+	send_shipping_notification: bool
+	address_to: Address
 
 
 @dataclass_json
 @dataclass
 class CreateOrderLineItemPrintDetails(CreateOrderLineItemSimpleProcessing):
-    """
-    Options to create an line item for an order by using product information and using simple print area information
-    and transformations. Stores and validate data between Python and Printify.
-
-    Author's note - It may be best to create a product with a specific variant first and then use
-    `CreateOrderByExistingProduct` to create orders.
-
-    Args:
-        variant_id (int): the variant of the product to use in an order
-        quantity (int): the number of copies to include int he line item for a specific product
-        print_provider_id (int): ID of the print provider
-        blueprint_id (int): ID of the blueprint for the product
-        print_areas (Dict[str, Any]): information on print areas for a variant. Warning!
-        This is unchecked and it is likely to raise a `PrintifyException` or `PrintiPyException`
-        when used to created orders.
-        print_details (Dict[str, Any): information on print details. Warning!
-        This is unchecked and it is likely to raise a `PrintifyException` or `PrintiPyException`
-        when used to created orders.
-    """
-    print_details: Dict[str, Any]
+	"""
+	Options to create an line item for an order by using product information and using simple print area information
+	and transformations. Stores and validate data between Python and Printify.
+
+	Author's note - It may be best to create a product with a specific variant first and then use
+	`CreateOrderByExistingProduct` to create orders.
+
+	Args:
+	    variant_id (int): the variant of the product to use in an order
+	    quantity (int): the number of copies to include int he line item for a specific product
+	    print_provider_id (int): ID of the print provider
+	    blueprint_id (int): ID of the blueprint for the product
+	    print_areas (Dict[str, Any]): information on print areas for a variant. Warning!
+	    This is unchecked and it is likely to raise a `PrintifyException` or `PrintiPyException`
+	    when used to created orders.
+	    print_details (Dict[str, Any): information on print details. Warning!
+	    This is unchecked and it is likely to raise a `PrintifyException` or `PrintiPyException`
+	    when used to created orders.
+	"""
+
+	print_details: Dict[str, Any]
 
 
 @dataclass_json
 @dataclass
 class CreateOrderByPrintDetails(__CreateOrder):
-    """
-    Options to create an order by print details. Stores and validate data between Python and Printify.
+	"""
+	Options to create an order by print details. Stores and validate data between Python and Printify.
 
-    Author's note - this is the `least desirable` way to create an order. Please use another `CreateOrberBy` method
+	Author's note - this is the `least desirable` way to create an order. Please use another `CreateOrberBy` method
 
-    Args:
-        external_id: ID of the external storefront
-        label: label for the order - typically an order number
-        line_items: list of items to include in order, specified by print details
-        shipping_method: ID of the shipping policy in the storefront
-        send_shipping_notification: flag to send or silence shipping notifications
-        address_to: address for the recipient
-    """
-    external_id: str
-    label: str
-    line_items: List[CreateOrderLineItemPrintDetails]
-    shipping_method: int
-    send_shipping_notification: bool
-    address_to: Address
+	Args:
+	    external_id: ID of the external storefront
+	    label: label for the order - typically an order number
+	    line_items: list of items to include in order, specified by print details
+	    shipping_method: ID of the shipping policy in the storefront
+	    send_shipping_notification: flag to send or silence shipping notifications
+	    address_to: address for the recipient
+	"""
+
+	external_id: str
+	label: str
+	line_items: List[CreateOrderLineItemPrintDetails]
+	shipping_method: int
+	send_shipping_notification: bool
+	address_to: Address
 
 
 @dataclass_json
 @dataclass
 class CreateOrderLineItemSku:
-    """
-    Options to create an line item for an order by using SKU. Stores and validate data between Python and Printify.
+	"""
+	Options to create an line item for an order by using SKU. Stores and validate data between Python and Printify.
 
-    Args:
-        sku: the SKU of an item to include in the order
-        quantity: the number of items to include
-    """
-    sku: str
-    quantity: int
+	Args:
+	    sku: the SKU of an item to include in the order
+	    quantity: the number of items to include
+	"""
+
+	sku: str
+	quantity: int
 
 
 @dataclass_json
 @dataclass
 class CreateOrderBySku(__CreateOrder):
-    """
-    Options to create an order by an SKU number. Stores and validate data between Python and Printify.
+	"""
+	Options to create an order by an SKU number. Stores and validate data between Python and Printify.
 
-    Args:
-        external_id: ID of the external storefront
-        label: label for the order - typically an order number
-        line_items: list of items to include in order, specified by SKUs
-        shipping_method: ID of the shipping policy in the storefront
-        send_shipping_notification: flag to send or silence shipping notifications
-        address_to: address for the recipient
-    """
-    external_id: str
-    label: str
-    line_items: List[CreateOrderLineItemSku]
-    shipping_method: int
-    send_shipping_notification: bool
-    address_to: Address
+	Args:
+	    external_id: ID of the external storefront
+	    label: label for the order - typically an order number
+	    line_items: list of items to include in order, specified by SKUs
+	    shipping_method: ID of the shipping policy in the storefront
+	    send_shipping_notification: flag to send or silence shipping notifications
+	    address_to: address for the recipient
+	"""
+
+	external_id: str
+	label: str
+	line_items: List[CreateOrderLineItemSku]
+	shipping_method: int
+	send_shipping_notification: bool
+	address_to: Address
 
 
 @dataclass_json
 @dataclass
 class Artwork:
-    """
-    Object representing an Image or Artwork. Stores and validate data between Python and Printify.
+	"""
+	Object representing an Image or Artwork. Stores and validate data between Python and Printify.
 
-    Args:
-        id: Artwork ID in Printify
-        file_name: filename in Printify
-        height: height of the image
-        width: width of the image
-        size: byte size of the image
-        mime_type: media type of the image, e.g., `image/png`
-        preview_url: URL to preview the image
-        upload_time: ISO date format of the time the image was uploaded
-    """
-    id: str
-    file_name: str
-    height: int
-    width: int
-    size: int
-    mime_type: str
-    preview_url: str
-    upload_time: str
+	Args:
+	    id: Artwork ID in Printify
+	    file_name: filename in Printify
+	    height: height of the image
+	    width: width of the image
+	    size: byte size of the image
+	    mime_type: media type of the image, e.g., `image/png`
+	    preview_url: URL to preview the image
+	    upload_time: ISO date format of the time the image was uploaded
+	"""
+
+	id: str
+	file_name: str
+	height: int
+	width: int
+	size: int
+	mime_type: str
+	preview_url: str
+	upload_time: str
 
 
 @dataclass_json
 @dataclass
 class Webhook:
-    """
-    Object representing a Webhook. Stores and validate data between Python and Printify.
+	"""
+	Object representing a Webhook. Stores and validate data between Python and Printify.
 
-    Args:
-        id: Webhook ID
-        shop_id: ID of the shop relating to the webhook
-        url: External webhook URL
-        topic: type of event to push data to
-    """
-    id: str
-    shop_id: str
-    url: str
-    topic: str
+	Args:
+	    id: Webhook ID
+	    shop_id: ID of the shop relating to the webhook
+	    url: External webhook URL
+	    topic: type of event to push data to
+	"""
+
+	id: str
+	shop_id: str
+	url: str
+	topic: str
 
 
 @dataclass_json
 @dataclass
 class CreateWebhook:
-    """
-    Options to create a webhook. Stores and validate data between Python and Printify.
+	"""
+	Options to create a webhook. Stores and validate data between Python and Printify.
+
+	Args:
+	    url: External webhook URL
+	    topic: type of event to push data to
+	"""
 
-    Args:
-        url: External webhook URL
-        topic: type of event to push data to
-    """
-    url: str
-    topic: str
+	url: str
+	topic: str
 
 
 @dataclass_json
 @dataclass
 class UpdateWebhook:
-    """
-    Options to update a webhook. All fields are optional. Stores and validate data between Python and Printify.
+	"""
+	Options to update a webhook. All fields are optional. Stores and validate data between Python and Printify.
 
-    Args:
-        url: External webhook URL
-        topic: type of event to push data to
-    """
-    url: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    topic: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
+	Args:
+	    url: External webhook URL
+	    topic: type of event to push data to
+	"""
+
+	url: Optional[str] = field(default=None, metadata=config(exclude=_exclude_if_none))
+	topic: Optional[str] = field(default=None, metadata=config(exclude=_exclude_if_none))
 
 
 @dataclass_json
 @dataclass
 class CreateProductPrintAreaPlaceholderImage(PrintAreaInfo):
-    """
-    Options to create a new image in a place holder for a print area.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        id: Image ID to use in the print area
-        x (float): Coordinate across the X axis for an image to start
-        y (float): Coordinate across the Y axis for an image to start
-        scale (float): The scaling factor for an image to be resized
-        angle (int): The angle at which an image will be rotated
-    """
-    id: str
+	"""
+	Options to create a new image in a place holder for a print area.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    id: Image ID to use in the print area
+	    x (float): Coordinate across the X axis for an image to start
+	    y (float): Coordinate across the Y axis for an image to start
+	    scale (float): The scaling factor for an image to be resized
+	    angle (int): The angle at which an image will be rotated
+	"""
+
+	id: str
 
 
 @dataclass_json
 @dataclass
 class CreateProductPrintAreaPlaceholder:
-    """
-    Options to create a new print area for a product placeholder. Stores and validate data between Python and Printify.
+	"""
+	Options to create a new print area for a product placeholder. Stores and validate data between Python and Printify.
 
-    Args:
-        position: The position of the print area
-        images: List of images, their size, and dimensions for the placeholder
-    """
-    position: str
-    images: List[CreateProductPrintAreaPlaceholderImage]
+	Args:
+	    position: The position of the print area
+	    images: List of images, their size, and dimensions for the placeholder
+	"""
+
+	position: str
+	images: List[CreateProductPrintAreaPlaceholderImage]
 
 
 @dataclass_json
 @dataclass
 class CreateProductPrintArea:
-    """
-    Options to create a new product print area. Stores and validate data between Python and Printify.
+	"""
+	Options to create a new product print area. Stores and validate data between Python and Printify.
+
+	Args:
+	    variant_ids: List of variants of the product to include from the print provider.
+	    placeholders: List of product placeholders - their dimensions and sizes
+	"""
 
-    Args:
-        variant_ids: List of variants of the product to include from the print provider.
-        placeholders: List of product placeholders - their dimensions and sizes
-    """
-    variant_ids: List[int]
-    placeholders: List[CreateProductPrintAreaPlaceholder]
+	variant_ids: List[int]
+	placeholders: List[CreateProductPrintAreaPlaceholder]
 
 
 @dataclass_json
 @dataclass
 class CreateProductVariant:
-    """
-    Options to create a new product variant. Stores and validate data between Python and Printify.
+	"""
+	Options to create a new product variant. Stores and validate data between Python and Printify.
 
-    Args:
-        id: Variant ID for a product from a print provider
-        price: Price the product will sell at. All numbers are whole integers, e.g., $12.95 is `1295`
-        is_enabled: Flag for enabling a variant in a store
-    """
-    id: int
-    price: int
-    is_enabled: bool
+	Args:
+	    id: Variant ID for a product from a print provider
+	    price: Price the product will sell at. All numbers are whole integers, e.g., $12.95 is `1295`
+	    is_enabled: Flag for enabling a variant in a store
+	"""
+
+	id: int
+	price: int
+	is_enabled: bool
 
 
 @dataclass_json
 @dataclass
 class CreateProduct:
-    """
-    Options to create a new product. Stores and validate data between Python and Printify.
+	"""
+	Options to create a new product. Stores and validate data between Python and Printify.
 
-    Args:
-        title: Display name of the product
-        description: Lengthy description of the item
-        blueprint_id: Blueprint ID from the Print Provider
-        print_provider_id: Print Provider ID
-        variants: List of product variants, their price, and if they are enabled
-        print_areas: List of product dimensions and print areas
-    """
-    title: str
-    description: str
-    blueprint_id: int
-    print_provider_id: int
-    variants: List[CreateProductVariant]
-    print_areas: List[CreateProductPrintArea]
-
-    def add_variant(self, variant: CreateProductVariant):
-        """
-        Appends a new variant to the product. Useful if variants are not all known at the time of creating the product
-
-        Args:
-            variant: New variant to attach to the new product
-        """
-        self.variants.append(variant)
-
-    def add_print_area(self, print_area: CreateProductPrintArea):
-        """
-        Appends a new pint area to the product. Useful if variants are not all known at the time of creating the product
-
-        Args:
-            print_area: New print area to attach to the new product
-        """
-        self.print_areas.append(print_area)
+	Args:
+	    title: Display name of the product
+	    description: Lengthy description of the item
+	    blueprint_id: Blueprint ID from the Print Provider
+	    print_provider_id: Print Provider ID
+	    variants: List of product variants, their price, and if they are enabled
+	    print_areas: List of product dimensions and print areas
+	"""
+
+	title: str
+	description: str
+	blueprint_id: int
+	print_provider_id: int
+	variants: List[CreateProductVariant]
+	print_areas: List[CreateProductPrintArea]
+
+	def add_variant(self, variant: CreateProductVariant):
+		"""
+		Appends a new variant to the product. Useful if variants are not all known at the time of creating the product
+
+		Args:
+		    variant: New variant to attach to the new product
+		"""
+		self.variants.append(variant)
+
+	def add_print_area(self, print_area: CreateProductPrintArea):
+		"""
+		Appends a new pint area to the product. Useful if variants are not all known at the time of creating the product
+
+		Args:
+		    print_area: New print area to attach to the new product
+		"""
+		self.print_areas.append(print_area)
 
 
 @dataclass_json
 @dataclass
 class UpdateProductExternal:
-    """
-    Options to update a product external information. Stores and validate data between Python and Printify.
+	"""
+	Options to update a product external information. Stores and validate data between Python and Printify.
 
-    Args:
-        id: Storefront ID
-        handle: The type of storefront
-        shipping_template_id: Shipping methods in the store the product will use
-    """
-    id: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    handle: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    shipping_template_id: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
+	Args:
+	    id: Storefront ID
+	    handle: The type of storefront
+	    shipping_template_id: Shipping methods in the store the product will use
+	"""
+
+	id: Optional[str] = field(default=None, metadata=config(exclude=_exclude_if_none))
+	handle: Optional[str] = field(default=None, metadata=config(exclude=_exclude_if_none))
+	shipping_template_id: Optional[str] = field(
+		default=None, metadata=config(exclude=_exclude_if_none)
+	)
 
 
 @dataclass_json
 @dataclass
 class UpdateProduct:
-    """
-    Options to update a product and its information. All fields are optional.
-    Stores and validate data between Python and Printify.
-
-    Args:
-        title: New product title
-        description: New product description
-        blueprint_id: New ID of a blueprint from the print provider
-        print_provider_id: New ID of the print provider
-        variants: New product variants - prices and eligibility - for the product
-        print_areas: New print areas - placeholders and printing specifications - for the product
-        external: New external information - storefront and shipping - for the product
-    """
-    title: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    description: Optional[str] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    blueprint_id: Optional[int] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    print_provider_id: Optional[int] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    variants: Optional[List[CreateProductVariant]] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    print_areas: Optional[List[CreateProductPrintArea]] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
-    external: Optional[UpdateProductExternal] = field(
-        default=None, metadata=config(exclude=_exclude_if_none)
-    )
+	"""
+	Options to update a product and its information. All fields are optional.
+	Stores and validate data between Python and Printify.
+
+	Args:
+	    title: New product title
+	    description: New product description
+	    blueprint_id: New ID of a blueprint from the print provider
+	    print_provider_id: New ID of the print provider
+	    variants: New product variants - prices and eligibility - for the product
+	    print_areas: New print areas - placeholders and printing specifications - for the product
+	    external: New external information - storefront and shipping - for the product
+	"""
+
+	title: Optional[str] = field(default=None, metadata=config(exclude=_exclude_if_none))
+	description: Optional[str] = field(default=None, metadata=config(exclude=_exclude_if_none))
+	blueprint_id: Optional[int] = field(default=None, metadata=config(exclude=_exclude_if_none))
+	print_provider_id: Optional[int] = field(
+		default=None, metadata=config(exclude=_exclude_if_none)
+	)
+	variants: Optional[List[CreateProductVariant]] = field(
+		default=None, metadata=config(exclude=_exclude_if_none)
+	)
+	print_areas: Optional[List[CreateProductPrintArea]] = field(
+		default=None, metadata=config(exclude=_exclude_if_none)
+	)
+	external: Optional[UpdateProductExternal] = field(
+		default=None, metadata=config(exclude=_exclude_if_none)
+	)
```

### Comparing `printipy-1.2.0/printipy/exceptions.py` & `printipy-1.2.1/printipy/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,85 @@
 class PrintiPyException(Exception):
-    """
-    When a request doesn't meet the minimum needs to send/receive information with Printify. AKA, user error.
+	"""
+	When a request doesn't meet the minimum needs to send/receive information with Printify. AKA, user error.
 
-    Examples:
-        >>> from printipy.api import PrintiPy
-        >>> api = PrintiPy(api_token='...', shop_id='...')
-        >>> try:
-        >>>   api.artwork.upload_artwork(...)
-        >>> except PrintiPyException e:
-        >>>   print(e)
-    """
-    pass
+	Examples:
+	    >>> from printipy.api import PrintiPy
+	    >>> api = PrintiPy(api_token='...', shop_id='...')
+	    >>> try:
+	    >>>   api.artwork.upload_artwork(...)
+	    >>> except PrintiPyException e:
+	    >>>   print(e)
+	"""
+
+	pass
 
 
 class PrintiPyParseException(PrintiPyException):
-    """
-    When unable to parse Printify's response into a PrintiPy. Please report these errors to the developer.
+	"""
+	When unable to parse Printify's response into a PrintiPy. Please report these errors to the developer.
+
+	Examples:
+	    >>> from printipy.api import PrintiPy
+	    >>> api = PrintiPy(api_token='...', shop_id='...')
+	    >>> try:
+	    >>>   api.products.get_products()
+	    >>> except PrintiPyParseException e:
+	    >>>   print(e)
+	"""
 
-    Examples:
-        >>> from printipy.api import PrintiPy
-        >>> api = PrintiPy(api_token='...', shop_id='...')
-        >>> try:
-        >>>   api.products.get_products()
-        >>> except PrintiPyParseException e:
-        >>>   print(e)
-    """
-    pass
+	pass
 
 
 class InvalidScopeException(Exception):
-    """
-    When the given API key isn't permitted to perform the operation.
-    Use a different API key from Printify or update the permissions of the given key.
-
-    Examples:
-        >>> from printipy.api import PrintiPy
-        >>> from printipy.data_objects import CreateProduct
-        >>> api = PrintiPy(api_token='...', shop_id='...')
-        >>> new_product = CreateProduct(...)
-        >>> try:
-        >>>   created_product = api.products.create_product()
-        >>> except InvalidScopeException e:
-        >>>   print(e)
-    """
-    pass
+	"""
+	When the given API key isn't permitted to perform the operation.
+	Use a different API key from Printify or update the permissions of the given key.
+
+	Examples:
+	    >>> from printipy.api import PrintiPy
+	    >>> from printipy.data_objects import CreateProduct
+	    >>> api = PrintiPy(api_token='...', shop_id='...')
+	    >>> new_product = CreateProduct(...)
+	    >>> try:
+	    >>>   created_product = api.products.create_product()
+	    >>> except InvalidScopeException e:
+	    >>>   print(e)
+	"""
+
+	pass
 
 
 class InvalidRequestException(Exception):
-    """
-    When Printify raised a 500 Server Error. Typically happens when the request contains incorrect data.
+	"""
+	When Printify raised a 500 Server Error. Typically happens when the request contains incorrect data.
 
-    Examples:
-        >>> from printipy.api import PrintiPy
-        >>> from printipy.data_objects import CreateProduct
-        >>> api = PrintiPy(api_token='...', shop_id='...')
-        >>> new_product = CreateProduct(...)
-        >>> try:
-        >>>   created_product = api.products.create_product()
-        >>> except InvalidRequestException e:
-        >>>   print(e)
-    """
-    pass
+	Examples:
+	    >>> from printipy.api import PrintiPy
+	    >>> from printipy.data_objects import CreateProduct
+	    >>> api = PrintiPy(api_token='...', shop_id='...')
+	    >>> new_product = CreateProduct(...)
+	    >>> try:
+	    >>>   created_product = api.products.create_product()
+	    >>> except InvalidRequestException e:
+	    >>>   print(e)
+	"""
+
+	pass
 
 
 class PrintifyException(Exception):
-    """
-    When Printify returns an error - usually contains information regarding malformed input
+	"""
+	When Printify returns an error - usually contains information regarding malformed input
+
+	Examples:
+	    >>> from printipy.api import PrintiPy
+	    >>> from printipy.data_objects import CreateProduct
+	    >>> api = PrintiPy(api_token='...', shop_id='...')
+	    >>> new_product = CreateProduct(...)
+	    >>> try:
+	    >>>   created_product = api.products.create_product()
+	    >>> except PrintifyException e:
+	    >>>   print(e)
+	"""
 
-    Examples:
-        >>> from printipy.api import PrintiPy
-        >>> from printipy.data_objects import CreateProduct
-        >>> api = PrintiPy(api_token='...', shop_id='...')
-        >>> new_product = CreateProduct(...)
-        >>> try:
-        >>>   created_product = api.products.create_product()
-        >>> except PrintifyException e:
-        >>>   print(e)
-    """
-    pass
+	pass
```

### Comparing `printipy-1.2.0/printipy.egg-info/PKG-INFO` & `printipy-1.2.1/printipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: printipy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Printify API for Python
 Home-page: https://github.com/lawrencemq/printipy
 Author: Lawrence Weikum
 Keywords: printify,print on demand,api
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: dataclasses-json
 
 # PrintiPy
 The Printify API for Python
 
 Printify's REST API gives your scripts or applications power to manage Printify shops. Create and update products, submit orders, build custom integrations, and so much more!
 
-Tested with Python 3.9 - 3.11.
+Tested with Python 3.9 - 3.12.
 
 ## Install
 
 ```shell
 pipenv install printipy
 ```
```

