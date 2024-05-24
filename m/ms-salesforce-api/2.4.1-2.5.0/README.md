# Comparing `tmp/ms_salesforce_api-2.4.1.tar.gz` & `tmp/ms_salesforce_api-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-2.4.1.tar", max compression
+gzip compressed data, was "ms_salesforce_api-2.5.0.tar", max compression
```

## Comparing `ms_salesforce_api-2.4.1.tar` & `ms_salesforce_api-2.5.0.tar`

### file list

```diff
@@ -1,39 +1,45 @@
--rw-r--r--   0        0        0    35149 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/LICENSE
--rw-r--r--   0        0        0     8326 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/README.md
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0     1244 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2926 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2205 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/__init__.py
--rw-r--r--   0        0        0     1620 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/__init__.py
--rw-r--r--   0        0        0     4925 2024-04-19 10:53:55.411235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/constants.py
--rw-r--r--   0        0        0    14992 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/dto/__init__.py
--rw-r--r--   0        0        0     5240 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py
--rw-r--r--   0        0        0     6011 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/export_data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    10789 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0      303 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/helpers.py
--rw-r--r--   0        0        0     3788 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/__tests__/__init__.py
--rw-r--r--   0        0        0    25119 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py
--rw-r--r--   0        0        0    10921 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/constants.py
--rw-r--r--   0        0        0     3967 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    35677 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2485 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/dto/__init__.py
--rw-r--r--   0        0        0     9817 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py
--rw-r--r--   0        0        0    12640 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    13717 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0        0 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/helpers/__init__.py
--rw-r--r--   0        0        0      303 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/helpers/string.py
--rw-r--r--   0        0        0     1055 2024-04-19 10:53:55.415235 ms_salesforce_api-2.4.1/pyproject.toml
--rw-r--r--   0        0        0     9153 1970-01-01 00:00:00.000000 ms_salesforce_api-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/LICENSE
+-rw-r--r--   0        0        0     8326 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0     1244 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2926 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2205 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/__init__.py
+-rw-r--r--   0        0        0     1532 2024-05-24 09:43:12.729689 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/__init__.py
+-rw-r--r--   0        0        0     1517 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/constants.py
+-rw-r--r--   0        0        0    14378 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/dto/AccountDTO.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/dto/__init__.py
+-rw-r--r--   0        0        0     4077 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/export_data/Bigquery.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/account/export_data/__init__.py
+-rw-r--r--   0        0        0     1620 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py
+-rw-r--r--   0        0        0     4975 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/constants.py
+-rw-r--r--   0        0        0    15701 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/dto/__init__.py
+-rw-r--r--   0        0        0     5381 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py
+-rw-r--r--   0        0        0     6011 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    10789 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0      303 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/helpers.py
+-rw-r--r--   0        0        0     3788 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    24839 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0    10921 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/constants.py
+-rw-r--r--   0        0        0     3967 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    35689 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2485 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/__init__.py
+-rw-r--r--   0        0        0     9829 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0    12640 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    13717 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/helpers/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/helpers/string.py
+-rw-r--r--   0        0        0     1055 2024-05-24 09:43:12.733688 ms_salesforce_api-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9153 1970-01-01 00:00:00.000000 ms_salesforce_api-2.5.0/PKG-INFO
```

### Comparing `ms_salesforce_api-2.4.1/LICENSE` & `ms_salesforce_api-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/README.md` & `ms_salesforce_api-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/__init__.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/constants.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Amount,
     Amount_EUR__c,
     CampaignId,
     Close_Month_Formula__c,
     CloseDate,
     ContactId,
     CurrencyIsoCode,
+    CreatedDate,
     EndDate__c,
     ExpectedRevenue,
     Fiscal,
     FiscalQuarter,
     FiscalYear,
     FRM_JiraDefaultName__c,
     GACLIENTID__c,
@@ -40,15 +41,16 @@
     MS_Account_Invoice_Country_Code__c,
     MS_Company_Origin__c,
     Name,
     Opportunity_Name_Short__c,
     Opportunity_requestor__c,
     OwnerId,
     Probability,
-    RecordTypeId,
+    Proposal_Delivery_Date__c,
+    RecordType.Name,
     ROI_Analysis_Completed__c,
     Servicios_Asociados__c,
     StageName,
     Start_Date__c,
     Tier_Short__c,
     TotalOpportunityQuantity,
     Year_Created__c,
