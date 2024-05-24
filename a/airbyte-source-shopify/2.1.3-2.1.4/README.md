# Comparing `tmp/airbyte_source_shopify-2.1.3.tar.gz` & `tmp/airbyte_source_shopify-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_shopify-2.1.3.tar", max compression
+gzip compressed data, was "airbyte_source_shopify-2.1.4.tar", max compression
```

## Comparing `airbyte_source_shopify-2.1.3.tar` & `airbyte_source_shopify-2.1.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     4529 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/README.md
--rw-r--r--   0        0        0      800 2024-05-23 11:35:37.167847 airbyte_source_shopify-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/__init__.py
--rw-r--r--   0        0        0     1538 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/auth.py
--rw-r--r--   0        0        0     3797 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/config_migrations.py
--rw-r--r--   0        0        0      398 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/run.py
--rw-r--r--   0        0        0    28417 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/abandoned_checkouts.json
--rw-r--r--   0        0        0     2548 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/articles.json
--rw-r--r--   0        0        0     2135 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/balance_transactions.json
--rw-r--r--   0        0        0     2151 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/blogs.json
--rw-r--r--   0        0        0     1889 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/collections.json
--rw-r--r--   0        0        0     1173 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/collects.json
--rw-r--r--   0        0        0     2162 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/countries.json
--rw-r--r--   0        0        0     3100 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/custom_collections.json
--rw-r--r--   0        0        0     2628 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/customer_address.json
--rw-r--r--   0        0        0      986 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/customer_saved_search.json
--rw-r--r--   0        0        0    10233 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/customers.json
--rw-r--r--   0        0        0     1621 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/discount_codes.json
--rw-r--r--   0        0        0     1775 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/disputes.json
--rw-r--r--   0        0        0    24211 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/draft_orders.json
--rw-r--r--   0        0        0     9939 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/fulfillment_orders.json
--rw-r--r--   0        0        0    23930 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/fulfillments.json
--rw-r--r--   0        0        0     2042 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/inventory_items.json
--rw-r--r--   0        0        0     1114 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/inventory_levels.json
--rw-r--r--   0        0        0     2806 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/locations.json
--rw-r--r--   0        0        0     1919 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_articles.json
--rw-r--r--   0        0        0     1881 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_blogs.json
--rw-r--r--   0        0        0     1925 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_collections.json
--rw-r--r--   0        0        0     1957 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_customers.json
--rw-r--r--   0        0        0     2008 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_draft_orders.json
--rw-r--r--   0        0        0     1800 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_locations.json
--rw-r--r--   0        0        0     1874 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_orders.json
--rw-r--r--   0        0        0     1985 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_pages.json
--rw-r--r--   0        0        0     1782 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_product_images.json
--rw-r--r--   0        0        0     1919 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_product_variants.json
--rw-r--r--   0        0        0     2078 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_products.json
--rw-r--r--   0        0        0     1873 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_shops.json
--rw-r--r--   0        0        0     1985 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_smart_collections.json
--rw-r--r--   0        0        0    26296 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/order_refunds.json
--rw-r--r--   0        0        0    10425 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/order_risks.json
--rw-r--r--   0        0        0   103922 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/orders.json
--rw-r--r--   0        0        0     2093 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/pages.json
--rw-r--r--   0        0        0     7004 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/price_rules.json
--rw-r--r--   0        0        0     1760 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/product_images.json
--rw-r--r--   0        0        0     4886 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/product_variants.json
--rw-r--r--   0        0        0    14495 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/products.json
--rw-r--r--   0        0        0     3598 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/products_graph_ql.json
--rw-r--r--   0        0        0     8137 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/shop.json
--rw-r--r--   0        0        0     2009 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/smart_collections.json
--rw-r--r--   0        0        0     2006 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/tender_transactions.json
--rw-r--r--   0        0        0     6603 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/schemas/transactions.json
--rw-r--r--   0        0        0     6367 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/scopes.py
--rw-r--r--   0        0        0        0 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/__init__.py
--rw-r--r--   0        0        0     1813 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/exceptions.py
--rw-r--r--   0        0        0    20372 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/job.py
--rw-r--r--   0        0        0    83122 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/query.py
--rw-r--r--   0        0        0     6526 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/record.py
--rw-r--r--   0        0        0     1704 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/retry.py
--rw-r--r--   0        0        0      328 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/status.py
--rw-r--r--   0        0        0     3629 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/tools.py
--rw-r--r--   0        0        0     1969 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/graphql.py
--rw-r--r--   0        0        0  1354903 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/schema.py
--rw-r--r--   0        0        0     8518 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/source.py
--rw-r--r--   0        0        0     5118 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/spec.json
--rw-r--r--   0        0        0    37215 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/streams/base_streams.py
--rw-r--r--   0        0        0    11680 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/streams/streams.py
--rw-r--r--   0        0        0     4678 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/transform.py
--rw-r--r--   0        0        0    13468 2024-05-23 10:58:31.000000 airbyte_source_shopify-2.1.3/source_shopify/utils.py
--rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4529 2024-05-24 12:51:12.116168 airbyte_source_shopify-2.1.4/README.md
+-rw-r--r--   0        0        0      800 2024-05-24 12:57:56.400493 airbyte_source_shopify-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/__init__.py
+-rw-r--r--   0        0        0     1538 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/auth.py
+-rw-r--r--   0        0        0     3797 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/config_migrations.py
+-rw-r--r--   0        0        0      398 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/run.py
+-rw-r--r--   0        0        0    28417 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/abandoned_checkouts.json
+-rw-r--r--   0        0        0     2548 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/articles.json
+-rw-r--r--   0        0        0     2135 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     2151 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/blogs.json
+-rw-r--r--   0        0        0     1889 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/collections.json
+-rw-r--r--   0        0        0     1173 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/collects.json
+-rw-r--r--   0        0        0     2162 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/countries.json
+-rw-r--r--   0        0        0     3100 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/custom_collections.json
+-rw-r--r--   0        0        0     2628 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/customer_address.json
+-rw-r--r--   0        0        0      986 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/customer_saved_search.json
+-rw-r--r--   0        0        0    10233 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/customers.json
+-rw-r--r--   0        0        0     1621 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/discount_codes.json
+-rw-r--r--   0        0        0     1775 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/disputes.json
+-rw-r--r--   0        0        0    24211 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/draft_orders.json
+-rw-r--r--   0        0        0     9939 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/fulfillment_orders.json
+-rw-r--r--   0        0        0    23930 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/fulfillments.json
+-rw-r--r--   0        0        0     2042 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/inventory_items.json
+-rw-r--r--   0        0        0     1773 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/inventory_levels.json
+-rw-r--r--   0        0        0     2806 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/locations.json
+-rw-r--r--   0        0        0     1919 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_articles.json
+-rw-r--r--   0        0        0     1881 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_blogs.json
+-rw-r--r--   0        0        0     1925 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_collections.json
+-rw-r--r--   0        0        0     1957 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_customers.json
+-rw-r--r--   0        0        0     2008 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_draft_orders.json
+-rw-r--r--   0        0        0     1800 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_locations.json
+-rw-r--r--   0        0        0     1874 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_orders.json
+-rw-r--r--   0        0        0     1985 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_pages.json
+-rw-r--r--   0        0        0     1782 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_product_images.json
+-rw-r--r--   0        0        0     1919 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_product_variants.json
+-rw-r--r--   0        0        0     2078 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_products.json
+-rw-r--r--   0        0        0     1873 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_shops.json
+-rw-r--r--   0        0        0     1985 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_smart_collections.json
+-rw-r--r--   0        0        0    26296 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/order_refunds.json
+-rw-r--r--   0        0        0    10425 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/order_risks.json
+-rw-r--r--   0        0        0   103922 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/orders.json
+-rw-r--r--   0        0        0     2093 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/pages.json
+-rw-r--r--   0        0        0     7004 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/price_rules.json
+-rw-r--r--   0        0        0     1760 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/product_images.json
+-rw-r--r--   0        0        0     4886 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/product_variants.json
+-rw-r--r--   0        0        0    14495 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/products.json
+-rw-r--r--   0        0        0     3598 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/products_graph_ql.json
+-rw-r--r--   0        0        0     8137 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/shop.json
+-rw-r--r--   0        0        0     2009 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/smart_collections.json
+-rw-r--r--   0        0        0     2006 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/tender_transactions.json
+-rw-r--r--   0        0        0     6603 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/schemas/transactions.json
+-rw-r--r--   0        0        0     6367 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/scopes.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/__init__.py
+-rw-r--r--   0        0        0     1813 2024-05-24 12:51:12.120168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/exceptions.py
+-rw-r--r--   0        0        0    20372 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/job.py
+-rw-r--r--   0        0        0    84915 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/query.py
+-rw-r--r--   0        0        0     6526 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/record.py
+-rw-r--r--   0        0        0     1704 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/retry.py
+-rw-r--r--   0        0        0      328 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/status.py
+-rw-r--r--   0        0        0     3629 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/tools.py
+-rw-r--r--   0        0        0     1969 2024-05-24 12:51:12.124168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/graphql.py
+-rw-r--r--   0        0        0  1354903 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/schema.py
+-rw-r--r--   0        0        0     8518 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/source.py
+-rw-r--r--   0        0        0     5118 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/spec.json
+-rw-r--r--   0        0        0    37215 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/streams/base_streams.py
+-rw-r--r--   0        0        0    11715 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/streams/streams.py
+-rw-r--r--   0        0        0     4678 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/transform.py
+-rw-r--r--   0        0        0    13468 2024-05-24 12:51:12.132168 airbyte_source_shopify-2.1.4/source_shopify/utils.py
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.1.4/PKG-INFO
```

### Comparing `airbyte_source_shopify-2.1.3/README.md` & `airbyte_source_shopify-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/pyproject.toml` & `airbyte_source_shopify-2.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.1.3"
+version = "2.1.4"
 name = "airbyte-source-shopify"
 description = "Source CDK implementation for Shopify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/__init__.py` & `airbyte_source_shopify-2.1.4/source_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/auth.py` & `airbyte_source_shopify-2.1.4/source_shopify/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/config_migrations.py` & `airbyte_source_shopify-2.1.4/source_shopify/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/abandoned_checkouts.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/articles.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/balance_transactions.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/blogs.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/collections.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/collects.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/countries.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/countries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/custom_collections.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/customer_address.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/customer_address.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/customer_saved_search.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/customer_saved_search.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/customers.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/discount_codes.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/discount_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/disputes.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/draft_orders.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/fulfillment_orders.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/fulfillment_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/fulfillments.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/fulfillments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/inventory_items.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/inventory_levels.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/tender_transactions.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8506944444444445%*

 * *Differences: {"'properties'": "{'id': {'description': 'Unique identifier for the tender transaction.', 'type': "*

 * *                 "{insert: [(1, 'integer')], delete: [1]}}, 'shop_url': {'description': 'The URL "*

 * *                 "of the shop where the transaction took place.'}, 'order_id': "*

 * *                 "OrderedDict([('description', 'The identifier of the order associated with the "*

 * *                 "transaction.'), ('type', ['null', 'integer'])]), 'amount': "*

 * *                 "OrderedDict([('description', 'The tra […]*

```diff
@@ -1,56 +1,100 @@
 {
     "additionalProperties": true,
     "properties": {
-        "admin_graphql_api_id": {
-            "description": "The unique identifier for the inventory levels in GraphQL format.",
+        "amount": {
+            "description": "The transaction amount in the specified currency.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "available": {
-            "description": "The quantity of items available for sale in the inventory.",
+        "currency": {
+            "description": "The currency in which the transaction amount is stated.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
         "id": {
-            "description": "The unique identifier for the inventory level.",
+            "description": "Unique identifier for the tender transaction.",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "inventory_item_id": {
-            "description": "The unique identifier for the associated inventory item.",
+        "order_id": {
+            "description": "The identifier of the order associated with the transaction.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "location_id": {
-            "description": "The unique identifier for the location related to the inventory level.",
+        "payment_details": {
+            "description": "Details about the payment made for the transaction.",
+            "properties": {
+                "credit_card_company": {
+                    "description": "The company associated with the credit card used for payment.",
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                },
+                "credit_card_number": {
+                    "description": "The masked credit card number used for payment.",
+                    "type": [
+                        "null",
+                        "string"
+                    ]
+                }
+            },
             "type": [
                 "null",
-                "integer"
+                "object"
             ]
         },
-        "shop_url": {
-            "description": "The URL of the shop where the inventory belongs.",
+        "payment_method": {
+            "description": "The method used for payment, e.g., credit card, PayPal, etc.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "updated_at": {
-            "description": "The date and time when the inventory level was last updated.",
+        "processed_at": {
+            "description": "The date and time when the transaction was processed.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
+        },
+        "remote_reference": {
+            "description": "Reference to an external system for the transaction.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "shop_url": {
+            "description": "The URL of the shop where the transaction took place.",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "test": {
+            "description": "Flag indicating whether the transaction was done in a testing environment.",
+            "type": [
+                "null",
+                "boolean"
+            ]
+        },
+        "user_id": {
+            "description": "Unique identifier of the user associated with the transaction.",
+            "type": [
+                "null",
+                "integer"
+            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/locations.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_articles.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_blogs.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_collections.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_customers.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_draft_orders.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_locations.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_orders.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_pages.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_product_images.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_product_variants.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_products.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_shops.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_shops.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/metafield_smart_collections.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/metafield_smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/order_refunds.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/order_risks.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/order_risks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/orders.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/pages.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/price_rules.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/price_rules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/product_images.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/product_variants.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/products.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/products_graph_ql.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/products_graph_ql.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/shop.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/shop.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/smart_collections.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/schemas/transactions.json` & `airbyte_source_shopify-2.1.4/source_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/scopes.py` & `airbyte_source_shopify-2.1.4/source_shopify/scopes.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/exceptions.py` & `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/job.py` & `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/job.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/query.py` & `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -738,15 +738,15 @@
         Field(name="handle"),
         Field(name="title"),
         Field(name="updatedAt"),
         Field(name="descriptionHtml", alias="bodyHtml"),
         Field(name="publications", fields=publications_fields),
         Field(name="sortOrder"),
         Field(name="templateSuffix"),
-        Field(name="productsCount"),
+        Field(name="productsCount", fields=[Field(name="count", alias="products_count")]),
     ]
 
     record_composition = {
         "new_record": "Collection",
         # each collection has `publications`
         "record_components": ["CollectionPublication"],
     }
@@ -760,14 +760,16 @@
             publications = record_components.get("CollectionPublication", [])
             if len(publications) > 0:
                 record["published_at"] = publications[0].get("publishedAt")
                 record.pop("record_components")
         # convert dates from ISO-8601 to RFC-3339
         record["published_at"] = self.tools.from_iso8601_to_rfc3339(record, "published_at")
         record["updatedAt"] = self.tools.from_iso8601_to_rfc3339(record, "updatedAt")
+        # unnest `product_count` to the root lvl
+        record["products_count"] = record.get("productsCount", {}).get("products_count")
         # remove leftovers
         record.pop(BULK_PARENT_KEY, None)
         yield record
 
 
 class CustomerAddresses(ShopifyBulkQuery):
     """
@@ -984,39 +986,84 @@
         "includeLegacy": "true",
         "includeInactive": "true",
     }
     record_composition = {
         "new_record": "InventoryLevel",
     }
 
+    # quantity related fields and filtering options
+    quantities_names_filter: List[str] = [
+        '"available"',
+        '"incoming"',
+        '"committed"',
+        '"damaged"',
+        '"on_hand"',
+        '"quality_control"',
+        '"reserved"',
+        '"safety_stock"',
+    ]
+    # quantities fields
+    quantities_fields: List[str] = [
+        "id",
+        "name",
+        "quantity",
+        "updatedAt",
+    ]
+
     inventory_levels_fields: List[Field] = [
         "__typename",
         "id",
-        Field(name="available"),
         Field(name="item", fields=[Field(name="id", alias="inventory_item_id")]),
         Field(name="updatedAt"),
     ]
 
+    def _quantities_query(self) -> Query:
+        """
+        Defines the `quantities` nested query.
+        """
+
+        return Query(
+            name="quantities",
+            arguments=[Argument(name="names", value=self.quantities_names_filter)],
+            fields=self.quantities_fields,
+        )
+
+    def _process_quantities(self, quantities: Iterable[MutableMapping[str, Any]] = None) -> Iterable[Mapping[str, Any]]:
+        if quantities:
+            for quantity in quantities:
+                # save the original string id
+                quantity["admin_graphql_api_id"] = quantity.get("id")
+                # resolve the int id from str id
+                quantity["id"] = self.tools.resolve_str_id(quantity.get("id"))
+                # convert dates from ISO-8601 to RFC-3339
+                quantity["updatedAt"] = self.tools.from_iso8601_to_rfc3339(quantity, "updatedAt")
+            return quantities
+        return []
+
     def query(self, filter_query: Optional[str] = None) -> Query:
+        # construct the `quantities` query piece
+        quantities: List[Query] = [self._quantities_query()]
         # build the nested query first with `filter_query` to have the incremental syncs
-        inventory_levels: List[Query] = [self.build("inventoryLevels", self.inventory_levels_fields, filter_query)]
+        inventory_levels: List[Query] = [self.build("inventoryLevels", self.inventory_levels_fields + quantities, filter_query)]
         # build the main query around previous
         # return the constructed query operation
         return self.build(
             name=self.query_name,
             edges=self.query_nodes + inventory_levels,
             # passing more query args for `locations` query
             additional_query_args=self.locations_query_args,
         )
 
     def record_process_components(self, record: MutableMapping[str, Any]) -> Iterable[MutableMapping[str, Any]]:
         """
         Defines how to process collected components.
         """
-
+        # process quantities
+        quantities = record.get("quantities", [])
+        record["quantities"] = self._process_quantities(quantities)
         # resolve `inventory_item_id` to root lvl +  resolve to int
         record["inventory_item_id"] = self.tools.resolve_str_id(record.get("item", {}).get("inventory_item_id"))
         # add `location_id` from `__parentId`
         record["location_id"] = self.tools.resolve_str_id(record[BULK_PARENT_KEY])
         # make composite `id` from `location_id|inventory_item_id`
         record["id"] = "|".join((str(record.get("location_id", "")), str(record.get("inventory_item_id", ""))))
         # convert dates from ISO-8601 to RFC-3339
```

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/record.py` & `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/record.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/retry.py` & `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/retry.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/bulk/tools.py` & `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/bulk/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/graphql.py` & `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/shopify_graphql/schema.py` & `airbyte_source_shopify-2.1.4/source_shopify/shopify_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/source.py` & `airbyte_source_shopify-2.1.4/source_shopify/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/spec.json` & `airbyte_source_shopify-2.1.4/source_shopify/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/streams/base_streams.py` & `airbyte_source_shopify-2.1.4/source_shopify/streams/base_streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class ShopifyStream(HttpStream, ABC):
     # define default logger
     logger = logging.getLogger("airbyte")
 
     # Latest Stable Release
-    api_version = "2023-07"
+    api_version = "2024-04"
     # Page size
     limit = 250
 
     primary_key = "id"
     order_field = "updated_at"
     filter_field = "updated_at_min"
```

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/streams/streams.py` & `airbyte_source_shopify-2.1.4/source_shopify/streams/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,22 +111,23 @@
 class MetafieldDraftOrders(IncrementalShopifyGraphQlBulkStream):
     bulk_query: MetafieldDraftOrder = MetafieldDraftOrder
 
 
 class Products(IncrementalShopifyGraphQlBulkStream):
     bulk_query: Product = Product
     # pin the api version
-    api_version = "2024-04"
 
 
 class ProductsGraphQl(IncrementalShopifyStream):
     filter_field = "updatedAt"
     cursor_field = "updatedAt"
     data_field = "graphql"
     http_method = "POST"
+    # pin the old api_version before this stream is deprecated
+    api_version = "2023-07"
 
     def request_params(
         self,
         stream_state: Optional[Mapping[str, Any]] = None,
         next_page_token: Optional[Mapping[str, Any]] = None,
         **kwargs,
     ) -> MutableMapping[str, Any]:
@@ -259,15 +260,14 @@
     cursor_field = "created_at"
     nested_entity = "refunds"
 
 
 class OrderRisks(IncrementalShopifyGraphQlBulkStream):
     bulk_query: OrderRisk = OrderRisk
     # the updated stream work only with >= `2024-04` shopify api version
-    api_version = "2024-04"
 
 
 class Transactions(IncrementalShopifySubstream):
     parent_stream_class = Orders
     slice_key = "order_id"
     data_field = "transactions"
     cursor_field = "created_at"
```

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/transform.py` & `airbyte_source_shopify-2.1.4/source_shopify/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/source_shopify/utils.py` & `airbyte_source_shopify-2.1.4/source_shopify/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.1.3/PKG-INFO` & `airbyte_source_shopify-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-shopify
-Version: 2.1.3
+Version: 2.1.4
 Summary: Source CDK implementation for Shopify.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