@@ -63,15 +65,14 @@
             Quantity,
             UnitPrice
         FROM
             OpportunityLineItems
     )
 FROM
     Opportunity
-
 """
 # WHERE
 #     Id='0063X000013A8JPQA0'
 
 DEFAULT_ALL_OPPORTUNITIES_CREATE_TABLE_QUERY = """
 CREATE TABLE all_opportunity (
     opportunity_id VARCHAR(255) PRIMARY KEY,
```

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,17 @@
         stage_name,
         start_date,
         tier_short,
         total_opportunity_quantity,
         year_created,
         opportunity_line_items,
         lkp_project,
+        created_date,
+        proposal_delivery_date,
+        record_type,
     ):
         self.opportunity_id = opportunity_id
         self.account_billing_country = account_billing_country
         self.account_owner = account_owner
         self.account_id = account_id
         self.amount = amount
         self.amount_eur = amount_eur
@@ -181,14 +184,17 @@
         self.stage_name = stage_name
         self.start_date = start_date
         self.tier_short = tier_short
         self.total_opportunity_quantity = total_opportunity_quantity
         self.year_created = year_created
         self.opportunity_line_items = opportunity_line_items
         self.lkp_project = lkp_project
+        self.created_date = created_date
+        self.proposal_delivery_date = proposal_delivery_date
+        self.record_type = record_type
 
     @staticmethod
     def from_salesforce_record(record):
         def _get_year_created(key: str):
             try:
                 year = int(record[key])
                 # We set allways the January first date because they want
@@ -206,14 +212,20 @@
 
             date_formatted = (
                 f"{datetime.now().year}-{month_num}-{day.zfill(2)}"
             )
 
             return date_formatted
 
+        def _get_record_type():
+            try:
+                return record["RecordType"]["Name"]
+            except (KeyError, TypeError):
+                return ""
+
         opportunity_line_items = record.get("OpportunityLineItems", {})
         if opportunity_line_items and isinstance(opportunity_line_items, dict):
             line_items_records = record.get("OpportunityLineItems", {}).get(
                 "records", []
             )
             opportunity_line_items = [
                 OpportunityLineItemDTO.from_salesforce_record(
@@ -312,14 +324,17 @@
             tier_short=normalize_value(record.get("Tier_Short__c", "")),
             total_opportunity_quantity=normalize_value(
                 record.get("TotalOpportunityQuantity", "")
             ),
             year_created=_get_year_created("Year_Created__c"),
             opportunity_line_items=opportunity_line_items,
             lkp_project=normalize_value(record.get("LKP_Project__c", "")),
+            created_date=record["CreatedDate"],
+            proposal_delivery_date=record["Proposal_Delivery_Date__c"],
+            record_type=_get_record_type(),
         )
 
     def to_dict(self):
         return {
             "opportunity_id": self.opportunity_id,
             "account_billing_country": self.account_billing_country,
             "account_owner": self.account_owner,
@@ -370,8 +385,11 @@
             "stage_name": self.stage_name,
             "start_date": self.start_date,
             "tier_short": self.tier_short,
             "total_opportunity_quantity": self.total_opportunity_quantity,
             "year_created": self.year_created,
             "opportunity_line_items": self.opportunity_line_items,
             "lkp_project": self.lkp_project,
+            "created_date": self.created_date,
+            "proposal_delivery_date": self.proposal_delivery_date,
+            "record_type": self.record_type,
         }
```

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,17 @@
                 "associated_services": "STRING",
                 "stage_name": "STRING",
                 "tier_short": "STRING",
                 "total_opportunity_quantity": "FLOAT",
                 "start_date": "DATE",
                 "year_created": "DATE",
                 "lkp_project": "STRING",
+                "created_date": "TIMESTAMP",
+                "proposal_delivery_date": "TIMESTAMP",
+                "record_type": "STRING",
             },
             "opportunity_line_item": {
                 "opportunity_id": "STRING",
                 "product_id": "STRING",
                 "profit_center_name": "STRING",
                 "country": "STRING",
                 "product_name": "STRING",
```

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/__init__.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,33 +452,29 @@
                 "group_end_date": "2100-12-12",
                 "group_groupid": "a0cAX000000TSWUYA4",
                 "group_name": "MAPFRE",
                 "group_owner_email": "employee1@test.com",
                 "group_pck_type": "Key Account",
                 "group_start_date": "2023-06-01",
                 "group_supervisor_email": "employee2@test.com",
-                "internal_comment": "",
                 "international_deparments": False,
                 "invoicing_country_code": "US",
                 "jira_task_url": "<a "
                 "href=https://makingscience.atlassian.net/browse/ESMSBD0001-7168 "
                 "target=_blank>View Jira Task</a>",
                 "last_updated_at": "2023-09-01T10:00:54.000+0000",
-                "lead_source": "Crosselling/upselling",
                 "maintance_project": False,
                 "ms_project_id": False,
-                "operation_coordinator_controller": "",
                 "operation_coordinator_email": "employee5@test.com",
                 "operation_coordinator_name": "",
                 "operation_coordinator_sub": "",
                 "operation_coordinator_sub_email": "employee5@test.com",
                 "opportunity": "",
                 "opportunity_extension": "",
                 "opportunity_name": "New Site Mapfre AAA",
-                "opportunity_percentage": 100.0,
                 "periodicity": "",
                 "profit_center": "200018",
                 "profitcenter": "",
                 "project_account": "",
                 "project_code": "USMSEX05508",
                 "project_id": "a00AX000002DVi1YAG",
                 "project_line_items": [
@@ -517,17 +513,15 @@
                 ],
                 "project_name": "MapfreAAA",
                 "project_start_date": "2022-08-01",
                 "project_tier": "Unkown",
                 "projectcode": "",
                 "projectid": "",
                 "quote": "",
-                "rejection_reason": "",
                 "revenue_details": "",
-                "stage": "Closed Won",
                 "status": "",
                 "subgroup_bqid": "5",
                 "subgroup_end_date": "2100-12-12",
                 "subgroup_groupid": "a0cAX000000TSWUYA4",
                 "subgroup_name": "MAPFRE USA",
                 "subgroup_owner_email": "employee1@test.com",
                 "subgroup_start_date": "2023-06-01",
```

#### html2text {}

```diff
@@ -184,52 +184,48 @@
 "a00AX000002DVi1YAG", "revenue_dedication": 103.2, } ], "comments": "",
 "controller_email": "employee4@test.com", "controller_sub_email":
 "employee3@test.com", "cost_center": "", "created_at": "2022-08-01T08:53:
 12.000+0000", "currency": "EUR", "end_date": "", "group_bqid": "1",
 "group_end_date": "2100-12-12", "group_groupid": "a0cAX000000TSWUYA4",
 "group_name": "MAPFRE", "group_owner_email": "employee1@test.com",
 "group_pck_type": "Key Account", "group_start_date": "2023-06-01",
-"group_supervisor_email": "employee2@test.com", "internal_comment": "",
-"international_deparments": False, "invoicing_country_code": "US",
-"jira_task_url": "
+"group_supervisor_email": "employee2@test.com", "international_deparments":
+False, "invoicing_country_code": "US", "jira_task_url": "
  "href=https://makingscience.atlassian.net/browse/ESMSBD0001-7168 "
 "target=_blank>View Jira Task
-", "last_updated_at": "2023-09-01T10:00:54.000+0000", "lead_source":
-"Crosselling/upselling", "maintance_project": False, "ms_project_id": False,
-"operation_coordinator_controller": "", "operation_coordinator_email":
+", "last_updated_at": "2023-09-01T10:00:54.000+0000", "maintance_project":
+False, "ms_project_id": False, "operation_coordinator_email":
 "employee5@test.com", "operation_coordinator_name": "",
 "operation_coordinator_sub": "", "operation_coordinator_sub_email":
 "employee5@test.com", "opportunity": "", "opportunity_extension": "",
-"opportunity_name": "New Site Mapfre AAA", "opportunity_percentage": 100.0,
-"periodicity": "", "profit_center": "200018", "profitcenter": "",
-"project_account": "", "project_code": "USMSEX05508", "project_id":
-"a00AX000002DVi1YAG", "project_line_items": [ { "country": None,
-"created_date": "2022-08-02T15:44:34.000+0000", "effort": "516", "ending_date":
-"2022-12-31", "id": "a0VAX000000EE0b2AG", "last_modified_date": "2023-06-20T22:
-33:36.000+0000", "ms_pli_name": "USA_UX/UI Design_USMSEX05508",
-"ms_project_code": None, "product_name": "UXUI Project", "project_id":
-"a00AX000002DVi1YAG", "quantity": 516.0, "starting_date": "2022-08-01",
-"total_price": 33540.0, "unit_price": 65.0, }, { "country": None,
+"opportunity_name": "New Site Mapfre AAA", "periodicity": "", "profit_center":
+"200018", "profitcenter": "", "project_account": "", "project_code":
+"USMSEX05508", "project_id": "a00AX000002DVi1YAG", "project_line_items": [
+{ "country": None, "created_date": "2022-08-02T15:44:34.000+0000", "effort":
+"516", "ending_date": "2022-12-31", "id": "a0VAX000000EE0b2AG",
+"last_modified_date": "2023-06-20T22:33:36.000+0000", "ms_pli_name": "USA_UX/UI
+Design_USMSEX05508", "ms_project_code": None, "product_name": "UXUI Project",
+"project_id": "a00AX000002DVi1YAG", "quantity": 516.0, "starting_date": "2022-
+08-01", "total_price": 33540.0, "unit_price": 65.0, }, { "country": None,
 "created_date": "2022-08-09T14:54:59.000+0000", "effort": "331", "ending_date":
 "2022-12-31", "id": "a0VAX000000ELU52AO", "last_modified_date": "2023-06-20T22:
 33:36.000+0000", "ms_pli_name": "ES_UX/UI Design_USMSEX05508",
 "ms_project_code": None, "product_name": "UXUI Project", "project_id":
 "a00AX000002DVi1YAG", "quantity": 331.0, "starting_date": "2022-08-01",
 "total_price": 21515.0, "unit_price": 65.0, }, ], "project_name": "MapfreAAA",
 "project_start_date": "2022-08-01", "project_tier": "Unkown", "projectcode":
-"", "projectid": "", "quote": "", "rejection_reason": "", "revenue_details":
-"", "stage": "Closed Won", "status": "", "subgroup_bqid": "5",
-"subgroup_end_date": "2100-12-12", "subgroup_groupid": "a0cAX000000TSWUYA4",
-"subgroup_name": "MAPFRE USA", "subgroup_owner_email": "employee1@test.com",
-"subgroup_start_date": "2023-06-01", "subgroup_subgroupid":
-"a19AX0000004simYAA", }, ) billing_line = opportunity["billing_lines"][0]
-self.assertDictEqual( billing_line, { "billing_amount": 6708.0, "billing_date":
-"2022-08-31", "billing_period_ending_date": "2022-08-31",
-"billing_period_starting_date": "2022-08-01", "billing_plan_amount": "6708",
-"billing_plan_billing_date": "2022-08-31", "billing_plan_item": "1",
+"", "projectid": "", "quote": "", "revenue_details": "", "status": "",
+"subgroup_bqid": "5", "subgroup_end_date": "2100-12-12", "subgroup_groupid":
+"a0cAX000000TSWUYA4", "subgroup_name": "MAPFRE USA", "subgroup_owner_email":
+"employee1@test.com", "subgroup_start_date": "2023-06-01",
+"subgroup_subgroupid": "a19AX0000004simYAA", }, ) billing_line = opportunity
+["billing_lines"][0] self.assertDictEqual( billing_line, { "billing_amount":
+6708.0, "billing_date": "2022-08-31", "billing_period_ending_date": "2022-08-
+31", "billing_period_starting_date": "2022-08-01", "billing_plan_amount":
+"6708", "billing_plan_billing_date": "2022-08-31", "billing_plan_item": "1",
 "billing_plan_service_end_date": "2022-08-31",
 "billing_plan_service_start_date": "2022-08-01", "created_date": "2022-08-
 09T14:56:23.000+0000", "currency": "USD", "hourly_price": 65.0, "id":
 "a0sAX000000I8lgYAC", "last_modified_date": "2022-10-16T18:56:34.000+0000",
 "name": "BL-000175313", "project_code": "USMSEX05508", "project_id":
 "a00AX000002DVi1YAG", "revenue_dedication": 103.2, }, )
 mock_make_request.assert_called() @patch
```

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/constants.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/constants.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py`

 * *Files 0% similar despite different names*

```diff
@@ -876,27 +876,27 @@
             "amount": self.amount,
             "invoicing_country_code": self.invoicing_country_code,
             "operation_coordinator_email": self.operation_coordinator_email,
             "operation_coordinator_sub_email": self.operation_coordinator_sub_email,  # noqa: E501
             "created_at": self.created_at,
             "last_updated_at": self.last_updated_at,
             "opportunity_name": self.opportunity_name,
-            "stage": self.stage,
-            "lead_source": self.lead_source,
+            # "stage": self.stage,
+            # "lead_source": self.lead_source,
             "project_code": self.project_code,
             "project_id": self.project_id,
             "project_name": self.project_name,
             "project_start_date": self.project_start_date,
             "controller_email": self.controller_email,
             "controller_sub_email": self.controller_sub_email,
             "profit_center": self.profit_center,
             "cost_center": self.cost_center,
             "project_tier": self.project_tier,
             "jira_task_url": self.jira_task_url,
-            "opportunity_percentage": self.opportunity_percentage,
+            # "opportunity_percentage": self.opportunity_percentage,
             "billing_lines": [bl.to_dict() for bl in self.billing_lines],
             "project_line_items": [
                 pli.to_dict() for pli in self.project_line_items
             ],
             "account_billing_country": self.account_billing_country,
             "account_business_name": self.account_business_name,
             "account_name": self.account_name,
@@ -945,21 +945,21 @@
             "comments": self.comments,
             "end_date": self.end_date,
             "international_deparments": self.international_deparments,
             "opportunity_extension": self.opportunity_extension,
             "maintance_project": self.maintance_project,
             "ms_project_id": self.ms_project_id,
             "operation_coordinator_name": self.operation_coordinator_name,
-            "operation_coordinator_controller": self.operation_coordinator_controller,  # noqa: E501
+            # "operation_coordinator_controller": self.operation_coordinator_controller,  # noqa: E501
             "operation_coordinator_sub": self.operation_coordinator_sub,
             "opportunity": self.opportunity,
             "periodicity": self.periodicity,
             "profitcenter": self.profitcenter,
             "project_account": self.project_account,
             "projectcode": self.projectcode,
             "revenue_details": self.revenue_details,
             "status": self.status,
-            "internal_comment": self.internal_comment,
-            "rejection_reason": self.rejection_reason,
+            # "internal_comment": self.internal_comment,
+            # "rejection_reason": self.rejection_reason,
             "projectid": self.projectid,
             "quote": self.quote,
         }
```

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,45 +30,45 @@
                 "controller_sub_email": "STRING",
                 "cost_center": "INTEGER",
                 "created_at": "TIMESTAMP",
                 "currency": "STRING",
                 "invoicing_country_code": "STRING",
                 "jira_task_url": "STRING",
                 "last_updated_at": "TIMESTAMP",
-                "lead_source": "STRING",
+                # "lead_source": "STRING",
                 "operation_coordinator_email": "STRING",
                 "operation_coordinator_sub_email": "STRING",
                 "opportunity_name": "STRING",
-                "opportunity_percentage": "FLOAT",
+                # "opportunity_percentage": "FLOAT",
                 "profit_center": "INTEGER",
                 "project_code": "STRING",
                 "project_id": "STRING",
                 "project_name": "STRING",
                 "project_start_date": "DATE",
                 "project_tier": "STRING",
-                "stage": "STRING",
+                # "stage": "STRING",
                 "autorenewal": "BOOLEAN",
                 "comments": "STRING",
                 "end_date": "DATE",
                 "international_deparments": "BOOLEAN",
                 "opportunity_extension": "STRING",
                 "maintance_project": "BOOLEAN",
                 "ms_project_id": "STRING",
                 "operation_coordinator_name": "STRING",
-                "operation_coordinator_controller": "STRING",
+                # "operation_coordinator_controller": "STRING",
                 "operation_coordinator_sub": "STRING",
                 "opportunity": "STRING",
                 "periodicity": "STRING",
                 "profitcenter": "STRING",
                 "project_account": "STRING",
                 "projectcode": "STRING",
                 "revenue_details": "BOOLEAN",
                 "status": "STRING",
-                "internal_comment": "STRING",
-                "rejection_reason": "STRING",
+                # "internal_comment": "STRING",
+                # "rejection_reason": "STRING",
                 "projectid": "STRING",
                 "quote": "STRING",
             },
             "billing_lines": {
                 "billing_amount": "FLOAT",
                 "billing_date": "DATE",
                 "billing_period_ending_date": "DATE",
```

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-2.5.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.4.1/pyproject.toml` & `ms_salesforce_api-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "2.4.1"
+version = "2.5.0"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-2.4.1/PKG-INFO` & `ms_salesforce_api-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 2.4.1
+Version: 2.5.0
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

